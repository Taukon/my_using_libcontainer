
### ファイルシステム作成

```
$ docker pull alpine
$ docker run --name alpine alpine
$ docker export alpine > alpine.tar
$ mkdir rootfs
$ tar -C rootfs -xvf alpine.tar
```

### 実行
```
$ go build -o mycontainer
$ sudo ./mycontainer
```