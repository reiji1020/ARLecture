# 素材の導入

1.ARマーカーとVuforiaをUnityに導入する

![alt text][u0]
[u0]:https://dl.dropboxusercontent.com/u/25806407/images/U0.png

`Asset>Import Package>Custum Package...`をクリックし，ファイルを追加してきます．
追加するファイルは以下の2つです．

* (AutumnAR).unitypackage : ARマーカーファイル
* vuforia-unity-android-ios-3-x-x.unitypackage : SDKパッケージ

2つのパッケージを追加すると，ファイル構成は以下のようになります．

![alt text][u1]
[u1]:https://dl.dropboxusercontent.com/u/25806407/images/U1.png

2.初音ミクのモデルと音楽データをUnityに導入する

モデルや音楽のデータを入れておくファイルを作りましょう．

Projectタブ内のAssetsフォルダの上で右クリックをして，Create->Folderをクリックし，**Resources**という名前のフォルダを作成して下さい．

![alt text][u2]
[u2]:https://dl.dropboxusercontent.com/u/25806407/images/U2.png

フォルダができたら，Resourcesフォルダの中にドラッグアンドドロップでモデルデータ，音楽データを入れて下さい．

![alt text][u3]
[u3]:https://dl.dropboxusercontent.com/u/25806407/images/U4.png

**音楽データについての注意**

デフォルトでは音楽データの3D Soundというオプションにチェックがついています．

ここにチェックが入っていると**きちんと音楽が鳴らないのでチェックを外して下さい．**

![alt text][u4]
[u4]:https://dl.dropboxusercontent.com/u/25806407/images/U5.png

チェックを外したら，`Apply`ボタンを押してください．

3.MMD4Mecanimを導入する

先ほどダウンロードしたMMD4Mecanimのファイルに，

`MMD4Mecanim.unitypackage`というファイルがあります．

これを1と同じ手順でUnityに読み込ませて下さい．

以上で素材の導入は終了です．
