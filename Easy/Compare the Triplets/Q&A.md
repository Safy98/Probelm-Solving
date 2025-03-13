# [Proplem Link](https://www.hackerrank.com/challenges/compare-the-triplets/problem)

# Solution:

```javascript
function compareTriplets(a, b) {
    const result = [0,0];
    for (let i = 0 ; i < a.length ; i ++){
        if(a[i]>b[i]){
            result[0]++;
        }
        else if(a[i]<b[i]){
            result[1]++;
        }
        
    }

    return result;
}
```
