# 答え合わせ

## 1

```
1
2
3
```

## 2

```js
console.log("I'm")
console.log("learning")
console.log("JavaScript!")
```

## 3

```js
console.log("月曜日");
console.log("火曜日");
console.log("水曜日");
console.log("木曜日");
console.log("金曜日");
```

## 4

`''`か`""`(引用符)で括られた範囲が文字列です。
文字列の始まりの為の引用符と、終わりの為の引用符はペアである必要があります。

```js
console.log("大盛り無料");
```

## 5

コンソールに出力するためのメソッドは`console.logs`ではなく`console.log`です
```js
console.log("おかわり有料");
```

## 6

プログラムを実行すると`SyntaxError: Unexpected identifier`というエラーが表示されます。このメッセージでは、問題を解決するための方法が直接示されていません。これは、エラーのトラブルシューティングを行う場合によくあることで、予期しない動作を解決するためにコードを詳しく調べる必要があります。

よく見ると、コードの2番目の`console.log`の呼び出しにマークが付いており、この部分に問題があることがわかります。
これはJavaScriptでは各行に1つの文のみが記述されていることが想定されているためです。
この場合、2番目と3番目の`console.log`関数呼び出しを別々の新しい行に移動することで、問題を解決できます。
```
/workspace/Main.js:4
console.log("イヌ") console.log("ネコ") console.log("ハムスター")
                  ^^^^^^^
```

#### 正しいコード:

`console.log(...)`の間に改行とセミコロン（`;`）を挿入しましょう。

```js
console.log("イヌ");
console.log("ネコ");
console.log("ハムスター");
```

## 7

プログラムを実行すると`SyntaxError: Unexpected token '{'`というエラーが表示されます。
関数呼び出しは、波括弧`{}`ではなく丸括弧`()`で囲む必要があります。
```js
console.log("オムライス");
```
