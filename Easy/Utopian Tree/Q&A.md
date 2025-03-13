# [Proplem Link](https://www.hackerrank.com/challenges/utopian-tree/problem)

# Solution:

```javascript
function utopianTree(n) {
  let result = 1;
  for (let i = 1; i <= n; i++) {
    if (i % 2 === 1) result *= 2;
    else result++;
  }
  return result;
}
```
