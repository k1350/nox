+++
title = "数式表示"
date = "2021-06-02"
description = "Katex による数式表示について"
series = ["Feature"]
math = true
+++
Katex による数式表示についての説明です。
<!--more-->
Katex による数式表示は JavaScript を使用するので、通常は余計なファイル読み込みを防ぐために機能をオフにしてあります。  
数式を表示したい場合、その記事の front matter で "math = true" を指定してください。  
その記事内でのみ数式を表示できるようになります。

**注:** 数式自体の書き方は Katex の公式サイトを見てください。 [Supported TeX Functions](https://katex.org/docs/supported.html)

### 使用例

{{< math.inline >}}
Inline math: \(\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…\)
{{</ math.inline >}}

Block math:
$$
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } 
$$
