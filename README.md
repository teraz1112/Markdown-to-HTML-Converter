# Markdown-to-HTML-Converter

## 概要
MarkdownをHTMLへ変換できるスクリプト

## デモ
![output](https://github.com/Aki158/Markdown-to-HTML-Converter/assets/119317071/128c78e8-07e3-481f-aaf4-d4db42557db1)

## 説明
このスクリプトは、コマンド入力を利用してMarkdownをHTMLへ変換できるスクリプトです。

Markdownは、簡単な記法を使って書式付きの文書を作成することができます。

Webエンジニアやwebデザイナーなどのコンテンツクリエーターは、Markdownで文書を作成することがあります。

MarkdownとHTMLそれぞれのファイルのイメージは、下記リンクから確認することができます。
- [Markdown](https://github.com/Aki158/Markdown-to-HTML-Converter/blob/main/sample.md)
- [HTML](https://github.com/Aki158/Markdown-to-HTML-Converter/blob/main/index.html)


## インストール

1. リポジトリをクローンする
```
git clone https://github.com/Aki158/Markdown-to-HTML-Converter.git
```

2. クローンしたリポジトリへ移動する
```
cd Markdown-to-HTML-Converter
```

## 開発環境の構築

開発環境を Docker を使用して立ち上げることが可能。以下、その手順。

1. 上記**インストール**を行う

2. Docker ビルド
   　以下を実行してビルド。なお、以下は Docker がインストール済みであることを前提とする

```
docker compose build
```

3. Docker 立ち上げ
   　以下を実行してコンテナを立ち上げ。

```
docker compose up -d
```

## 使用方法
1. Markdownファイル(.md)を用意する
2. スクリプトを実行する
3. 生成されたファイル(.html)を確認する

#### コマンドの入力使用例
```
python3 file-converter.py markdown ../python_practice/sample.md ../python_practice/index.html
```

## 使用技術
<table>
<tr>
  <th>カテゴリ</th>
  <th>技術スタック</th>
</tr>
<tr>
  <td>開発言語</td>
  <td>Python</td>
</tr>
<tr>
  <td rowspan=2>インフラ</td>
  <td>Ubuntu</td>
</tr>
<tr>
  <td>Docker</td>
</tr>
<tr>
  <td rowspan=2>その他</td>
  <td>Git</td>
</tr>
<tr>
  <td>Github</td>
</tr>
</table>

## 機能一覧
![image](https://github.com/Aki158/Markdown-to-HTML-Converter/assets/119317071/e38f9ff0-4e14-4f40-92e3-736bed508215)

| 機能 | 内容 |
| ------- | ------- |
| markdown | markdownをhtmlに変換します。 |
| エラーハンドリング | コマンドが正しく入力されていない場合は、下記のようなメッセージが表示されて終了します。<br>・inputpathが存在しない場合:`Inputfile does not exist...`<br>・入力されるコマンドが4つではない場合:<br>　`　Wrong usage!`<br>　`useage : python3 file-converter.py markdown inputfile outputfile`<br>入力されたコマンドが、markdownでない場合:`Command not found...` |

### 補足
#### 用語集
[説明](#説明)で登場する用語について補足します。

用語の意味がわからない時は、下記表を確認してください。

| 用語 | 意味 |
| ------- | ------- |
| Markdown | 簡単な記法で読みやすく、HTMLなどの他の形式に変換できることを目的としたテキストベースの軽量マークアップ言語です。 |
| HTML | Webページを作成するための標準的なマークアップ言語です。<br>テキスト、画像、リンク、フォームなどのWebコンテンツをブラウザに表示する際に必要となる指示を提供しています。 |
| スクリプト | 一連のコマンドや命令を記述したテキストファイルのことで、コンピュータに特定のタスクを自動的に実行させるために使用されます。<br>スクリプトは、特定のスクリプト言語（例：Bash、Python、Perl、Ruby、JavaScriptなど）で書かれます。<br>今回は、Pythonを使用してスクリプトを作成しています。 |
| ターミナル | コンピュータに対してテキストベースのコマンド入力と出力を行うインターフェースのことです。<br>このインターフェースは、コマンドラインインターフェース（CLI）とも呼ばれます。<br>[デモ](#デモ)の途中に登場する黒い画面のことです。 |
| コマンド | コンピュータに対して特定の操作を実行するよう指示するテキストベースの命令です。<br>コマンドを入力することで、コンピュータは、コマンドの意味を読み取りアクションをおこします。 |

## 参考文献
### 公式ドキュメント
- [Python](https://docs.python.org/ja/3/)

### 参考にしたサイト
- [Python_Download](https://www.python.org/downloads/)
- [pipのインストールガイド](https://pip.pypa.io/en/stable/installation/)
- [markdownのプロジェクトの説明](https://pypi.org/project/Markdown/)
- [Markdown記法一覧](https://qiita.com/oreo/items/82183bfbaac69971917f#:~:text=Markdown%EF%BC%88%E3%83%9E%E3%83%BC%E3%82%AF%E3%83%80%E3%82%A6%E3%83%B3%EF%BC%89%E3%81%AF%E3%80%81,%E3%82%82%E9%96%8B%E7%99%BA%E3%81%95%E3%82%8C%E3%81%A6%E3%81%84%E3%82%8B%E3%80%82)
- [HTML の基本](https://developer.mozilla.org/ja/docs/Learn/Getting_started_with_the_web/HTML_basics)
