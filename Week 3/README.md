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
