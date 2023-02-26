### 查看某次commit中某个文件的修改内容

```sh
# 查询该文件的所有commit，选择目标commit
git log <filename>

# 查看commitID对应的文件的修改内容
git show <commitID> <filename>

```

### 查询某次commit中都修改了哪些文件

```sh
git log <commitID> --stat
```

### 查询某个文件在所有commit中都修改了哪些内容

```sh
git log -p <filename>
```