# 【問題】関数の拡張

## 1

[このリンク](https://paiza.io/projects/AwRCA02lI2crW3QvoeTuhg)を開き、`greet`関数を下記の様に修正してください。

- この関数に更に引数`gender`を１つ追加しましょう。
- `gender`には`'男'`または`'女'`という文字列が渡されます。
- `'男'`が渡された場合は、挨拶文の先頭に`'僕は'`を追加します
- `'女'`が渡された場合は、挨拶文の先頭に`'私は'`を追加します
- `gender`が`'男'`でも`'女'`でもない場合は何も追加しません。
```js
function greet(name, age) {
    const greetingMessage = name + 'です。こんにちは。' + age + '歳です。';
    return greetingMessage;
}
```
