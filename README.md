# ku2022_1

locファイル<br>
ポーズグラフ最適化前のロボット位置を記録している．
locoptファイル
ポーズグラフ最適化後のロボット位置を記録している．
1列目 : 走行開始からのカウント数
2列目 : 走行開始からの時間 [ms]
3列目 : 位置 X座標 [m]
4列目 : 位置 Y座標 [m]
5列目 : 位置 Z座標 [m] (2D SLAMなので常に0)
6列目 : 姿勢 ロール [rad] (2D SLAMなので常に0)
7列目 : 姿勢 ピッチ [rad] (2D SLAMなので常に0)
8列目 : 姿勢 ヨー [rad]


proxファイル
各ロボット位置から観測された近接点のロボット座標位置を記録している．
1列目 : 走行開始からのカウント数
2列目 : 走行開始からの時間 [ms]
3列目 : 近接点数
4列目以降は各近接点について次のことを記録している
4列目 : 近接点ID
5列目 : この近接点が記録され続けているカウント数
6列目 : 近接点が属する物体の移動速度
7列目 : 方位角 [rad]
8列目 : 仰俯角 [rad]
9列目 : 距離 [m]


absproxファイル
ポーズグラフ最適化前のワールド座標系での近接点の位置を記録している．
absproxoptファイル
ポーズグラフ最適化後のワールド座標系での近接点の位置を記録している．
1列目 : 走行開始からのカウント数
2列目 : 走行開始からの時間 [ms]
3列目 : 位置 X座標 [m]
4列目 : 位置 Y座標 [m]
5列目 : 位置 Z座標 [m]


matchファイル
ループ検出の結果を記録している．
1列目 : ループが結ばれたノードAの近接点観測時系列データID (1つの近接点観測時系列データのみを用いる場合は常に1)
2列目 : ループが結ばれたノードAのカウント数
3列目 : ループが結ばれたノードAの時間 [ms]
4列目 : ループが結ばれたノードBの近接点観測時系列データID (1つの近接点観測時系列データのみを用いる場合は常に1)
5列目 : ループが結ばれたノードBのカウント数
6列目 : ループが結ばれたノードBの時間 [ms]
7列目 : ループ区間ID
8列目 : ループ区間に含まれるループの数
9列目 : ループ区間の類似度スコア
10列目: 順ループ区間か逆ループ区間か 0:false, 1:true
11列目以降はループの近接点対について記録している
