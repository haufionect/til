# JS：console 调试技巧

```js
console.log("值：", obj);          // 打印对象比拼字符串直观
console.table(users);              // 数组/对象列表格展示
console.time("loop");              // 计时
for (let i = 0; i < 1000; i++) {}
console.timeEnd("loop");
console.count("hit");              // 计数，调了几次一目了然
```

- `console.log` 传多个参数，不用字符串拼接。
- `console.table` 看数组最直观，`console.time/timeEnd` 测性能不用手写 Date。
- 调试完删掉 console，不然生产日志会被刷屏。
