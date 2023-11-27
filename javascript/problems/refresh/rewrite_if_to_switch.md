# Rewrite the "if" into a "switch" 
## Write the code using switch which would correspond to the following if..else:
```javascript
let a = +prompt('a?', '');

if (a == 0) {
  alert( 0 );
}
if (a == 1) {
  alert( 1 );
}

if (a == 2 || a == 3) {
  alert( '2,3' );
}
```

Solution:
```javascript
let a = +prompt('a?', '');
var r;
switch (a) {
    case 0:
        r = 0;
        break;
    case 1:
        r = 1;
        break;
    case 2:
    case 3:
        r = '2,3';
        break;
}
alert(r)
```
