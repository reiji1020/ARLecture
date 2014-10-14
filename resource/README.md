# 素材を集めよう

## 初音ミクの3Dモデル

まずメインとなる初音ミクの3Dモデルをダウンロードしましょう．

[VPVP Wiki](http://www6.atwiki.jp/vpvpwiki/pages/1.html)では初音ミクに限らず，MikuMikuDanceで使える多くのキャラクターのモデルを探すことが出来ます．

私のオススメは[Lat式初音ミク](http://www6.atwiki.jp/vpvpwiki/pages/204.html)です．

[Tda式初音ミク](http://www6.atwiki.jp/vpvpwiki/pages/446.html)なども人気ですが，ポリゴン数やモデルに貼りつける画像の多さから，スマートフォン向けのアプリには向かないという欠点があります．

[七葉1052式初音ミク](http://dic.nicovideo.jp/a/%E4%B8%83%E8%91%891052%E5%BC%8F%28%E4%BB%AE%29)はポリゴン数が少ないながらも標準モデルと同様の器用さ・扱いやすさ・
魅力を兼ね備えたモデルです．

今回はとりあえず[Lat式初音ミク](http://www6.atwiki.jp/vpvpwiki/pages/204.html)を使ってコンテンツを作っていきましょう．

~~おすすめの理由はかわいいからです！！~~

では，[初音ミクのデータを紹介しているページ](http://www6.atwiki.jp/vpvpwiki/pages/298.html)へ移動して，配布先と書かれているリンクをクリックして下さい．

![alt text][mmd0]
[mmd0]:https://dl.dropboxusercontent.com/u/25806407/images/mmd0.png

リンク先に，Downloadと書かれた赤いボタンがあるので，ここをクリックしてモデルのダウンロードを行なって下さい．

ダウンロードしたファイルはzipで圧縮されているので，解凍しておきましょう．

## モーションデータと楽曲

音楽に合わせて初音ミクを踊らせたいので，振り付けと音楽が必要です．

`モーションデータ`というのは，キャラクターモデルの手足や表情の座標をフレーム毎に記録したデータです．

今回はMMD用に作られたモーションデータを使用して，初音ミクを動かしたいと思います．


扱う楽曲は以下のものです．

[ねこみみスイッチ](http://www.nicovideo.jp/watch/sm14365789)


[ねこみみスイッチ モーションデータ](https://bowlroll.net/file/421)


この楽曲を選んだ理由ですが，モーションデータはおおまかに

・表情モーションだけのもの

・体を動かすだけのもの

・表情と体の動きを一緒に扱えるもの

この3つに分けられます．

種類としては体を動かすだけのものが多く，表情は自分でMMDソフトウェア上で自由に作ることが出来るようになっています．

今回は時間が限られているため，表情も一緒になったモーションデータを使用したいと思います．~~そしてかわいいからです~~

モーションデータに関しては，上のリンクからモデルデータと同じようにダウンロードして下さい．

楽曲は以下のURLにアクセスし，

[ねこみみスイッチ 楽曲データ](http://www.youtube.com/watch?v=DKHyxZnFnvg)(Youtubeのサイトです)

ここのURLをコピーして，

[YouTubemp3](http://www.youtube-mp3.org/jp)(動画から音楽を抜き出すオンラインサービスです)

真ん中にあるテキストボックスに貼り付け，`動画変換`ボタンをクリックします．

![alt text][mmd1]
[mmd1]:https://dl.dropboxusercontent.com/u/25806407/images/mmd1.png

![alt text][mmd2]
[mmd2]:https://dl.dropboxusercontent.com/u/25806407/images/mmd2.png


## プログラム

[MMD4Mecanim](http://stereoarts.jp/)

MMD用のモーションデータ・モデルはそのままではUnityで扱うことが出来ません．従って，Unityで扱えるようにデータを変換する必要があります．

そこで，**MMD4Mecanim**というプログラムを使用します．

このプログラムは，モーションデータとモデルデータを指定するとUnityでもデータが扱えるように変換してくれる優れたソフトウェアです．

上記URLの真ん中あたりにあるリンクからダウンロードして下さい．

![alt text][mmd3]
[mmd3]:https://dl.dropboxusercontent.com/u/25806407/images/mmd3.png

これで全ての素材が出揃いました！

次のチャプターに進みましょう．