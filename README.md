# airbus_ship_challenge_code_latest

現状の進め方
アブレーションによって、精度を比較し、少しずつアップデートしていく。

現状Lossについて
BCE + Tversky(Recall:Precision = 4:6)が一番精度が高い。

HistGradientBoostingについては、閾値が0になってしまった。
→detectorモデルを作成し、船あり、船なしのモデルを作成。それと並行して、segmentationの学習データの比率を見て精度、閾値を見てみる。

それがうまくいったら、treeで再度実行したい。
