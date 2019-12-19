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
#### Holiday VIII - Duty Free
```javascript
function dutyFree(normPrice, discount, hol){
return Math.floor(hol/(normPrice * discount / 100));
}
```
#### How many times should I go?
```javascript
function howManyTimes(annualPrice, individualPrice) {
  return Math.ceil(annualPrice/individualPrice);
}
```
#### Formatting decimal places #1
```javascript
function twoDecimalPlaces(number) {
return Math.trunc(number*100)/100;
}
```
#### Lario and Muigi Pipe Problem
```javascript
function pipeFix(numbers){
let arr = [];
for (i = numbers[0]; i <= numbers[numbers.length-1]; i++){
arr.push(i)
}
return arr;
}
```
#### Calculate Price Excluding VAT
```javascript
function excludingVatPrice(price){
  return  price === null ? -1 : Number((price / 1.15).toFixed(2))
}
```
#### Parse nice int from char problem
```javascript
function getAge(inputString){
return parseInt(inputString,10);
}
```
#### Bin to Decimal
```javascript
function binToDec(bin){
  return parseInt(bin, 2);
}
```
#### Parse float
```javascript
function parseF(s) {
  return Number.isNaN(parseFloat(s)) ? null : parseFloat(s)
}
```
#### Count the Monkeys!
```javascript
function monkeyCount(n) {
let arr = [];
for (let i = 1; i <= n; i++){
arr.push(i);
}
return arr;
}
```
#### Sum Arrays
```javascript
function sum (numbers) {
let sum = 0;
  for (i = 0; i < numbers.length; i++){
  sum = sum + numbers[i];
}
    return sum;
    
};
```
#### Is every value in the array an array?
```javascript
const arrCheck = value => value.every(Array.isArray);
```
#### Enumerable Magic #3 - Does My List Include This?
```javascript
function include(arr, item){
  for (let i = 0; i < arr.length; i++){
    if (arr[i] === item){
      return true;
    } 
  }
  return false;
}
```
#### Difference of Volumes of Cuboids
```javascript
function findDifference(a,b ){
  let v1 = 1;
  let v2 = 1;
  for (let i = 0; i< a.length; i++){
    v1 = v1*a[i];
  }
  for (let i = 0; i< b.length; i++){
    v2 = v2*b[i];
  }
  return Math.abs(v2-v1)
}
```
#### Difference of Volumes of Cuboids
```javascript
function findDifference(a, b)
{
let v1 = a.reduce((x,y) => x*y);
let v2 = b.reduce((x,y) => x*y);
return  Math.abs(v2-v1);
}
 
```
#### Total amount of points
```javascript
function points(games) {
 let count = 0;
  for (i = 0; i < games.length; i++) {
    if (games[i][0] > games[i][2]) count = count + 3;
    if (games[i][0] === games[i][2]) count = count + 1;
  }
 return count;
}
```
#### Find the first non-consecutive number
```javascript
function firstNonConsecutive(arr) {
  for (let i = 0; i < arr.length-1 ; i++) {
   if (arr[i+1]-arr[i]!==1) return arr[i+1];
  }
return null;
}
```
#### How good are you really?
```javascript
function betterThanAverage(arr, yourPoints) {
let sum = 0;
  let average; 
  for (let i = 0; i < arr.length; i++){
  sum = sum + arr[i];
    average = sum/arr.length;
  }
  return yourPoints > average? true: false;
}
```
#### Calculate average
```javascript
function find_average(arr) {
let sum = 0;
  for (let i = 0; i < arr.length; i++){
  sum = sum + arr[i];
}
return  sum/arr.length;
}
```
#### Sum of Odd Cubed Numbers
```javascript
function cubeOdd(arr) {
let sum = 0;
for (let i = 0; i < arr.length; i++){
  if (typeof arr[i] !== 'number') return undefined;
  if (arr[i] % 2!==0)
{
  sum = sum + (arr[i]**3);
  }
}
return sum;
}
```
#### Find Maximum and Minimum Values of a List
```javascript
var min = function(list){
    
    return Math.min(...list);
}

var max = function(list){
    
    return Math.max(...list);
}
```
#### Sum of two lowest positive integers
```javascript
function sumTwoSmallestNumbers(numbers){  
  numbers = numbers.sort(function(a, b){return a - b; });
  return numbers[0] + numbers[1];
}
```
#### Remove the minimum
```javascript
function removeSmallest(numbers) {
  let arr = [];
  let min = numbers[0];
  for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] < min) {
     min = numbers[i];
    }
  }
  for (let j = 0; j < numbers.length; j++) {
    if (j !== numbers.indexOf(min)) {
      arr.push(numbers[j]);
    } 
  }
  return arr;
}
```
#### Unfinished Loop - Bug Fixing #1
```javascript
function createArray(number){
  let newArray = [];
  for(let i = 1; i <= number; i++){
    newArray.push(i);
  }
  return newArray;
}
```
#### Find the divisors!
```javascript
function divisors(n) {
  let arr = [];
  for (let i = 2 ; i <= n-1; i++){
    if (n % i === 0 ){ 
      arr.push(i)
    } 
  }
  if (arr.length === 0) {
    return `${n} is prime`;
  }
  return arr;
}
```
#### No Loops 2 - You only need one
```javascript
function check(a,x){
return a.includes(x);
}
```
#### A wolf in sheep's clothing
```javascript
function warnTheSheep(queue) {
const index = queue.indexOf('wolf');
  return index === queue.length-1 ? "Pls go away and stop eating my sheep"
  :`Oi! Sheep number ${queue.length-1-index}! You are about to be eaten by a wolf!`
}
```
#### Find numbers which are divisible by given number
```javascript
const divisibleBy = (numbers, divisor) =>
  numbers.filter(el => el % divisor === 0);
```
#### Removing Elements
```javascript
function removeEveryOther(arr){
  return arr.filter((el, i) => i % 2 === 0);
}
```
#### Well of Ideas - Easy Version
```javascript
function well(x){
const ideas = x.filter(idea => idea === 'good').length;

  if (ideas > 2) return 'I smell a series!';
  if (ideas > 0) return 'Publish!';
  return 'Fail!';
}
```
#### Find how many times did a team from a given country win the Champions League?
```javascript
function countWins(winnerList, country) {
   return winnerList.filter(el => el.country === country).length;
}

```
#### filterEvenLengthWords
```javascript
function filterEvenLengthWords(words) {
  return words.filter (el => el.length % 2 ===0);
}
```
#### Array.diff
```javascript
function array_diff(a,b) {
return a.filter(el => !b.includes(el))
}
```
#### Find Duplicates
```javascript
function duplicates(arr) {
 return arr.filter((el, i) => i !== arr.indexOf(el) && i === arr.lastIndexOf(el));
}
```
#### Train to remove duplicates from an array with filter()
```javascript
function unique(arr) {
return arr.filter((el, i) => i === arr.indexOf(el)); 
}
```
#### Divide and Conquer
```javascript
function divCon(x){
let sum1 = 0;
let sum2 = 0;
for (let i = 0; i < x.length; i++){
if (typeof x[i] === 'string'){
sum1 = sum1 + +x[i]
} else {
sum2 = sum2 + x[i]
}
}
return sum2-sum1;
}
```
#### String Templates - Bug Fixing #5
```javascript
function buildString(...template){
  return `I like ${template.join(', ')}!`;
}
```
#### Enumerable Magic #1 - True for All?
```javascript
function all( arr, fun ){
 return arr.every(fun); 
}
```
#### Grasshopper - Array Mean
```javascript
function findAverage(nums) {
 let result = nums.reduce((acc, curr) => acc + curr); 
  return result/nums.length;
}
```
#### Beginner - Reduce but Grow
```javascript
function grow(x){
return x.reduce((acc, curr) => acc * curr, 1);
}
```
#### Array plus array
```javascript
function arrayPlusArray(arr1, arr2) {
  let arr3 = arr1.concat(arr2);
  return arr3.reduce((acc, curr) => acc + curr); 
}
```
#### SpeedCode #2 - Array Madness
```javascript
function arrayMadness(a, b) {
let result1 = a.reduce((acc, curr) => acc + Math.pow(curr,2),0); 
  let result2 = b.reduce((acc, curr) => acc + Math.pow(curr,3),0); 
  return result1 > result2;
}
```
#### Beginner - Lost Without a Map
```javascript
function maps(x){
return x.map(el => el*2);
}
```
#### Remove First and Last Character Part Two
```
function array(arr){
return arr.split(',').slice(1,-1).join(' ')|| null;
}
```
#### Jenny's secret message
```javascript
function greet(name){
return name === "Johnny"? "Hello, my love!" : "Hello, " + name + "!";
}
```
#### get character from ASCII Value
```javascript
function getChar(c){
 return String.fromCodePoint(c);
}
```
#### Is this my tail?
```javascript
function correctTail(bod, tail) {
 return bod[bod.length - 1] === tail ? true : false;
    }
```
#### Numbers to Letters
```javascript
function switcher(x){
let alf = ' zyxwvutsrqponmlkjihgfedcba!? ';
return x.map(i => alf[i]).join('');
}
```
#### Regex count lowercase letters
```javascript
function lowercaseCount(str){
return (str.match(/[a-z]/g) || []).length;
}
```
#### Regex count lowercase letters -add
````javascript
function lowercaseCount(str){
  let alf = ' abcdefjhigklmnopqrstuvwxyz';
  let count = 0;
 for (let i = 0; i< str.length; i++){
 if (alf.indexOf(str[i]) >= 0) {
            count++;
 }
        }
  return count;
 }
````
#### Spacify
```javascript
function spacify(str) {
  let s = '';
  for (let i = 0; i< str.length; i++){
    s = s + str[i] + ' ';
  }
 return s.slice(0,-1);
}
```
#### Spacify
```javascript
function spacify(str) {
  return str.split("").join(" ");
}
```
#### Is it a palindrome?
```javascript
function isPalindrome(x) {
  let s = '';
for (let i = x.length - 1; i >= 0; i--){
  s = s + x[i];
}
  return s.toLowerCase() === x.toLowerCase();
}
```
#### Is it a palindrome? -add
```javascript
function isPalindrome(x) {
  let s = x.split('').reverse().join('');
  return s.toLowerCase() === x.toLowerCase();
}
```
#### Mumbling
```javascript
function accum(s) {
  const res = [];
  for (let i = 0; i < s.length; i++) {
    let row = s[i].toUpperCase();
    for (let j = 0; j < i; j++) {
      row += s[i].toLowerCase();
    }
    res.push(row);
  }
  return res.join('-');
}
```
#### Find the capitals
```javascript
function capitals(word) {
 let arr = [];
  for (let i = 0; i < word.length; i++){
    if (word[i] === word[i].toUpperCase()){
      arr.push(i)
    }
  }
  return arr;
}
```
#### repeatIt
```javascript
var repeatIt = function(str, n) {
return  typeof str === 'string' ? str.repeat(n) : 'Not a string'
  }
```
#### Draw stairs
```javascript
function drawStairs(n) {
  let str = '';
  let w = ' ';
  for (let i = 0; i < n; i++){
    str = str + w.repeat(i)+'I' + '\n';
  }
    return str.slice(0,-1);
}
```
     