# EdTechプラットフォーム開発
学校のICT化をサポートするSaas型プラットフォーム

## 概要
インフラ、サーバーサイド、フロントエンドと幅広く開発していました。
社内複数チームを経験した後にCRE立ち上げをを行い、その後プロダクトチームのエンジニアリーダーとして10人のエンジニアチームのテクニカルリード、マネジメントを行いました。
Ruby/Railsバージョンアップ、サービスマネージャーなど組織横断課題の解決や組織課題にも取り組み、幅広い経験ができました。

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

* [ログ収集基盤の構築](log_collection.md)
* [Railsセキュリティバグトリアージ対応](rails_security_bug_triage.md)
* [エンジニアオンボーディング](engineer_onbording.md)

#### 2019/05 - 2019/07
チーム: プロダクトチーム
<br>
役割: Railsエンジニア

* [QAチーム立ち上げサポート](qa_team_supoprt.md)
* [Ruby/Rails/その他gemバージョンアップ](ruby_gems_upgrade.md)

#### 2019/08 - 2020/06
チーム: CREチーム
<br>
役割: CRE

* [CREチーム立ち上げ](cre_team_build.md)
* [システム監視設計、運用](system_monitoring.md)
* [エンジニアオンボーディング](engineer_onbording.md)

#### 2020/07 - 
チーム: プロダクトチーム
<br>
役割: エンジニアリーダー


## カテゴリ毎の実績
#### 組織への取り組み
* [QAチーム立ち上げサポート](qa_team_supoprt.md)
* [CREチーム立ち上げ](cre_team_build.md)
* [エンジニアオンボーディング](engineer_onbording.md)

#### サービス運用/DevOps 
* [システム監視設計、運用](system_monitoring.md)
* [ログ収集基盤の構築](log_collection.md)
* [Ruby/Rails/その他gemバージョンアップ](ruby_gems_upgrade.md)
* [Railsセキュリティバグトリアージ対応](rails_security_bug_triage.md)

#### [プロダクト開発](achievements/product_summary.md)
* 
