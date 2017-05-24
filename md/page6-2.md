

**getDefaultPorps**

インスタンス作成時に親コンポーネントが値を指定しなかった場合にデフォルト値として使用される。

```
React.createClass({
  getDefaultProps: function() {
    return {name: "Hello!"}
  },
  ...
});

```

**getInitialState**

コンポーネントのインスタンス作成時に状態を初期化するために呼び出される。

```
React.createClass({
  getInitialState: function() {
    return {name: "foo"}
  },
  ...
});

```
