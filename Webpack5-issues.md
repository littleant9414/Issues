# 🔎 Webpack5


## 🔺 Issue

🔸 vue

  ```javascript
    //  issue :
    You forgot to add 'mini-css-extract-plugin' plugin 

    // system :
    windows 10 64bit

    // discussion : 
    https://github.com/stephencookdev/speed-measure-webpack-plugin/issues/167

    // solutioin : 
    1. mini-css-extract-plugin seems conflict with  SpeedMeasurePlugin.
    2. in my case, i remove `SpeedMeasurePlugin` from my `webpack.config.js` and `mini-css-extract-plugin` works fine.
  ```
  