# SWE-agent テスト

## セットアップ

`setup.sh`を実行し、秘密鍵設定ファイルの生成をする。もしOSの関係でファイルに改行文字が残った場合、手動で削除し`keys.cfg`となるようにする。

また、```docker pull sweagent/swe-agent:latest```を実行し、docker imageを取得する。

## LLMのAPIキーを設定する

今回はGPT4を使う前提で話を進める。```OPENAI_API_KEY: '<your-api-key>'```を実際のAPIキーに置き換える。なお、キーは[ポータル](https://platform.openai.com/api-keys)から発行できる。
また、呼び出しに必要なクレジットを追加しておくこと。

## エージェントを実行

- マシン上でDockerを起動し、```docker compose up```でプログラムを実行する。
- 出力はoutput/output.txtに吐き出されます。
