# ImageNet 競技会 - チートをしてでも

<br/>

2015 年に百度のチーム、「データスヌーピング（データののぞき見）」と呼ばれる _ズル_ を行った。

<div class="grid grid-cols-2">
<div class="w-min mx-auto">

一般的な流れ

```mermaid
graph TD
    A[モデルの作成] --> B[予測]
    B -- 週に2回まで --> C[予測結果を確認]
    C -- 結果を元に改善 --> A
```

</div>
<div>

百度のチーム

<div class="grid grid-cols-2">
<div>

```mermaid
graph TD
    A[モデルの作成] --> B[予測]
    A --> B
    A --> B
    A --> B
    B --> C[予測結果を確認]
    B --> C
    B --> C
    B --> C
    C --> A
    C --> A
    C --> A
    C --> A
```

</div>
<div>

何度もテストの結果を得ることで、テストデータに適合したモデルを作成可能に

</div></div></div></div>

<!--

ImageNet 競技会での優勝が単なる研究的な側面だけではなく、企業にとっての営利活動としての側面を持ちはじめたころに事件はおきました。

ズルをしてしまった理由は、相手よりも優れたプログラムを開発しなければならないという重圧によるものだった。

もちろん、テストデータを使った学習は説明するまでもなくしてはならない行為だ。

当たり前だが、この大会では百度のチームは失格となることとなった。

また、優勝チームのトップ５正答率は95％を超えており、他のチームもかなり高い結果を出している。
-->