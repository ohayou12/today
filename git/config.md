### 查看git配置

```sh
git config --list
```

### 设置全局用户名和邮箱

```sh
git config global user.name "yourName"
git config global user.email "yourEmail"
```

### 设置局部用户名和邮箱

```sh
git config user.name "yourName"
git config user.email "yourEmail"
```

### 删除、添加远程地址

```sh
# 删除
git remote rm origin

# 添加
git remote add origin [gitUrl]
```
