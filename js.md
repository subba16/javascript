
## hasOwnProperty 
```javascript
const object1 = new Object();
object1.property1 = 42;

console.log(object1.hasOwnProperty('property1'));
// expected output: true

hasOwnProperty returns true even if the value of the property is null or undefined
o = new Object();
o.propOne = null;
o.hasOwnProperty('propOne');   // returns true
o.propTwo = undefined;  
o.hasOwnProperty('propTwo');   // returns true
```

## spread Operator

```javascript
const parts = ['shoulders', 'knees']; 
const lyrics = ['head', ...parts, 'and', 'toes']; 
//  ["head", "shoulders", "knees", "and", "toes"]

```

