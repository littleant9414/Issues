# Vue


## 🔺 Notice

  ```javascript
    // 組件樣式問題 : 腳手架按照引入順序渲染畫面
  ```

## 🔺 Issue

🔸 vue

  ```javascript
    //  issue :
    $ vue create vue_test
    bash: vue: command not found

    // system :
    windows 10 64bit

    // solutioin : 
    npm install vue @vue/cli
  ```

🔸 Eslint

```javascript
  // issue : 
  Do not access Object.prototype method 'hasOwnProperty' from target object no-prototype-builtins

  // system
  windows 10 64bit

  // discussion : 
  https://ourcodeworld.com/articles/read/1425/how-to-fix-eslint-error-do-not-access-objectprototype-method-hasownproperty-from-target-object-no-prototype-builtins
  https://cn.eslint.org/docs/rules/no-prototype-builtins

  // solution : 
  Object.prototype.hasOwnProperty.call(obj, key)
```

🔸 install elementUI

```javascript
  // issue
  Error: Cannot find module 'babel-preset-es2015'

  // system
  windows 10 64bit

  // discussion
  https://blog.csdn.net/zy21131437/article/details/108029284

  // solution
  1. yarn add @babel/preset-env -D
  2. modified babel.config.js

  // babel.config.js
  module.exports = {
    presets: ["@vue/cli-plugin-babel/preset", ["@babel/preset-env", { modules: false }]],
    plugins: [
      [
        "component",
        {
          libraryName: "element-ui",
          styleLibraryName: "theme-chalk",
        },
      ],
    ],
  }
```
