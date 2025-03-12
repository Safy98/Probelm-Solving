# [Proplem Link](https://www.hackerrank.com/challenges/simple-array-sum/problem)

# Solution:

```javascript
function simpleArraySum(ar) {
  const result = ar.reduce((acc, el) => {
    return acc + el;
  }, 0);

  return result;
}
```

OR

```javascript
function simpleArraySum(ar) {
  return ar.reduce((acc, el) => acc + el, 0);
}
```
