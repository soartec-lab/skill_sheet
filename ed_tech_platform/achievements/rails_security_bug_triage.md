# Railsセキュリティバグトリアージ対応

コードレビューからSQLインジェクション、オープンリダイレクトを発見しトリアージ、修正まで行いました。
また、以下の様にセキュリティ対応のフローなど整備がされていない中で自主的に対応しプロダクト全体の品質を向上する事ができました。

## 課題
* セキュリティバグに対する体制がない(だれが、どうやってのフローが決まっていない)

## やった事

サービスに影響のあるセキュリティバグの情報公開がされた時に、トリアージ及び対策を行いました。
また各プロセスの時間計測、課題を挙げる事で組織体制の強化に貢献しました。

### 実際のトリアージ内容
1. 発生したインシデントの情報を収集し、自社で対応すべきものかどうかを判断する
2. 対応方法の整理
* バージョンアップする or パッチをあてる
* デグレートする箇所がないか
* リリースの方法(一部のサービスで適応するなど)
3. 関係者へ周知

### 実際トリアージにかかった時間
発生したインシデントの情報を収集し、自社で対応すべきものかどうかを判断する
-> 30分

対応方法の整理
-> 2時間

合計 2時間30分

関係者の周知までにかかった時間
-> 12日

GMOべパぼのセキュリティ対策室と同等のスピード
https://tech.pepabo.com/2019/03/18/analysis-rails-vulnerabilities/

### その後

セキュリティバグに対する体制ができました。