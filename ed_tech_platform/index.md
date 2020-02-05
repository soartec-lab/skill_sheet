# 学校のICT化をサポートするSaas型プラットフォーム

## サービスについて
* 2019年5月時点で2500校の学校(全国の高校の2校に1校)が導入
* ユーザー数116万人

## 技術スタック
アプリケーションレイヤーは機能毎に分かれ、データベースは共通のものを参照している、"分断されたモノリス"構成で1つのサービスを構築しています。
その為各ソフトウェアのバージョンは使用していた中での最新バージョンのみ記述します。

### サーバサイド
#### 言語
* Ruby 2.7
* PHP 7.3

#### フレームワーク 
* Rails 6.1
* grape
* Rspec
* FuelPHP

### フロントエンド
#### 言語
* JavaScript
* CoffeeScript

#### フレームワーク/ライブラリ
* AngularJS 1.6.4
* React.js 15.4.1
  * MobX
* Backbone.js 1.2.3
  * marionette.js
* jQuery 1.11.1

#### テンプレートエンジン
* Pug
* slim
* haml
* erb
* ejs

### インフラ
#### Paas
* AWS

#### webサーバ、プロキシ

* Nginx

#### コンテナ
* Docker

#### データベース
* MySQL 5.7
* Elasticsearch 6.3
* Redis 2.8

#### CI/CD
* CircleCi
* AWS CodeDeploy
* dependency bot

#### 監視
* Datadog
* Mackerel
* Newreric
* Skylight
* Sentry
* Bugsnag

#### Iaas
* Terraform
* AWS CloudFormation
* itamae

### その他
* Github

## 分析、管理ツール

### BIツール
* GoogleAnaliytics
* Google DetaPoprtal
* Google BigQuery
* AWS Athena
* Datadogコンソール

### タスク管理
チケット管理ツールは乱立していましたが最終的にAsanaに統一されました。

* Asana
* Jira
* Backlog
* torello

### ドキュメント管理
* Confluence
* esa 