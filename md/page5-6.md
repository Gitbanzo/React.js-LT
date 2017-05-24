
### 状態の更新

`this.setState({foo:"bar"});`で状態の更新

直接代入(`this.state.foo = "bar";`)するのは禁止。

`this.setState`を使用する事。

<p style="color:red;">直接代入では`render`が呼ばれず再描画されません。</p>


### 初期値の設定

```javascript
getInitialState: function() {
   return {title: ""}
}
```
