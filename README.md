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
#### Do you speak "English"?
```javascript
function spEng(sentence){
let word = 'English'.toUpperCase();
return sentence.toUpperCase().includes(word);
}
```
#### Rock Paper Scissors!
```javascript
const rps = (p1, p2) => {
  if (p1 === p2) return 'Draw!';
  if (
    (p1 === 'scissors' && p2 === 'paper') ||
    (p1 === 'rock' && p2 === 'scissors') ||
    (p1 === 'paper' && p2 === 'rock')
  )
    return 'Player 1 won!';
  if (
    (p2 === 'scissors' && p1 === 'paper') ||
    (p2 === 'rock' && p1 === 'scissors') ||
    (p2 === 'paper' && p1 === 'rock')
  )
    return 'Player 2 won!'
};
```
#### Don't give me five!
```javascript
function dontGiveMeFive(start, end) {
  let count = 0;
  for (let i = start; i <= end; i++) {
    if (i.toString().includes("5")===false) {
      count++;
    }
  }
  return count;

}
```     
#### Binary Addition
```javascript
function addBinary(a,b) {
 return (a+b).toString(2);
}
```
#### Find the position!
```javascript
function position(letter){
let alf = ' abcdefghijklmnopqrstuvwxyz';
return `Position of alphabet: ${alf.indexOf(letter)}`;
}
```
#### String ends with?
```javascript
function solution(str, ending){
  return str.endsWith(ending);
}
```
#### Credit Card Mask
```javascript
function maskify(cc) {
  let s = cc.slice(-4);
  let r = cc.slice(0,-4)
  .split('')
  .map(el => '#')
  .join('');
return r + s;
}
```
#### Vowel remover
```javascript
function shortcut(string){
return string.replace(/[aeiou]/g, '')
}
```
#### Correct the mistakes of the character recognition software
```javascript
function correct(str){
return str.replace(/5/g, 'S').replace(/1/g, 'I').replace(/0/g, 'O');
}
```
#### Fake Binary
```javascript
function fakeBin(x){
return x.replace(/[0-4]/g, 0).replace(/[5-9]/g, 1);
}
```
#### Exclamation marks series #2: Remove all exclamation marks from the end of sentence
```javascript
function remove(s){
 return s.replace(/!+$/g, '')
}
```
#### FIXME: Replace all dots
```javascript
var replaceDots = function(str) {
  return str.replace(/\./g, '-');
}
```
#### Reversed Words
```javascript
function reverseWords(str){
  return str.split(' ').reverse().join(' '); // reverse those words
}
```
#### Squash the bugs
```javascript
function findLongest(str){
 let arr = str.split(" ");
  let longest = 0;
  for (let i = 0; i < arr.length; i++){
    if (arr[i].length > longest){
      longest = arr[i].length;
    }
  }
 return longest;
}
```
#### Highest and Lowest
```javascript
function highAndLow(numbers){
 let arr = numbers.split(' ');
 let min = arr[0];                    
 let max = arr[0];                    
    for (let i = 1; i < arr.length; i++){ 
 arr[i] = +arr[i];
    if (arr[i] < min) {                 
  min = arr[i];                     
}
    if (arr[i] > max) {                
  max = arr[i];                     
}
}
  return  `${max} ${min}`;
}
```
#### 
Every possible sum of two digits
```javascript
function digits(num){
  let arr = num.toString().split('');
  let arr1 = [];
  for (let i = 0; i < arr.length; i++){ 
    for (let j = 1+i; j < arr.length; j++){
      arr1.push(+arr[i]+ +arr[j]);
    }
}
 return arr1;
}
```
#### Welcome!
```javascript
let welcomeObj = {
  english: 'Welcome',
  czech: 'Vitejte',
  danish: 'Velkomst',
  dutch: 'Welkom',
  estonian: 'Tere tulemast',
  finnish: 'Tervetuloa',
  flemish: 'Welgekomen',
  french: 'Bienvenue',
  german: 'Willkommen',
  irish: 'Failte',
  italian: 'Benvenuto',
  latvian: 'Gaidits',
  lithuanian: 'Laukiamas',
  polish: 'Witamy',
  spanish: 'Bienvenido',
  swedish: 'Valkommen',
  welsh: 'Croeso',
};

function greet(language) {
  return welcomeObj [language] || welcomeObj.english;
  }
```
#### Duck Duck Goose
```javascript
function duckDuckGoose(players, goose) {
  return players[(goose-1) % players.length].name;
}
```
#### Make a function that does arithmetic!
```javascript
function arithmetic(a, b, operator){
  if (operator === 'add') return a + b;
  if (operator === 'subtract') return a - b;
  if (operator === 'multiply') return a * b;
  if (operator === 'divide') return a / b;
}
```
#### makeBackronym
```javascript
let makeBackronym = function(string){
 return string.toUpperCase().split('').map(elem=>dict[elem]).join(' ');
}
```
#### Check three and two
```javascript
function checkThreeAndTwo(arr) {
  let c1 = 0;
  let c2 = 0;
  let c3 = 0;
  for (let i = 0; i < arr.length; i++){
    if (arr[i] === "a") c1 = c1 + 1;
    if (arr[i] === "b") c2 = c2 + 1;
    if (arr[i] === "c") c3 = c3 + 1;
  }

  return (c1 === 2 || c2 === 2 || c3 === 2) && (c1 === 3 || c2 === 3 || c3 === 3);
}
```
#### Job Matching #1
```javascript
function match(candidate, job) {
  if(!candidate.minSalary || !job.maxSalary) throw "Error!";
  return (candidate.minSalary * 0.9) <= job.maxSalary;
}
```
#### Numbers to Objects
```javascript
function numObj(s){
  let arr = [];
 for (let i = 0; i < s.length; i++){
   const obj = {};
   obj[s[i]] = String.fromCharCode(s[i]);
   arr.push(obj)
 }
  return arr;
}
```
#### Numbers to Objects
```javascript
function numObj(s){
return s.map(el => ({[el]: String.fromCharCode(el)}));
}
```
#### Coding Meetup #5 - Higher-Order Functions Series - Prepare the count of languages
```javascript
function countLanguages(list) {
  let obj = {};
  for (i = 0; i< list.length; i++){
    if (obj[list[i].language]) {
      obj[list[i].language] = obj[list[i].language] + 1;
    } else {
      obj[list[i].language] = 1;
    }
  }
  return obj;
}
```
#### What is my name score? #1
```javascript
//let alpha={'ABCDE':1,'FGHIJ':2,'KLMNO':3,'PQRST':4,'UVWXY':5}
function nameScore(name) {
	let str = name.toUpperCase().split('');
	let score = 0;
	let result = {};
	for (let x in alpha) {
		for (let i = 0; i < str.length; i++) {
			if (x.includes(str[i]) === true) {
				score += alpha[x];
			}
		}
	}

	result[name] = score;
	return result;
}
```
#### Power
```javascript
function numberToPower(number, power){
let result = 1;
  for (let i = 1;i <= power;i++) {
   result = result * number
  }
return result;
}
```
#### No zeros for heros
```javascript
function noBoringZeros(n) {
  while(n%10===0 && n!==0){n/=10;}
  return n;
}
```
#### The wheat/rice and chessboard problem
```javascript
function squaresNeeded(grains){
 const arr=[0];
 for (let i=0;i<63;i++){
 arr.push(Math.pow(2,i));
 if (grains<arr[i]){
   return i-1;}
 }
}
```
#### simple calculator
```javascript
function calculator(a,b,sign){
  if ((typeof a === "number") && (typeof b === "number")) {
    switch (sign) {
    case "+":
      return a + b;
    case "-":
      return a - b;
    case "*":
      return a * b;
    case "/":
      return a / b;
    }
  }
  return "unknown value";
}
```
#### Price of Mangoes
```javascript
function mango(quantity, price){
return (quantity - Math.floor(quantity / 3))* price;
}
```
#### The Office I - Outed
```javascript
function outed(meet, boss){
  let sum = 0;
for(let key in meet){
  sum = sum + meet[key];
}
  let average = (sum + meet[boss])/Object.values(meet).length;
  return average > 5 ? 'Nice Work Champ!':'Get Out Now!'
}
```
#### The Office I - Outed
```javascript
function outed(meet, boss){
  return (Object.values(meet).reduce((acc,curr) => acc+curr,0) + meet[boss]) / Object.values(meet).length <= 5 ? 'Get Out Now!' : 'Nice Work Champ!';
}
```
#### How many days are we represented in a foreign country?
```javascript
function daysRepresented(trips){
  let arr=[];
  for (let i=0; i<trips.length; i++){
    for (let j=trips[i][0]; j<=trips[i][1]; j++)
      if (arr.indexOf(j)===-1)
        arr.push(j);}
  return arr.length;
}
```
#### You're a square!
```javascript
function isSquare(n){
  return Number.isInteger(Math.sqrt(n));
}
```
#### All Star Code Challenge #22
```javascript
function toTime(seconds) {
return `${Math.floor(seconds/3600)} hour(s) and ${Math.floor((seconds/60)) % 60} minute(s)`;
}
```
#### Tortoise racing
```javascript
function race(v1, v2, g) {
  if (v1 >= v2) return null;

  let time = g / (v2 - v1);
  let h = Math.trunc(time);
  let m = Math.trunc((time * 60) % 60);
  let s = Math.trunc((time * 3600) % 60);

  return [h, m, s];
}
```
#### Most valuable character
```javascript
function solve(st) {
  return st.split('').sort()
.reduce((acc , curr) => st.lastIndexOf(acc) - st.indexOf(acc) < st.lastIndexOf(curr) - st.indexOf(curr) ? curr : acc);
}
```
#### Permute a Palindrome
```javascript
function permuteAPalindrome (input){
  let arr = input.split('').sort();
  console.log(arr);
  const obj = {};
  let c = 0;
   for (let i = 0; i < arr.length; i++){
     if (obj[arr[i]]){
     obj[arr[i]] = obj[arr[i]]+1; 
     } else {
       obj[arr[i]] = 1;
     }
   }
  let count = 0;
   for(let key in obj){
     if (obj[key] %2 !==0) {
       count++;
       if (count > 1) return false;
     }                                                     
   }
  return true;            
  }
```
#### The Office II - Boredom Score
```javascript
const score = {
  accounts: 1,
  finance: 2,
  canteen: 10,
  regulation: 3,
  trading: 6,
  change: 6,
  IS: 8,
  retail: 5,
  cleaning: 4,
  'pissing about': 25,
};

function boredom(staff){
  const teamScore = Object.values(staff).reduce((acc, curr) => acc + score[curr], 0);
  if (teamScore <= 80) return 'kill me now';
 if (teamScore >= 100) return 'party time!!';
 return 'i can handle this';

}
```
#### Santa's Naughty List
```javascript
function findChildren(santasList, children) {
  let arr = [];
  for (i = 0; i < children.length; i++){
     for (j = 0; j < santasList.length; j++){
        if (arr.indexOf(children[i])===-1 && santasList[j]===children[i] ) {
      arr.push(children[i]);
    }
     }
   
  }
  return arr.sort();
}
```
#### Get number from string
```javascript
function getNumberFromString(s) {
return +s.replace(/\D/gi, '');
}
```
#### Unique In Order
```javascript
  function uniqueInOrder(iterable) {
  let arr = [];
  for(let i = 0; i < iterable.length; i++) {
    if(iterable[i] !== arr[arr.length-1]) { //if (iterable[i] != iterable[i+1]) arr.push(iterable[i]);
      arr.push(iterable[i]);
    }
  }
  return arr;
}
```
#### Can Santa save Christmas?
```javascript
function determineTime(dur){
  let sec = 0;
  for (let i = 0; i < dur.length; i++) {
   let newArr = dur[i].split(':');
   sec += newArr[0] * 3600 + newArr[1] * 60 + +newArr[2];
  }
  return sec <= 24 * 3600;
}
```               
#### Tail Swap
```javascript
 function tailSwap(arr) {
  let result = arr.join(':').split(':');
   return [`${result[0]}:${result[3]}`, `${result[2]}:${result[1]}`];
 }                
```
#### Get the Middle Character
```javascript
function getMiddle(s)
{
  let m = Math.trunc(s.length / 2);
    if (s.length % 2 !== 0){
      return s[m];
    } else {
      return s[m-1]+s[m];
    }
  }
```
#### Isograms
```javascript
function isIsogram(str){
let arr = str.toUpperCase().split('');
 const nonDuplicates = arr.filter(el => arr.indexOf(el) === arr.lastIndexOf(el));
  return nonDuplicates.join('').length>=str.length;
}
```
#### Jaden Casing Strings
```javascript
String.prototype.toJadenCase = function () {
return this.split(' ').map(el => el[0].toUpperCase() + el.slice(1)).join(' ');
};
```
#### Exes and Ohs
```javascript
function XO(str) {
  const arr = str.toLowerCase().split('');
  const x = arr.filter(el => el === 'x');
  const o = arr.filter(el => el === 'o');
  return x.length === o.length?;
}
```
#### Growth of a Population
```javascript
function nbYear(p0, percent, aug, p) {
  let y = 0;
  while (p0 < p) {
   p0 += p0 * percent / 100 + aug;
    y++;
  }
  return y;
}
```
#### Two to One
```javascript
function longest(s1, s2) {
let arr = s1.concat(s2).split('').sort();
  let obj = {};
  for (i = 0; i< arr.length; i++){
    if (obj[arr[i]]) {
      obj[arr[i]] = obj[arr[i]]+1;
    } else {
      obj[arr[i]] = 1;
    }
  }
  return Object.keys(obj).join('');
}
```
#### Two to One
```javascript
function longest(s1, s2) {
return s1.concat(s2)
.split('')
.sort()
.filter((el,index,arr) => el !== arr[index - 1])
.join('');
}
```
#### Printer Errors
```javascript
function printerError(s) {
  let s1 = s.split('').sort().join('');
  let s2 = s1.replace(/[a-m]/gi, '');
  return `${s2.length}/${s.length}`;
}
```
#### Printer Errors/2
```javascript
function printerError(s) {
    let count = 0;
    for(let i = 0; i < s.length; i++) {
      if (s[i] > "m") {
        count++;
      }
    }
    return count+"/"+s.length;
}
```
#### List Filtering
```javascript
function filter_list(l) {
  return l.filter(el => typeof el === 'number');
}
```
#### Ones and Zeros
```javascript
function binaryArrayToNumber(arr){
  return parseInt(arr.join(''), 2);
}
```
#### Categorize New Member
```javascript
function openOrSenior(data){
return data.map(([age, handicap]) => (age > 54 && handicap > 7) ? 'Senior' : 'Open');
}
```
#### Categorize New Member.2
```javascript
function openOrSenior(data){
  let rez=[];
  for(let i = 0; i < data.length; i++){
    if(data[i][0] > 54 && data[i][1] > 7) {
      rez.push("Senior");
    } else {
      rez.push("Open");
    }
    }
      return rez;
  }

```
#### Friend or Foe?
```javascript
function friend(friends){
  return friends.filter(el => el.length === 4);
}
```
#### Number of People in the Bus
```javascript
function number(busStops){
  let sum = 0;
  for (let i = 0; i < busStops.length; i++){
    sum = sum + busStops[i][0]-busStops[i][1];
  }
return sum;
}
```
#### Number of People in the Bus/2
```javascript
let number = function(busStops){
  return busStops.reduce((acc, cur) => {
    return acc + (cur[0] - cur[1]) 
  }, 0) 
}
```
#### Money, Money, Money
```javascript
function calculateYears(P, i, t, d) {
let years = 0;
while (P < d){
    P = P + P*i - P*i*t;
    years++
    }
    return years;
}
```
#### Reverse words
```javascript
function reverseWords(str) {
return str.split("").reverse().join("").split(" ").reverse().join(" ");
}
```
#### Reverse words/2
```javascript
function reverseWords(str) {
  const reversedWords = [];
  const orderReversedWords = [];
  for (let i = str.length - 1; i >= 0; i--) reversedWords.push(str[i]);
  const words = reversedWords.join("").split(" ");
  for (let i = words.length - 1; i >= 0; i--)
    orderReversedWords.push(words[i]);
  return orderReversedWords.join(" ");
}
```
#### Triple Trouble
```javascript
function tripleTrouble(one, two, three){
  let str = '';
  for (let i = 0; i < one.length; i++){
    str = str + one[i]+two[i]+three[i];
  }
  return str;
 }
```
#### The Wide-Mouthed frog!
```javascript
function mouthSize(animal) {
  return animal.toLowerCase() === "alligator"? "small":"wide";
}
```
#### Find the stray number
```javascript
function stray(numbers) {
 const nonDuplicates = numbers.filter(el => numbers.indexOf(el) === numbers.lastIndexOf(el));
 return nonDuplicates[0];
}
```
#### Count the Digit
```javascript
function nbDig(n, d) {
let count=0;
    for (let i = 0;i <= n;i++){
      let square=(i*i+"").split("");
      square.forEach((s)=>s == d ? count++ : null)
    }
  return count;
}
```
#### Count the Digit/2
```javascript
function nbDig(n, d) {
 let str = '';
    for(let i = 0; i <= n; i++){
      str += Math.pow(i, 2);
    }
  return str.split(d).length-1;
}
```
#### The highest profit wins!
```javascript
function minMax(arr){
  let res = [];
  let min = arr[0];
  let max = arr[0];
  for (let i = 0; i< arr.length; i++){
    if (arr[i] < min){
      min = arr[i];
    } else  
      if (arr[i]>max){
         max = arr[i];
      }
  }
   res.push(min,max);
  return res;
}
}
```
#### The highest profit wins!/2
```javascript
function minMax(arr){
let s = arr.sort((a,b) => a-b);
  return [s[0],s[s.length-1]];
}
```
#### Sum of a sequence
```javascript
function sequenceSum(begin, end, step) {
  sum = 0;
  for (let i = begin; i <= end ;  i+=step){
    sum = sum + i;
  }
 return begin > end ? 0 : sum;
}
```
#### Sum of all the multiples of 3 or 5
```javascript
function findSum(n) {
  let sum = 0;
  for (let i = 3 ; i<=n;i++){
    if (i % 3 === 0 || i % 5 === 0){
      sum = sum + i;
    }
  }
  return sum;
}
}
```
#### Maximum Length Difference
```javascript
function mxdiflg(a1, a2) {
  if (a1.length === 0 || a2.length === 0) return -1;
  let s1 = a1.map(el => el.length);
  let s2 = a2.map(el => el.length);
  return Math.max(Math.max(...s1) - Math.min(...s2), Math.max(...s2) - Math.min(...s1));
}
```
#### Maximum Length Difference/2
```javascript
const mxdiflg = (a1, a2) => {
  if (a1.length === 0 || a2.length === 0)  return -1;
  a1 = a1.map((el=> el.length)).sort((a,b)=>a-b);
  a2 = a2.map((el=> el.length)).sort((a,b)=>a-b);
  const max1 = a1[a1.length - 1]- a2[0];
  const max2 = a2[a2.length - 1] - a1[0];
  return max1 > max2 ? max1 : max2;
};
```
#### Create Phone Number
```javascript
function createPhoneNumber(numbers){
  let n = numbers.join('');
  return `(${n.substring(0, 3)}) ${n.substring(3, 6)}-${n.substring(6)}`;
}
```
#### Create Phone Number/2
```javascript
function createPhoneNumber(numbers){
  let format = "(xxx) xxx-xxxx";
  for(let i = 0; i < numbers.length; i++)
  {
    format = format.replace('x', numbers[i]);
  }
  return format;
}
```
#### Double Sort
```javascript
function dbSort(a){
  let s = [];
  let s1 = [];
  for (let i =0;i<a.length;i++){
    if (typeof a[i] === 'number'){
      s.push(a[i]);
    } else if (typeof a[i] === 'string'){
      s1.push(a[i]);
    }
  }
return s.sort((a,b)=>a-b).concat(s1.sort());
}
```
#### You're a square!
```javascript
function isSquare(n){
  return (Number.isInteger(Math.sqrt(n)));
}
```
#### Sum of odd numbers
```javascript
function rowSumOddNumbers(n) {
return Math.pow(n,3);
}
```
#### Holiday II - Plane Seating
```javascript
function planeSeat(a){
  let b = a.replace(/[a-z]/gi,'');
  let c = a.replace(/[0-9]/gi,'');
  let arr = [];

  for (let i = 0; i < 1; i++){
    arr.push(b,c);
  }
if (c ==='I'||c ==='J') return 'No Seat!!';  
if (arr[0] > 0 && arr[0] < 21 && arr[1].match(/[A-C]/)) return 'Front-Left';
if (arr[0] > 0 && arr[0] < 21 && arr[1].match(/[D-F]/)) return 'Front-Middle';
if (arr[0] > 0 && arr[0] < 21 && arr[1].match(/[G-K]/)) return 'Front-Right';
if (arr[0] > 20 && arr[0] <41 && arr[1].match(/[A-C]/)) return 'Middle-Left';
if (arr[0] > 20 && arr[0] <41 && arr[1].match(/[D-F]/)) return 'Middle-Middle';
if (arr[0] > 20 && arr[0] <41 && arr[1].match(/[G-K]/)) return 'Middle-Right';
if (arr[0] > 40 && arr[0] <61 && arr[1].match(/[A-C]/)) return 'Back-Left';
if (arr[0] > 40 && arr[0] <61 && arr[1].match(/[D-F]/)) return 'Back-Middle';
if (arr[0] > 40 && arr[0] <61 && arr[1].match(/[G-K]/)) return 'Back-Right';
return 'No Seat!!';
}
```
#### Maximum Multiple
```javascript
function maxMultiple(divisor, bound){
return Math.trunc(bound/divisor) * divisor;
}
```
#### Borrower Speak
```javascript
function borrow(s){
  return s.toLowerCase().replace(/\W/g, '');
}
```
#### Ironman Triathlon
```javascript
function iTri(s){
  let total = 140.6;
  if (s === 0) return 'Starting Line... Good Luck!';
  if (s < 2.4) return {Swim:`${(total-s).toFixed(2)} to go!`};
  if (s < 2.4 + 112) return {Bike:`${(total-s).toFixed(2)} to go!`};
  if (s < (total - 10)) return {Run:`${(total-s).toFixed(2)} to go!`};
  if (s < total) return {Run:'Nearly there!'};
  return "You're done! Stop running!";
}
```
#### Find the odd int
```javascript
function findOdd(A) {
 let obj = {};
  for (let i = 0; i< A.length; i++){
    if (obj[A[i]]) {
      obj[A[i]] = obj[A[i]]+1;
    } else {
      obj[A[i]] = 1;
    }
  }
  for(let key in obj) {
      if ((obj[key])%2!==0){
        return +key;
     }
  }
}
```
#### Find the odd int/2
```javascript
function findOdd(A) {

  for(let i = 0;i < A.length;i++)
  {
    let notDuplic=A.filter(el=>el===A[i]);
    if(notDuplic.length%2!==0)
    return notDuplic[0];
  }
}
```
#### Multiples of 3 or 5
```javascript
function solution(n){
    let sum = 0;
    for (let i = 3 ; i < n;i++){
        if (i % 3 === 0 || i % 5 === 0){
            sum = sum + i;
        }
    }
    return sum;
}
```
#### Persistent Bugger.
```javascript
function persistence(num) {
  let count = 0;
  num = num.toString();
  while (num.length > 1) {
    count++;
    num = num.split('').reduce((a, b) => a * b).toString();
  } return count;
}
```
#### Persistent Bugger-2
```javascript
function persistence(num) {
let count = 0;
   for (let i = 0; num > 9; i++) {
     num = num.toString().split('').reduce((acc, curr) => acc * curr);
     count++
   }
   return count;
}
```
#### Counting Duplicates
```javascript
function duplicateCount(text){
  let arr = text.toLowerCase().split('').sort();
  return arr.filter((el, i) => i !== arr.indexOf(el) && i === arr.lastIndexOf(el)).length;
}
```
#### Duplicate Encoder
```javascript
function duplicateEncode(word){
  return word
    .toLowerCase()
    .split('')
    .map((el, i, arr)=> arr.indexOf(el) === arr.lastIndexOf(el) ? '(' : ')')
    .join('');
}
```
#### Duplicate Encoder/2
```javascript
function duplicateEncode(word){
 word = word.toLowerCase();
  let str ='';
  for (let i = 0;i < word.length; i++){
    if (word.indexOf(word[i])===word.lastIndexOf(word[i])){
      str = str + '(';
    } else {
        str = str + ')';
        }
  }
  return str;
}
```
#### Find The Parity Outlier
```javascript
function findOutlier(arr){
  let even = arr.filter(el => el % 2 === 0);
  let odd = arr.filter(el => el % 2 !== 0);
  return even.length === 1 ? even[0] : odd[0];
}
```
#### Sum of Digits / Digital Root
```javascript
function digital_root(num) {
   for (let i = 0; num > 9; i++) { //пока число двузначное, считаем сумму
     num = num.toString().split('').reduce((acc, curr) => +acc + +curr);
   }
   return num;
}
//console.log(digital_root(456)) / 6
```
#### Tribonacci Sequence
```javascript
function tribonacci(signature,num){
  if(num === 0) return [];
  for(let i=0; i<num-3; i++){
    signature.push(signature[i] + signature[i+1] + signature[i+2]);
  } return signature.slice(0, num);
}
console.log([2,4,7], 10) // [2, 4, 7, 13, 24, 44, 81, 149, 274, 504]
```
#### Kebabize
```javascript
function kebabize(str) {
 return str.replace(/[0-9]/g, '').replace(/([A-Z])/g, "-$1").toLowerCase().replace(/^-/, '');
console.log(kebabize('camelsHave3Humps'));
}
```
