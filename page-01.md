# Unityを起動しよう
まずはUnityを起動しましょう。
![image01](img/img-1.png)
Unityを起動すると、上の画像のようにUnityプロジェクトの作成画面になります。

左のテンプレートで2Dか3Dかを選択します。今回は3Dにします。

プロジェクト名は「Unity Sample」としてください。
<br />
<br />

{% hint style='info' %}
もし同じサーバー内に同時に保存する場合は、名前の前に学籍番号などをつけて自分のプロジェクトだとわかるようにしてください。
{% endhint %}
<br />
<br />
保存先は指定の場所に保存してください。特に指定がなかったら、デスクトップに保存しましょう。

全て設定が終わったら右下の作成ボタンを押してください。

しばらく待つとUnityの開発画面が開かれます。
<br />
<br />
***

# Unityの画面構成

## レイアウトのカスタマイズ

Unityが開かれると、下の画像のような画面が出てきます。

![image02](img/img-2.png)

これがUnityのデフォルトの開発画面なのですが、少しわかりにくいので画面を変えたいと思います。

<br />
<br />

Unityの右上に「Default」のボタンがあるので、そちらを押して表示された中から「2 by 3」を選択してください。

![image03](img/img-3.png)

<br />
<br />

そうすると、下の画像のようになりました。もう少し変更します。

![image04](img/img-4.png)
<br />
<br />

Projectウィンドウの右側の三本線のアイコンをクリックしてください。そして、出てきたリストの中から「One Column Layout」を選択しましょう。

![image05](img/img-5.png)

<br />
<br />

そうすると、このようにProjectウィンドウが見やすくなります。

![image06](img/img-6.png)

<br />
<br />

これで画面のカスタマイズは完了です。

今回は「2 by 3」の画面で進めますが、開発画面は自分のやりやすいレイアウトで問題ありません。

<br />
<br />

## 画面の構成

Unityの画面構成は主に以下のようになっています。

![image07](img/img-7.png)

### ①. シーンビュー
　ゲームを組み立てるためのメイン画面です。素材を配置してゲームのシーンを作成するのが主な役割です。
### ②. ゲームビュー
　ゲームを実行した時の見え方を確認するほか、ゲーム時の処理スピードや負荷のかかり方などを解析できます。
### ③. ヒエラルキーウィンドウ
　シーンビューに配置したオブジェクトの名前を一覧で表示します。また、オブジェクト同士の階層構造を表示したり編集したりできます。
### ④. プロジェクトウィンドウ
　ゲームで使う素材を管理します。このウィンドウに画像や音声などの素材をドラック＆ドロップすることで、Unityにゲームの素材として追加することができます。
### ⑤. インスペクターウィンドウ
　インスペクターウィンドウには、シーンビューで選択したオブジェクトの詳しい情報が表示されます。インスペクターでオブジェクトの座標・回転・スケールや色、形などを設定します。
### ⑥. 操作ツール
　シーンビューに配置したオブジェクトの座標や回転、サイズを調整したり、シーンビューの見え方を調整したりするためのツールです。
### ⑦. 実行ツール
　ゲームの実行や停止を行うツールです。

<br />

最初は何がどういう意味か全く分からないと思いますが、これらは何度も作っていくうちに自然に覚えられるので、今は言葉だけ覚えておけば大丈夫です。
<br />
<br />

# オブジェクトの配置

では早速UnityのScene上にオブジェクトを配置したいと思います。

ヒエラルキーウィンドウから「Create -> 3D Object -> Plane」を選択してください。
<br />

![image08](img/img-8.png)

<br />
<br />

これでScene内に四角い平面が表示されました。

![image09](img/img-9.png)

<br />
<br />
画面右側にたくさんの項目が出てきたと思いますが、これはインスペクターウィンドウで選択されているオブジェクトの詳細情報です。試しにPlaneのScaleを「x = 2, y = 1, z = 2」にしてみましょう。

![image10](img/img-10.png)

<br />
<br />
そうすると、SceneとGameビューのPlane（平面）が２倍の大きさになりました。
<br />
<br />

# マテリアルを追加

次にただの白い平面では寂しいので、色をつけたいと思います。

色をつけるためには新たにマテリアルというものを追加する必要があります。

![image11](img/img-11.png)

プロジェクトウィンドウから「Create -> Material」を選択してください。

<br />
<br />
次に、今作成したMaterialを選択していると、インスペクターウィンドウに下の画像のように白い四角が表示されているかと思います。この白い四角をクリックしてください。

![image12](img/img-12.png)

<br />
<br />
そうすると、下の画像のようなカラーパレットが表示されたかと思います。

このカラーパレットで色を設定できます。外側の広い円でカラーを選び、内側の四角形の場所で色の濃さを選びます。選び終わったら左上のバツボタンで閉じてしまいましょう。

![image13](img/img-13.png)

<br />
<br />
色の作成が終わったら「New Material」をScene上のPlaneにドラッグ＆ドロップでつけてください。

![image14](img/img-14.png)

<br />
<br />
そうすると、平面に色をつけることができました。

![image15](img/img-15.png)

<br />
<br />

# 球体の追加

次に球体（Sphere）を追加します。

ヒエラルキーウィンドウから「Create -> 3D Object -> Sphere」を選択してください。

![image16](img/img-16.png)

<br />
<br />
スフィアが画面からずれていた場合は、SphereのインスペクターウィンドウのTransformの右側の歯車アイコンをクリックし、Resetを選択してください。これでスフィアが画面の中央に表示されます。

![image17](img/img-17.png)

<br />
<br />
このままではスフィアが地面に埋まってしまっているので、Sceneウィンドウの左上の十字矢印マークを選択し、緑色の矢印（y座標）を少し上に引っ張ってスフィアを浮かせてください。下の画像くらい浮かせられたらOKです。

![image18](img/img-18.png)

{% hint style='info' %}
## Challenge
スフィアのカラーを変更してみましょう。
{% endhint %}

<br />
<br />

# Sceneを保存しよう

ここまで記述終わったらSceneを保存しておきましょう。

Unity左上のFile（ファイル）からSave（セーブ）を選択してください。これでこのシーンを保存することができます。保存場所は任意の場所にしてください。

保存をしないと、予期せぬトラブルでUnityが終了してせっかく作ったシーンが最初に戻ってしまうという悲劇がおきてしまいます。

保存は今後もこまめにしておきましょう。

![image19](img/img-19.png)