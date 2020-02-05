# 学校のICT化をサポートするSaas型プラットフォーム

## サービスについて
* 2019年5月時点で2500校の学校(全国の高校の2校に1校)が導入
* ユーザー数116万人

## 技術スタック
アプリケーションレイヤーは機能毎に分かれ、データベースは共通のものを参照している、"分断されたモノリス"構成で1つのサービスを構築しています。
その為各ソフトウェアのバージョンは使用していた中での最新バージョンのみ記述します。

### サーバサイド
* Ruby 2.7
  * Rails 6.1
  * grape
  * Rspec

* PHP 7.3
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

### データベース
* MySQL 5.7
* Elasticsearch 6.3
* Redis 2.8

### CI/CD
* CircleCi
* AWS CodeDeploy
* dependency bot

### 監視
* Datadog
* Mackerel
* Newreric
* Skylight

### BIツール
* GoogleAnaliytics
* Google DetaPoprtal
* Google BigQuery
* AWS Athena
* Datadogコンソール