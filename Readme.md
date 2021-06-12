# front-training
フロントの勉強

# 段落を表すー```<p>```
```<p>```タグは「paragraph」の略で「段落」
```<p>```要素という。

# 入力フォームを表すー```<input>```
四角形が現れ枠線内をタップまたはクリックすると、
テキストが入力できる。
```<input>```要素という。

# 入れ子構造
```<p><input><p>```
囲っている```<p>```要素のことを「親要素」
中の```<input>```要素を「子要素」という。

# type属性
入力フォームの形状や入力される内容を指定する。
•email メールアドレスの入力のみ許可する。
•password パスワードの入力欄。入力された内容を隠す。

# name属性
入力フォームに名前をつける。

# value属性
入力フォームに表示される内容を示す。

# ボタンを設置するー```<button>```
ボタンは```<button>```要素で設置する。次のような書式で記述する。
```<button type="ボタンタイプ">ラベル</button>```
type属性には次のいずれかを設定する。
・submit 送信ボタン。これをクリックするとフォームが送信される。
•reset リセットボタン。入力した内容をクリアにするボタン。
・button JavaScriptと組み合わせて利用するときに使われる。

# CSSの書式
プロパティ：値；
余白を示すのは「margin」

# レイアウトを調整する~ ```<divタグ>```
複数の要素をまとめるためのタグがいくつかある。
代表的なのが```<div>```タグです。
divisionの略で「分割」という意味がある。
divタグの場合、タグ自身には意味を持たせられない為、
グローバル属性のid属性かclass属性を使って「しるし」
をつけるのが一般的。

# ブロックを中央に揃える
左右の「margin」を「auto」とすると、CSSで自動的に
Webブラウザーの幅が取得されて、真ん中に来るように
調整されます。Webブラウザーの幅を変えても、ちゃんと
計算し直されて配置される。

# 枠線を引くーborder
borderプロパティは、要素に枠線を引くための
プロパティです。
書式 //border: 枠線の幅　枠線の種類　枠線の色;
・border-with  枠線の幅
・border-style  枠線の種類
・border-color  枠線の色
・border-top   上部の枠線
•border-right  右側の枠線
•border-left   左側の枠線
・border-top-widh  上の枠線の幅
・border-top-style  上の枠線の種類
・border-top-color   上の枠線の色

# 要素内の余白を設定するーpadding
「padding」プロパティは余白の設定です。
「margin」プロパティとの違いは「要素の中の余白」
という点です。
```<div>```要素や```<button>```要素など
要素の中に文章が入り込む場合、要素内余白がないと
上下左右がくっついた状態になります。ここに余白を
設定するのが「padding」プロパティです。

# ボタンを作成する
ボタンの角を少し丸めて「角丸」を作成するプロパティが
「border-radius」プロパティです。

# ドロップシャドウをかけるーbox shadow
ブロックに影をつける、いわゆる「ドロップシャドウ」
は「box-shadow」プロパティを使います。
```<button>```要素の最後に追加しましょう。
box-shadow: x位置　y位置　ぼかし　色
「ぼかし」の値は大きくするほどぼけた感じになり、
小さくするほどくっきりした影になります。「色」には
カラーコードやrgbなどでの色指定が利用できます。