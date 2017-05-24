

### 2.2.2 babelify
Browserifyの処理中にbabelを処理を組み込むモジュール
- [babel/babelify: Browserify transform for Babel](https://github.com/babel/babelify)

BabelはJSX,AltJSやES6(ES2015)をES5にコンパイル、import/export構文をrequire構文に変換してくれる。
- [Babel · The compiler for writing next generation JavaScript](http://babeljs.io/)

インストール
```
$ npm install --save-dev babelify
$ npm install --save-dev babel-preset-es2015 babel-preset-react
```

#### 実行
```
browserify ./src/app.js -o ./dist/bundle.js -t [ babelify --presets [ es2015 react ] ]
```
