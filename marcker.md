# マーカーの作成

では，早速マーカーを作っていきましょう．

トップページ上部の`TargetManager`をクリックしてください．

![alt text][vss4]
[vss4]:https://dl.dropboxusercontent.com/u/25806407/images/toTargets.png

画面が変わったら，`Create Database`をクリックして，マーカーを保存するためのフォルダを作ります．

![alt text][vss5]
[vss5]:https://dl.dropboxusercontent.com/u/25806407/images/Target_Manager___Vuforia_Developer_Portal.png

![alt text][vss6]
[vss6]:https://dl.dropboxusercontent.com/u/25806407/images/createdatabase.png

フォルダを作ることができたら，フォルダをダブルクリックしてフォルダの中に入りましょう．

ここで`Add Target`ボタンをクリックします．

![alt text][vss7]
[vss7]:https://dl.dropboxusercontent.com/u/25806407/images/makemarcker.png

ここでマーカーとして利用する画像の情報を入力します．

上から
・マーカーの名前（自由につけて構いません）
・マーカーの形(※)
・画像の幅
・実際の画像をアップロード

となっています．

※マーカーの形というのは，認識するマーカーの形がどういった形であるかという質問です．立方体型，円柱・円錐型に対応していますが，今回は画像1枚で利用でき，最もシンプルなタイプであるSingle Imageタイプのマーカーを使用します．

Addボタンを押すと，アップロードした画像に特徴点を付ける作業が始まります．

特徴点生成には2〜3分ほど時間がかかるので，待って下さい．

このような画面が出てくれば画像生成終了です．

![alt text][vss8]
[vss8]:https://dl.dropboxusercontent.com/u/25806407/images/makeImage.png

自分でマーカーを作る時は，右側の☆の数が**最低でも3つ以上の☆が付くような画像**をマーカーにするようにしてください．

☆が余りにも少ないと，ARコンテンツを正しく表示できない場合があります．

これでARマーカーを作ることが出来ました．

次はUnityで使えるような形で画像をダウンロードしましょう．

![alt text][vss9]
[vss9]:https://dl.dropboxusercontent.com/u/25806407/images/download.png

![alt text][vss10]
[vss10]:https://dl.dropboxusercontent.com/u/25806407/images/download2.png

Createボタンをクリックすると，画像と必要なデータのダウンロードが始まります．

Vuforia上で作業をするのはここまでです．

マーカーの作り方はとても重要ですので，覚えておいて下さい．
