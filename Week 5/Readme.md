## Week 5 Challenges

## Week challenges Monday
## Find the missing letter
### Instructions
<img width="535" alt="Captura de Pantalla 2022-05-12 a la(s) 8 28 10 p  m" src="https://user-images.githubusercontent.com/91048093/168199380-1166e15e-40ef-43fb-85fc-4f869e9c6efe.png">

### Solution
```javascript
function findMissingLetter(array)
{
  for (let i = 0; i < array.length; i++) {
    if (array[i+1].charCodeAt() !== array[i].charCodeAt()+1) {
      return String.fromCharCode(array[i].charCodeAt() + 1);
    }
  }
}
```
## Week Challenge Thursday
## Whats your poison?
### Instructions
<img width="537" alt="Captura de Pantalla 2022-05-26 a la(s) 10 12 55 a  m" src="https://user-images.githubusercontent.com/91048093/170529152-5eeaf60b-450f-418b-9d16-8016f0ba51fc.png">

### Solution
```javascript
function find(rats) {
    let n = 0;
    for (let i = 0; i < rats.length; i++) {
      n += 2**rats[i];
    }
    
    return n;
}
```

## Array.diff
### Instructions
<img width="527" alt="Captura de Pantalla 2022-05-26 a la(s) 10 25 40 a  m" src="https://user-images.githubusercontent.com/91048093/170531414-75955eca-74ab-49a3-86c4-9292723ea1f0.png">

### Solution 
```javascript
function array_diff(a, b) {
  return a.filter((i) => !b.includes(i));
}
```
