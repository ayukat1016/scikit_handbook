# scikit-learnデータ分析　実装ハンドブック

![scikit](https://user-images.githubusercontent.com/40778791/108866924-0475b080-7638-11eb-8ea4-4a14f9e24eb5.PNG)

書籍「[scikit-learnデータ分析ハンドブック](https://www.amazon.co.jp/scikit-learn-%E3%83%87%E3%83%BC%E3%82%BF%E5%88%86%E6%9E%90-%E5%AE%9F%E8%B7%B5%E3%83%8F%E3%83%B3%E3%83%89%E3%83%96%E3%83%83%E3%82%AF-Python%E3%83%A9%E3%82%A4%E3%83%96%E3%83%A9%E3%83%AA%E5%AE%9A%E7%95%AA%E3%82%BB%E3%83%AC%E3%82%AF%E3%82%B7%E3%83%A7%E3%83%B3-%E6%AF%9B%E5%88%A9/dp/4798055425)」のサポートサイトです。本書籍で使用するサンプルコードがまとめてあります。

## 章の構成
- 第1章：機械学習とは何か 
- 第2章：scikit-learnと開発環境  
- 第3章：回帰   
- 第4章：分類    
- 第5章：クラスタリング    
- 第6章：次元削減   
- 第7章：モデルの評価    
- 第8章：Preprocessing、実データ分析
- 第9章：scikit-learn API

## 正誤表
| ページ | 誤 | 正 | 補足 |
|:-----------|:------------|:------------|:------------|
| 3章 p81：モデルからのパラメータの取り出しの直前 | 記載漏れ | パラメータから住宅価格の上昇下落に影響がある特徴量がわかります。2.573のRMは上昇。|  |
| 3章 p130：MSE trainの数値 | 11.724 | 11.72 |  |
| 4章 p186：y=0のヒンジ損失関数| -1+θx | 1+θx |  |
| 7章 p290：分類評価方法の表の左上| （FalseNegative） | （True Negative） |  |
| 7章 p290：分類評価方法の表の左下| （FalseNegative） | （False Negative） |  |
| 8章 p353：ソースコードの6行目 | x_pos =　df['POSIX'].reshape(-1,1) | x_pos =　x_pos.reshape(-1,1)またはx_pos =　df['POSIX'].values.reshape(-1,1) |  |
| 8章 p420：ソースコードの1行目 |sumweight = (normratings*user_corr_top5).sum(axis = 1)| sumweight = ((normratings.notnull())*user_corr_top5.abs()).sum(axis = 1) |  |
| 8章 p420：ソースコードの5行目 | predict.sort_values(ascending = False) | predict.sort_values(ascending = False).head() |  |

## ライブラリのバージョン
- matplotlib:3.1.2
- numpy:1.17.4
- pandas:0.25.3
- sklearn:0.21.3
- mlxtend:0.14.0

## 問い合わせ
本書のお問い合わせ、ご要望、記載の誤植があれば以下メールアドレスにお問い合わせください。
ayukat101699@yahoo.co.jp
