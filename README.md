# Xのカスタマイズ!
2023年7月24日。

Twitterの名が"X"へ変わり、一ユーザーとして驚きを隠せなかったためロゴ部分で遊んでみる。

お使いのブラウザのDevToolsのコンソールで実行してみよう!
## Xロゴ前に文字列を入れたい!
```JavaScript
let word = "文字列";
document.querySelector('[aria-label="Twitter"] div').insertAdjacentHTML("beforeend", `<span style="font-size: 1.7rem;font-weight: normal;">${word}</span>`);
```
<img width="162" alt="image" src="https://github.com/kawa-nobu/x_customize/assets/44832116/7b69d2c5-388d-43e4-80f1-58ea355e7115">

## Xロゴ後に文字列を入れたい!
```JavaScript
let word = "文字列";
document.querySelector('[aria-label="Twitter"] div').insertAdjacentHTML("afterbegin", `<span style="font-size: 1.7rem;font-weight: normal;">${word}</span>`);
```
<img width="165" alt="image" src="https://github.com/kawa-nobu/x_customize/assets/44832116/999e68cc-e166-4cf5-aa0b-06ce9fc65766">
