```
JS_Parse_Error {
  message: 'SyntaxError: Unexpected character \'`\'',
  filename: 'bundle.js',
  line: 2017,
  col: 14,
  pos: 62514,
  stack: 'Error\n
    at new JS_Parse_Error (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:1545:18)\n
    at js_error (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:1553:11)\n
    at parse_error (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:1677:9)\n
    at Object.next_token [as input] (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:1949:9)\n
    at next (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2078:25)\n
    at vardefs (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2512:48)\n
    at const_ (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2533:27)\n
    at eval (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2271:30)\n
    at eval (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2139:24)\n
    at block_ (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2432:20)\n
    at eval (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2404:25)\n
    at function_ (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2410:15)\n
    at expr_atom (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2625:24)\n
    at maybe_unary (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2795:19)\n
    at expr_ops (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2830:24)\n
    at maybe_conditional (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2835:20)\n
    at maybe_assign (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2859:20)\n
    at maybe_assign (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2867:32)\n
    at expression (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2878:20)\n
    at simple_statement (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2317:55)\n
    at eval (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2186:19)\n
    at eval (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2139:24)\n
    at block_ (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2432:20)\n
    at eval (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2404:25)\n
    at function_ (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2410:15)\n
    at expr_atom (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2625:24)\n
    at maybe_unary (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2795:19)\n
    at expr_ops (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2830:24)\n
    at maybe_conditional (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2835:20)\n
    at maybe_assign (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2859:20)\n
    at expression (eval at <anonymous> (/Users/yuta_hiroto/Programming/webpack2.1.0-verification/node_modules/uglify-js/tools/node.js:28:1), <anonymous>:2878:20)' }
```

criminal: babal-loader  
cause: babel-loader can't load options property.  
babel-loader's ci: https://travis-ci.org/babel/babel-loader/jobs/166650418#L612  
supplemental:  
babel-loader has a query of options(https://github.com/webpack/webpack/issues/3118#issuecomment-252997261) when `webpack@1.13.2`.  

```
?{"babelrc":false,"cacheDirectory":"/tmp/","presets":["react",["es2015",{"modules":false}],"stage-0"],"env":{"development":{"plugins":[["react-transform",{"transforms":[{"transform":"react-transform-hmr","imports":["react"],"locals":["module"]},{"transform":"react-transform-catch-errors","imports":["react","redbox-react"]}]}],"transform-runtime","add-module-exports","transform-class-properties"]},"production":{"plugins":["transform-runtime","add-module-exports","transform-class-properties"]}}}
```

However, babel-loader can not get options when `webpack@2.1.0-beta.25`.  
The loaderOptions (this.query is empty string) is empty object.  

here: https://github.com/babel/babel-loader/blob/master/index.js#L80  
