# REPLを使う

REPLとはRead-Eval-Print-Loopのことで、インタラクティブにNode.jsを実行できます。
Node.jsの利用シーンはwebサーバやCLIツールが多いですが、
REPLに慣れておくと動作確認などに便利です。

REPLを起動するには

```
$ node
```

をターミナルで実行します。`$`はターミナルのプロンプトを示すものです。

計算もできます。

```
> 1+2
3
```

終了するにはCtrl-Dか`.exit`とします。

```
> .exit
```

もうすこし複雑な計算をしてみましょう。

```
> [1,2,3,4].reduce((a,b)=>(a+b),0)
10
```

関数を使うとさらにいろいろなこともできるでしょう。

```
> p=x=>x*x
> f=(x,g)=>x.map(g)
> f([1,2,3,4],p)
```

## 課題

- REPLでいろいろ実行してみる
  - 数値計算、文字列処理、アスキーアート

## 参考情報

- https://nodejs.org/dist/latest-v6.x/docs/api/repl.html