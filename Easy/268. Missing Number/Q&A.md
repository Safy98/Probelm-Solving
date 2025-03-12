# [Problem Link](https://leetcode.com/problems/missing-number/description/)

# Solution:

## Best Solution O(1):

```javascript
const missingNumber = function (nums) {
  const originalSum = (nums.length * (nums.length + 1)) / 2;
  const calcSum = nums.reduce((acc, el) => acc + el, 0);
  return originalSum - calcSum;
};
```

OR

## Working Solution: O(n)

```javascript
const missingNumber = function (nums) {
  const sorted = nums.sort((a, b) => a - b);

  for (let i = 0; i < nums.length; i++) {
    if (i !== sorted[i]) return i;
  }
  return nums.length;
};
```
