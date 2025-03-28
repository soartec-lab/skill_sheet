# SmartHR
[SmartHR](https://smarthr.jp/)の開発

## サービス説明

「SmartHR」から各企業が導入しているさまざまな外部サービスへワンクリックでログインできる「IdP機能（シングルサインオン機能）」です。

## 概要

プロダクトエンジニアとして、ID基盤の開発・運用及び、ID管理プロダクトの新規開発を行いました。ID管理プロダクト開発では0->1フェーズから参画し、開発及びプロダクト全体の技術選定を行いました。

https://smarthr.jp/release/69501
https://www.itmedia.co.jp/news/articles/2407/01/news131.html

## アーキテクチャ

フロントエンドは`Next.js`の`static export`を用いて静的なファイルを出力し配信し、バックエンドはバックエンドはモジュラーモノリス構成の`rails`アプリケーションで`API`を公開している`SPA`構成です。

<br/>

バックエンドはモジュラーモノリス構成の`rails`にモジュールとして新機能を実装しました。
フロントエンドは`pnpm`の`worksace`でモノレポ管理しているため`package`を新規に作成し`Next.js`アプリを構築する形で実装しました。
フロントエンドとバックエンドは`REST API`で通信を行うので`OpenAPI`による`API`管理とスキーマ駆動開発を行っていしました。スキーマ駆動を担保するためにバックエンドでは`committee`gemを用いて`Request Spec`でのスキーマとの整合性を担保し、フロントエンドでは`orval`を使用し`SWR`での`API`アクセス及び`hooks`の自動生成を行っていました。

技術スタックの詳細は[こちら](technology_stack.md)

## 期間毎の実績
### ~ サービスローンチ
#### 役割: プロダクトエンジニア・システム面でのリード

ローンチのタイミングでどの機能をどこまで作るか決まっていない状態から議論に参加しました。過去の開発経験を生かしチームメンバーへの情報共有や、技術的観点での実現性や、リリース後のグロース、サービス運用についての観点でMVPのスコープ定義に貢献しました。
開発においては技術的な意識決定、ベース部分を実装したり、アプリケーションの中で複雑性が高い機能を担当する事で開発全体の不確実性を下げると同時に全体の品質底上げに貢献しました。

<br/>

開発組織全体として、モジュラーモノリスでのアプリ構築は実績が少なかったためモジュール間の境界付けと依存関係の管理や`packwerk`の設定などやルール化をキャッチアップしながら定めていき、開発ではレビューの中で知見を共有しながらアークテクチャ上の品質を担保しました。
フロントエンドについては、`Next.js`を含むフレームワークやコアライブラリーの選定から、ビルドした静的ファイルの配信方法までの意思決定を行いました。

<br/>

全体のアプリケーション構成のアーキテクチャでは、ドメインの特性やグロースの見立て、運用コストや開発の生産性・体験という技術的な側面や、新規機能開発を言うビジネス上の側面など多角的に情報を収集し最適解となるよう努めました。
大きな意思決定においては、運用の中で変更可能にする、他者に知見を共有する、チーム内の集合地から最適な意思決定をを決定できるようにデザインドキュメントを作成していました。
