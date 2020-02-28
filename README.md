# tseslint-no-implied-eval

1. git clone https://github.com/yeonjuan/tseslint-no-implied-eval.git
1. npm install
2. npm run lint

* ./test.ts
```ts
const foo = () => {};

setTimeout(foo, 0);
setInterval(foo, 0);
```

* result
```
  3:12  error  Implied eval. Consider passing a function  @typescript-eslint/no-implied-eval
  4:13  error  Implied eval. Consider passing a function  @typescript-eslint/no-implied-eval
```

