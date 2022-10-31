| 命令 | 参数                                           |          |
| ---- | ---------------------------------------------- | -------- |
| -X   | [POST,]                                        | 请求方法 |
| -d   | '{"username": "john", "password": "changeme"}' | 请求参数 |
| -H   | Content-Type: application/json                 | 请求头   |

```sh
curl -H "Content-Type: application/json" -X POST -d "id=asd" http://localhost:8080
```

##

```sh

curl -X POST http://localhost:3000/auth/login -d '{"username": "john", "password": "changeme"}' -H "Content-Type: application/json"
```
