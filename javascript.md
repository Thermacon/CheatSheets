# JavaScript Cheat Sheet

| Table of Contents |
|---|
| [Types](#types) |
|[Loops](#loops)|

## Types
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
String(100) // "100"
String(true) // "true"
```
---
#### Number()  
Convert to a number.
```javascript
Number("100") // 100
Number(true) // NaN
Number("") // 0
Number(true) // 1
```

## Loops
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