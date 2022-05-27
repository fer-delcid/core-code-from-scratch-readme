## Week 6 Challenges

## Week challenges Monday
## Square(n) Sum
### Instructions
<img width="543" alt="Captura de Pantalla 2022-05-26 a la(s) 10 51 15 a  m" src="https://user-images.githubusercontent.com/91048093/170536077-bf137c7e-6105-45f6-8572-e961583775cd.png">

### Solution
```javascript  
export function squareSum(numbers: number[]): number {
  return numbers.reduce((prev: number, curr: number) => prev + Math.pow(curr, 2),0);
}
  ```
