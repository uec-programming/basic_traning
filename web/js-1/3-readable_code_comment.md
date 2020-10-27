---
tags: Web_JavaScript_1
lang: ja-jp
breaks: false
---

<style>
iframe{
  border: none;
  width: 100%;
  min-height: 12em;
}
</style>

# 2-3 読みやすいコードを書こう

今回は、プログラムを読む人にとってわかりやすいコードを書きましょう。

## 改行と空白

前回は1つの文を書きました。文はいくつも続けて書くことができます。

```javascript=
alert('こんにちは');alert('元気ですか？');
```

このまま1つの行に続けて書いていくと読みにくくなりそうです。文が終わるたびに改行した方が良さそうです。

```javascript=
alert('こんにちは');
alert('元気ですか？');
```

改行を入れた場合と入れない場合で、結果に違いはありません。単語の途中で区切らなければ半角スペースや改行はどこに入れても良いので、読みやすいコードを書くように心がけましょう。

:::success
:o: 正しく実行でき、読みやすい例
```javascript=
alert('こんにちは');
alert('元気ですか？');
```
:::

:::warning
:warning: 正しく実行できるが、読みにくい例
```javascript=
alert   (  'こんにちは'
    )      ;  alert(
'元気ですか？'
)
;
```
:::

:::danger
:x: 正しく実行できない例
```javascript=
a  l  e rt ('こんにちは');
ale  r t('元気ですか？');
```
:::

> [color=#d400f5]
> 
> ### :rocket: **練習**
> 
> 自由に空白や改行を追加して、振る舞いを試してみましょう。また、あえて間違った例を実行して、赤字のエラーが表示されることを確認してみましょう。
> <iframe src="https://uec-programming.github.io/basic_training/web-sample/editor.html?code=alert('こんにちは');\nalert('元気ですか？');"></iframe>
> 

## コメント

コードを書いてしばらく経つと、そのコードの意味が思い出せなくなることがあります。後で見返したときにわかるよう、コードの中には自分の言葉で**コメント**を残すことができます。日本語で書くことができます。コメントの部分は実行時には無視されるので何を書いても構いません。また、コメントは他の人がコードを読むときにも役立ちます。

```javascript=
// 1行のコメント

alert('こんにちは'); // ここもコメント

/* ここからここまで */

/* ここから始まって
複数行コメントが
終わるのは
ここまで */
```

1行コメントは、`//`から行末までがコメントになります。

複数行コメントは、`/*`から`*/`までがコメントになり、改行を挟むことができます。

<!--
JSPrimer
https://jsprimer.net/basic/comments/

MDN
https://developer.mozilla.org/ja/docs/Web/JavaScript/Guide/Grammar_and_types#Comments
-->

> [color=#d400f5]
> 
> ### :rocket: **練習**
> 
> コメントを書いたり消したりして、振る舞いを確かめましょう。
> 
> <iframe src="https://uec-programming.github.io/basic_training/web-sample/editor.html?code=// こんにちはと画面に表示\nalert('こんにちは');\n\nalert('元気ですか？');"></iframe>
> 

> [color=#f5d400]
> ### :pencil2: **まとめ**
> 
> :white_check_mark: **改行**や**空白**は、人が読みやすいように使う。  
> :white_check_mark: **コメント**を使えば、コードの説明などを残すことができる。  
> 

:::info
**:bulb: 学習のコツ**

プログラミングの学習で、わからないことやエラーが出た時には画面を見ながら考えても解決しません。すぐに**教材を振り返るか検索**して解決しましょう。そして、手が止まる時間が3分を超える前に講師に質問しましょう。

そして、それでも難しくてわからない時には、**わからないことをわからないまま**にする覚悟も必要です。学習を進めて慣れていくうちに、理解できるようになっているはずです。
:::