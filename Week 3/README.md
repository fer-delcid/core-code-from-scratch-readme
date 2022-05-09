# Core-Code Week 3
## Core code challenges Monday
## Who Likes It?
### Instructions
<img width="527" alt="Captura de Pantalla 2022-04-26 a la(s) 7 18 51 p  m" src="https://user-images.githubusercontent.com/91048093/165419070-be4708a4-e4e3-4a62-b427-bf8877ecc0f6.png">

### Solution
```javascript
function likes(names) {
  // TODO
  if(names.length==0)return 'no one likes this';
  if(names.length==1)return names[0]+' likes this';
  if(names.length==2)return names[0]+' and '+names[1]+' like this';
  if(names.length==3)return names[0]+', '+names[1]+' and '+names[2]+' like this';
  return (names[0] +', ' +names[1] +' and ' +(names.length - 2) +' others like this');
}
```
## Bit Counting
### Instructions
<img width="524" alt="Captura de Pantalla 2022-04-28 a la(s) 9 13 30 a  m" src="https://user-images.githubusercontent.com/91048093/165785453-58d90d46-aae0-4d7d-903c-c65702577397.png">

### Solution
```javascript
var countBits = function(n) {
  let bin = n.toString(2);
  let cont=0;
  for(let i=0; i<bin.length; i++){
    if(bin[i]==='1')cont++;
  }
  return cont;
};
```
## Your Order, Please
### Instructions
<img width="539" alt="Captura de Pantalla 2022-04-28 a la(s) 11 14 39 p  m" src="https://user-images.githubusercontent.com/91048093/165888491-d0fa9196-6f73-4f16-8e72-ef6f1ae0e264.png">

### Solution
```javascript
function order(words) {
  let arrayOrd = [];
  let palabras = words.split(' ');
  for (let i = 0; i < palabras.length; i++) {
    let numero = getWordNumber(palabras[i]);
    arrayOrd[numero] = palabras[i];
  }
  return cleanUndefined(arrayOrd).join(' ');
}

function getWordNumber(word) {
  for (let i = 0; i < word.length; i++) {
    if (!Number.isNaN(Number(word[i]))) return word[i];
  }
}

function cleanUndefined(array) {
  let result = [];
  for (let i = 0; i < array.length; i++) {
    if (array[i] != undefined) result.push(array[i]);
  }
  return result;
}
```
## Core Code challenges Tuesday
## Simple Pig Latin
### Instructions
<img width="540" alt="Captura de Pantalla 2022-04-29 a la(s) 12 50 28 a  m" src="https://user-images.githubusercontent.com/91048093/165897101-149c04f5-16fc-41ec-8185-bdbad7df583a.png">

### Solution
```javascript
function pigIt(str){
  //Code here
  let arr = [];
  let words = str.split(' ');
  
  for(let i=0; i<words.length; i++){
    arr[i]=finalWord(words[i]);
  }
  
  return arr.join(' ');
}

function finalWord(word){
  let wordLe=word.length;
  let nueva = '';
  let pMarks = ['!', '¡', '?', '¿', '.', ',', ':', ';'];
  
  for(let i=0; i<pMarks.length; i++){
    if(word===pMarks[i]){
      return word;
    }
  }
  
  for(let i=0; i<wordLe; i++){
    let aux = word[0];
    nueva = word.substring(1,wordLe)+aux+'ay';
  }
  return nueva;
}
```
## Decode The Morse Code
### Instructions
<img width="529" alt="Captura de Pantalla 2022-05-03 a la(s) 12 18 31 p  m" src="https://user-images.githubusercontent.com/91048093/166517189-e121f432-c0b0-4cd2-84f4-4829980e2c7f.png">

### Solution
```javascript
decodeMorse = function(morseCode){
  let morseWords = morseCode.split('   ');
  let words=[];
  for(let i=0; i<morseWords.length; i++){
    words[i]=decoWord(morseWords[i]);  
  }
  return words.join(' ').trim();
}

function decoWord(morseWord){
  let s = morseWord.split(' ');
  let sn = [];
  for(let i=0; i<s.length; i++){
    sn[i]=MORSE_CODE[s[i]];
  }
  return sn.join('');
}
```
## Valid Parenthesis
### Instructions
<img width="533" alt="Captura de Pantalla 2022-05-04 a la(s) 8 41 13 a  m" src="https://user-images.githubusercontent.com/91048093/166705737-9caf7fd2-3bc9-4ffd-87d5-db52c6915a49.png">

### Solution
```javascript
function validParentheses(parens) {
  // your code here ..
  let cantidadP = 0;
  for (let i = 0; i < parens.length; i++) {
    if (cantidadP < 0) return false;
    if (parens[i] === '(') cantidadP++;
    if (parens[i] === ')') cantidadP--;  
  }
  
  if(cantidadP==0){
    return true;
  }else{
    return false;
  }
}
```

## Unique Order
### Instructions
<img width="545" alt="Captura de Pantalla 2022-05-09 a la(s) 12 22 57 a  m" src="https://user-images.githubusercontent.com/91048093/167351924-ff84f321-2f07-4c8b-9b39-a6768bce5329.png">

### Solution
```javascript
var uniqueInOrder=function(iterable){
  //your code here - remember iterable can be a string or an array
  let arr = [];
  let aux;
  for (let i = 0; i < iterable.length; i++) {
    if (iterable[i] !== aux) {
      aux = iterable[i];
      arr.push(aux);
    }
  }
  return arr;
}
```
## Week Challenges Thursday
