# 【解答】制御構造の練習

## 1

```
繰り返し処理
繰り返し処理
繰り返し処理
```

## 2
```js
for (let i = 1; i < 6; i++) {
    console.log(i);
}
```
または
```js
for (let i = 1; i <= 5; i++) {
    console.log(i);
}
```

## 3

```js
for (let i = 1; i <= 9; i++) {
    console.log(i + 'の段');
    for (let j = 1; j <= 9; j++) {
        console.log(i + ' * ' + j + ' = ' + (i * j));
    }
}
```
