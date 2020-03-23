# JavaScript Split Array Into Groups of the Same Size

```javascript
const items = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
const size = 3;
const groups = items.reduce((a, c, i, s) => i % size === 0 ? [...a, s.slice(i, i + size)] : a, []);
// [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11]]
```
