> 可选参数大写表示强制，如：
>
> - `gb -m [newName]`分支重命名
> - `gb -M [newName]`强制重命名

### 查看本地所有分支

```sh
git branch
# 简写
gb
```

### 查看远程所有分支

```sh
git branch -r
# 简写
gbr
```

### 查看本地与远程所有分支

```sh
git branch -a
# 简写
gba
```

### 重命名当前分支

```sh
git branch -M [newBranchName]
# 简写
gb -M [newBranchName]
```

### 重命名非当前分支

```sh
git branch -M [originBranchName] [newBranchName]
# 简写
gb -M [originBranchName] [newBranchName]
```

### 创建一个本地分支

```sh
git branch [newBranchName]

# 简写
gb [newBranchName]
```

### 创建一个本地分支并切换到该分支

```sh
git checkout -b [branchName]

# 简写
gco -b [branchName]
```

### 以远程分支为源，创建一个本地分支

```sh

git checkout -b [branchName] origin/[remoteBranchName]

# 简写
gco -b [branchName] origin/[remoteBranchName]
```

### 删除本地分支

```sh

git branch -d [branchName]

# 简写
gb -d [branchName]

# 强制删除
gb -D [branchName]
```
