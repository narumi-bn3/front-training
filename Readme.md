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

# フォームのラベルを指定するー```<label>```
```<label>```要素は```<input>```要素などの
フォームパーツと共に利用される。各フォームパーツの
「ラベル」を設定するためのもので、「for」という特別な属性を指定できます。
```<label>```要素の書式。
```<label for="<input>要素などフォームパーツのid属性">ラベル名</label>```
```<input type="..." id="..."...>```
for属性には、そのラベルの対象となるフォームパーツのid属性を指定します。

# ```<label>```要素はインライン

# 表示の方法を設定するーdisplay
displayプロパティは、インラインとブロックを相互に交換するときによく利用されます。
・inline インラインにする
・block  ブロックにする
もう一つよく使われるのが、表示を消す「none」です。
・none  表示させなくする

# インラインで要素をグループ化するー```<span>```
```<span>```要素は```<div>```と同様にそれ自身は大きな意味はなく、ある範囲をマークアップしてidやclassを付加できる便利なタグ。```<div>```との違いは、インラインであるという点。他の要素が隣り合わせになってしまった場合に、行が折り返されずに表示される。

# 文字の太さを調整するーfont-weight
font-weightプロパティは、文字の太さを変化させるプロパティ。設定できる値は、100から900までの100ずつの単位と、「normal」「bold」「lighter」「bolder」の４種類です。標準はnormalおよび、400です。
ただし、必ず太さが変わるとは限らない。ユーザーが閲覧している環境に、その太さの「フォントデータ」が入っていなければ設定されず、「normal」と同じ状態になります。特に、数字での指定は９種類もの太さの環境を持っているユーザーはなかなかおらず、細かな設定はほとんど意味がない状態になる。実質的に利用されるのは「bold」と「normal」程度になる。

# Javascript 
# 動作させたい対象を示すオブジェクト
オブジェクト(object)は英語で「もの」と言った意味がありますが、「対象」と考えるといい。Javascriptでは、Webブラウザー内のさまざまな要素に対して「命令」をすることができる。その対象となるものがオブジェクト。
#　命令の内容を示すメソッド
メソッド(method)は「方法」などの意味がありますが、ここでは「命令」と考える。先のオブジェクト(対象)に対して、「なにを」して欲しいのかを示します。
# 命令の詳細を示すパラメーター
パラメーター(Parameter)は、「設定値」などの意味ですが、メソッドに対して細かい調整を加えていきます。例えば「document.write」メソッドは、そのままでは「画面に表示したい」ということしか分からず、「なにを」という部分が足りません。これを、バラメーターで指定します。

# オブジェクト.メソッド（パラメーター）
# 誰に.どうする（なにを）

# document.write('20xx/1/23');

# 文書に.表示する('20xx/1/23'を);

# 演算子
javascriptは足し算や引き算などの「四則演算」をすることができる。かけ算は「*(アスタリスク)」、割り算は「/(スラッシュ)」
記号で表します。通常の計算と同様に演算子の優先順位も正しく行われます。足し算を先に行いたい場合は、「()」を使うのも通常の数学と同様です。

# クオーテーション記号の役割
クオーテーション記号には「文字列として扱う」という意味があります。そのまま画面に表示して欲しい場合は、前後に「`」を付加します。これを付加しない場合は、javascriptは内容を理解してなんらかの処理を行おうとします。これをプログラム用語で「評価」などど言います。

# 文字列連結
クオーテーション記号が必要な文字列と、必要のない数式などをつなげるには「+」を使います。足し算の「+」と非常にややこしいのですが、役割が少し異なっているので気をつけましょう。
ここでは、「10＋3の結果は」という文字列と「10＋３」という演算、そして「です」という文字列をつなぐために、それぞれを「＋」記号で連結しています。