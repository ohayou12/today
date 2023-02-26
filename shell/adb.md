## ADB(Android Debug Bridge)

### 获取序列号：

```sh
adb get-serialno
```

### 查看连接计算机的设备：

```sh
adb devices
```

### 重启机器：

```sh
adb reboot
```

### 重启到 bootloader，即刷机模式：

```sh
adb reboot bootloader
```

### 重启到 recovery，即恢复模式：

```sh
adb reboot recovery
```

### 查看 log：

```sh
adb logcat
```

### 终止 adb 服务进程：

```sh
adb kill-server
```

### 重启 adb 服务进程：

```sh
adb start-server
```

### 获取机器 MAC 地址：

```sh
adb shell cat /sys/class/net/wlan0/address
```

### 获取 CPU 序列号：

```sh
adb shell cat /proc/cpuinfo
```

### 安装 APK：

```sh
adb install <apkfile> //比如：adb install baidu.apk
```

### 保留数据和缓存文件，重新安装 apk：

```sh
adb install -r <apkfile> //比如：adb install -r baidu.apk
```

### 安装 apk 到 sd 卡：

```sh
adb install -s <apkfile> // 比如：adb install -s baidu.apk
```

### 卸载 APK：

```sh
adb uninstall <package> //比如：adb uninstall com.baidu.search
```

### 卸载 app 但保留数据和缓存文件：

```sh
adb uninstall -k <package> //比如：adb uninstall -k com.baidu.search
```

### 启动应用：

```sh
adb shell am start -n <package_name>/.<activity_class_name>
```

### 查看设备 cpu 和内存占用情况：

```sh
adb shell top
```

### 查看占用内存前 6 的 app：

```sh
adb shell top -m 6
```

### 刷新一次内存信息，然后返回：

```sh
adb shell top -n 1
```

### 查询各进程内存使用情况：

```sh
adb shell procrank
```

### 杀死一个进程：

```sh
adb shell kill [pid]
```

### 查看进程列表：

```sh
adb shell ps
```

### 查看指定进程状态：

```sh
adb shell ps -x [PID]
```

### 查看后台 services 信息：

```sh
adb shell service list
```

### 查看当前内存占用：

```sh
adb shell cat /proc/meminfo
```

### 查看 IO 内存分区：

```sh
adb shell cat /proc/iomem
```

### 将 system 分区重新挂载为可读写分区：

```sh
adb remount
```

### 从本地复制文件到设备：

```sh
adb push <local> <remote>
```

### 从设备复制文件到本地：

```sh
adb pull <remote> <local>
```

### 列出目录下的文件和文件夹，等同于 dos 中的 dir 命令：

```sh
adb shell ls
```

### 进入文件夹，等同于 dos 中的 cd 命令：

```sh
adb shell cd <folder>
```

### 重命名文件：

```sh
adb shell rename path/oldfilename path/newfilename
```

### 删除 system/avi.apk：

```sh
adb shell rm /system/avi.apk
```

### 删除文件夹及其下面所有文件：

```sh
adb shell rm -r <folder>
```

### 移动文件：

```sh
adb shell mv path/file newpath/file
```

### 设置文件权限：

```sh
adb shell chmod 777 /system/fonts/DroidSansFallback.ttf
```

### 新建文件夹：

```sh
adb shell mkdir path/foldelname
```

### 查看文件内容：

```sh
adb shell cat <file>
```

### 查看 wifi 密码：

```sh
adb shell cat /data/misc/wifi/\*.conf
```

### 清除 log 缓存：

```sh
adb logcat -c
```

### 查看 bug 报告：

```sh
adb bugreport
```

### 获取设备名称：

```sh
adb shell cat /system/build.prop
```

### 查看 ADB 帮助：

```sh
adb help
```

### 跑 monkey：

```sh
adb shell monkey -v -p your.package.name 500
```
