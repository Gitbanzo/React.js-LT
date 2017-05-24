
### プロパティを渡す
`<Title name="..."/>`の`name`部分

任意に指定可能。

### プロパティの取得
`this.props.foo`で取得可能

`foo`の部分は呼び出し元で設定した属性になる。

サンプルソースでは`name`になる。

### デフォルト値の設定

`getDefaultProps`を使用する事でデフォルト値の設定が可能。

```javascript
getDefaultProps: function() {
   return { name: "Title" }
}
```
