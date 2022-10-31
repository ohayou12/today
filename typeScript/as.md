使用`as`约束

```ts
const Persons = [
  { name: "一花" },
  { name: "二乃" },
  { name: "三玖" },
  { name: "四叶" },
  { name: "五月" },
] as const; 

// type NameType = "一花" | "二乃" | "三玖" | "四叶" | "五月"
// 如果不使用 as const，NameType = string
type NameType = typeof Persons[number]["name"];

// error：不能将类型“"六海"”分配给类型“"一花" | "二乃" | "三玖" | "四叶" | "五月"”。
const name: NameType = "六海";
```
