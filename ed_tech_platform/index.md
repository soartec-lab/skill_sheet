# EdTechプラットフォーム開発
学校のICT化をサポートするSaas型プラットフォーム

## 概要
インフラ、サーバーサイド、フロントエンドと幅広く開発していました。
社内複数チームを経験した後にCRE立ち上げを行い、その後プロダクトチームのテックリードとしてプロダクトマネージャーと協業しプロダクト戦略の策定や、 10人前後エンジニアチームのテクニカルリード、ピープルマネジメントを行いプロダクト開発を推進しました。
またサービスマネジメント、エンジニアメンター、組織編成、プロダクト再建など組織横断課題の解決にも携わり幅広い経験ができました。

## サービスについて
* 2019年5月時点で2500校の学校(全国の高校の2校に1校)が導入
* ユーザー数116万人

## アプリケーションについて
### アーキテクチャ
アプリケーションレイヤーは機能毎に分かれ、データベースは共通のものを参照している、"分断されたモノリス"構成で1つのサービスを構築しています。
バックエンドは、サブシステム毎にPHPとRubyで開発しており、Railsアプリにはレイヤードアーキテクチャ、CQRSを採用し保守性の高いアーキテクチャへの改善を行なっています。
フロントエンドはSPA、MPA構成がサブシステムによって異なっています。

 技術スタックの詳細は[こちら](technology_stack.md)

## 期間毎の実績
#### 2018/10 - 2019/04
チーム: カスタマーサクセスチーム
<br>
役割: Railsエンジニア

* [ログ収集基盤の構築](achievements/log_collection.md)
* [Railsセキュリティバグトリアージ対応](achievements/rails_security_bug_triage.md)
* [繁忙期のCX改善施策](achievements/cx_kaizen_projrct.md)
* [エンジニアオンボーディング](achievements/engineer_onbording.md)

#### 2019/05 - 2019/07
チーム: プロダクトチーム
<br>
役割: Railsエンジニア

* [QAチーム立ち上げサポート](achievements/qa_team_supoprt.md)
* [Ruby/Rails/その他gemバージョンアップ](achievements/ruby_gems_upgrade.md)

#### 2019/08 - 2020/06
チーム: CREチーム
<br>
役割: CRE

* [CREチーム立ち上げ](achievements/cre_team_build.md)
* [システム監視設計、運用](achievements/system_monitoring.md)
* [エンジニアオンボーディング](achievements/engineer_onbording.md)

#### 2020/07 - 
チーム: プロダクトチーム
<br>
プロダクトチーム役割: テックリード
<br>
組織横断役割: エンジニアメンター、サービスマネジメント

* [DevOpsなマインドセットと組織文化作り](https://note.com/soartec_lab/n/n649db2915142)
  * SLO/SLI定義/PWG/ポストモーテム
* [採用、チーミング]()
  * エンジニアJD策定
  * 振り返り(VSM/タイムライン/learning metrix/KPT/YWT)
* [プロダクトの技術戦略]
  * システム構成のas-is/to-be
  * ロードマップと目標設定
* [プロダクト戦略に最適なブランチ戦略、リリースフロー、検証環境の選定]()
* [機能クローズ]()
* [インシデント対応フローの最適化]()

* [ECS for Fagateへのインフラリプレイス]()
* [ECSでのblue/greenデプロイ、カナリアリリース実現のインフラ構築]()
* [FuentBitを使用したECSのログ収集基盤構築]()
* [railsアプリケーションでリードレプリカDBを活用するインフラ構築]()
* [チームでのrails含むgemのアップデート]()
* [railsアプリのasettsコンパイラをsprocketsからwebpackerへ移行]()
* [新規プロダクトローンチ]


## カテゴリ毎の実績
#### 組織への取り組み
* [QAチーム立ち上げサポート](achievements/qa_team_supoprt.md)
* [CREチーム立ち上げ](achievements/cre_team_build.md)
* [エンジニアオンボーディング](achievements/engineer_onbording.md)

#### サービス運用/DevOps 
* [システム監視設計、運用](achievements/system_monitoring.md)
* [ログ収集基盤の構築](achievements/log_collection.md)
* [Ruby/Rails/その他gemバージョンアップ](achievements/ruby_gems_upgrade.md)
* [Railsセキュリティバグトリアージ対応](achievements/rails_security_bug_triage.md)

#### [プロダクト開発]
* [繁忙期のCX改善施策](achievements/cx_kaizen_projrct.md)
* [特定機能の運用負荷軽減](achievements/operation_kaizen_project.md)
* [外部API連携処理のリプレイス](achievements/api_replace.md)
* [BIプロダクト新規開発](achievements/launch_bi_product.md)
