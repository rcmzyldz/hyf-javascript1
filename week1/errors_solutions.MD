# Second Part Homework
Resource: [Janke Learning Errors](https://github.com/janke-learning/errors/blob/master/README.md)

## 1. Malformed while loop
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
let x = {b:'e'};
let y = x.b;
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
Uncaught SyntaxError: Invalid or unexpected token
```
classification:
* creation phase
* syntax

the fix:
```js
let a = 'this is\ntwo lines';
```
my notes: A specific language construct was expected, but something else was provided. This is a simple typo.

## 6. Improper end of statement
broken code:
```js
let a = 1:
```
error message:
```
Uncaught SyntaxError: Unexpected token :

```
classification:
* creation phase
* syntax

the fix:
```js
let a = 1;
```
my notes: idem

## 7. Malformed array
broken code:
```js
let myArray = [1, 2, 3;
```
error message:
```
Uncaught SyntaxError: Unexpected token ;

```
classification:
* creation phase
* syntax

the fix:
```js
let myArray = [1, 2, 3];
```
my notes: idem
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
Uncaught SyntaxError: Unexpected token {

```
classification:
* creation phase
* syntax

the fix:
```js
function getNine () {
  let x = 6;
  let y = 3;
  return x + y;
}
let result = getNine();
```
my notes: Brackets for ```param``` is missing,  so the argument can't be passed to the function.

## 9. Improper nested quotes 1
broken code:

```js
let innerHtml = "<p>Click here to <a href="#Home">return home</a></p>";
```

error message:

```
Uncaught SyntaxError: Invalid or unexpected token
```
classification:
* creation phase
* syntax

the fix:

```js
let innerHtml = '<p>Click here to <a href="#Home">return home</a></p>';
```

my notes: Quoting Strings with single quotes.

## 10.Improper nested quotes 2
broken code:
```js
let nested_messages = 'remind yourself ''i can do this!'' at least once a day';
```
error message:
```
Uncaught SyntaxError: Unexpected string
```
classification:
* creation phase
* syntax

the fix:
```js
let nested_messages = 'remind yourself \'i can do this!\' at least once a day';
```
my notes: Fixed it backlash.

## 11. Reassigning to constant
broken code:

```js
const a = 9;
a = 0;
```
error message:
```
Uncaught SyntaxError: Identifier 'a' has already been declared
TypeError: Assignment to constant variable.
```

classification:
* Execution phase
* Semantic

the fix:
```js
const a = 9;
```
my notes: The variable identifier cannot be reassigned.

## 12. Unassigned const declaration
## unassigned const declaration
broken code:
```js
const a;
a = 0;
```
error message:
```
Uncaught SyntaxError: Missing initializer in const declaration
```
classification:
* creation phase
* syntax

the fix:
```js
const a = 0;
```
my notes: **An initializer for a constant is required.** You must specify its value in the same statement in which it's declared (which makes sense, given that it can't be changed later).

## 13. Is not a function
broken code:

```js
let array = [];
array.length()
```
error message:

```
Uncaught TypeError: array.length is not a function
```

classification:
* execution phase
* semantic

the fix:

```js
let array = [];
array.length;
```

my notes: It attempted to call a value from a function, but the value is not actually a function. The ```length``` property is an instance of type Array sets or returns the number of elements in that array, thus not a function.
