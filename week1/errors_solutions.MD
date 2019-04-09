# Second Part Homework Javascript1
Resource: [Janke Learning Errors](https://github.com/janke-learning/errors/blob/master/README.md)

## 1. Malfomed while loop
broken code:
```js
let value = 0;
while (value < 9)
  value++;
};
```
error message:
```
Uncaught SyntaxError: Unexpected token }
```
classification:
* creation phase
* syntax

the fix:
```js
let value = 0;
while (value < 9) {
  value++;
};
```
## 2. Missing variable name

broken code:
```js
var = 5;
```
error message:
```
Uncaught SyntaxError: Unexpected token =
```
classification:
* creation phase
* syntax

the fix:
```js
var five = 5;
```
my notes: always give a name to your variables.

## 3. Too-far object access
broken code:
```js
let a = {b:3};
let b = a.b.3
```
error message:
```
Uncaught SyntaxError: Unexpected number
```
classification:
* creation phase
* syntax

the fix:
```js
let a = {b:3};
let b = a.b
```

## 4. Access property directly
broken code:
```js
let x = {b:'e'};
let y = b.e;
```
error message:
```
ReferenceError: b is not defined
```
classification:
* execution phase
* semantic

the fix:
```js

```
my notes: There is a non-existent variable referenced somewhere. This variable needs to be declared, or make sure it is available in the current script or scope.


## 5. Improper multi-line string
broken code:
```js
let a = 'this is
two lines';
```
error message:
```
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:
## 6. Improper end of statement
broken code:
```js
let a = 1:
```
error message:
```
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:
## 7. Malformed array
broken code:
```js
let myArray = [1, 2, 3;
```
error message:
```
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:
## 8. Missing arguments
broken code:
```js
function getNine {
  let x = 6;
  let y = 3;
  return x + y;
}
let result = getNine();
```
error message:
```
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:

## 9. Improper nested quotes 1
broken code:
```js
let innerHtml = "<p>Click here to <a href="#Home">return home</a></p>";
```
error message:
```
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:

## 10.Improper nested quotes 2
broken code:
```js
let nested_messages = 'remind yourself ''i can do this!'' at least once a day';
```
error message:
```
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:

## 11. Reassigning to constant
broken code:
```js
const a = 9;
a = 0;
```
error message:
```
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:

## 12. Unassigned const declaration
## unassigned const declaration
broken code:
```js
const a;
a = 0;
```
error message:
```
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:
## 13. Is not a function
broken code:
```js
let array = [];
array.length()
```
error message:
```
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
```
your notes:
