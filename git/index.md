### 合并时间线

拉取代码时使用`git pull --rebase`替代`git pull`

```sh

```

### 查看某块代码的作者

```sh
# 查看文件编辑历史
git blame [filename]

# 查看10-20行的编辑历史
git blame -L 10,20 [filename]

# 查看10-30行的编辑历史
git blame -L 10,+20 [filename]
```

### 显示 commit 记录、时间线

```sh
git log --oneline --graph --decorate --color

# 简写
glog
```

### 显示 commit 记录并显示详细信息

执行`git log --pretty=raw`

- commit commitId
- tree 表示当前版本中所有目录和文件的 MD5（如果不修改内容创建 2 个 commit，则它们的 tree 相同）
- parent 父节点 commitId
- author 作者
- committer 作者

```sh
git log --pretty=raw

#
commit 1a728973a250fd85e969fd3a8e2fe75da1a31435
tree c5d532e1d629b173387328337c4451643b8de75d
parent 20920afaf4c04107bd9a6f21ef4759895ac3337c
author ohayou <864633493@qq.com> 1641831771 +0800
committer ohayou <864633493@qq.com> 1641831791 +0800

    feat: commit
```

### 显示全局配置文件的内容

```sh
git config --global -l
```

### 设置别名

```sh
# 设置别名
git config --global --alias.xx "log --oneline --graph --decorate"

# gxx命令实际上将执行 git log --oneline --graph --decorate
gxx
```

### 已存在的项目关联至git
```sh
# 添加远程仓库地址
git remote add origin [远程仓库地址]
# 切换到master分支
git branch -M master
```