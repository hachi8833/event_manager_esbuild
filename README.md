# README


```sh
# Docker環境セットアップ
dip bundle install
```

```sh
# Railsバージョン確認
dip rails -v
```

```sh
# esbuildの場合
dip rails new . -j esbuild
```

以後の操作も、コマンド冒頭に`dip`を付ける点だけが異なります。

```sh
# 例
dip bundle add shakapacker --strict
```

なお、`yarn`は既にセットアップに含まれているので、以下は実行不要です。

```sh
# 実行不要
npm i -g yarn
```
