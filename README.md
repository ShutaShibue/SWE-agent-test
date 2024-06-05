# SWE-agent テスト

## Docker hubからイメージをダウンロード

```docker pull sweagent/swe-agent:latest```

## LLMのAPIキーを設定する

プロジェクトのルートディレクトリに```keys.cfg```を作成する。
今回はGPT4を使う前提で話を進める。```OPENAI_API_KEY: '<your-api-key>'```を書き込む。なお、キーは[ポータル](https://platform.openai.com/api-keys)から発行できる。\\
また、呼び出しに必要なクレジットを追加しておくこと。

## エージェントを実行

```run.sh```には使用するモデル、ターゲットとなるissueのリンク等が記載されているため、必要に応じて変更する。
```source run.sh```で実行する。

出力はoutput.txtに吐き出されます。
