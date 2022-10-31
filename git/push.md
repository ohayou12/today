### 本地分支提交到远程分支

```sh
git push  origin [originBranchName]

# 简写
gp  origin [originBranchName]
```

### 本地分支提交到远程分支（并设置默认推送分支）

```sh
# -u 是 --set-upstream 的简写
# -u 指定默认主机(此处为origin)，后续可通过 git push 直接推送到该主机分支
git push -u origin [originBranchName]

# 简写
gp -u origin [originBranchName]
```
