# solved-tasks
#### Sum of Multiples
```javascript
function sumMul(n,m){
  let sum = 0;
  if (n <=0 || m <=0)return "INVALID";
  for (let i = n; i < m; i=i+n ){
    sum = sum + i
}
  return sum;
}
```
#### Sum of the first nth term of Series
```javascript
function SeriesSum(n) {
  let sum = 0;
  let divider = 1;
  for (let i = 0; i < n; i ++) {
    if (i === 0) {
      sum = 1;
    } else {
      divider = divider + 3;
      sum = sum + (1 / divider);
    }
  }
  return sum.toFixed(2);
}
```
#### Filter the number
```javascript
function FilterString(value) {
  let arr = value.split('');
  let result = 0;
  for (let i = 0; i < arr.length; i++){
     if (isNaN(arr[i]) === false) {
     result = result + arr[i];
   }
}
  return +result;
}
```
#### isReallyNaN
```javascript
const isReallyNaN = (val) => {
  return Number.isNaN(val);
};
```
#### Is integer safe to use?
```javascript
function SafeInteger(n) {
return Number.isSafeInteger(n);
}
```
#### Invert values
```javascript
function invert(array) {
  for (let i = 0; i < array.length; i ++){
  if (array[i]< 0 || array[i] > 0 ){
   array[i] = - array[i]
}
}
  return array;
}
```
#### Closest elevator
```javascript
function elevator(left, right, call){
return Math.abs(call-left) < Math.abs(call-right) ? 'left' : 'right';
}
```
#### Alan Partridge II - Apple Turnover
```javascript
function apple(x){
return Math.pow(x,2) > 1000?'It\'s hotter than the sun!!':'Help yourself to a honeycomb Yorkie for the glovebox.'
}
```
#### Squares sequence
```javascript
function squares(x, n) {
  var arr = [];
  for(let i = 0; i < n; i++){
    arr.push(x);
    x = x * x;
  }
  return arr;
} 
```
#### Square Every Digit
```javascript
function squareDigits(num){
  let n = num.toString().split('');
  for (let i = 0; i < n.length;i++){
    n[i]=(n[i]*n[i]);
  }
  return +n.join('');
}
```
#### Find the next perfect square!
```javascript
function findNextSquare(sq) {
   return Math.sqrt(sq)%1===0 ? Math.pow(Math.sqrt(sq)+1,2) : -1
}
```

#### Powers of 2
```javascript
function powersOfTwo(n){
let arr = [];
for (let i = 0; i <= n; i++){
arr[i] = Math.pow(2,i)
}
  return arr;
}
```
#### 5 without numbers !!
```javascript
function unusualFive() {
let str = 'Five!'
  return str.length;
}
```
#### Odd or Even?
```javascript
function oddOrEven(array) {
let sum = 0;
   for (let i = 0; i < array.length; i++){
   sum = sum + array[i];
   }
   return sum%2===0?'even':'odd';
}
```
