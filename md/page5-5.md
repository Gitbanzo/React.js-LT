
## 5.2 State(状態)
- コンポーネント内部でのみ使用される。
- 表示内容を決定するための単純なデータのみをStateに保存する。

```javascript
//フォームコンポネート
var Form = React.createClass({
    //初期値の設定
    getInitialState: function() {
        return {title: ""}
    },
    //input要素のチェンジイベント
    onChange: function(event) {
        //状態の更新
        //NG : this.state.title = event.target.value;
        this.setState({title: event.target.value});
    },
    render: function() {
        return (
                <input type="text" name="title" value={this.state.title} onChange={this.onChange}/>
        );
    }
});
```
