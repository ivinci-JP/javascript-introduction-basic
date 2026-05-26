# if文(条件分岐)

最も基本的な条件分岐の方法として`if`文を紹介します。
`if`文ではある条件が満たされた場合のみ実行される処理を書くことができます。

## 構文の説明

if文は大きく分けて「条件式」と条件が満たされた場合に実行される処理で構成されています。

```js
if (/* 条件式 */) {
    /* 条件式がtrueの場合に実行される処理 */
}
```

「条件式」が`true`なら`{...}`の内側が実行され、

```js
if (true) {
    console.log('実行される');
}
```

「条件式」が`false`なら`{...}`の内側は実行されません。

```js
if (false) {
    console.log('実行されない');
}
```

## 使用方法

通常は「条件式」には`true`や`false`を直接書かず、
[boolean(真偽値型)](/04-data-type/boolean.html)のページで紹介した論理演算子や比較演算子を活用して、条件を記述します。
たとえば、

```js
const age = 21;

if (age >= 20) {
    console.log(`喫煙可`);
}
```
や
```js
const name = 'トルネコ';

if (name !== 'ロト') {
    console.log(`勇者じゃない`);
}
```
などです。

### もっと複雑な条件分岐

`if`文では条件を満たす場合の処理を書くことができますが、
条件を満たさない場合の処理を書く方法が`else`です。
`else`は`if`文とセットで使用します。

```js
if (/* 条件式 */) {
    /* 条件式がtrueの場合に実行される処理 */
} else {
    /* 条件を満たさない場合の処理 */
}
```

先程のサンプルコードを拡張してみましょう。

```js
const age = 21;

if (age >= 20) {
    console.log(`喫煙可`);
} else {
    console.log(`喫煙不可`);
}
```
や
```js
const name = 'トルネコ';

if (name !== 'ロト') {
    console.log(`勇者じゃない`);
} else {
    console.log(`勇者`);
}
```

## さらに複雑な条件分岐

`if`と`else`を組み合わせることで、もっと複雑な条件式も書くことができます。

```js
if (/* 条件式1 */) {
    /* 条件式1がtrueの場合に実行される処理 */
} else if (/* 条件式2 */) {
    /* 条件式2がfalseの場合に実行される処理 */
} else if (/* 条件式3 */) {
    /* 条件式3がfalseの場合に実行される処理 */
} else {
    /* 条件を満たさない場合の処理 */
}
```

例えばこの様に、幾つでも条件を追加することができます。

```js
const age = 18;

if (age < 6) {
    console.log('幼児');
} else if (age < 13) {
    console.log('小学生');
} else if (age < 16) {
    console.log('中学生');
} else if (age < 19) {
    console.log('高校生');
} else if (age < 23) {
    console.log('大学生');
} else {
    console.log('その他');
}
```

## 実際にいじってみる

[このリンク](https://paiza.io/projects/Kh_JAJljfW2P2Hmo51TcaA)を開いて、
サンプルコードの条件式や変数の値を変更してみて、動作を確認しましょう。
