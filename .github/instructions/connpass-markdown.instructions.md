---
description: connpass向けMarkdownガイド（.mdファイル用）
applyTo: "**/*.md"
---

# connpass イベントページ用Markdownガイド

本文は connpass が対応している Markdown 記法に合わせて記述してください。対応範囲は公式ヘルプ
https://help.connpass.com/organizers/markdown
の内容に従います。

## connpassで使えるMarkdown（要点）

### 段落
- 1行以上の空行で段落を分けます。

### 見出し
- `#`〜`######` による見出し（H1〜H6）

### 文字装飾
- イタリック: `*text*` または `_text_`
- 太字: `**text**` または `__text__`
- 打ち消し線: `~~text~~`

### リンク
- インラインリンク（titleあり）: `[text](http://example.com/ "title")`
- インラインリンク（titleなし）: `[text](http://example.com/)`
- URL単体は自動リンク（例: `http://example.com`）

### リスト
- 番号なし: `*` / `+` / `-`
- 番号あり: `1.` のように `数字.`

### 引用
- 行頭 `>`

### コード
- 文中コード: バッククオート `` `code` ``
- 複数行コード: 3連バッククオート（フェンス）
	- 言語指定例: ` ```python `

### 水平線
- `-` / `*` / `_` を3文字以上（例: `***`, `- - -`）

### テーブル
- `|` と `:` によるテーブル記法（左/中央/右寄せ指定）

### 画像
- `![alt](https://...)`
- `![alt](https://... "title")`
- 画像サイズを変えたい場合は HTML の `img` タグを使用します（例: `<img src="..." width="500">`）

## HTML（許可タグ/属性）

connpassでは一部のHTMLタグ/属性のみ利用できます。それ以外のタグや属性は除去されます。

- `b`: `style`, `align`
- `blockquote`: `style`
- `em`: `style`, `align`
- `strong`: `style`, `align`
- `strike`: `style`, `align`
- `del`: （属性なし）
- `a`: `href`, `title`, `rel`
- `i`: `style`, `align`
- `br`: （属性なし）
- `ul`: （属性なし）
- `ol`: （属性なし）
- `li`: （属性なし）
- `u`: （属性なし）
- `pre`: （属性なし）
- `code`: （属性なし）
- `p`: `style`, `align`
- `h1`〜`h6`: `style`
- `hr`: `style`
- `span`: `style`
- `div`: `style`, `align`
- `font`: `size`, `style`, `color`
- `table`: `style`, `border`
- `thead`: （属性なし）
- `tbody`: （属性なし）
- `tfoot`: （属性なし）
- `th`: `align`, `style`, `colspan`, `rowspan`
- `td`: `align`, `style`, `colspan`, `rowspan`
- `tr`: `style`
- `img`: `src`, `alt`, `title`, `width`, `height`, `style`