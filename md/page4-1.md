
## 4.JSX
JSX(JavaScript XML)は、Reactコンポーネント内でマークアップ言語を記述するためのシンタックス。

JSX なしでも開発は可能。

```
//HTML
<h1 class="lead">React</h1>

//JSX
render:function(){
    return(<h1 className="lead">React</h1>);
}
//Without JSX
render:function(){
   return(
      React.createElement('h1', {className: "lead"}, "React");
   );
}
```

JSXを使用することで**可読性**があがるので使ってほうがよい。

ただし、JSXを使用する場合コンパイルが必要になる。

方法として
- オンラインで変換: [cdnjs -babel-core](https://cdnjs.com/libraries/babel-core)

```
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.23/browser.min.js"></script>
```

- オフラインで変換: babelifyなど

[サンプルソース -Lession2](https://dl.dropboxusercontent.com/u/23360824/lt/react.js_lession/lession2/index.html)
