# typst_simple_doc_template

簡単な Typst ドキュメントのテンプレートと、シンプルな `maketitle` パッケージを含むリポジトリです。

## 概要
- このリポジトリは、Typst で文書を素早く作成するための最小限テンプレートを提供します。
- サンプル本体は `doc.typ` にあり、再利用可能なタイトル生成ロジックは `simple_maketitle/` に格納しています。

## 目次
- 構成ファイル: `doc.typ`
- パッケージ: `simple_maketitle/0.1.0/lib.typ` と `simple_maketitle/0.1.0/typst.toml`

- 定理環境: `@preview/theorion:0.6.0` を利用しています（`doc.typ` 内で `#import "@preview/theorion:0.6.0": *` として読み込んでいます）。

## 必要環境
- Typst がインストールされていること（公式インストール手順に従ってください）。

## 使い方
1. リポジトリをクローンまたはダウンロードします。
2. `doc.typ` を編集して内容をカスタマイズします。
3. Typst でコンパイルします。例:

```bash
typst compile doc.typ
```

上記コマンドにより PDF（または Typst のデフォルト出力）が生成されます。

## カスタマイズ
- `simple_maketitle` の中の `lib.typ` を編集すると、ドキュメントの表紙やメタ情報の出力を調整できます。
- 必要に応じて `doc.typ` にインポート/コピーして利用してください。

## 貢献
- 改善提案・バグ報告は Issues で受け付けます。簡単な修正であればプルリクエストも歓迎します。

## ライセンス
- 本プロジェクトは `LICENSE` に従います。

---
作成者: Eito-Kubota

## サードパーティ依存
- Theorion: `@preview/theorion:0.6.0` を利用しています（`doc.typ` 内で `#import "@preview/theorion:0.6.0": *` として読み込んでいます）。
	- リポジトリ: https://github.com/OrangeX4/typst-theorion
	- ライセンス: MIT License (https://github.com/OrangeX4/typst-theorion/blob/main/LICENSE)
	- 備考: 本リポジトリでは Theorion のソースコードを同梱していません。Theorion をコピーして同梱・再配布する場合は、Theorion 側の著作権表示とライセンス条項に従ってください。