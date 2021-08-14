# 🔎 Vue

## 🔺 Issue

🔸  ERROR  Error: Rule can only have one resource source 

  ```javascript
    //  issue :
     ERROR  Error: Rule can only have one resource source (provided resource and test + include + exclude)...

    // system :
    windows 10 64bit

    // discussion
    https://stackoverflow.com/questions/66082397/typeerror-this-getoptions-is-not-a-function

    // solutioin : 
    yarn version : v1.22.11
    1. Delete package-lock.json
    2. Delete node modules
    3. Used yarn: Yarn install
    4. yarn serve

  ```

🔸  Syntax Error: TypeError: this.getOptions is not a function

  ```javascript
    //  issue :
     Syntax Error: TypeError: this.getOptions is not a function ...

    // system :
    windows 10 64bit

    // discussion
    https://stackoverflow.com/questions/66082397/typeerror-this-getoptions-is-not-a-function

    // solution : 
    package.json => "sass-loader": "^10",
  ```
