
ライフサイクルメソッドも利用可能
```javascript
var foo = {
  getDefaultProps: function() {
    return {
      title: "mixin"
    };
  },
  getInitialState() {
    return {
      value: "mixin"
    };
  }
}

var Hello = React.createClass({
  mixins: [foo],
  render() {
    return <div>{this.props.title} {this.state.value}</div>
  }
});
```
