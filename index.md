# トップページ

## 自己紹介
東京都在住フリーランスエンジニアです。
<br/>
これまでのキャリアは自分のやりたい、なりたい目標に対してその時必要な事を全力でやる事で成長する泥臭いキャリア成形をしてきました。
<br/>
<br/>
[未経験からテスター、エンジニアとしてキャリアチェンジ](./carrier_start.md)し、
[タクシー配車サービス](taxi/index.md)、[EdTechプラットフォーム開発](ed_tech_platform/index.md)、[Saas管理機能付きIdaas](saas_management_idp/index.md)と複数のサービス回数に参加していく中でエンジニア組織のマネジメント、テックリード、CREチームの立ち上げなど経験してきました。
<br/>
また、単発の依頼としてRailsアプリケーションのソースコード、アーキテクチャのレビューやプロダクト開発の技術観点でのレビューも経験しました。
<br/>
これまで使用した[技術スタックの一覧はこちら](all_technology_stack.md)に一覧を書いています。
<br/>
<br/>
合わせて、[rails](https://contributors.rubyonrails.org/contributors/soartec-lab/commits)をはじめ[複数のOSS]((contribute_oss_list.md))にコントリビュートや
[登壇](https://speakerdeck.com/soarteclab/railsbaziyonatupushi-dong-wu-yu)、[教材の執筆](https://www.techpit.jp/courses/79)を通して培ってきた経験や知見の共有も行っています。

### やりたい事/興味のある事

1. DXの様にソフトウェアエンジニアリングの考え方やプラクティスを非エンジニアリング領域に活用する事で大きな生産性を得る事や、それに伴う組織作りに興味があります。

2. 自身でプロダクト開発を行いながらPMFを実現しその後にも価値を提供し続ける、CRE、PMM、グロースハックなどの分野に興味があります。

3. 目の前と未来をの数字と技術資産を理解した上で技術とビジネスを繋げる様なことがしたいです。その上で自分の好きだと思ったプロダクトを開発したいです。またプロダクトの表面だけではなく、それを支える組織力や技術力といった基盤を作るスキルを培いたいです。

### 得意な事
#### 開発速度を担保した高品質Railsアプリケーションの構築/運用
以下の経験を活かし、開発速度、メンテナンス性を担保したRailsアプリケーションの構築はもちろん、レガシーなどの理想の状態ではない既存アプリケーションに対する再建が得意です。

* [必要に応じてライブラリにPRを送り対応する経験](https://qiita.com/SoarTec-lab/items/f979336bd25d7b3a8cd2)。
* [railsバージョンアップ](ed_tech_platform/achievements/operation.md)経験。
* セキュアコーディングも得意で、実際に既存システムのコードリーディングからSQLインジェクション、オープンリダイレクトなどを発見しトリアージ、修正した経験もあります。
* パフォーマンスチューニングも得意です。コードリーディング、ツールを使用して、原因特定から対応まで行った経験があります。([チューニングを解説している教材も執筆しています](https://www.techpit.jp/courses/79))
* レイヤードアーキテクチャの採用、運用経験から適切な責任分解などの再設計を行った経験があります。
* ファットコントローラーなどの複雑なや実装やテストのない環境で安全にリファクタリングを行った経験や知見があります。

また以下の様な難易度の高いシステムの構築を経験しています。

* UDPプロトコル、メッセージキューなどを採用した対高トラフィックサービスの構築
* レイヤードアーキテクチャを採用したシステム設計
* 決済連携や認証基盤などセンシティブな機能

#### インフラ/CI/CD構築、運用
AWSの基本的なサービスは理解しています。
特に、ECSを使った本番環境でのコンテナ運用は以下の通り多くの経験をしています。

* EC2からECS Fargateへのインフラ移行の構築、本番環境での運用経験があります。
* ALB、ECSを仕様し安全にリードレプリカDBを活用し、アプリケーションの負荷分散を行うインフラアーキテクチャを設計、実装しました。
* ECSのログ収集のインフラアーキテクチャの設計、実装を行いました。
* ECSでのblue/greenデプロイ、カナリアリリースの実装、運用を行いました。

#### プロダクト開発
プロダクトの戦略策定からカスタマーサクセス、グロースハックなどの考え方を活用し、BMLループを回し施策に取り組み、プロダクトグロースを行う事が得意です。
また、お問い合わせ対応やインシデント対応といったサービス運用の経験もしてきました。

#### 組織マネジメント
エンジニアリーダー、新チーム立ち上げ、運営などの経験から、開発組織の生産性最大化及び組織のできる事の限界を広げる事が得意です。

* 戦略策定
  * ミッション、ビジョンの設定
  * KPI設定
  * SLO/SLI設定、運用
  * ロードマップ策定
* チーム作り、運営
  * 採用面談 - オンボーディング設計
  * 目標設定、管理、サポート
  * 振り返り
* 技術サポート、継承
* プロジェクト管理
* 障害対応、障害管理
* プロダクト戦略に則ったブランチ戦略、開発フロー、開発環境の整備

など

### パフォーマンスの発揮に遅れが出る環境
以下の環境は先に改善する事に時間が割かれるのでパフォーマンスを発揮するまで時間がかかる可能性が高いです。
嫌ではなく改善する事は好きです。

* 余計なステークホルダーが多く本質ではない、手間や時間がかかる環境。
* コミュニケーションがメンバーの肩書きや、印象、声の大きさに左右される環境。
* 現状の不満を吐き出すだけで終わり、どうやって解決するか？の議論ができない環境。

### SNS
* [GitHub](https://github.com/soartec-lab)
* [Twitter](https://twitter.com/SoartecL)
* [Qiita](https://qiita.com/SoarTec-lab)
* [SpeakerDeck](https://speakerdeck.com/soarteclab)
* [note](https://note.com/soartec_lab)

### OSS
railsをはじめ、複数のRubyGemsにコントリビュートしています。
[コントリビュートしたリポジトリ一覧](contribute_oss_list.md)

また、自身で作成したgemも公開しています。
[RubyGems](https://rubygems.org/profiles/soartec-lab)

railsへのコントリビューターという理由で以下のアンケートに参加する事ができました。

* Beihang University(北京航空航天大学) のアンケート「様々なCIツールのユーザーレビューの要約を抽出する研究がOSSコントリビューターの技術選定に役立つか(訳)」

> As you have contributed to the project rails which adopts continuous integration tools, your opinion is very valuable for us.

Federal University of Piaui(ピアウイ連邦大学)とBlekinge Institute of Technology (ブレーキンゲ工科大学)のアンケート「OSSプロジェクトのコントリビューターのコード知識とロイヤリティ調査アンケート(訳)」

> To support the onboarding of software developers, code reviews, and code maintenance, we have been investigating, different approaches to measure code knowledge/familiarity.
> To improve our understanding of code knowledge/familiarity, we need your help. 

### 登壇
* [ClassiのRuby/Railsバージョンアップ始動物語](https://speakerdeck.com/soarteclab/railsbaziyonatupushi-dong-wu-yu)
* [＜業務未経験者さん向け＞実務で必要な技術力を知ろう！](https://techpit.connpass.com/event/209751/)

### 教材執筆
* [Railsアプリケーションのパフォーマンス改善をしながらN+1問題を解決するスキルを身に付けよう！](https://www.techpit.jp/courses/79)
  * [執筆のインタビュー](https://note.com/techpit/n/nd8c2aed9448f)

## 参画プロジェクト
* [タクシー配車サービス](taxi/index.md)
* [EdTechプラットフォーム開発](ed_tech_platform/index.md)
* [Saas管理機能付きIdaas](saas_management_idp/index.md)
