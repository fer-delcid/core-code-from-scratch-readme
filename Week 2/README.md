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



