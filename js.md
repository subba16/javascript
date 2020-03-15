

![](https://user-images.githubusercontent.com/26511983/76691845-571fad80-661d-11ea-88da-1b31f6b009ad.png)

![](https://user-images.githubusercontent.com/26511983/76691851-728ab880-661d-11ea-8efc-4ed19f339448.png)

![](https://user-images.githubusercontent.com/26511983/76691865-8c2c0000-661d-11ea-85d5-ef3afc03733f.png)

## call back is pushed to the event queue once they are done

![](https://user-images.githubusercontent.com/26511983/76691882-b1b90980-661d-11ea-8a26-4c22185a2ba7.png)

![](https://user-images.githubusercontent.com/26511983/76691919-f6dd3b80-661d-11ea-835a-de25a5762199.png)

## Event loop - If stack is empty, it will push call back to the stack to run call back

![](https://user-images.githubusercontent.com/26511983/76691935-23915300-661e-11ea-96a8-d01dc1193220.png)

![](https://user-images.githubusercontent.com/26511983/76691951-3f94f480-661e-11ea-96b0-a473391b5837.png)

## same with XHR call

![](https://user-images.githubusercontent.com/26511983/76692021-be8a2d00-661e-11ea-915e-828f7f00fade.png)

## Render has high priority than event queue. it waits for stack clear.
### callbacks - sync and async

![](https://user-images.githubusercontent.com/26511983/76692110-c6969c80-661f-11ea-8b5e-3ccaf9a66a03.png)

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

