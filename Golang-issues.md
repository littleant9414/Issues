# Golang

## 🔺 issue

💠 go path

```go
  // issue
  main.go:5:2: package go_code/project01/utils is not in GOROOT (D:\xxx\Go\src\xxx\xxx\utils)

  // system
  windows 10 64bit

  // discussion
  https://stackoverflow.com/questions/61845013/package-xxx-is-not-in-goroot-when-building-golang-project

  // solution
  go env -w GO111MODULE=off
```
