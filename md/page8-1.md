
## 8.Mixin
-------------------------

コンポーネントの共通な振る舞いを共通化することが可能。
オブジェクトを配列として指定する。
mixinとコンポーネントで同一名のメソッドを定義するとエラーになる。
```javascript
//ミックインで使うオブジェクト
var Logger = {
    log: function(val){
      console.log(val);  
    }
}

var Hello = React.createClass({
  mixins: [Logger], //ミックスインを使う
  render() {
    this.log("render");
    return <div>Hello</div>
  }
});
```
