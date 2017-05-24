
### 5.1 Prop(プロパティ)

---------

#### 特徴
- 外部から渡させる値(プロパティ)
- 単一の情報源として使用する。
- propsは不変(イミュータブル)として扱い、コンポーネント内で`this.props`の値を変更したり`this.setProps`を呼び出したりしてはいけない。


```javascript
var Title = React.createClass({
    /* デフォルト値設定 */
    getDefaultProps: function() {
        return {name: "Hello!"}
    },
    render: function() {
        return (
            /* プロパティの取得 */
            <h1>{this.props.name}</h1>
        );
    }
});

var App = React.createClass({
    render: function() {
        return (
            <div>
                /* プロパティを渡す */
                <Title name="React.js Lession"/>
            </div>
        );
    }
});

```
