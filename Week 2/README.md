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
