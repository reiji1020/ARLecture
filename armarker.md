# ARマーカーを作ってみよう

なんだかんだで座学が長引いてしまった感じがありますが，これからは沢山手を動かしてもらいます！

ARマーカーを作ってみましょう．
同梱の画像を使用します．

この画像です．5分で作りました．

![alt text][armarker]
[armarker]:https://dl.dropboxusercontent.com/u/25806407/images/ARMarcker.png

画像をARマーカーとして使用するには，この画像に含まれる**特徴点と**呼ばれるデータを計算しなければなりません．

`特徴点`とは，画像中に含まれる**エッジ**(輪郭)や線の繋がる場所，点が集合する場所などのある種の特徴の事を指します．

この特徴点の配置をコンピューターはデータとして持っておき，類似した特徴点の配置をもつ画像を認識した時，ARコンテンツを表示するといった仕組みです．

では特徴量計算をしましょう．

といってもこの計算には便利なツールが存在しますので，そちらを利用します．

https://developer.vuforia.com/

上のURLをクリックしてサイトにアクセスしてください．

ARマーカーを作ったり，ARコンテンツを簡単に作成することができるツールに`Vuforia`というものがあります．

今回はこのVuforiaを活用して，ARマーカーを作っていきましょう．

![alt text][vss0]
[vss0]:https://dl.dropboxusercontent.com/u/25806407/images/Vuforia_Developer_Portal.png

##事前準備
ツールを使用するためには会員登録が必要です．

ページ上部の**Registar**ボタンを押して会員登録を行なって下さい．

![alt text][vss1]
[vss1]:https://dl.dropboxusercontent.com/u/25806407/images/Create_a_new_account___Vuforia_Developer_Portal1.png

![alt text][vss2]
[vss2]:https://dl.dropboxusercontent.com/u/25806407/images/Create_a_new_account___Vuforia_Developer_Portal2.png

答えなければいけない項目がたくさんありますが，きちんと入力して下さい．

会員登録が終了すると，ページ上部の**Login**ボタンから会員専用ページにアクセスすることができるようになります．

![alt text][vss3]
[vss3]:https://dl.dropboxusercontent.com/u/25806407/images/login.png

##SDKの入手

Vuforiaで作ったマーカーを使用するためのSDK(Software Developer Tool)を入手します．

![alt text][sdk0]
[sdk0]:https://dl.dropboxusercontent.com/u/25806407/images/sdk1.png

トップページの下部にVuforia3.0をダウンロードするリンクがあるので，クリックして下さい．

![alt text][sdk1]
[sdk1]:https://dl.dropboxusercontent.com/u/25806407/images/sdk2.png

最初はAndroid用のSDKをダウンロードするページが開いていると思います．

左端の`Unity Extension`をクリックしてから，`Download Unity Extension 3.0.x for Android & iOS`をクリックして，SDKのダウンロードを行なって下さい．


##マーカーの作成
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

Web上で作業をするのはここまでです．

マーカーの作り方はとても重要ですので，覚えておいて下さい．
