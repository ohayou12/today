## 定制 npm 包

### 1、发布 npm 包之前需要先拥有 npm 账号

[npm 官网](https://www.npmjs.com/)

```sh

# 登录npm
npm login

# 发布包
npm publish

# 发布包(scoped)
npm publish --access [public/restricted]
```

## 本地调试开发包

- 链接包：在根目录执行`yarn link`，此时`package.json`中的`name`作为包名被软链接到`yarn`全局安装目录
- 安装包：在开发项目执行`yarn link packageName`

## 更新包版本号

- update_type:
- 1. major: 主版本号
- 2. minor: 次版本号
- 3. patch: 修订号

```sh
# npm version <update_type>

# prev version 1.1.1
npm version patch
# next version 1.1.2

```
