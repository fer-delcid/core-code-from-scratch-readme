# Core Code Week 4

## Week Challenge Wednesday
## Simple Validation of a username
### Instructions
<img width="525" alt="Captura de Pantalla 2022-05-10 a la(s) 9 25 37 a  m" src="https://user-images.githubusercontent.com/91048093/167665040-769d0c1c-4111-4fe0-8249-8ef066977c4c.png">

### Solution
```javascript
function validateUsr(username) {
  return /^([a-z]+|[0-9]+|_){4,16}$/.test(username);
}
```
## Get Number From String
### Instructions
