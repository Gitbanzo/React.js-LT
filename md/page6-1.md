
## 6.ライフサイクル
-----------

コンポーネントが生成されてから破棄されるまでライフサイクルメソッドを提供する。

### 生成時(マウント)
下記順番で呼ばれる。
- getDefaultPorps
- getInitialState
- componentWillMount
- render
- componentDidMount

### 生成後(アップデート)
- componentWillRecieveProps
- shouldComponentUpdate
- componentWillUpdate
- render
- componentDidUpdate

### 破棄(アンマウント)
- componentWillUnmount
