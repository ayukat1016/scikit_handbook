# scikit-learnデータ分析　実装ハンドブック

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
