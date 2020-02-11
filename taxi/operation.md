# サービス運用

インフラ領域のスキルレベルが高くないチームだったので運用コストも高く、基盤整備や運用改善をたくさんしました。

## やった事

### CI/CD
#### これまで

止まってたJenkins

#### 改善後
CircleCiに移行し、以下のジョブを自動化
* 自動テスト
* 静的解析(Rubocop)
* git conffrict確認
* 自動デプロイ

### アプリケーションログ監視

#### これまで

* ログ監視はしていない
* ログはローカルストレージ(EBS)に保存
* 障害発生時はEC2にSSHログインし調査
* オートスケール発生時はインスタンスが削除されログが消える

#### 改善後

* CloudWatchLogsを導入しログを監視
* ログはS3へ退避
* IAMでユーザ管理しているのでEC2にSSHせずログだけをAWSコンソールからだれでも見れる
* CloudWatchアラートで特定文字列を検知しメール通知
* リカバリできるものはアラートを検知し、AWS lambdaまたは、Rundeckで自動リカバリ

### RDBMSログ

#### これまで

* ログ出力設定はデフォルト
* 監視なし

#### 改善後

* パラメータチューニングし必要な情報を出力
  * スロークエリ(duration logs)
  * 調査期間中は、スロークエリ発生時に対象クエリの実行計画出力 
  * ロッククエリの出力
  * セッションタイムアウトログ
* AWS lambda + cloud event構成のバッチでログ、統計情報を取り込み、ログ解析しアラート検知

### EC2サーバリソース監視

#### これまで

なし

#### 改善後

* CloudWatchメトリクスを採取
  * collectdでEC2のメモリ、CPU、ディスク使用量をAWSに取り込む
  * プロセスの死活監視
* 取り込んだリソースをCloudWatchで監視

### DBサーバ
#### これまで
PostgresqlをEC2にインストール

#### 改善後
AWS RDSに移行しました。
DB移行ツール、移行後の確認ツールを自作し対応しました。

### cronバッチ

#### これまで

EC2サーバのcrontabをchefで管理

#### 改善後

バッチ管理ツールにRundeckを採用してジョブスクリプトはgit管理しました。
その後以下の理由でCloudFormation + CloudwatchEvent + lambda構成に移行しました。

* CloudFormationで管理する事で、他プロジェクト(他AWSアカウント)に流用できる
* 管理ツール的なバッチと、アプリケーションバッチ双方共に一元管理できる
* AWSコンソールor開発環境から操作できるので、バッチスケジュール変更が容易

### 本番環境デプロイ

#### これまで

* スキルを持った人が夜間に対応
  * 属人性が高い
* ダウンタイム15分程度
* 手順に従いデプロイ

#### 改善後
chef、terraform、shellscriptを使ってblue/greenデプロイ自動化ツール作成をし以下の課題解決を行いました。

* 属人化の解消
* ダウンタイムなし(0秒)
* リリース後の切り戻しも数分
* いつでもリリースできるようになった