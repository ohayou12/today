## navigation.sendBeacon(url,[data])

[MDN 文档](https://developer.mozilla.org/zh-CN/docs/Web/API/Navigator/sendBeacon)

通过`HTTP POST`方式向服务器异步发送数据。浏览器

```js
const url = "http://localhost:8000/api/report";

const data = {
  type: "click",
  message: "点击了xx图片",
};

const isSend = navigation.sendBeacon(url, [data]);
```
