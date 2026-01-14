# 執筆方法
- 1: 日本語で書き、[intoc](https://github.com/stakiran/intoc) で目次を付ける
    - VSCode タスクから呼び出し可能。intoc は PATH を通す必要アリ
- 2: 英語に翻訳する
    - translator.py を VSCode タスクで呼び出して翻訳する
- 3: 英語部分の目次を intoc で反映し直す

## 翻訳の戦略
今のところ、2万文字超えの inedx.md を一発で翻訳させている。gpt-4.1-mini ならタイムアウト 3 分もあれば入るようだ。

一般的には 4.1-mini のような速度重視モデルで分割・並列実行させるみたい。

- 使えるモデル: [Limits - OpenAI API](https://platform.openai.com/settings/organization/limits)
