# solved-tasks
#### Sum of Multiples
```javascript
function sumMul(n,m){
  let sum = 0;
  if (n <=0 || m <=0)return "INVALID";
  for (i = n; i < m; i=i+n ){
    sum = sum + i
}
  return sum;
}
```