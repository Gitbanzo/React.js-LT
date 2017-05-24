
**componentWillReceiveProps**

コンポーネントのプロパティ（props）は親コンポーネントにより任意のタイミングで変更される。
その場合、componentWillReceivePropsが呼ばれるので、そこで新しいpropsの値を参
照して、それを基にコンポーネントの状態（state）を変更したり、その他の処理を行うことが可
能。

```
React.createClass({
    componentWillReceiveProps: function(nextProps) {
        this.setState({
            likesIncreasing: nextProps.likeCount > this.props.likeCount
        });
    }
});

```

**shouldComponentUpdate**

shouldComponentUpdateを使って最適化すること
で、速度向上の目的で使用する。
trueかfalseを返す必要がある。デフォルトはtrueを返し、falseを返すとrenderが呼ばれなくなる。
propsやstateの比較処理を独自実装する場合に使用する。

```
React.createClass({
    shouldComponentUpdate: function(nextProps, nextState) {
        return nextProps.user !== this.props.user || nextState.user !== this.state.user;
    },
    ...
});

```
