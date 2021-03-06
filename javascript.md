# JavaScript Cheat Sheet

## Contents
| Section |
|---|
| [Types](#types) |
| [Math](#math) |
| [Conditionals](#conditionals) |
|[Loops](#loops)|

## Types
[Top](#contents)

#### Types  
- string
- number
- boolean
- object
- function
- array
- date
---
#### Typeof  
Get the type of a value.
```javascript
typeof 100 //number
typeof true //boolean
typeof {"test": true} //object
```
---
#### String()  
Convert to a string.
```javascript
String(100); // "100"
String(true); // "true"
```
---
#### Number()  
Convert to a number.
```javascript
Number("100"); // 100
Number(true); // NaN
Number(""); // 0
Number(true); // 1
```
## Math
[Top](#contents)

#### Addition  
Add one value to anouther.
```javascript
c = 1 + 2; // 3
a += 2; // a + 2
b++; // b + 1
```
---
#### Subtraction  
Subtract one value from anouther.
```javascript
c = 2 - 1; // 1
a -= 2; // a - 2
b--; // b - 1
```
---
#### Multiplication  
Multiply two values.
```javascript
c = 2 * 6; // 12
a *= 2; // a * 2
```
---
#### Division  
Divide one value from anouther.
```javascript
c = 1 / 2; // 0.5
a /= 2; // a / 2
```
---
#### Exponentiation
Get one value to the power of anouther.
```javascript
c = 3 ** 2; // 9
a **= 2; // a<sup>2</sup>
```
---
#### Modulus
Get the remainder of a division oporation.
```javascript
a = 5 % 2; // 1
b = 10 % 5; // 0
```
---
#### Math object methods  
| Method | Description |
|-|-|
|abs(x)|Returns the absolute value of x.|
|ceil(x)|Returns x rounded up to the nearest int.|
|floor(x)|Returns x rounded down to the nearest int.|
|max(x, y, z, ..., n)|Returns the largest value.|
|min(x, y, z, ..., n)|Returns the smallest value.|
|pow(x, y)|Returns x raised to the y power.|
|random()|Returns a random number from 0 <= x > 1.|

## Conditionals
[Top](#contents)

#### If  
Run code if a condition returns true.
```javascript
if (x > y) {
  x -= y;
}
````
---
#### Else  
Code to run if a condition is false.
```javascript
if (x > y) {
  x -= y;
} else {
  y -= x;
}
````
---
#### Else if  
Code to run if a condition is false and anouther condition is true.
```javascript
if (x > y) {
  x -= y;
} else if (y == x) {
  x, y = 0;
} else {
  y -= x;
}
```
---
#### Switch  
Select code to run based on a value.
```javascript
switch(x) {
  case 1:
    console.log(x == 1);
    break;
  case 2:
    console.log(x == 2);
    break;
  default:
    console.log(x);
}
```

## Loops
[Top](#contents)

#### For  
Loop through a block of code x times.
```javascript
for (i = 0; i < 10; i++) {
  console.log(i);
}
```
---
#### For/in  
Loop through items in an object.
```javascript
for (x in object) {
  console.log(x.value);
}
```
---
#### For/of  
Loop over iterable data types (arrays, strings, etc).
```javascript
for (x of array) {
  console.log(array[x]);
}
```
---
#### While
Loop over code while a condition is true.
```javascript
var i = 0;
while(i < 10) {
  i++;
  console.log(true);
}
```
---
#### Break  
Stop a loop while it is still going.
```javascript
for (i = 0; i < 10; i++) {
  if (i === 3) { break; }
  console.log(i);
}
console.log("broke");
```
---
#### Continue  
Jump over one iteration of the loop.
```javascript
for (i = 0; i < 10; i++) {
  if (i === 3) { continue; }
  console.log(i);
}
```
