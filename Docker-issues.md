# Docker

## 🔺 issue

💠 docker info(command line)

```javascript
  // issue
  Server: ERROR: Got permission denied while trying to connect to the Docker daemon socket

  // system
  Ubuntu 20.4

  // discussion
  https://newbedev.com/shell-error-got-permission-denied-while-trying-to-connect-to-the-docker-daemon-socket-at-unix-var-run-docker-sock-get-http-2fvar-2frun-2fdocker-sock-v1-24-info-dial-unix-var-run-docker-sock-connect-permission-denied-code-example

  // solution
  1. sudo groupadd [groupname]
  2. sudo chmod 666 /var/run/docker.sock
  3. sudo usermod -aG docker ${USER}
```
