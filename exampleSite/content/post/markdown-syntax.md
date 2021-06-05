+++
title = "Markdown の書き方"
date = "2019-03-11"
description = "基本的な Markdown の文法の紹介です。"
tags = ["markdown","css","html"]
+++

基本的な Markdown の文法の紹介です。
<!--more-->

## 見出し

HTML の `<h1>`—`<h6>`

# H1
## H2
### H3
#### H4
##### H5
###### H6

## 段落

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

空行を開けずに改行したい場合は行末に半角スペースを二つ付けます。  
このように改行できます。

## 引用

#### 帰属表示なし

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use *Markdown syntax* within a blockquote.

#### 帰属表示あり

> Don't communicate by sharing memory, share memory by communicating.  
> — Rob Pike[^1]

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## 表

   Name | Age
--------|------
    Bob | 27
  Alice | 23

#### 表の中で Markdown 使用

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

## コードブロック

#### backticks によるコードブロック

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

#### 半角スペース 4 つによるコードブロック

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### Hugo のハイライトショートコード使用によるコードブロック
{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## リスト

#### 番号付きリスト

1. First item
2. Second item
3. Third item

#### 番号なしリスト

* List item
* Another item
* And another item

#### 子ありリスト

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese

## その他の生の HTML — abbr, sub, sup, kbd, mark
**注：** 以下のような生の HTML を表示したい場合は config.toml に

```
[markup.goldmark.renderer]
unsafe= true
```

と記載してください。デフォルトでは正しく表示されません。

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.
