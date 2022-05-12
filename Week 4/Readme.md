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
<img width="546" alt="Captura de Pantalla 2022-05-12 a la(s) 1 18 10 a  m" src="https://user-images.githubusercontent.com/91048093/168013853-bfc48cc4-ff8e-42f4-94bc-afb63afe6319.png">

### Solution
```javascript
function getNumberFromString(s) {
  return Number(s.replace(/\D/g, ''));
}
```

## Week Challenges Thursday
## String Cleaning
### Instructions
<img width="538" alt="Captura de Pantalla 2022-05-12 a la(s) 1 24 23 a  m" src="https://user-images.githubusercontent.com/91048093/168014977-f4ca2ffb-c775-4d0f-a2e5-11d1b828b533.png">

### Solution
```javascript
function stringClean(s){
  return s.replace(/\d/g,'');
}
```

## Password Validation
### Instructions
<img width="543" alt="Captura de Pantalla 2022-05-12 a la(s) 1 27 21 a  m" src="https://user-images.githubusercontent.com/91048093/168015504-2ed2a35f-f0d4-419e-a251-28ca55288bc2.png">

### Solution
```javascript
function validate(password) {
  return /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[a-zA-Z0-9]{6,}$/.test(password);
}
```

