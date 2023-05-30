---
sidebar_position: 6
sidebar_label: プラグインレビュー
---

# プラグインのレビュープロセス

私たちはプラグイン ストアの構築の初期段階にあります。このページでは、プラグイン レビュー プロセスについて私たちがどのように考えているか、そしてプラグイン レビュー プロセスがどのようになるかについての基本的な概要を説明します。

> プラグインのレビュープロセスは時間の経過とともに大きく変化します。プラグインを構築するプロセスを改善する方法についてのフィードバックをお待ちしています。

## 優れたプラグインとは何か

レビュー プロセスの目的は、ChatGPT のプラグインが安全であることを確認し、便利な機能を提供し、高品質のユーザー エクスペリエンスを提供することです。長期的には、正式に策定する際にレビュープロセスを経るのが日常的なことになると予想されます。

当面は、大規模な言語モデルの独自の機能がなければ不可能だった、新しい魔法のようなエクスペリエンスをユーザーに提供するプラグインが最大の価値を提供すると期待しています。

これまでのところ、最も魅力的なプラグインのカテゴリーは次のとおりです。

- ユーザー固有の知識ソース、または検索が困難な知識ソースの検索 (Slack での検索、ユーザーのドキュメントまたは別の独自データベースの検索)。
- 他のプラグインとうまく相乗するプラグイン (モデルに週末の計画を依頼し、モデルにフライト/ホテル検索とディナー予約検索の使用をブレンドさせます)。
- モデルに計算能力を与えるプラグイン (Wolfram、OpenAI コード インタープリターなど)。
- ゲームなど、ChatGPT の新しい使用方法を導入するプラグイン。

## プラグインの状態

プラグインを開発する場合、プラグインはいくつかのステータスのいずれかになり、レビュー プロセスのどの段階にあるか、誰が使用できるかを示します。現時点では、プラグインのステータスはいくつかのみです。プラグイン システムが進化するにつれて、これも変化すると予想されます。

| スターテス | 説明                                                         | 開発者アクセス | ユーザーのアクセス |
| :--------- | :----------------------------------------------------------- | :------------- | :----------------- |
| 未検証     | プラグインが開始されるデフォルトのステータス。               | 15             | 0                  |
| 承認済み   | OpenAI はプラグインを審査し、このプラグインが一般ユーザーによる使用を承認されていると判断しました。 | 無制限         | 無制限             |
| 禁止された | OpenAI はプラグインを審査し、プラグインを禁止する必要があると判断しました。 | 0              | 0                  |

プラグインを送信し、要件を満たしていないために拒否された場合でも、プラグインは「未検証」状態のままであることに注意してください。

## ユーザーの種類

現在、プラグインへのアクセスに関しては 3 つのカテゴリーのユーザーについて話しています。

| ユーザータイプ          | 説明                                                         |
| :---------------------- | :----------------------------------------------------------- |
| ChatGPT Plus ユーザー   | ChatGPT Plus ユーザーは、当社の審査プロセスを経て一般使用が承認されたプラグインへのアクセスが許可されています。 |
| プラグイン開発者        | ChatGPT Plus ユーザーには、開発中のプラグインを開発、使用、テストする権限が与えられています。 |
| 通常の ChatGPT ユーザー | 現時点では、プラグを持たない通常の ChatGPT ユーザーはプラグインにアクセスできません。 |

## プラグインストア

プラグインをプラグイン ストアで利用できるようにするには、OpenAI によるレビューが必要です。プラグインを審査のために送信する前に、プラグインが以下の基準を満たしていることを確認してください。

- 当社の[コンテンツポリシーを遵守します](https://openai.com/policies/usage-policies)
- 当社の[ブランドガイドラインに準拠しています](https://openai.com/brand)
- 提出物に記載されている機能
- 有益なエラーメッセージを提供します
- 特徴を説明する操作名
- シンプルで簡潔なマニフェスト ファイルを提供します
- 正しい文法を使用し、プラグインの説明を句読点で終了します。
- ユーザーの混乱を避けるために、プラグインの説明に地理的または機能的な制限を明確に記載します。
- プラグイン名や説明にプラグイン、ChatGPT、OpenAI などの単語を使用しないでください。

これらの基準のいずれかが欠けている場合、プラグインは拒否されますが、更新されたら再度送信できます。

## レビューのためにプラグインを送信

> レビューのために送信したプラグインについては、プラグインを送信してから 7 日以内に返信されることが予想されます。

現在、新しいプラグインを順次レビューしています。[プラグイン送信ボット](https://platform.openai.com/docs/plugins/review#)を使用して、プラグインをレビューのために送信できます。ボットを表示するには、サインインする必要があります。

プラグインの提出のステータスを表示するには、ログインしていることを確認し、このページの右上隅にある [ヘルプ] を選択してください。「メッセージ」の下に、プラグインの提出が表示されます。審査プロセス中にプラグインのステータスが変更されると、通知されます。