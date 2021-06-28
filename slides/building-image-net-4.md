---
preload: false
clicks: 2
class: relative
---

# ImageNet の構築 - WordNet の出現

<br />

[WordNet](https://wordnet.princeton.edu/)とは単語の関係をグラフとして解釈するためのデータベースです。

<div v-if="$slidev.nav.clicks < 1" v-click-hide>

例: 「ゴールデンレトリバー」

```mermaid
graph LR
  ゴールデンレトリバー --> 犬
  犬 --> 哺乳類
  哺乳類 --> 脊椎動物
  脊椎動物 --> 動物
  動物 --> 生物
```

</div>

<div v-if="$slidev.nav.clicks == 1">

例: 「ゴールデンレトリバー」とその周辺

```mermaid
graph LR
  ゴールデンレトリバー --> 犬
  チワワ --> 犬
  犬 --> 哺乳類
  猫 --> 哺乳類
  哺乳類 --> 脊椎動物
  脊椎動物 --> 動物
  動物 --> 生物
  ヒマワリ --> 生物
```

</div>

<div v-click="2">

例: 「ゴールデンレトリバー」と「猫」を WordNet を使って比較

```mermaid
graph LR
  ゴールデンレトリバー --> 犬
  チワワ --> 犬
  犬 --> 哺乳類
  猫 --> 哺乳類
  哺乳類 --> 脊椎動物
  脊椎動物 --> 動物
  動物 --> 生物
  ヒマワリ --> 生物
```

<arrow x1="100" y1="300" x2="150" y2="270" width="2" arrowSize="1" />

<div class="absolute top-76 left-10 w-30">
<img src="/images/golden_retriever_1.png" />
<img src="/images/golden_retriever_2.jpeg" />
<img src="/images/golden_retriever_3.png" />
</div>
  
<arrow x1="300" y1="480" x2="310" y2="400" width="2" arrowSize="1" />

<div class="absolute top-115 left-60 w-30 flex">
<img src="/images/cat_1.jpeg" class="w-30" />
<img src="/images/cat_2.jpeg" class="w-30" />
<img src="/images/cat_3.jpeg" class="w-30" />
</div>

<Circle x="413" y="333" r="45" width="2" color="red" />

<arrow x1="475" y1="255" x2="430" y2="290" width="2" arrowSize="1" />

<div class="absolute top-60 left-120 w-30 flex">
ここまで同じ
</div>

</div>

<!--

-->
