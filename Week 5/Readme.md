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
