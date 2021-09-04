# Nuxtjs

## 🔺 issue

💠 install

```javascript
  // issue
  WARN  Though the "loose" option was set to "false" in your @babel/preset-env config,
  it will not be used for @babel/plugin-proposal-private-property-in-object since the "loose" mode option was set to "true" for @babel/plugin-proposal-private-methods.
  The "loose" option must be the same for @babel/plugin-proposal-class-properties,
  @babel/plugin-proposal-private-methods and @babel/plugin-proposal-private-property-in-object (when they are enabled): you can silence this warning by explicitly adding
  ["@babel/plugin-proposal-private-property-in-object", { "loose": true }]
  to the "plugins" section of your Babel config.

  // system
  windows 10 64bit

  // discussion
  https://stackoverflow.com/questions/68663581/latest-nuxt-v2-15-7-install-with-babel-loose-option-warnings

  // solution
  1. by add below to nuxt.config.js :
  build: {
    babel: {
      plugins: [
        '@babel/plugin-proposal-class-properties',
        '@babel/plugin-proposal-private-methods',

        // or with JUST the line below 
        ['@babel/plugin-proposal-private-property-in-object', { loose: true }]
      ],
    },
  }
```
