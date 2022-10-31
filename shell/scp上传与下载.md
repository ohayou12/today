## scp 下载服务器文件到本地

可选项
- -C（**大写C**）复制过程中压缩文件或目录
- -r 递归目录及子目录
- -P（**大写P**） 指定端口。例：`-P8808`
- -p（**小写P**）保留文件访问及修改

```sh
# scp [option] <server username>@<server ip>:<server path> <local path>

scp user@123.123.123.123:/home/dist ~/dist 

```

## scp 上传本地文件到服务器

可选项
- -C（**大写C**）复制过程中压缩文件或目录
- -r 递归目录及子目录
- -P（**大写P**） 指定端口。例：`-P8808`
- -p（**小写P**）保留文件访问及修改

```sh
# scp [option] <local path> <server username>@<server ip>:<server path>

scp ~/dist user@123.123.123.123:/home/dist 

```