## controller 中设置状态码

```typescript
import { Post,HttpCode,Res } from "@nestjs/common";
...

// 设置状态码
@Post()
@HttpCode(204)
create(@Res() res){
    res.status = 201
    return 'hello world!'
}

// 动态设置状态码
@Post()
create(@Res() res){
    res.status = 201
    return 'hello world!'
}
```

## 重定向

```typescript
import { Get,Response,Redirect } from "@nestjs/common";
...

// 默认状态码为302
@Get()
@Redirect("http://ohayou.top", 302)
login(@Res() res: Response){
    return 'login'
}

// 默认状态码为302
@Get()
@Redirect("http://ohayou.top", 302)
login(@Res() res: Response){
    res.redirect(' http://ohayou.top','404')
    return 'login'
}


```
