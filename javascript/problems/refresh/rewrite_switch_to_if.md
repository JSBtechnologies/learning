# Rewrite the "switch" into an "if" 
## Write the code using if..else which would correspond to the following switch:
```javascript
switch (browser) {
  case 'Edge':
    alert( "You've got the Edge!" );
    break;

  case 'Chrome':
  case 'Firefox':
  case 'Safari':
  case 'Opera':
    alert( 'Okay we support these browsers too' );
    break;

  default:
    alert( 'We hope that this page looks ok!' );
}
```

Solution:
```javascript
if (browser == 'Edge') {
    alert( "You've got the Edge!" );
} else if (['Chrome', 'FireFox', 'Safari', 'Opera'].indexOf(browser) > -1) {
    alert( 'Okay we support these browsers too' );
} else {
    alert( 'We hope that this page looks ok!' );
}
```
