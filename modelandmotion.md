# モデルとモーションを変換する

モデルとモーションを変換して，ミクに登場してもらいましょう．

Resources→Lat式ミクVer2.31フォルダのにはモデルを構成する様々なデータが入っています．この中で，**Unityのアイコンの『Lat式ミクVer2.31_Nomal.MMD4Mecanim.asset』**というファイルを探して下さい．

![alt text][u5]
[u5]:https://dl.dropboxusercontent.com/u/25806407/images/U6.png

このとき，Inspectorタブに利用規約が表示されます．
**きちんと読んで利用規約に同意してから使用するようにしましょう．**

利用規約に同意すると，このような画面に移行します．

モデルデータは指定されているので，モーションデータを指定しましょう．

![alt text][u6]
[u6]:https://dl.dropboxusercontent.com/u/25806407/images/U7.png

`nekomimi_lat`というモーションデータを探し出し，指定して下さい．

指定ができたら，下の`Process`ボタンをクリックして，モデルが変換できるまで待って下さい．

![alt text][u7]
[u7]:https://dl.dropboxusercontent.com/u/25806407/images/U8.png

![alt text][u8]
[u8]:https://dl.dropboxusercontent.com/u/25806407/images/U9.png

とうとうミクを登場させることが出来ました！

カメラを動かしてもっと間近で見ましょう．

![alt text][u9]
[u9]:https://dl.dropboxusercontent.com/u/25806407/images/U10.png

しかし少しモデルが暗く見づらいですね．

GameObjectタブからDirectionalLightを選び，光源を設置しましょう．

![alt text][u10]
[u10]:https://dl.dropboxusercontent.com/u/25806407/images/U11.png

ミクが明るく見えるようになりました！

![alt text][u11]
[u11]:https://dl.dropboxusercontent.com/u/25806407/images/U12.png

## ただでさえ天使のミクさんをさらに天使にするコツ

今のままではモデルのエッジ(縁)が目立ちますね．

このエッジを滑らかにして，モデルをよりキレイに見せる方法を紹介します．

EditタブからProjectSetting→Quallityをクリックして下さい．

![alt text][u12]
[u12]:https://dl.dropboxusercontent.com/u/25806407/images/U13.png

Inspectorsタブに，チェックボックスが沢山並んでいる部分があります．
Levelが6つあり，下に行くほど素材をキレイに表示することが出来ますが，PCや端末のリソース(バッテリー，メモリ，etc...)を消費します．

生協指定PCは十分にリソースが確保されているはずですので，一番下のFantasticを指定しましょう．

このとき，FantasticオプションのAnti Aliasingを『8x Multi Sampling』(最高レベル)に指定してください．

![alt text][u13]
[u13]:https://dl.dropboxusercontent.com/u/25806407/images/U14.png

![alt text][u14]
[u14]:https://dl.dropboxusercontent.com/u/25806407/images/U15.png

どの端末をFantasticにするかはみなさんのもつ端末に任せます．

iPhoneを使っている人はiOSアプリ，Android端末(Xperia,GALAXY,ARROWSなど)を使っている人はAndroidアプリのクオリティをFantasticにしてください．


このままでは，ミクは動いてくれません．

変換したモーションを，ミクに設定する必要があります．

ミクの素材が入った`Lat式ミクVer2.31`のフォルダの中で右クリックをして，Create->Animator Controllerをクリックしてください．

![alt text][u15]
[u15]:https://dl.dropboxusercontent.com/u/25806407/images/U16.png

Animator Controllerを作ったら，名前をつけてください．自由につけてかまいません．思いつかなければ「nekomimi」でよいでしょう．


Animator Controllerを作成すると，Sceneタブの横にAnimatorタブが出来ます．これをクリックして，アニメーションを設定する画面を開いて下さい．

次に，初音ミクのモデルデータの右側にある小さな矢印をクリックし，**モーションの名前のついたファイル**(Nullではない)を探します．今回の場合は，nekomimiという名前が付いています．

これをAnimatorタブの中にドラッグ・アンド・ドロップしてください．

![alt text][u16]
[u16]:https://dl.dropboxusercontent.com/u/25806407/images/U17.png

これでアニメーションファイルの設定は終了です．

次にミクにこのファイルを設定しましょう．

Hierarchyタブの中にあるミクのモデルをクリックし，Inspectorタブを見ると，Animatorというオプションを確認できます．

ここの**controller**という場所に，先ほど作ったAnimator Controllerをドラッグ・アンド・ドロップしてください．

![alt text][u17]
[u17]:https://dl.dropboxusercontent.com/u/25806407/images/U18.png

これでミクにモーションファイルを設定することが出来ました．

最後に，音楽データを設定してミクに踊ってもらいましょう．

Animatorオプションの下に，5つのボタンが並んでいます．

ここの『Anim』というボタンをクリックして，Audio ClipにResourcesフォルダに置いておいた音楽ファイルをドラッグ・アンド・ドロップして下さい．

![alt text][u18]
[u18]:https://dl.dropboxusercontent.com/u/25806407/images/U19.png

これでミクに関する全ての設定が終わりました．
上にある再生ボタンを押して，ミクが踊るかどうか確認して下さい．

![alt text][u19]
[u19]:https://dl.dropboxusercontent.com/u/25806407/images/U20.png
