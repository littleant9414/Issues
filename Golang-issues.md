# Golang

## 🔺 issue

💠 go path

```go
  // issue
  folder name can not contain "&" symbol
```

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

💠 go version

```go
  // issue
 xxx redeclared in this block	previous declaration at ...

  // system
  windows 10 64bit

  // solution
  must clean entire old version files before install new version
```
