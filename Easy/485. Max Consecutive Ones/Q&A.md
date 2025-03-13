# [Proplem Link](https://leetcode.com/problems/max-consecutive-ones/description/)

# Solution:

```javascript
const findMaxConsecutiveOnes = function (nums) {
  let temp = 0;
  let max = 0;
  for (num of nums) {
    if (num === 0) {
      if (temp > max) {
        max = temp;
      }
      temp = 0;
    } else {
      temp++;
    }
  }
  if (temp > max) {
    max = temp;
  }
  return max;
};
```
