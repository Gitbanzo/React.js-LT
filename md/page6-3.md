
**componentWillMount**

初回の描画が行われる直前に呼ばれる。
renderメソッドが呼び出される前にコンポーネ
ントの状態を変更したい場合、ここで行う。

```
React.createClass({
 componentWillMount(){

 },
 ...
});

```

**render**

仮想DOMの生成。省略できないライフサイクルメソッド。

```
React.createClass({
  render: function() {
    return (
        <h1>Title</h1>
    );
  }
});

```
