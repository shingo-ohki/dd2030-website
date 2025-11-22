# デジタル民主主義WEB 11/12~11/19 のGitHub活動まとめ

こんにちは！デジタル民主主義WEB開発の進捗をお知らせします。今週は過去に更新が止まっていた週報をまとめて補完する作業などが完了し、新しいIssueもいくつか立ち上がっています。以下に詳しくご紹介します。

---

## 今週完了したタスク

### ■ [Issue #176](https://github.com/digitaldemocracy2030/website/issues/176)  
「更新が漏れている過去の分の活動状況を補完する」  
作成者: shingo-ohki  
過去に止まっていた活動状況の更新をしっかり反映できるように修正が行われ、Issueがクローズされました。ユーザにとっては、「以前の週報がまとめて確認できるようになった」というメリットがあります。

### ■ [PR #178](https://github.com/digitaldemocracy2030/website/pull/178)  
「update weekly summary(week27-35)」  
作成者: shingo-ohki  
過去の週報を大幅に更新・追加するPull Requestです。+2116行もの更新があり、week27からweek35まで一気に補完されました。shingo-ohkiさんの貢献により、大きく遅れていた履歴が整い、サイト利用者も過去の状況をきちんと把握できるようになりました。

### ■ [PR #175](https://github.com/digitaldemocracy2030/website/pull/175)  
「feat: Google Tag Managerを追加し、依存関係を更新」  
作成者: moai-redcap  
[Issue #174](https://github.com/digitaldemocracy2030/website/issues/174) の要望を受けて、Google Tag Managerが導入されました。依存関係が更新され、サイト上のアクセス解析やリリース管理がしやすくなっています。ユーザからは見えにくい変更ですが、開発・運営面ではとても重要なアップデートです。

---

## 進行中 (未完了) のタスクと議論

### ■ [Issue #177](https://github.com/digitaldemocracy2030/website/issues/177)  
「今後の更新を可能な限り自動化する」  
作成者: shingo-ohki  
週次更新などの手動作業を減らして継続的に開発を進められるよう、より高度な自動化を検討しています。今後、GitHub Actionsやbot活用などをどう組み合わせるか、みなさんのアイデアを歓迎しています。

### ■ [Issue #174](https://github.com/digitaldemocracy2030/website/issues/174)  
「Google Analytics を導入してアクセス解析をできるようにする」  
作成者: shingo-ohki  
すでに[PR #175](https://github.com/digitaldemocracy2030/website/pull/175)でGoogle Tag Managerが導入されたことで一歩進んでいますが、本格的なアクセス解析の議論は続いています。Slackの #2_広報_pr チャンネルでも「どれくらいページが見られているかを知りたい」といった話題が出ており、アクセス解析を充実させる方法を模索中です。

### ■ [Issue #173](https://github.com/digitaldemocracy2030/website/issues/173)  
「毎週のプロジェクトの活動状況の更新処理が適切に動いていない」  
作成者: shingo-ohki  
自動更新のフローが途中で止まってしまい、手動のステップが必要だった問題をどう解決するかが議論されています。現行のGitHub Actionsの設定や、Pull Requestの運用方針を見直す場となっていますので、運用改善のアイデアをぜひ共有ください。

### ■ [PR #171](https://github.com/digitaldemocracy2030/website/pull/171)  
「Week27 Summary Update」  
作成者: github-actions[bot]  
自動生成された週次サマリのアップデートです。すでに同様の更新が[PR #178](https://github.com/digitaldemocracy2030/website/pull/178)でマージされていますが、こちらも廃案にするのかマージするのかなど、どう扱うか議論が必要です。GitHub Actions + 人的確認の流れを整備する上でも重要なケースになっています。

---

## おわりに

今週は遅れていた週報更新がまとめて完了したほか、新機能としてGoogle Tag Managerの導入など、サイトの改善が着実に進みました。並行して自動化や週報更新の課題が引き続き議論されています。  
もし興味を持ったら、IssueやPull Requestにコメントを残してみたり、実装に挑戦してみたりしてくださるととても嬉しいです。みなさんの多様な視点で、よりよいデジタル民主主義WEBを一緒に育てていきましょう！