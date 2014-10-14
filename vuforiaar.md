# ARで表示できるようにする

次に，この踊るミクをARで表示できるようにしていきましょう．

あと一息です．頑張っていきましょう！

Asset＞Qualcomm Reality＞Prefabsの中にある

* ARCamera
* ImageTarget

というファイルを，Hierarchyフォルダに追加して下さい．

![alt text][u20]
[u20]:https://dl.dropboxusercontent.com/u/25806407/images/U21.png

※初音ミクのモデルが白い板に埋まってしまっている人は，Hierarchyタブで初音ミクのモデルを選択し，緑の矢印をドラッグして板の上に乗るように調整して下さい．

`ImageTarget`は，どういった画像をマーカーとして使うか，その画像を認識した時どのようなコンテンツを表示するかをまとめて指定できるプログラムです．

`ARCamera`は，ImageTargetで指定した画像を見つけ出すためのプログラムです．

### ImageTargetの設定

私達が作りたいものは，

* 初音ミクの画像を読み込んだら
* 初音ミクにダンスを踊ってもらう

アプリです．初音ミクの画像と，初音ミクのモデルデータをImageTargetに設定しましょう．

#### 画像の設定

HierarchyタブでImageTargetを選択し，Inspectorタブの中のImageTarget Behaviors内，Datasetオプションを自分で作ったマーカーの名前に変更する．(例ではAutumnAR)

![alt text][u21]
[u21]:https://dl.dropboxusercontent.com/u/25806407/images/U23.png

![alt text][u22]
[u22]:https://dl.dropboxusercontent.com/u/25806407/images/U24.png

これで画像の設定は終了です．

#### コンテンツの設定

Hierarchyタブの初音ミクのモデルデータを，ImageTargetにドラッグ・アンド・ドロップします．

![alt text][u23]
[u23]:https://dl.dropboxusercontent.com/u/25806407/images/U22.png

このままでは，ミクが小さすぎて全くみえないので，大きさを調整します．

モデルデータを選択した状態でInspectorタブの中で，Transformオプションの中のScaleをXYZ共に0.5に設定しましょう．

![alt text][u24]
[u24]:https://dl.dropboxusercontent.com/u/25806407/images/U25.png

これでモデルの設定は終了です．

ね？簡単でしょ？

最後にHierarchyからMain Cameraを削除し，ARCameraの位置を調整して，終了です．


![alt text][u25]
[u25]:https://dl.dropboxusercontent.com/u/25806407/images/U26.png

※Unityをインストールして30日間は，UnityPro(有料版，13万程度)の機能を使用することが出来ます．

この30日間の間であれば，PCのインカメラを使用してARの挙動を確認することが出来ますので，試してみてください．
