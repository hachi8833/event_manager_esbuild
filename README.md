# README

以下のチュートリアルを進めるのに便利なDocker環境です。

* [Rails 7とReactによるCRUDアプリ作成チュートリアル（翻訳）｜TechRacho by BPS株式会社](https://techracho.bpsinc.jp/?p=118031&preview=true#4-1)

## 必要なもの

以下のインストールが必要です。ホストOS環境はmacOSで検証していますが、Linux、Windows（WSL2）でも動くと思います。

* DockerとDocker Compose環境
* dip↓

[![bibendi/dip - GitHub](https://gh-card.dev/repos/bibendi/dip.svg)](https://github.com/bibendi/dip)


```sh
# dipをインストールする
gem install dip
```

## セットアップ

以下を実行すればセットアップが完了します。Gemfileを上書きするかどうか尋ねられたらyを入力してください（READMEの上書きはどちらでも構いません）。

```sh
dip provision
```

チュートリアルの[esbuildの場合](https://techracho.bpsinc.jp/?p=118031&preview=true#4-1)のpackage.jsonのカスタマイズ部分からチュートリアルを開始できます。

以下を実行すればRailsサーバーが起動します。

```sh
dip dev
```

チュートリアルの以後の操作では、`rails`や`npm`コマンドの冒頭に`dip`を付けるだけで同様に進められます（`touch`や`mkdir`などのシェルコマンドについては`dip`は不要です）。

```sh
# 例
dip npm i prop-types
```
