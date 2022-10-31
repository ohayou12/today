## infer

```ts
type NameType = "一花" | "二乃" | "三玖" | "四叶" | "五月";

type Score = "及格" | "不及格";

type Wife<P1, P2> = (name: P1, score: P2) => { name: P1; score: P2 };
type NameType1<P> = P extends Wife<infer R, string> ? R : never;

const wife: NameType1<Wife<NameType, string>> = "二乃";
```
