# Polimoney 8/20~8/27 のGitHub活動まとめ

今週もPolimoneyプロジェクトへのご協力、ありがとうございます。ここでは8月20日から8月27日までのIssue・Pull Requestの動きをまとめます。  
まずは完了したタスクを紹介し、その後、まだ未完了のタスクでどのような議論が行われているかをお伝えします。ぜひ興味があるテーマに参加してください！

---

## 完了したIssue (3件)

### [Issue #180](https://github.com/digitaldemocracy2030/polimoney/issues/180) サーバーサイドでのEmailバリデーションの追加
- 作成者: YukihiroArakawa
- 不正なメールアドレス形式をサーバーサイドでチェックできるようになりました。  
  - ユーザーは、誤ったメールアドレスを入力して登録を試みた際に即エラーに気づけるようになります。  
  - データベースには不正な形式のメールアドレスが保存されなくなり、運用者側としては調査コストが減ります。

### [Issue #172](https://github.com/digitaldemocracy2030/polimoney/issues/172) スマホで開いた時にもSNS共有リンクが表示されるようにする
- 作成者: noritaka1166
- スマホアクセス時にSNS共有リンクが表示されない問題が解消されました。  
  - PCだけでなくスマホからもすぐSNSでシェアできるようになり、情報拡散がしやすくなります。

### [Issue #101](https://github.com/digitaldemocracy2030/polimoney/issues/101) 「polimoney」検索結果で表示されるアイキャッチ画像の変更
- 作成者: Nozomi-M21
- 検索結果に特定の個人写真が表示されてしまっていた問題が修正されました。  
  - 政治的中立性を確保するために、DD2030ロゴなど共通のアイキャッチに置き換えられています。

---

## 今週マージされたPull Request (7件)

下記は先週から今週にかけてマージされたPRです。新機能から設定変更まで、さまざまな貢献がありました。ぜひどんな人が何を直しているのか、チェックしてみてください。

1. [PR #185](https://github.com/digitaldemocracy2030/polimoney/pull/185) chore: PR作成時にGO言語のlintを実行するワークフローを作成  
   - 作成者: YukihiroArakawa  
   - PR作成時にGoのlintersを走らせるワークフローが追加され、同時にプロジェクト全体をgofmtで整形。自動レビューとコード品質アップに繋がります。

2. [PR #184](https://github.com/digitaldemocracy2030/polimoney/pull/184) refactor: オプショナルチェーンを使用  
   - 作成者: noritaka1166  
   - フロントエンド（JavaScript/TypeScript）でオプショナルチェーンに書き換え、ガード条件をシンプルに。AIが自動生成したコメントを削除したなど、軽微なリファクタリグのPRです。

3. [PR #183](https://github.com/digitaldemocracy2030/polimoney/pull/183) refactor: SNSボタンコンポーネントの分離  
   - 作成者: noritaka1166  
   - SNSシェアボタンを専用コンポーネントとして分離。読みやすく再利用しやすい構造に整理されました。

4. [PR #182](https://github.com/digitaldemocracy2030/polimoney/pull/182) feat: backendにemailのバリデーションロジックを追加  
   - 作成者: YukihiroArakawa  
   - [Issue #180](https://github.com/digitaldemocracy2030/polimoney/issues/180) に対応したサーバーサイドのメールアドレス形式チェック機能追加。テストも含めて実装されています。

5. [PR #181](https://github.com/digitaldemocracy2030/polimoney/pull/181) プロフィール用エンドポイントを用意  
   - 作成者: shumizu418128  
   - [Issue #120](https://github.com/digitaldemocracy2030/polimoney/issues/120) に関連。認証済ユーザーが自分のプロフィールを取得できるAPIが追加。今後のマイページ機能実装がより進めやすくなります。

6. [PR #179](https://github.com/digitaldemocracy2030/polimoney/pull/179) chore: BUG Report の形式不備修正  
   - 作成者: noritaka1166  
   - バグ報告用テンプレートのYAML構文エラー修正。新機能ではありませんが、バグ報告がスムーズに行えるよう改善されました。

7. [PR #178](https://github.com/digitaldemocracy2030/polimoney/pull/178) VS Code のフォーマッタ設定を追加  
   - 作成者: grassfieldk  
   - VS CodeでBiomeのフォーマッタを使うための設定が追加。開発環境を合わせることで、不要な差分やフォーマットのズレを減らし、レビューしやすくなります。

---

## 未完了のタスクでの議論 (1件)

今週は大きく更新があったIssueのうち、まだクローズしていないものが1件あります。  
議論を継続中ですので、興味がある方はぜひ参加してみてください。

### [Issue #134](https://github.com/digitaldemocracy2030/polimoney/issues/134) [シェア機能]タイトルとサムネイルを変更する
- 作成者: kotaro-yamasaki  
- シェアした際、政治家個別ページならその政治家さんの名前や写真をシェアカードに出したいという要望があります。  
- 現在はタイトルやサムネイルが固定で"Polimoney"とロゴ画像だけになっているため、動的に変化させる方法についての議論が続いています。  
- データベースとの連携やサーバーサイドレンダリングの仕組みが未確定で、調整が必要。「結局、DBが整うかフロントでOGPを生成するか」などの議論点があるようです。

---

## おわりに

今週はサーバーサイドのEmailバリデーションやSNSシェアボタン周りのリファクタなど、ユーザーにとっての使い勝手向上と開発者にとっての開発効率化が進みました。一方で、スマートなOGP対応など、まだ議論が必要な機能もあります。  
興味のある方はぜひIssueやPRにコメントしてください。OSS開発は多様な視点からのアイデアが大歓迎です。皆さまのご協力、ご参加をお待ちしています！