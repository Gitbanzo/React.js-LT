
#### `React.createClass`でコンポーネントを作成する。

```javascript
var Title = React.createClass({
    // 必須
    render: function(){
        return (
           /* 要素 */
        );
    }
});
```

- コンポーネントを組み合わせて作っていく。
- 複数のコンポーネントは返せない。

```
// NG
var Title = React.createClass({
  render() {
    return (
      <div>
        <h1>hello</h1>
      </div>
      <div>
        <h2>World!</h2>
      </div>
    )
  }
});

// OK
var Title = React.createClass({
  render() {
    return (
      <div>
        <div>
          <h1>hello</h1>
        </div>
        <div>
          <h2>World!</h2>
        </div>
      </div>
    )
  }
});

```
