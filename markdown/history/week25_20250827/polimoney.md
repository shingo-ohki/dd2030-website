# Polimoney 8/20〜8/27 のGitHub活動まとめ

今週もPolimoneyプロジェクトで多くのIssueがクローズされ、さらに新たな機能追加やリファクタリングが盛り上がりました。以下に、完了したIssueやマージされたPull Request、そして現在進行中の議論をまとめます。少しでも興味のある方は、ぜひIssueやPRでの議論に参加してみてください！

---

## 今週完了した主なIssue

### [Issue #180](https://github.com/digitaldemocracy2030/polimoney/issues/180) サーバーサイドでのEmailバリデーションの追加
- 作成者: YukihiroArakawa
- サーバーサイドでメールアドレス形式を検証する機能を追加する提案。  
- ユーザーにとっては、登録時のメールアドレス入力ミスを減らせるメリット。  
- すでに [PR #182](https://github.com/digitaldemocracy2030/polimoney/pull/182) で実装が完了しています。

### [Issue #172](https://github.com/digitaldemocracy2030/polimoney/issues/172) スマホ対応でのSNS共有リンク表示
- 作成者: noritaka1166
- スマホからアクセスした時にSNS共有ボタンが表示されない問題を改善したい、という要望。
- SNSボタン機能のリファクタリング（[PR #183](https://github.com/digitaldemocracy2030/polimoney/pull/183) など）とも関連し、無事完了しました。

### [Issue #101](https://github.com/digitaldemocracy2030/polimoney/issues/101) 「polimoney」検索結果で表示されるアイキャッチ画像の変更
- 作成者: Nozomi-M21
- 検索結果に意図しない人物写真が表示される問題をロゴ画像に変更しようという提案。
- 実際に画像の表示を変更し、政治的中立性を保つ改善が行われました。

---

## 今週マージされたPull Request

### [PR #185](https://github.com/digitaldemocracy2030/polimoney/pull/185) chore: PR作成時にGO言語のlintを実行するワークフローを作成
- 作者: YukihiroArakawa  
- 内容: Go言語のコード整形とlintをPR時に自動でチェックするワークフローを追加。  
- レビュー労力の削減やコード品質の向上に貢献。

### [PR #184](https://github.com/digitaldemocracy2030/polimoney/pull/184) refactor: オプショナルチェーンを使用
- 作者: noritaka1166  
- 内容: フロントエンドでの条件分岐を短縮化し、不要コメントを削除。  
- ユーザー体験には変化はありませんが、コードがよりシンプルに。

### [PR #183](https://github.com/digitaldemocracy2030/polimoney/pull/183) refactor: SNSボタンコンポーネントの分離
- 作者: noritaka1166  
- 内容: SNS共有ボタンを独立したコンポーネントとして切り出し。  
- 今後の拡張や他の画面での再利用が容易になります。

### [PR #182](https://github.com/digitaldemocracy2030/polimoney/pull/182) feat: backendにemailのバリデーションロジックを追加
- 作者: YukihiroArakawa  
- 内容: [Issue #180](https://github.com/digitaldemocracy2030/polimoney/issues/180) を受け、サーバーサイドにメールアドレスの形式チェック機能を実装。  
- ユーザー登録の信頼性が向上。

### [PR #181](https://github.com/digitaldemocracy2030/polimoney/pull/181) プロフィール用エンドポイントを用意
- 作者: shumizu418128  
- 内容: 認証ユーザー用のプロフィールを取得する新規APIを追加。  
- ユーザーが自分のプロフィールを確認・更新する機能の土台を実装。

### [PR #179](https://github.com/digitaldemocracy2030/polimoney/pull/179) chore: BUG Report の形式不備修正
- 作者: noritaka1166  
- 内容: バグ報告テンプレートの構文誤りを修正。  
- バグ報告の際に自動ラベルづけが正常に動作するようになりました。

### [PR #178](https://github.com/digitaldemocracy2030/polimoney/pull/178) VS Code のフォーマッタ設定を追加
- 作者: grassfieldk  
- 内容: Visual Studio Code の統一フォーマット設定をプロジェクトに追加。  
- 開発者同士のコード整形ルールをそろえ、レビュー時の差分を減らしています。

---

## まだ進行中のIssue・議論

### [Issue #134](https://github.com/digitaldemocracy2030/polimoney/issues/134) [シェア機能]タイトルとサムネイルを変更する
- 作成者: kotaro-yamasaki  
- SNSでのシェア時に、ページごとに異なるタイトルとサムネイル画像を表示したいという要望。  
- 現在はひとまずPolimoneyのデフォルト画像が設定されていますが、ページに紐づく政治家さんの写真などを表示する案が議論されています。  
- “DB構造が整ったら実装”という声もあり、引き続き意見募集しています。

---

## 参加の呼びかけ

- 完了したIssueやマージされたPRを見ると、多様な開発者が機能追加・ワークフロー改善・バグ修正など様々な側面で貢献していることがわかります。  
- 未完了のIssueでは特にシェア機能の拡張が盛り上がっており、UI/UXデザイナーやフロントエンドエンジニアの皆さんにもご参加いただけると嬉しいです。  
- OSS開発に興味がある方は、ぜひ遠慮なくIssueやPRでコメントしてみてください！

今後ともPolimoneyを盛り上げ、より良いデジタル民主主義の実現を一緒に目指していきましょう。  