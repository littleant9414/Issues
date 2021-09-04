# Git

## 🔺 issue

💠 git email

```go
  // issue
  remote: error: GH007: Your push would publish a private email address.

  // system
  windows 10 64bit

  // discussion
   https://cloud.tencent.com/developer/article/1835148

  //  solution
  1. git config --global user.email
  2. go to github settings => Emails => copy 'xxx@users.noreply.github.com' 
  3. git config --global user.email "xxx@users.noreply.github.com"
  4.git commit --amend --reset-author => enter :x to save and exit from vim
  5. git pull 
  6. git push

```
