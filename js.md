
![](https://user-images.githubusercontent.com/26511983/76691809-f1cbbc80-661c-11ea-8cfa-d7857f62a3f3.png)
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

let arr1 = [0, 1, 2];
let arr2 = [3, 4, 5];

arr1 = [...arr2, ...arr1]; 
//  arr1 is now [3, 4, 5, 0, 1, 2]

concatenate two arrays

const arr1 = [0, 1, 2];
const arr2 = [3, 4, 5];

arr1 = [...arr1, ...arr2]; 
//  arr1 is now [0, 1, 2, 3, 4, 5]

const obj1 = { foo: 'bar', x: 42 };
const obj2 = { foo: 'baz', y: 13 };

const clonedObj = { ...obj1 };
// Object { foo: "bar", x: 42 }

const mergedObj = { ...obj1, ...obj2 };
// Object { foo: "baz", x: 42, y: 13 }
```

