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
## Growth of a population
### Instructions
<img width="543" alt="Captura de Pantalla 2022-06-01 a la(s) 12 33 10 p  m" src="https://user-images.githubusercontent.com/91048093/171477309-75e00eb2-b69d-4ba9-b345-cab03661f155.png">

### Solution
```javascript
export class G964 {

    public static nbYear = (p0, percent, aug, p) => {
        // your code
      let tot =p0;
      let years = 0;
      percent = percent/100;
      while (tot < p) {
        tot = parseInt(tot + tot * percent + aug);
        years++;
      }
    return years;
    }
  
}
```
