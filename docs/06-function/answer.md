# 【解答】関数の拡張

## 1

[解答](https://paiza.io/projects/-Qkc-Z6bNZ31gXmCNglOkQ)の一例です。

```js
function greet(name, age, gender) {
    const greetingMessage = name + 'です。こんにちは。' + age + '歳です。';
    if (gender === '男') {
        return '僕は' + greetingMessage;
    }
    if (gender === '女') {
        return '私は' + greetingMessage;
    }
    return greetingMessage;
}
```
