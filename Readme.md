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

# 計算結果を保持しておくー変数ー
ここで記述した「answer」は「変数」という、さまざまな値を保存しておくためのjavascriptの機能の１つ。これをプログラミング用語で「代入」といいます。「var」じゃ「Variable（可変という意味）」の単語の略称で、変数を作る（＝宣言するといいます）ときに記述します。続けて「変数名」とその最初の内容（初期値）を記述します。さらに、変数を計算などの一部として使うこともでき、「再代入」することもできます。

# 日時を扱うーDateオブジェクト
今日の日付を知るためのメソッドである「getDate」メソッドです。

# Date.getFullYear
年を４桁で取得します。（例：2017）

# Date.getMonth
月を取得します。ただし、取得する数字は０から始まってしまうため、目的の数字にするには１を加える必要があります。

# Date.getDate
日付を取得します。

# 要素内にテキストを挿入するーDOM操作ー
完成プログラムのように、時刻表示の内容を置き換えるにはDOM（ドム）を使います。DOM(Document Object Model)とは、HTMLの要素をプログラムの対象（＝オブジェクト）として扱うための手段で、API(Application Programing Interfaace)と呼ばれるものの一種です。
document.writeメソッドを利用する場合以外は、```<script>```要素は必ず```<body>```要素の最後か、```<head>```要素内に記述します。

# 「もしも」で処理を分けるーif構文ー
「getSeconds」メソッドは現在の秒を取得できる、Dateオブジェクトのメソッドです。
このとき画面には１桁の数字（0-9）か、２桁の数字が表示されます。『もし、現在の秒が１桁(=10未満)なら、数字の前に0を付け足す』この「もし」を実現できるのが「if構文」です。

# if構文の書式
if (条件分）{
  条件分がtrue(YES)の場合の処理}
  ifの後の「()」の中に書かれた条件分が満たされているかを判断し、満たされている場合は「()」の中の処理を行い、満たされなければ「()」の中は飛ばされます（処理は行われません）。secondsは、「現在の秒」を代入した変数です。これが「10未満」であるかを判断するため「< 10」という記述があります。つまり、「現在の秒が１０未満なら」という意味があります。この「<」という記号を「比較演算子」と言います。

  # よく使う処理をまとめておくーfunctionー
  同じようなプログラムが何度も登場するのは効率が悪いので、これを１箇所にまとめるのが「ファンクション」です。ファンクション（function）は「機能」といった意味がありますが、プログラミング用語では「関数」などと呼ぶ場合もあります。
  ファンクションの定義で、returnの後には、そのファンクションで行なった処理の結果を記述します。そしてファンクションを呼び出すことで、処理した結果を「返り値」として得ることができるようになるのです。

  # イベントを定義するーaddEventListener
  「addEventListener」というメソッドは、ユーザーの操作(＝event）の監視役（Listener)を定義します。

  # イベントの定義
  要素.addEventListener(イベントの種類,処理);

  # 自動で何度もプログラムを実行するーsetInterval
  見ている間ずっと変わり続けるようにするには「setInterval」というメソッドを使います。
  # setIntervalの書式
  タイマーID = setInterval(処理、間隔);

  # floorメソッドの書式
  整数 = Math.floor(少数)；

  # STOPボタンを作成する
  同じ操作で動作を切り替えられるボタンを「ドグルボタン」といいます。
  # 要素にクラスを追加する書式
  要素.classList.add(`追加するクラス名`);

  # 要素からクラスを消去する書式
  要素.classList.remove(`消去するクラス名`);

  # ボタンクラスの場合
  ```<button class="btn btn-danger">STOP</button>```

  # タイマーを止めるーclearInterval
  動き出したタイマーを止めるには「clearInterval」メソッドを使います。

  # clearIntervalメソッドの書式
  window.clearInterval(タイマーID);
  「タイマーID」とは、「setInterval」メソッドの返り値として得ることができる情報です。

  # Capter5 JSONデータ

  # 要素の位置を固定するーpossition:fixedー
  ここで、「possition」を「fixed」に設定しています。これは「画面上に固定する」という指定です。どこに固定するのかを「top」「left」「right」「bottom」プロパティのいずれかで設定します。このとき、要素同士が重なり合うことになりますが、「おどちらの要素が上にかぶるか」というのは、HTMLのタグが「後」に書かれたものの方が、優先度が高くなります。

  # 重なり会う要素の優先度を設定するーz-indexー
  z-indexプロパティは、数値で重なりの優先度を指定することができます。「優先度」に指定する数値は、0が最小で、最大では1,000,000,000といった非常に大きな数を指定することができます。大きい数字ほど、基本的には上位に表示されます。サンプルでは「100」という数字を指定しました。1、2、3•••といった数値を指定するよりは、100,200,500,1000など、ある程度の幅をとった数字を指定した方が、要素の追加などで調整するときに、既存の要素の数字をずらすなどの作業を避けることができるため、安心です。

  # JSONデータを用意する
  写真のデータの元となる「JSON」というデータを準備します。JSONとは「JavaScriptObjectNotation」の略称で、JavaScriptとの相性が非常に良いデータ形式です。

  # まとめて値を管理するーArrayー
  JSONデータを代入している「images」という変数は、ちょっと特殊な形をしています。これはArrayという形のオブジェクトで、一般的には「配列」と呼ばれます。Arrayオブジェクトは（配列）は、複数の値をひとまとめにして管理することができます。Dateオブジェクトなどと同じように、まずArrayオブジェクトのインスタンスを作成し、パラメーターに、挿入したい内容を羅列していきます。

  # 配列の書式
  var 配列名 = [値1,値2,値3...];

  # 新しい要素を作るーdocument.createElementー
  「document.creatElement」は、新しく要素を作成するためのメソッドです。パラメーターに要素名を指定すると、「Element」オブジェクトが作成されます。
  これは、「document.getElementById」で要素を指定したときに生成されるオブジェクトと同じものです。そのため、「innerHTML」プロパティでコンテンツを入れるなどの操作が可能です。

  # 要素を追加するーappendChildー
  dosument.createElementメソッドで作った要素は、dosument.appendChaildメソッドで画面上の要素に追加をすることで、表示させることができます。要素は作っただけでは表示されないので、かならず追加の作業が必要です。

  # appendChildメソッドの書式
  追加する場所.appendChild(要素);