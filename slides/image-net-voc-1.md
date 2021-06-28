# ImageNet 競技会 - NN よりも SVM

<br/>

2010 年、ImageNet プロジェクトは[ILSVRC(ImageNet 広範囲を対象とした視覚認識競技会)](https://image-net.org/challenges/LSVRC/)を開催した。

ILSVRC では訓練画像の数が約 120 万枚で、カテゴリー候補が 1000 個と、PASCAL と比べて非常に大きなデータセットとなっている。

また、画像のラベルの予測には「トップ５正解率」が用いられた。

Ranking by learning methods(2010 年度の結果)

- Descriptor Coding + SVM, 0.28 --- NEC-UIUC
- Fisher kernel + SVM, 0.34 --- XRCE
- LI2C, 0.58 --- NTU_WZX
- KNN, 0.61 --- LIG
- Canonical Correlation Analysis, 0.79 -- NII

\* number indicates flat cost with 5 predictions

https://image-net.org/static_files/files/pascal_ilsvrc.pdf

<!--
トップ５正解率

競技会に参加しているプログラムは各画像について五つのカテゴリーを答えることができる。そのなかのひとつが正しければ、プログラムはその画像で正解したとみなされる。
-->
