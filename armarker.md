# ARマーカーを作ってみよう

なんだかんだで座学が長引いてしまった感じがありますが，これからは沢山手を動かしてもらいます！

ARマーカーを作ってみましょう．
同梱の画像を使用します．

この画像です．5分で作りました．

![alt text][armarcker]
[armarcker]:https://dl.dropboxusercontent.com/u/25806407/images/ARMarcker.png


画像をARマーカーとして使用するには，この画像に含まれる**特徴点と**呼ばれるデータを計算しなければなりません．

`特徴点`とは，画像中に含まれる**エッジ**(輪郭)や線の繋がる場所，点が集合する場所などのある種の特徴の事を指します．

この特徴点の配置をコンピューターはデータとして持っておき，類似した特徴点の配置をもつ画像を認識した時，ARコンテンツを表示するといった仕組みです．

では特徴量計算をしましょう．

といってもこの計算には便利なツールが存在しますので，そちらを利用します．

https://developer.vuforia.com/

上のURLをクリックしてサイトにアクセスしてください．

ARマーカーを作ったり，ARコンテンツを簡単に作成することができるツールに``Vuforia``というものがあります．

今回はこのVuforiaを活用して，ARマーカーを作っていきましょう．

![alt text][vss0]
[vss0]:https://dl.dropboxusercontent.com/u/25806407/images/vss0.png

ツールを使用するためには会員登録が必要です．

ページ上部の**Registar**ボタンを押して会員登録を行なって下さい．

![alt text][vss1]
[vss1]:https://dl.dropboxusercontent.com/u/25806407/images/vss1.png

![alt text][vss2]
[vss2]:https://dl.dropboxusercontent.com/u/25806407/images/vss2.png

答えなければいけない項目がたくさんありますが，きちんと入力して下さい．

会員登録が終了すると，ページ上部の**Login**ボタンから会員専用ページにアクセスすることができるようになります．

![alt text][vss3]
[vss3]:https://dl.dropboxusercontent.com/u/25806407/images/vss3.png

では，早速マーカーを作っていきましょう．
ログインができるようになったら，ページ上部の`TargetManager`をクリックしてください．

![alt text][vss4]
[vss4]:https://dl.dropboxusercontent.com/u/25806407/images/vss4.png

