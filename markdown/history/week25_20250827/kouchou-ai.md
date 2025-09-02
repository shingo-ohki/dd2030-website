# 広聴AI 8/20〜8/27 のGitHub活動まとめ

先週は2件のIssueがクローズされ、2件の新機能が追加される形で大きく進展しました。また、新たに1件のIssueが立ち上がり、1件のPRで活発な議論が続いています。

---

## 完了したタスク

### 1. [Issue #692](https://github.com/digitaldemocracy2030/kouchou-ai/issues/692) ハイフンで終わるIDが受理されないことを注意書きやエラーで知らせたい
- 作成者: yuneko1127  
- 担当PR: [PR #697](https://github.com/digitaldemocracy2030/kouchou-ai/pull/697)  
- 実装者: mochizuki-pg + Devin  
- 概要:  
  - 新たにバリデーションを追加し、「ハイフンで終わるIDは使えない」旨のエラーメッセージを表示  
  - 細かい入力制限やエラーメッセージがユーザにわかりやすくなりました

### 2. [Issue #441](https://github.com/digitaldemocracy2030/kouchou-ai/issues/441) headerにプロダクト名を表示する
- 作成者: UtkNggc  
- 担当PR: [PR #695](https://github.com/digitaldemocracy2030/kouchou-ai/pull/695)  
- 実装者: mochizuki-pg + Devin  
- 概要:  
  - ヘッダー左上のロゴを「デジタル民主主義2030」から「広聴AI」に変更し、サブ表記として「part of project デジタル民主主義2030」を追加  
  - Figmaで作成されたロゴ画像を適用し、PC・SP両方の画面に対応  

---

## 未完了のタスクと議論の状況

### 1. [Issue #696](https://github.com/digitaldemocracy2030/kouchou-ai/issues/696) 広聴AIで作成したレポートの誤った解釈を防止する方法
- 作成者: shingo-ohki  
- 背景:  
  - レポートの結果を可視化ツールとして使った際に「数値＝客観的根拠」と誤解されやすい問題が浮上  
  - 「質的な調査ツール」だという前提の解説や注意書きが必要との声が多数  
- 議論されている内容:  
  - データの偏りやノイジーマイノリティを拾う点への注意書きをどこに実装するか  
  - ブログやマニュアルへの掲載だけでなく、Webサイト上でポップアップなどを出す案  
  - 「課題発見ツール」と割り切った方が誤解を減らせるのでは？といった提案も  
  - 表示イメージや文字サイズなどUI・UX的な検討も進みそう

### 2. [PR #688](https://github.com/digitaldemocracy2030/kouchou-ai/pull/688) fix: Azure Deploy 時に client コンテナの環境変数が未設定になる
- 作成者: shingo-ohki  
- 背景:  
  - [Issue #642](https://github.com/digitaldemocracy2030/kouchou-ai/issues/642) で追加されたAzureデプロイワークフローに不備があり、clientコンテナの一部環境変数が正しく設定されていない  
  - [Issue #682](https://github.com/digitaldemocracy2030/kouchou-ai/issues/682) へのコメントで指摘があり、修正が進行中  
- 議論されている内容:  
  - ワークフロー全体で環境変数を設定するタイミングの見直し  
  - コンテナごとにSecretを設定する際のセキュリティと効率化  
  - CIの通し方や単体テストが十分かどうか  
  - 実際のAzure側でデプロイが通るかの検証レポートの共有  

---

## 貢献への呼びかけ

- 「ハイフンで終わるIDは使えない」という細かなエラーメッセージ周りの修正から、大きなUI変更まで、多様な貢献が行われています。  
- 新しく立ち上がった [Issue #696](https://github.com/digitaldemocracy2030/kouchou-ai/issues/696) のように、技術的な実装だけでなく、説明文やチュートリアルのアイデア出し・実装も歓迎です。  
- [PR #688](https://github.com/digitaldemocracy2030/kouchou-ai/pull/688) では、Azureへのデプロイフローやセキュリティ周りに興味のある方が参加してくださると助かります。  
- アイデアや改善提案をIssueに書いていただくだけでも大きな助けになりますし、コードの修正やドキュメントへの追記も大歓迎です。  

今後も「広聴AI」はさらなる機能追加・改善を行い、多くの公共テーマのオンライン対話をサポートしていきます。ぜひGitHubリポジトリでの議論や開発にご参加ください！  