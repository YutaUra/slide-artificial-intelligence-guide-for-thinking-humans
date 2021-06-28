---
preload: false
---

# ImageNet の構築 - PASCAL VOC

<br />

**「[PASCAL ビジュアルオブジェクトクラス競技会](http://host.robots.ox.ac.uk/pascal/VOC/index.html)」** は 2005 年から 2010 年まで開催され、年に一度行われる形式の競技会のなかで最も有名でした。

[2010 年度の大会](http://host.robots.ox.ac.uk/pascal/VOC/voc2010/index.html)では、（[Flickr](https://www.flickr.com/) からダウンロードされた）約<span class="inline-block px-1 text-yellow-500">15,000</span>枚の写真が使われた。

<img src="/images/pascal-example.png" class="w-[80%] mx-auto" />

<!--
PASCAL VOC: The PASCAL Visual Object Classes

そのすべてに、「人」「イヌ」「ウマ」「ヒツジ」「車」「自転車」「ソファー」「鉢植えの植物」といった 20 の物体カテゴリーに基づいたラベルが人間の手でつけられた。

「分類部門原注 3」

その画像内に前述の 20 のカテゴリーの物体が存在しているかどうかを、カテゴリーごとに判定した結果として出力できるコンピュータービジョンプログラムだ。

表示している画像は、認識が難しいとされていた、鉢植えの中の植物の画像
-->
