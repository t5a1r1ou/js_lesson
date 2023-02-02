---
theme: unicorn
class: 'text-center'
highlighter: shiki
lineNumbers: false
info: |
  ## JavaScript講座
drawings:
  persist: false
css: unocss
layout: new-section
section-image: "../assets/images/javascript.png"
---

<h1 class="text-lg">JavaScript講座</h1>

<p class="text-lg pt-5">~ 書いて慣れるJavaScript ~</p>

<p class="pt-12">2023/2/1,2023/2/2</p>

<style>
  h1 {
    font-size: 3rem !important;
  }
</style>

<!--
  - 挨拶
  - コードをとにかく書いてJavaScriptに慣れてもらう
  - 前編後編あります
 -->

---
layout: intro
introImage: '../assets/images/icon.png'
---

<p class="mb-1 text-sm">エンジニアグループ</p>

# 中井 柊太

<!--
  - 自己紹介
  - エンジニア歴
  - 関わっているプロジェクト
-->

---
layout: center
---

<p class="text-lg">今回の目標</p>
<h1 v-click>JavaScriptに対する苦手意識をなくそう！</h1>

<!--
  - JavaScriptアレルギーを治そう
  - KARTE,GAタグくらいなら余裕
-->

---
layout: new-section
sectionImage: "../assets/images/javascript.png"
---

<div class="flex justify-center">

  <h1 class="pr-0 text-left -indent-8 ml-8">1. JavaScriptって<br>何ができる？</h1>

</div>

<!--
  - ご存知かもしれませんが、JavaScriptでできること
-->
---
layout: image-right
class: justify-center
---

# Webサイトでは...

<ul class="text-xl text-left">
  <li>リッチな動きを作る</li>
  <li>モーダルやアコーディオン、カルーセルの動きを作る</li>
</ul>
<ul class="text-xl text-left" v-click="1">
  <li>UI全体を構築する</li>
  <li>..etc</li>
</ul>

<div class="absolute right-0 w-lg -z-1" v-click="1">
  <img src="/assets/images/web-js.png" />
</div>

<!--
  - アートっぽいリッチな動き
  - モーダルやカルーセル、アコーディオンの動き
  - UI全体を構築
  - React,Vue=フロントエンドでJavaScriptが使われていない最近のサイトはほとんどないと言ってもいいくらい
-->

---
layout: image-left
class: justify-center
---

# 他にも...

<ul class="text-xl text-left">
  <li>サーバーサイドのプログラムを書くことができる</li>
  <li>モバイルアプリやデスクトップアプリを作る</li>
  <li>...etc</li>
</ul>

<div class="absolute left-0 w-lg -z-1">
  <img src="/assets/images/native-server-js.png" />
</div>

<!--
  - 他にも、サーバーサイドのプログラムやモバイルやデスクトップのアプリもJavaScriptを使って作れる
-->

---
layout: new-section
sectionImage: "../assets/images/javascript.png"
---

<h1 class="pl-3 pr-0 text-left text-xs -indent-9 ml-9">2. とにかくJavaScriptをさわってみよう</h1>

~ 自己紹介ページを作ろう ~

<!--
  - 簡単な自己紹介ページを作ります。
  - あまり詳しい説明はせずに、コードをとにかく真似して書いてもらってコードが動くことを体験してもらう
-->

---
layout: image-right
class: justify-center
---

# 目標物確認

<h2>
  <a href="https://shutanakai.github.io/js_lesson/" class="text-indigo-800" target="_blank" >https://shutanakai.github.io/js_lesson/</a>
</h2>

<div class="absolute right-0 w-lg -z-1">
  <img src="/assets/images/js_lesson1.png" />
</div>

<!--
  - 目標のサイト確認
-->

---
layout: center
---


# ソースコードのダウンロード・エディタの用意([URL](https://hakuhodody-my.sharepoint.com/personal/sd000243_hakuhodody-holdings_co_jp/_layouts/15/onedrive.aspx?FolderCTID=0x0120000D2FDF8E4F61F940A189BA9BD5CEE4CE&id=%2Fpersonal%2Fsd000243%5Fhakuhodody%2Dholdings%5Fco%5Fjp%2FDocuments%2F110%5F%E6%AD%A3%E7%A4%BE%E5%93%A1%E3%83%BB%E5%A5%91%E7%B4%84%E7%A4%BE%E5%93%A1%E5%85%B1%E9%80%9A%2F004%5F%E7%A4%BE%E5%86%85%E5%8B%89%E5%BC%B7%E4%BC%9A%2FWedemy%2FJavaScript%2Fjs%5Flesson%2Ezip&parent=%2Fpersonal%2Fsd000243%5Fhakuhodody%2Dholdings%5Fco%5Fjp%2FDocuments%2F110%5F%E6%AD%A3%E7%A4%BE%E5%93%A1%E3%83%BB%E5%A5%91%E7%B4%84%E7%A4%BE%E5%93%A1%E5%85%B1%E9%80%9A%2F004%5F%E7%A4%BE%E5%86%85%E5%8B%89%E5%BC%B7%E4%BC%9A%2FWedemy%2FJavaScript))

<p></p>

<p class="text-xl font-bold text-indigo-800">
  VSCodeをインストールした方:<br>
  「js_lesson」というフォルダをVSCodeで開く
</p>

<p class="text-xl font-bold text-indigo-800">
  VSCodeをインストールしていないMacの方:<br>
  「テキストエディット」というアプリを開き、ツールバーのファイルから「js_lesson/assets/script.js」を開く
</p>


<p class="text-xl font-bold text-indigo-800">
  VSCodeをインストールしていないWindowsの方:<br>
  「メモ帳」を開き、上部のメニューから「開く」でjs_lesson/assets/script.js」を開く
</p>

<p class="text-xl font-bold text-indigo-800">
  index.htmlをブラウザで開く
</p>


<!--
  - ソースコードの共有(チャット)
  - VSCodeハンズオン
  - Macハンズオン
  - Windows口頭

-->

---
layout: center
---

# HTMLとCSSとJavaScriptの関係

<ul style="list-style: none;">
  <li>

  **HTML** = Webページを構成する文章。タグと呼ばれるパーツのようなものの組み合わせ。

  </li>
  <li>

  **CSS** = パーツの装飾。見た目のカスタマイズ。

  </li>
  <li>

  **JavaScript** = 動きの定義。DOMと呼ばれるHTMLをJSで扱えるようにしたものを通じて動きを設定する。

  </li>
</ul>

<!--
  - コードを書く前にHTML,CSS,JavaScriptの関係について軽く説明
  - HTML = Webページを構成する文章。タグと呼ばれるパーツの組み合わせ。
  - CSS = 見た目の装飾、カスタマイズ。JavaScriptでも操作できる。
  - JS = 超簡単に言うと動きの設定、定義。DOMと呼ばれるHTMLをJavaScriptで扱えるようにしたものを通じてコードを書くことで動きを設定することができる。
-->


---
layout: center
---

# 最初のコード(おまじない)


```js {all|2,3,9|5,6,7|all}

// DOM(JavaScriptでHTMLを解釈したもの)の読み込み、CSS、画像といったリソースの読み込みが完了したら、中を実行する
window.addEventListener("load", () => {

  // ここにコードを書いていく
  // 検証ツールのConsoleにログとして"Hello JavaScript!"を表示する
  console.log("Hello, JavaScript!");

});

```

<style>
  .slidev-code {
    font-size: 1rem !important;
    line-height: 1.7 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - __コードを書く__
  - DOMやCSS・画像等リソースの読み込みが終わったら中を実行するコード
  - 今は何も勉強していない状態だから、おまじないくらいに思ってもらっていい
  - 検証ツールを使うとconsole.log()の括弧の中身をブラウザのコンソールで確認ができる
-->

---
layout: center
---

# 実装の流れを確認

<p></p>

<p class="text-xl font-bold text-indigo-800" v-click="1">名前、職種の箇所をJavaScriptを使って取得、確認する</p>

<p class="text-xl font-bold text-indigo-800" v-click="2">JavaScriptを使って名前、職種を書き換える</p>

<p class="text-xl font-bold text-indigo-800" v-click="3">ボタンをクリックした時にログを表示する</p>

<p class="text-xl font-bold text-indigo-800" v-click="4">ボタンをクリックした時に名前、職種を書き換える</p>

<!--
  - 実装の流れの確認
  - 名前と職種のところをJSを使って取得して、コンソールに表示させることで確認
  - それを使って、名前と職種のところをご自身のものに書き換え
  - ボタンをクリックした時に、コンソールにボタンがクリックされましたというログを表示
  - ボタンをクリックした際に名前と職種を書き換える

  - まずは名前のところをJSで取得する

  - __コードを書く__
-->


---
layout: center
---

# 名前を取得してログで確認する

<div class="text-left">

  script.js

  ```js

  // 名前のタグの中身をログに出力する
  console.log(document.querySelector(".profile__title").innerHTML);

  ```

  <p class="pt-5">index.html</p>

  ```html

  <h1 class="profile__title">shuta nakai</h1>

  ```

</div>

<style>
  .slidev-code {
    font-size: 1rem !important;
    line-height: 1.7 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - 書いたコードの確認
  - この値を変更することで名前の変更をすることができる

  - __コードを書く__
-->

---
layout: center
---

# 名前を書き換える

```js

document.querySelector(".profile__title").innerHTML = "taro yamada";

```

<div v-click class="pt-10">

  <div class="pb-3">

  # 職種を書き換える

  </div>

  ```js

  document.querySelector(".profile__desc").innerHTML = "ディレクターです。";

  ```

</div>

<style>
  .slidev-code {
    font-size: 1rem !important;
    line-height: 1.7 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - 書いたコードの確認
  - チャレンジ「職種を書き換える」

  [next]

  - __コードを書いて答え合わせ__

  - ボタンの取得・確認を進める
  - __コードを書く__

  - ボタンのクリック時に「ボタンがクリックされました」とコンソールに表示する
  - __コードを書く

-->

---
layout: center
---

# ボタンをクリック時に処理を実行する

```js {all|2,3,7|5|all}

  // ボタンをクリックした時にこの中を実行する
document.querySelector(".profile__next").addEventListener("click", () => {

  console.log("ボタンがクリックされました。");

});

```


<style>
  .slidev-code {
    font-size: 1rem !important;
    line-height: 1.7 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - 書いたコードの確認
  - [next]
  - このボタンがクリックされたら、
  - [next]
  - この中身が実行される
  - [next]
  - という実装になっている
  - DOMの読み込みのところと同じ

  - チャレンジ[ボタンが押されたら、名前と職種のところが趣味の名前とその詳細に変わる]

  - __答え合わせのコードを書く__

-->

---
layout: center
---

# ボタンをクリック時にテキストを書き換える

```js

  // ボタンをクリックした時にこの中を実行する
document.querySelector(".profile__next").addEventListener("click", () => {

  document.querySelector(".profile__title").innerHTML = "ギター";
  document.querySelector(".profile__desc").innerHTML = "たまに弾いています。";

});

```


<style>
  .slidev-code {
    font-size: 1rem !important;
    line-height: 1.7 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--

  - 書いたコードの確認

  - (時間があれば画像の表示を入れ替える__コードを書く__)
-->

---
layout: center
---

# 画像の表示を切り替える

<div class="text-left">

  script.js

  ```js

    document.querySelector(".profile__image").src = "入れ替えたい画像のパス";

  ```

  <p class="pt-5">index.html</p>

  ```html

  <img src="画像パス" alt="" class="profile__image" />

  ```

</div>

<style>
  .slidev-code {
    font-size: 1rem !important;
    line-height: 1.7 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - 画像の書き換えにはsrcを使って書き換える

  - (時間があれば、ボタン非表示の__コードを書く__)
-->

---
layout: center
---

# ボタンを非表示にする

<div class="text-left">

  script.js

  ```js

    document.querySelector(".profile__next").style.display = "none";

  ```

  <p class="pt-1">style.css</p>

  ```css

    .profile__next {
      display: inline-flex;　/* これをdisplay: none;にする */
    }
  ```

  <p class="pt-1">index.html</p>

  ```html

  <button class="profile__next">次へ</button>

  ```

</div>

<style>
  .slidev-code {
    font-size: .8rem !important;
    line-height: 1.7 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - CSSを書き換えるにはstyleを書き換える

  - コードの完成形の場所の共有
-->


---
layout: new-section
sectionImage: "../assets/images/javascript.png"
---

<h1 class="pl-3 pr-0 text-left -indent-8 ml-8">3. JavaScriptの<br>基本文法を知ろう<br>(前編)</h1>

~ 絶対に勝てるじゃんけんゲームを作る ~

<!--
  - また別のサイトを作っていく
  - それを通じてJavaScriptの基本文法を学んでいく
  - ソースコードの準備のアナウンス(途中からの人がいないかも確認)
-->

---
layout: center
---

# 3-0 ここまでの復習

---
layout: image-right
class: justify-center
---

# 目標物確認

<h2>
  <a href="https://shutanakai.github.io/janken_lesson/" class="text-indigo-600" target="_blank" >https://shutanakai.github.io/janken_lesson/</a>
</h2>

<div class="absolute right-0 w-lg -z-1">
  <img src="/assets/images/js_lesson2.png" />
</div>


<!--
  - 目標のサイトの確認
  - 初期状態の確認

  - __コードを書く__
-->

---
layout: center
---

# 最初のコード


```js

// DOMの読み込み、CSS、画像といったリソースの読み込みが完了したら、中を実行する
window.addEventListener("load", () => {

  // ここにコードを書いていく

});

```

<style>
  .slidev-code {
    font-size: 1rem !important;
    line-height: 1.7 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>


<!--
  - 読み込みが終わったら実行するコードの確認(復習)
-->

---
layout: center
---

# 実装の確認

<p></p>

<p class="text-xl font-bold text-indigo-800" v-click="1">最初に絶対に勝てるじゃんけんゲームを作る</p>

<p class="text-xl font-bold text-indigo-800" v-click="2">文法を学びながらリファクタリング（コードの改善）</p>

<p class="text-xl font-bold text-indigo-800" v-click="3">ランダムで出してくるCPU</p>

<p class="text-xl font-bold text-indigo-800" v-click="4">じゃんけんのロジックを実装して完成</p>


<!--
  - 実装の流れの確認
  - 絶対に勝てるグーボタンから実装
  - __コードを書く__

-->

---
layout: center
---

# 絶対に勝てるグーボタンを押した時

```js

// グーボタンを押した時
document.querySelector(".navigation__button--rock").addEventListener("click", () => {

  // じゃんけんの画像の変更
  document.querySelector(".cardBox__img--you").src = "./assets/images/rock.png";
  document.querySelector(".cardBox__img--cpu").src = "./assets/images/scissors.png";

  // 結果の反映
  document.querySelector(".card__title").innerHTML = "ぽんっ！";
  document.querySelector(".card__result").innerHTML = "あなたのかち！";

});
```

<style>
  .slidev-code {
    font-size: .83rem !important;
    line-height: 1.7 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - 書いたコードの確認
  - チョキボタン、パーボタンもコピペしながら__コードを書く__
  - まだこのコードには問題点がある

-->


---
layout: image-right
class: justify-center
---

# 問題点

<ul class="text-xl">
  <li v-click="1">同じ値を何度も取得している</li>
  <li v-click="2">変更への対応が辛い</li>
  <li v-click="3">何が書いてあるかわかりづらい</li>
</ul>

<div class="pt-5" v-click="4">
  <p class="absolute text-5xl text-indigo-600 font-bold">すべて変数を使うことで解決できます！</p>
</div>

<div class="absolute right-0 w-lg -z-1">
  <img src="/assets/images/scream1.jpg" />
</div>

<!--
  - 問題点の確認
  - [click]
  - 同じ値を何度も取得している => 冗長だし、何度も取得すると、その回数分処理が走って処理が重くなる
  - [click]
  - 変更への対応が辛い => 例えば、クラス名が変わると全部変える必要が出てくる
  - [click]
  - 何が書いてあるのかわかりづらい => document.querySelectorのコードの意味を毎回追いながら読解するため、読むのに時間がかかる。他人のコードだと尚更
  - [click]
  - 全て変数を使うことで、解決することができる
-->

---
layout: center
---

# 3-1 変数


---
layout: image-right
class: justify-center
---

# 変数とは

<div class="pt-3">
  データ(値)の入れ物(箱)<br>
  箱についている名前が<span class="text-indigo-600 font-bold">変数名</span>であり、箱の中身が実際の値といったイメージ
</div>

<div class="absolute right-0 w-lg">
  <img src="/assets/images/variant-image.png" />
</div>

<!--
  - 変数はイメージでこの図のようなもの
  - データの入れもの、箱、その箱の名前が変数名と言ったイメージ
  - ちなみにエンジニアに変数ってなんですか？って聞くと、普段当たり前の概念としてつかっているので意外と答えに詰まる
　-->

---
layout: image-right
class: justify-center
---

# 変数の定義・使い方

<div class="pt-3">

  プログラミングの「=」は「等しい」という意味ではなく、「右辺を左辺に代入する」という意味<br>
  「let」は「これから変数を定義します」という宣言で、その後ろに変数名を書き、値を代入する

  <div class="pt-4">

  ```js

  let name = "John";

  // コンソールに"John"が出力される
  console.log(name);

  // 文字列の中で変数を使うときは、
  //バッククォートを使い、${}で囲む
  // Hello, John!と表示される
  console.log(`Hello, ${name}!`);
  ```

  </div>

</div>

<div class="absolute right-0 w-lg">
  <img src="/assets/images/variant-assign-image.png" />
</div>

<!--
  - プログラミングの=は「等しい」という意味ではなく、「右辺を左辺に代入する」という意味
  - let => これから変数を定義しますという宣言のようなもので、その後ろに変数名を書いて値を代入する
  - 定義した変数はその後のコードで使える
  - この場合だと、コンソールにJohnという文字列が表示される
  - 文字列の中で変数を使う際には、バッククォートを使い、ドルマークとこのカッコで囲むことで、使用できる

  - このサンプルコードを実際に動かしてみる(じゃんけんゲームには影響しません)


  - __じゃんけんゲームに使われているコードに変数を取り入れる__

  - 問題点解消の確認

  - letで再代入
  - エラーが出るようにするには

　-->

---
layout: center
---

# letとconstの違い

再代入をできるかできないか<br>
constで定義した変数に再代入(更新)しようとするとエラーが出る

<div class="w-full">

```js

const firstName = "shuta";

firstName = "taro"; // エラーが出る

let lastName = "nakai";

lastName = "tanaka"; // 値が更新(再代入)される

```

</div>

<!--
  - constを使った定数は再代入することができず、再代入しようとするとエラーが出る
  - letではエラーが出ない
  - constで定義した定数は後から値を更新しようとするとちゃんとエラーが出てくれるため、予期せぬ更新を防ぎ、より安全なコードを書くことができる

  - __constに書き換えるコードを書く__

  - ここまで書いたコードの答えの場所を共有する

  - まだまだ、直したい部分がたくさんある
-->

---
layout: image-right
class: justify-center
---

# またまた問題点

<ul class="text-xl">
  <li v-click="1">同じような処理を何度も書いている</li>
  <li v-click="2">変更への対応が辛い</li>
  <li v-click="3">何をやっているかわかりづらい</li>
</ul>

<div class="pt-5" v-click="4">
  <p class="absolute text-5xl text-indigo-600 font-bold">すべて関数を使うことで解決できます！</p>
</div>

<div class="absolute right-0 w-lg -z-1">
  <img src="/assets/images/scream2.jpg" />
</div>

<!--
  - [click]
  - 同じような処理を何度も書いている
  - やっている処理自体はボタンで変わらず、それぞれの画像のソースがそれぞれのボタンで違うだけ
  - [click]
  - 変更への対応が辛い
  - 「ぽんっ！」を「ぽんっ！！！！」に変えたい場合、全ての箇所で変更する必要がある
  - [click]
  - ぱっと見では何をやっているかわからない
  - [click]
  - 関数を使えば解決できる

-->

---
layout: center
---

# 3-2 関数

<!--
  - 関数とは
-->

---
layout: image-right
class: justify-center
---

# 関数とは・定義


<div class="pb-3">

いくつかの処理をまとめたもの<br>
関数を定義するには、`function()`と書き、その後`{}`をかいて、
その中にその関数で行う処理を書いていく<br>
関数を定義した際に使用した変数名を用いて、「変数名()」と書くことで関数の中の処理を実行できる

</div>

```js

const introduce = function() {

  // ①挨拶をする
  console.log("Hello!");

  // ②名前を言う
  console.log("I'm nakai.");
}

// introduce関数の呼び出し
introduce();

```

<div class="absolute right-0 w-lg">
  <img src="/assets/images/function-image.png" />
</div>

<style>
  .slidev-code {
    font-size: .9rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - 関数とは、いくつかの処理をまとめたもの
  - この例では、２つの処理をintroduceという関数でまとめている
  - 関数を定義するには、`function()`と書き、その後`{}`をかいて、その中にその関数で行う処理を書く
  - 変数名()と書くことで、関数を実行することができる。これを関数の呼び出しという　

  - __サンプルコードを書いてブラウザで確認__

  - 別の書き方もある
-->

---
layout: center
---

# アロー関数

<div class="text-left">

関数の別の書き方<br>
`function()`を`() =>`に置き換えている

</div>

<div class="w-full">

```js

const introduce = () => {

  // ①挨拶をする
  console.log("Hello!");

  // ②名前を言う
  console.log("I'm nakai.");
}

// introduce関数の呼び出し
introduce();

```

</div>

<!--
  - アロー関数という
  - functionで作る関数とほぼ意味は同じ
  - `function()`のところを`()=>`に置き換えているだけ
  - 最近の開発ではfunctionよりもアロー関数を定義する場合が多く感じる
  - 細かい違いは難しいので、この講座では取り上げない

  - __先ほどのサンプルコードを書き換える__

  - これ以降では、関数はアロー関数をつかって書いていく

  - もう一つ関数の大事な概念を紹介
-->

---
layout: image-right
class: justify-center
---

# 引数とは

<div class="pb-0">

関数に与える追加情報のようなもの<br>
関数を呼び出すときに一緒に値を渡すことで、関数の中で引数の値を利用できる<br>
`() =>`の`()`の中に値を渡すことができ、これを引数と呼ぶ
</div>

```js

const introduceTo = (person) => {

  // ①personに挨拶をする
  console.log(`Hello, ${person}!`);

  // ②名前を言う
  console.log("I'm nakai.");
}

// introduceTo関数の呼び出し
introduceTo("Tanaka") // Hello, Tanaka! I'm nakai.
introduceTo("Yamada");// Hello, Yamada! I'm nakai.

```

<div class="absolute right-0 w-lg">
  <img src="/assets/images/attribute-image.png" />
</div>

<style>
  .slidev-code {
    font-size: .9rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - 引数=関数に与える追加情報
  - 関数の中で引数の値を利用することができる
  - introduceToという関数に引数personを定義している
  - 引数にたなかを渡した時は、Hello, Tanakaになり、山田を渡したときはHello, Yamadaになる

  - __サンプルコードを書いてブラウザで確認__

  - じゃんけんゲームのコードを修正する

  - __グーボタンを押した時の処理を関数に置き換える__

  - チャレンジ[チョキボタン、パーボタンも同じように実装する]

-->

---
layout: new-section
sectionImage: "../assets/images/javascript.png"
---

<h1 class="pl-3 pr-0 text-left -indent-8 ml-8">4. JavaScriptの<br>基本文法を知ろう<br>(後編)</h1>

~ じゃんけんゲームを完成させる ~

<!--
  ということで、引き続き、新しい文法を学んで、じゃんけんゲームを完成させたいと思います。
-->

---
layout: center
---

# 4-0 ここまでの復習

<p></p>

<a class="text-xl font-bold text-indigo-800 block" href="https://hakuhodody-my.sharepoint.com/personal/sd000243_hakuhodody-holdings_co_jp/_layouts/15/onedrive.aspx?FolderCTID=0x0120000D2FDF8E4F61F940A189BA9BD5CEE4CE&id=%2Fpersonal%2Fsd000243%5Fhakuhodody%2Dholdings%5Fco%5Fjp%2FDocuments%2F110%5F%E6%AD%A3%E7%A4%BE%E5%93%A1%E3%83%BB%E5%A5%91%E7%B4%84%E7%A4%BE%E5%93%A1%E5%85%B1%E9%80%9A%2F004%5F%E7%A4%BE%E5%86%85%E5%8B%89%E5%BC%B7%E4%BC%9A%2FWedemy%2FJavaScript%2Fjs%5Flesson%2Ezip&parent=%2Fpersonal%2Fsd000243%5Fhakuhodody%2Dholdings%5Fco%5Fjp%2FDocuments%2F110%5F%E6%AD%A3%E7%A4%BE%E5%93%A1%E3%83%BB%E5%A5%91%E7%B4%84%E7%A4%BE%E5%93%A1%E5%85%B1%E9%80%9A%2F004%5F%E7%A4%BE%E5%86%85%E5%8B%89%E5%BC%B7%E4%BC%9A%2FWedemy%2FJavaScript" target="_blank">ソースコード</a>

<!--
  - 講座の目標から触れる
  - 昨日の内容の振り返り
    - 自己紹介サイト
      - document.querySelector(".class")
    - じゃんけんゲーム
      - 変数(letとconst)
      - 関数(アロー関数、引数)
  - ファイルの場所のアナウンス
-->

---
layout: image-right
class: justify-center
---

# またまたまた問題点

<ul class="text-xl">
  <li v-click="1">同じような処理を何度も書いている</li>
  <li v-click="2">変更への対応が辛い</li>
</ul>

<div class="pt-5" v-click="3">
  <p class="absolute text-5xl text-indigo-600 font-bold">配列と繰り返し処理を使って<br>改善しましょう！</p>
</div>

<div class="absolute right-0 w-lg -z-1">
  <img src="/assets/images/scream3.jpg" />
</div>


<style>
  .slidev-layout p:not(.mb-0) {
    line-height: 1.1;
  }
</style>

<!--
  - まだコードの改善の余地がある
  - [click]
  - まだ同じような処理を何度も書いている
  - グーチョキパーのボタンに関しては、与えている引数がちがうだけで、実行している処理は全て同じ関数
  - (正直このままの方が見やすいという意見もエンジニアの中ではあると思うが、今回は研修のため、あえてここをリファクタリングしていく)
  - [click]
  - もしじゃんけんがレベルアップして、100個くらい出し方が増えたとしたら、このボタンが押された時の処理というのを100回書くことになる
  - [click]
  - 配列と繰り返し処理を使って、複数の要素を同時に扱う方法を学ぶ
-->

---
layout: center
---

# 4-1 配列・for文

<!--
  - 配列とfor文について学ぶ
-->

---
layout: center
---

# 配列とは・定義

複数の値をまとめたもの<br>
配列を定義するには`[a, b, c]`のようにする<br>
配列も1つの値なので、変数に定義できる<br>
配列の中の値にはそれぞれインデックス番号がついていて、0から始まる

<div class="w-full">

```js

const fruits = ["apple", "banana", "orange"];

// ["apple", "banana", "orange"]が表示される
console.log(fruits);

// appleが表示される
console.log(fruits[0]);

// bananaが表示される
console.log(fruits[1]);

// orangeが表示される
console.log(fruits[2]);
```
</div>

<style>
  .slidev-code {
    font-size: .9rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 2rem !important;
  }
</style>

<!--
  - 配列とは複数の値をまとめたもの、このように書く
  - 値をまとめた一つのグループで一つの値なので、変数に定義できる
  - インデックス番号がそれぞれの配列の中の値についている

  - サンプルコードの確認

  - もし、このフルーツが100種類のフルーツの値をコンソールに書き出したいとしたら

-->

---
layout: center
---

# 繰り返し処理・for文

同じ処理を行わせたいときに用いる制御文<br>
例えば、下の例のように数字を1から出力し、最終的に100まで出力する場合、<br>
このままの書き方であれば、100回同じ処理を書く必要があるが、<br>
forを使えばこれだけの記述で実現できる

<div grid="~ cols-2 gap-2" m="-t-2">


<p class="mb-0">100種のバナナの配列から一つずつ出力する</p>

<p class="pt-1 mb-0">同じ処理</p>

```js{4-14}

const fruits = [...Array(100)].map((_, i) => `fruit${i+1}`);

// fruitsという配列には100種類のフルーツが定義されている
console.log(fruits);

console.log(fruits[0]);
console.log(fruits[1]);
console.log(fruits[2]);
console.log(fruits[3]);

// ...
```

```js{4-11}

const fruits = [...Array(100)].map((_, i) => `fruit${i+1}`);

// fruitsという配列には100種類のバナナが定義されている
console.log(fruits);

for (let index = 0; index <= 99; index = index + 1) {
  console.log(fruits[index]);
}
```

</div>

<style>
  .slidev-code {
    font-size: .8rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 1rem !important;
  }
</style>

<!--
  - 繰り返し処理を行うことで対応できる
  - 先ほどの例からフルーツを100種類全部出力するとなった時、左の書き方だとこの２行を100回分書く必要がある
  - for文という構文を使うと3行で書くことができる

  - サンプルコードを確認。
-->

---
layout: image-right
class: justify-center
---

# for文の書き方

<div class="pb-0">


for文では「変数の定義」「条件式」「変数の更新」の3つを括弧の中にかく<br>
括弧の中ではそれぞれをセミコロン（;）で区切る
</div>

```js

for (let number = 1; number <= 100; number = number + 1) {
  console.log(number);
}
```

<div class="absolute right-0 w-lg">
  <img src="/assets/images/for-image.png" />
</div>

<style>
  .slidev-code {
    font-size: .9rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem !important;
  }
</style>

<!--
  - for文の書き方
  - 変数の定義、条件式、変数の更新の処理の3つをカッコの中に順番に
  - それぞれをセミコロンでくぎる。

  - 変数の定義 = forの中で使われる変数の定義、ここでは、numberの定義
  - 変数の更新(3つ目) = 処理が実行されるたび実行される処理
  - 条件式 = この条件を満たす時、処理を行う

  - サンプルコードの解説

  - 条件式で出てきた大なり小なりみたいな記号について
-->

---
layout: image-right
class: justify-center
---

# 大小を比べる演算子

<div class="pb-0">

for文で使用した`<=`は大小を比較する比較演算子と呼ばれる<br>
数学で使われる「≦」「≧」「<」「>」とほぼ同じで、<br>
「≦」は`<=`、「≧」は`>=`で表現される
</div>

```js

// <= は比較演算子
for (let number = 0; number <= 99; number = number + 1) {
  console.log(number);
}
```

<div class="absolute right-0 w-lg">
  <img src="/assets/images/comparison-image.png" />
</div>

<style>
  .slidev-code {
    font-size: .9rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem !important;
  }
</style>

<!--
  - 比較演算子という
  - 数学とかで使われる大なり小なりと同じ
  - 前のページのサンプルコードを確認
-->

---
layout: center
---

# for文を使ってみよう

<p class="text-lg pt-5 text-indigo-600 font-bold">
練習：配列のインデックスとfor文を使ってanimalsの配列から順番に値を取り出し、出力する
</p>

ヒント：配列の長さ(値の個数)は`animals.length`とすることで取得できます。

<p v-click="1">

ヒント2: 配列のインデックス番号は`0`から始まるので、indexが0~3の時に繰り返し処理が実行されるように注意

</p>

<div class="w-full">

```js

const animals = ["dog", "cat", "horse", "lion"];
console.log(animals.length); // 4
```

<div v-click="2" class="pt-1">

<p class="text-xl text-purple font-bold">答え</p>

```js

for (let index = 0; index <= animals.length - 1; index = index + 1) {
  console.log(animals[index]);
};
// または、
for (let index = 0; index < animals.length; index = index + 1) {
  console.log(animals[index]);
};

```

</div>
</div>

<style>
  .slidev-code {
    font-size: .9rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 1rem !important;
  }
</style>

<!--
  - [チャレンジ]for文を使って配列の値をそれぞれ出力してみる

  [click]
  - ヒント

  [click]
  - 答え

  - __CPUの出す手を作る手前までコードを書く__
-->

---
layout: center
---

# 残りの実装

<p></p>

<p class="text-4xl font-bold text-indigo-800 mt-5" v-click>CPUが出す手をランダムにする</p>


<p class="text-4xl font-bold text-indigo-800 mt-5" v-click>じゃんけんの勝ち、あいこ、負けを判定する</p>

<!--
  - CPUが出す手をランダムにする
  - じゃんけんの勝敗を判断するロジックを書く
-->


---
layout: center
---

# CPUが出す手をランダムにする(参考)

`Math.random()`という関数で0から1未満のランダムな値を取得<br>
（`Math.random() * 3`というように3かけることで0~3未満のランダムな値を取得できる）<br>
`Math.floor()`で小数点以下を切り捨てると0,1,2のランダムな整数を取得できる
<br>`handParams[ランダムな0,1,2の整数]`とするとCPUのランダムな手が決まる

<div class="w-full">

```js

const handParams = ["rock", "scissors", "paper"];

// 0~2のランダムな整数を取得
const randomIndex = Math.floor(Math.random() * 3);

console.log(handParams[randomIndex]);
// rock, scissors, paperをランダムに取得できる

```

</div>

<!--
  - 難しいのでここは理解しなくていい、コピペで

  - Math.random()という関数は0から1のランダムな数値を取得できる
  - Math.random() * 3とすると0から3のランダムな値になる
  - それを小数点以下を切り捨てるMath.floor()を使うことで、整数0,1,2をランダムに取得できる

  - サンプルコードを確認
  - __CPUのランダムな出す手の実装をする__

-->

---
layout: center
---

# 残りの実装

<p></p>

<p class="text-4xl font-bold text-indigo-800" v-click="1">じゃんけんの勝ち、あいこ、負けを判定する</p>

<!--
  - ブラウザで足りない機能を確認
  - [click]
  - 後はじゃんけんの勝敗の判定のみ
  - その判定に必要な文法を最後に学ぶ
-->

---
layout: center
---

# 4-2 条件分岐・if文


<!--
  - 条件分岐・if文について
-->

---
layout: image-right
class: justify-center
---

# 条件分岐・if文の書き方

<div class="pb-0">

ある条件が成り立つときだけある処理を行うというプログラム
</div>

```js

const number = 12;

if (number >= 10) {
  console.log("numberは10以上です");
} else if (number >= 5) {
  console.log("numberは5以上です");
} else {
  console.log("numberは5未満です");
}
// numberは10以上です

```

<div class="absolute right-0 w-lg">
  <img src="/assets/images/if-image.png" />
</div>

<style>
  .slidev-code {
    font-size: .9rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 1.5rem !important;
  }
</style>

<!--
- 条件分岐とは、ある条件が成り立つ時だけある処理を行うという処理
  - if文を用いると「もしまるまるならばなになにするという」条件分岐が可能になる
  - ifの後ろのカッコの中に条件式をかいて、それが成り立つ場合に`{}`の中身が実行される
  - else以降は条件を満たさない時になる
  - もう一つ条件がある場合はelse ifとする

  - サンプルコードを確認
-->

---
layout: center
---

# 等価演算子とは


<p class="pt-5">左と右の値が等しいかどうか比べるもの</p>

<div class="w-full">

```js

// 3の時だけアホになる処理
for (let i = 1; i <= 5; i++) {
  if (i === 3) {
    console.log("ｻｱｧｧｧｧｧｧeji33$ﾝ!!??");
  } else {
    console.log(i);
  };
};
```
</div>

<!--
  - 等価演算子は左と右の値が等しいか比べるもの

  - サンプルコードの確認（コピペ）
  - この後のじゃんけんのコードで等価演算子を使う
-->


---
layout: center
---


# 複数の条件式 かつ・または

<p class="pt-5">

  複数の条件を組み合わせるには「かつ」、「または」という表現が必要<br>
  JavaScriptで「かつ」は`&&`、「または」は`||`で表される

</p>

<div class="w-full">

```js

// 3の倍数と３がつく時だけ絶叫する処理
for (let i = 1; i <= 100; i++) {

  // 3の倍数かどうか
  const isMultiple3 = i % 3 === 0;

  // 3を含むかどうか
  const contains3 = String(i).indexOf("3") >= 0;

  // ３の倍数かまたは3を含む場合、数字を叫ぶ
  if (isMultiple3 || contains3) {
    console.log(`${i}!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!`);
  } else {
    console.log(i);
  };
};
```
</div>

<style>
  .slidev-code {
    font-size: .9rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 1.5rem !important;
  }
</style>

<!--
  - じゃんけんのロジックには複数の条件を組み合わせることが必要
  - 条件をand条件、「かつ」で表現するにはアンドマークを２つ重ねる
  - 条件をor条件、「または」で表現するには縦棒を2つ重ねる
  - 某芸人が3の倍数または数字に3を含むときに数字を絶叫する処理
  - 3の倍数かどうかや3を含むかどうかの式はこの講座では触れてない部分なので、理解する必要はない
  - この二つの条件をつなげている縦棒が２つあるところがまたはの意味になる
  - and条件にするにはアンドマークを2つ重ねる

  - __サンプルコードを確認__

-->

---

<h1 class="text-center pr-10">じゃんけんのロジックをかいてみよう</h1>

<ul class="w-7/12 mx-auto">
  <li v-click="1">もし同じ値だったら <span class="text-2xl font-bold text-indigo-800">「あいこ！」</span></li>
  <li class="pt-5" v-click="2">もし
    <ul>
      <li>あなたがグー<code>rock</code>かつCPUがチョキ<code>scissors</code>、または、</li>
      <li>あなたがチョキ<code>scissors</code>かつCPUがパー<code>paper</code>、または、</li>
      <li>あなたがパー<code>paper</code>かつCPUがグー<code>rock</code></li>
    </ul>
    だったら <span class="text-2xl font-bold text-indigo-800">「あなたのかち！」</span>
  </li>
  <li class="pt-5" v-click="3">それ以外だったら <span class="text-2xl font-bold text-indigo-800">「あなたのまけ...」</span></li>
</ul>

<!--
  - じゃんけんのロジックを確認

  - __あいこのところまで実装__
  - [チャレンジ]勝つ場合、負ける場合を実装

  __*コードをかく__

-->

---
layout: image-right
class: "justify-center px-0"
---

# じゃんけんのロジックのコード

```js

if (you === cpu) {
  cardResult.innerHTML = "あいこ！";
} else if (
  (you === "rock" && cpu === "scissors") ||
  (you === "scissors" && cpu === "paper") ||
  (you === "paper" && cpu === "rock")
) {
  cardResult.innerHTML = "あなたのかち！";
} else {
  cardResult.innerHTML = "あなたのまけ...";
}
```

<div class="absolute right-0 w-md" v-click>
  <img src="/assets/images/congratulations.jpg" />
  <img class="absolute -bottom-15 w-md" src="/assets/images/congratulations-text.png" />
</div>

<style>
  .slidev-code {
    font-size: .9rem !important;
    line-height: 1.4 !important;
    text-align: left !important;
    background-color: #efefef !important;
    padding: 0 3rem 1.5rem !important;
  }
</style>

<!--
  - ゲーム完成の確認
-->

---
layout: center
---

# いかがだったでしょうか

<!--
  - 限られた時間の中だったので、説明が不十分だったりした部分もあったかもしれませんが、
  - たくさんコードを追ったと思うので、JavaScriptに慣れるという当初の目標は少しは達成できていれば嬉しい限りです。
-->

---
layout: center
---

<h1>まだまだJavaScriptは奥深い...</h1>

<div v-click>
  <p class="absolute left-1/4 bottom-2/3 text-xl font-bold text-indigo-800">クラス</p>
  <p class="absolute right-2/5 bottom-3/4 text-xl font-bold text-indigo-800">オブジェクト</p>
  <p class="absolute right-1/5 bottom-2/5 text-xl font-bold text-indigo-800">スコープ</p>
  <p class="absolute right-2/3 bottom-2/7 text-xl font-bold text-indigo-800">クロージャー</p>
  <p class="absolute right-3/7 bottom-2/7 text-xl font-bold text-indigo-800">非同期処理</p>
  <p class="absolute right-2/5 bottom-1/7 text-xl font-bold text-indigo-800">prototype</p>
  <p class="absolute right-2/9 bottom-2/7 text-xl font-bold text-indigo-800">即時関数</p>
  <p class="absolute right-2/7 bottom-4/7 text-xl font-bold text-indigo-800">TypeScript</p>
  <p class="absolute right-3/5 bottom-4/7 text-xl font-bold text-indigo-800">React</p>
</div>

<!--
  しかし、まだまだJavaScriptは奥深く、
  この講座では触れられなかった概念も
  [click]
  たくさんあります。
  私もまだまだ勉強中の身ですが、もっと勉強して、
  もしまた皆さんに講座できることがあれば、よりわかりやすく、面白いものを作れるようにできたらなと思います。
-->

---
layout: center
---

# ありがとうございました！

<!--
  ありがとうございました。
-->
