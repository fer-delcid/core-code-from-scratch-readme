# Core-Code Week 2 

## Week Challenge Tuesday
## Multiply
### Instructions
<img width="565" alt="Captura de Pantalla 2022-04-19 a la(s) 7 05 17 p  m" src="https://user-images.githubusercontent.com/91048093/164126453-905c6175-5eb7-4282-b706-1480b0981ff1.png">

``` JavaScript

function multiply(a, b){
  a * b
}

```
### Solution
``` JavaScript

function multiply(a, b){
  return a * b
}

```
## ASCII Total
### Instructions

<img width="551" alt="Captura de Pantalla 2022-04-21 a la(s) 7 23 02 p  m" src="https://user-images.githubusercontent.com/91048093/164578221-78f9c88c-feab-4421-8953-cc388f0b6425.png">

### Solution
```JavaScript
function uniTotal (string) {
  let suma=0;
  for(var i=0; i<string.length; i++){
    suma+=string.charCodeAt(i);
  }
  return suma;
}
```

## Char from ASCII Value
### Instructions
<img width="545" alt="Captura de Pantalla 2022-04-21 a la(s) 8 54 30 p  m" src="https://user-images.githubusercontent.com/91048093/164587090-fee78193-de41-474a-ad8a-b8d739e2df5f.png">

### Solution
```javascript
function getChar(c){
  let ans=String.fromCharCode(c);
  return ans;
}
```

## Binary Addition
### Instruction
<img width="542" alt="Captura de Pantalla 2022-04-22 a la(s) 11 42 33 a  m" src="https://user-images.githubusercontent.com/91048093/164766523-b189c7e6-9916-40c9-974e-c2d22afce007.png">

### Solution
```javascript
function addBinary(a, b) {
  let suma=a+b;
  return suma.toString(2);
}
```

## Student´s Final Grade
### Instruction
<img width="533" alt="Captura de Pantalla 2022-04-22 a la(s) 11 44 21 a  m" src="https://user-images.githubusercontent.com/91048093/164766749-6471ecee-0fec-422e-b174-468c8271e14e.png">

### Solution
```javascript
function addBinary(a, b) {
  return (a + b).toString(2);
}
```
## Week Challenge Wednesday
## Holiday VIII - Duty Free
### Instructions
<img width="543" alt="Captura de Pantalla 2022-04-22 a la(s) 12 29 40 p  m" src="https://user-images.githubusercontent.com/91048093/164773494-558bc79d-e23c-4205-b41b-6e54466c3083.png">

### Solution
```javascript
function dutyFree(normPrice, discount, hol){
  let total = hol / ((discount * normPrice) / 100);
  return Math.floor(total);
}
```

## Twice As Old
### Instructions
<img width="549" alt="Captura de Pantalla 2022-04-26 a la(s) 3 13 31 p  m" src="https://user-images.githubusercontent.com/91048093/165393406-9a885dd7-4a6a-4220-a6b7-9ae73dad1a26.png">

### Solution
```Javascript
function twiceAsOld(dadYearsOld, sonYearsOld) {
  let years = dadYearsOld - 2 * sonYearsOld;
  return Math.abs(years);
}
```
## Valid Spaces
### Instructions
<img width="529" alt="Captura de Pantalla 2022-04-26 a la(s) 3 23 09 p  m" src="https://user-images.githubusercontent.com/91048093/165394678-efbf7abb-d207-4fa3-b3b3-c4e3a6bb86a1.png">

### Solution
```javascript
function validSpacing(s) {
  // write your code here
  if(s.charAt(0) === ' ' || s.charAt(s.length - 1) === ' ') { 
     return false;
  }
  
  for(let i = 0; i < s.length; i++) {
    if(s.charAt(i) === ' '){ 
      if(i != 0 && s.charAt(i-1) === ' ') {
        return false;
      }
      if(i != (s.length - 1) && s.charAt(i+1) === ' ') {
        return false;
      }
    }
  }
  
  return true;
}
```
## Fake Binary
### Instruction
<img width="541" alt="Captura de Pantalla 2022-04-26 a la(s) 3 33 13 p  m" src="https://user-images.githubusercontent.com/91048093/165396124-9be8a2c8-220e-40cc-ae5e-2f20d42b57c1.png">

### Solution
```javascript
function fakeBin(x){
   let total = '';
  for (let i = 0; i < x.length; i++) {
    if (parseInt(x[i]) < 5) {
      total +=  '0';
    } else {
      total +=  '1';
    }
  }
  return total;
}
```
## Week Challenge Thursday
## Remove All Exclamation Marks From The End Of Sentence 
### Instruction
<img width="536" alt="Captura de Pantalla 2022-04-26 a la(s) 3 52 51 p  m" src="https://user-images.githubusercontent.com/91048093/165398669-76d018ba-5e9a-4dba-b726-b96f490e9f65.png">

### Solution
```javascript
function remove (string) { 
  let r = '';
  for(var i=string.length-1; i>0 ; i--){
    if(string.charAt(i) !== '!'){
      r = string.substring(0, i+1);
      break;
    }
  }
  return r;
}
```
## Vowel Remover
### Instruction
<img width="547" alt="Captura de Pantalla 2022-04-26 a la(s) 4 04 55 p  m" src="https://user-images.githubusercontent.com/91048093/165400154-fbefab16-da3e-4834-aa4d-455962530498.png">

### Solution
```javascript
function shortcut (string) {
  let r = '';
  for(let i=0; i<string.length; i++){
    if(string[i]!=='a'&& 
       string[i]!=='e'&&
       string[i]!=='i'&&
       string[i]!=='o'&&
       string[i]!=='u')
    {
      r = r + string[i];
    }
  }
  return r;
}
```
## Rock Paper Scissors
### Instruction
<img width="527" alt="Captura de Pantalla 2022-04-26 a la(s) 4 17 50 p  m" src="https://user-images.githubusercontent.com/91048093/165401853-787d287a-02c3-452a-b5d8-7aa47480c75e.png">

### Solution
```javascript
const rps = (p1, p2) => {
  let p1w='Player 1 won!';
  let p2w='Player 2 won!';
  if(p1===p2) return 'Draw!';
  if(p1==='scissors'&&p2==='paper')return p1w;
  if(p1==='paper'&&p2==='rock')return p1w;
  if(p1==='rock'&&p2==='scissors')return p1w;
  return p2w;
};
```
## Persistent Bugger
### Instructions
<img width="549" alt="Captura de Pantalla 2022-04-26 a la(s) 4 52 25 p  m" src="https://user-images.githubusercontent.com/91048093/165405635-01ba485d-3f84-4774-903b-d75b790bc96d.png">

### Solution
```javascript
function persistence(num) {
   //code me
  let t = 0;
  let n = [];
  while (num >= 10) {
    n = num.toString().split('');
    num = 1;
    for (let i = 0; i < n.length; i++) {
      num *= n[i];
    }
    t++;
  }
  return t;
}
```




