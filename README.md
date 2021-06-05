# Nox
Hugo のシンプルなダークテーマです。個人ブログ用途です。

**公式のレビューは受けておらず、[Hugo Themes](https://themes.gohugo.io/) には掲載されていません。不具合がある可能性があります。**

![tn](https://github.com/k1350/nox/blob/main/images/tn.png)![screenshot](https://github.com/k1350/nox/blob/main/images/screenshot.png)

## 主な特徴
- ダークテーマ
- レスポンシブ対応
- Katex による数式表示
- 絵文字
- OGP と Twitter カード
## 使い方
Git submodule としてください。Hugo のサイトのルートディレクトリ内で下記コマンドを打ちます。

```sh
git submodule add https://github.com/k1350/nox.git themes/nox
```

その他の情報は Hugo の [公式サイト](https://gohugo.io/getting-started/installing/) を見てください。
## 設定
色々複雑なので、まず exampleSite を動かしてみることをおすすめします。

exampleSite 内の記事にも幾らか情報を書いてあります。  

あと OGP と Twitter カードは Hugo の組み込みテンプレートを使っているので、Hugo 公式サイトの使い方説明を見てください。
- [Configure Open Graph](https://gohugo.io/templates/internal/#configure-open-graph)
- [Configure Twitter Cards](https://gohugo.io/templates/internal/#configure-twitter-cards)

### カスタマイズについて
詳しくは [Hugo's Lookup Order](https://gohugo.io/templates/lookup-order/) に書いてありますが、テーマそのものは弄らずに自由に内容を上書きすることができます。  
特に使用頻度が高そうな部分はカスタマイズしやすいようにしています。

テーマをカスタマイズするには、まずサイトのルートディレクトリに layouts というディレクトリを作成します。

`</head>` の直前に記述したいものがある場合、layouts/partials/head_custom.html というファイルを作成し、その中に書いてください。  

`</body>` の直前に記述したいものがある場合、layouts/partials/body_custom.html というファイルを作成し、その中に書いてください。
