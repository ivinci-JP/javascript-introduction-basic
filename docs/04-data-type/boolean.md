# boolean(真偽値型)

`boolean`（真偽値）について説明するのはこれが始めてです。
真偽値はプログラミングを習得する上で、とても重要なデータ型なので、
ぜひ文字列や数値と同じ様に使いこなせる様になりましょう。

`boolean`には２つの値しかありません。
`true`（真）と`false`（偽）です。

- `true` / `false`
- `1` / `0`
- 真 / 偽
- はい / いいえ
- 肯定 / 否定
- 合 / 否
- 要 / 否
- 可 / 不可
- ON / OFF

`boolean`はこの様な二択の値を表現します。

## 論理演算子

### 論理和（`OR`）演算子

論理和を求めるには`||`（論理和演算子）を使用します。
`||`の左辺と右辺の内、1つ以上が`true`である場合に`true`となり、
どちらも`false`の場合に`false`となります。

```js
console.log(true  || false); // true
console.log(false || true);  // true
console.log(true  || true);  // true
console.log(false || false); // false
```

### 論理積（`AND`）演算子

論理積を求めるには`&&`（論理積演算子）を使用します。
`&&`の左辺と右辺の両方が`true`の場合に`true`となり、
１つでも`false`の場合は`false`となります。

```js
console.log(true  && false); // false
console.log(false && true);  // false
console.log(true  && true);  // true
console.log(false && false); // false
```

### 否定 (`NOT`)演算子

論理値の否定値、反転値を求めるには`!`（論理否定演算子）を使用します。
`OR`や`AND`は左辺と右辺の2つの値を評価する二項演算子ですが、
`NOT`は1つの値を評価する単項演算子です。
論理値の直前に記述することで、評価対象の論理値を反転します。
`!true`なら`false`と評価され、`!false`なら`true`と評価されます。

```js
console.log(!true);  // false
console.log(!false); // true
```

## 比較演算子

2つの値を比較し、`boolean`値で結果を返す演算子です

### 厳密等価演算子 (`===`)

2つの値が**等しいこと**を検査し、真偽値で結果を返します。

```js
// 数値の比較
console.log(123 === 123); // true
console.log(123 === 124); // false

// 文字列の比較
console.log('abc' === 'abc'); // true
console.log('ABC' === 'ABC'); // true
console.log('abc' === 'ABC'); // false

// 真偽値の比較
console.log(true === true); // true
console.log(false === false); // true
console.log(true === false); // false
```

### 厳密不等価演算子 (`!==`)

2つの値が**等しくないこと**を検査し、真偽値で結果を返します。

```js
// 数値の比較
console.log(123 !== 123); // false
console.log(123 !== 124); // true

// 文字列の比較
console.log('abc' !== 'abc'); // false
console.log('ABC' !== 'ABC'); // false
console.log('abc' !== 'ABC'); // true

// 真偽値の比較
console.log(true !== true); // false
console.log(false !== false); // false
console.log(true !== false); // true
```

### 大なり演算子 (`>`)

大なり演算子 (`>`)は、左辺の値が右辺の値より**大きい**場合は`true`を返し、それ以外の場合は`false`を返します。

```js
console.log(2 > 3); // false
console.log(3 > 2); // true
console.log(2 > 2); // false
```

### 大なりイコール演算子 (`>=`)

大なりイコール演算子 (`>=`)は、左辺の値が右辺の値**以上**の場合は`true`を返し、それ以外の場合は`false`を返します。

```js
console.log(2 >= 3); // false
console.log(3 >= 2); // true
console.log(2 >= 2); // true
```

### 小なり演算子 (`<`)

小なり演算子 (`<`)は、左辺の値が右辺の値より**小さい**場合は`true`を返し、それ以外の場合は`false`を返します。

```js
console.log(2 < 3); // true
console.log(3 < 2); // false
console.log(2 < 2); // false
```

### 小なりイコール演算子 (`<=`)

小なりイコール演算子 (`<=`)は、左辺の値が右辺の値**以下**の場合は`true`を返し、それ以外の場合は`false`を返します。

```js
console.log(2 <= 3); // true
console.log(3 <= 2); // false
console.log(2 <= 2); // true
```
