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

💠 go path (redis)

```go
  // issue
  could not import github.com/gomodule/redigo/redis (cannot find package "github.com/gomodule/redigo/redis" in any of 
  xxx\xxx\xxx\xxx  (from $GOROOT)

  // system
  windows 10 64bit

  // discussion
  https://myapollo.com.tw/zh-tw/golang-go-module-tutorial/

  // solution
  1. cd [project]
  2. go mod init github.com/[username]/[myproject]
  3. go get -u github.com/gomodule/redigo/redis
  4. [project]/[file].go => import "github.com/gomodule/redigo/redis"
```

💠 go version

```go
  // issue
 xxx redeclared in this block previous declaration at ...

  // system
  windows 10 64bit

  // solution
  must clean entire old version files before install new version
```
