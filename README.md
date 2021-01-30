# Introduction

## RubyGem 環境の用意

jekyllrb-jp GitHub Page を参照して、Ruby 環境をセットアップする。

http://jekyllrb-ja.github.io/docs/installation/

## Jekyll と bundle のインストール

```ruby
gem install jekyll bundler
```

## 静的サイトの生成

リポジトリを clone し、ソースをローカル環境に用意する。
以下のコマンドにより、ソースをビルドして静的サイトを生成する。
```
bundle exec jekyll serve
```
ローカルサーバ上 `http://localhost:4000` にて、生成されたサイトを確認する。  
Markdown等ファイルを編集しながら、反映のされ方を確認し進めることができる。
サイトの設定ファイル `_config.yml` の内容を変更したときには、実行し直す必要があるため注意する。

### (補足)

- サーバにアップロード用のファイルを生成するだけの場合は、以下の実行コマンドを使用する。
```
bundle exec jekyll build
```
- 先頭の `bundle exec`をつけることにより、 `Gemfile` で定義された Jekyll のバージョンをビルドに指定することができる。

## 記事の投稿

Markdownで記載した記事は、`_posts` フォルダ内に格納する。Front Matter の記載方法に注意する。

[→Learn More](https://iihito-kyokai.github.io/sample/introduction/2021/01/07/sample.html)

## Reference

- jekellrb-ja GitHub Pages [→Link](https://jekyllrb-ja.github.io/)
これを見れば安心。Jekyll 環境のセットアップ方法や、Jekyll 特有のコンテンツの使い方等が記載されている。

- mk-mode.com?[→Link](https://www.mk-mode.com/blog/2019/01/27/jekyll-with-minimal-mistakes/)  
Jekyll テーマ `Minimal Mistakes` のサイト設定に関して、詳細に解説されている。
