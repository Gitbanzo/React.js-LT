
**componentDidMount**

初回の描画が成功して実際のDOMが表示されると、componentDidMountの中で
React.findDOMNode(this)経由で実際のDOMにアクセスすることが可能。
実際のDOMにアクセスすることが目的。
例えば表示された要素の高さを調べたり、タイマーを設定したりする場合、もしくはjQueryのプラグインを利用する場合
などに使用。

```
React.createClass({
    componentDidMount() {

    },
    ...
});

```
