
## Not Suport Event

React.jsがサポートしてないイベントやjQueryプラグインのイベントなどを使用したい場合は
componentDidMount()にイベントを登録する。

```
var Box = React.createClass({
  getInitialState() {
    return {
      windowWidth: window.innerWidth
    };
  },
  handleResize(e) {
    this.setState({windowWidth: window.innerWidth});
  },
  componentDidMount() {
    window.addEventListener('resize', this.handleResize);
  },
  componentWillUnmount() {
    window.removeEventListener('resize', this.handleResize);
  },
  render() {
    return <h1>Current window width: {this.state.windowWidth}</h1>;
  }
});
React.render(<Box />, mountNode);

```
