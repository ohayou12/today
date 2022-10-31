##

在 watch 中监听的属性默认不会在页面首次渲染时执行，使用`immediate`属性将可以强制 `vue` 在首次加载完成后执行

```javascript
export default {
    ...

    watch: {
        name: {
            immediate: true,
            handler() {
                console.log('我在页面首次渲染完成后将会执行')
            }
        }
    }
}
```
