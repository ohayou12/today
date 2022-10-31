### 查看所有tag
```sh
git tag
```

### 创建tag（以当前分支最新的commit创建tag）
```sh
git tag <tagName>
```

### 创建tag（以某个特定的commit创建tag）
```sh
git tag -a <tagName> <commitId>

```

### 推送tag到远程仓库

```sh
# 推送多个tag
git push origin <tagName>

# 推送所有tag
git push origin --tags
```