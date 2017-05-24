
**サンプル**

```
React.createClass({
  _onClick(event){
    alert(event.target.value); //押したよ!
  },
  render() {
    return <button type="button" className="btn btn-info" onClick={this._onClick} value="押したよ!">Event</button>;
  }
});

```
