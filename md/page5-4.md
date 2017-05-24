
### プロパティの定義
`propTypes`でpropの定義と必須を指定する事が可能。
```javascript
propTypes: {
    href: React.PropTypes.string.isRequired, //必須
    name: React.PropTypes.string //任意
}
```

PropType種類
- React.PropTypes.array
- React.PropTypes.bool
- React.PropTypes.func
- React.PropTypes.number
- React.PropTypes.object
- React.PropTypes.string


isRequiredが設定されていた場合
>bundle.js:18925 Warning: Failed propType: Required prop `href` was not specified in `Anchor`. Check the render method of `App`.

[サンプルソース -Lession3](https://dl.dropboxusercontent.com/u/23360824/lt/react.js_lession/lession3/index.html)
