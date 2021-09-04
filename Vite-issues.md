# Vite

## 🔺 issue

💠 install

```javascript
  // issue
  Could not install from "Files\nodejs\node_cache\_npx\14456" as it does not contain a package.json file.

  // system
  windows 10 64bit

  // discussion
  https://github.com/zkat/npx/issues/146
  https://stackoverflow.com/questions/57747895/npm-err-code-enolocal-npm-err-could-not-install-from-ibrahi-appdata-roaming-n

  // solution
  command line : npm config get cache
  show : C:\xxx\xxx xxx\AppData\Roaming\npm-cache
  change to : C:\Users\xxx~xxx\AppData\Roaming\npm-cache
  // the cache path cannot include space