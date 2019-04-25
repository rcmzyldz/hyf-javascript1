# [freeCodeCamp](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/debugging) Introduction to the Debugging Challenges

### Index
1. [Use the JavaScript Console to Check the Value of a Variable](Use the JavaScript Console to Check the Value of a Variable)
1. [Understanding the Differences between the freeCodeCamp and Browser Console](Understanding the Differences between the freeCodeCamp and Browser Console)
1. [Use typeof to Check the Type of a Variable](Use-typeof-to-Check-the-Type-of-a-Variable)
1. [Catch Misspelled Variable and Function Names](Catch-Misspelled-Variable-and-Function-Names)
1. [Catch Unclosed Parentheses, Brackets, Braces and Quotes](Catch-Unclosed-Parentheses,-Brackets,-Braces-and-Quotes)
1. [Catch Mixed Usage of Single and Double Quotes](Catch-Mixed-Usage-of-Single-and-Double-Quotes)
1. [Catch Use of Assignment Operator Instead of Equality Operator](Catch-Use-of-Assignment-Operator-Instead-of-Equality-Operator)
1. [Catch Missing Open and Closing Parenthesis After a Function Call](Catch-Missing-Open-and-Closing-Parenthesis-After-a-Function-Call)
1. [Catch Arguments Passed in the Wrong Order When Calling a Function](Catch-Arguments-Passed-in-the-Wrong-Order-When-Calling-a-Function)
1. [Catch Off By One Errors When Using Indexing](Catch-Off-By-One-Errors-When-Using-Indexing)
1. [Use Caution When Reinitializing Variables Inside a Loop](Use-Caution-When-Reinitializing-Variables-Inside-a-Loop)
1. [Prevent Infinite Loops with a Valid Terminal Condition](Prevent-Infinite-Loops-with-a-Valid-Terminal-Condition)

### Exercise
## Use the JavaScript Console to Check the Value of a Variable
```js
let a = 5;
let b = 1;
a++;
console.log(a);


let sumAB = a + b;
console.log(sumAB);
```

## Understanding the Differences between the freeCodeCamp and Browser Console
```js
// Open your browser console
let outputTwo = "This will print to the browser console 2 times";
// Use console.log() to print the outputTwo variable
console.log(outputTwo);

let outputOne = "Try to get this to log only once to the browser console";


// Use console.clear() in the next line to print the outputOne only once
console.clear();


// Use console.log() to print the outputOne variable
console.log(outputOne);

```

## Use typeof to Check the Type of a Variable
```js
let seven = 7;
let three = "3";
console.log(seven + three);
// Add your code below this line
console.log(typeof seven);
console.log(typeof three);
```

## Catch Misspelled Variable and Function Names
```js
let receivables = 10;
let payables = 8;
let netWorkingCapital = receivables - payables;
console.log(`Net working capital is: ${netWorkingCapital}`);
```

## Catch Unclosed Parentheses, Brackets, Braces and Quotes
```js
let myArray = [1, 2, 3];
let arraySum = myArray.reduce((previous, current) =>  previous + current);
console.log(`Sum of array values is: ${arraySum}`);
```

## Catch Mixed Usage of Single and Double Quotes
```js
let innerHtml = "<p>Click here to <a href='#Home'>return home</a></p>";
console.log(innerHtml);
```

## Catch Use of Assignment Operator Instead of Equality Operator
```js
let x = 7;
let y = 9;
let result = "to come";

if(x === y) {
  result = "Equal!";
} else {
  result = "Not equal!";
}

console.log(result);
```

## Catch Missing Open and Closing Parenthesis After a Function Call
```js
function getNine() {
  let x = 6;
  let y = 3;
  return x + y;
}

let result = getNine();
console.log(result);
```

## Catch Arguments Passed in the Wrong Order When Calling a Function
```js
function raiseToPower(b, e) {
  return Math.pow(b, e);
}
let exp = 3;
let base = 2;
let power = raiseToPower(base, exp);
console.log(power);
```

## Catch Off By One Errors When Using Indexing
```js
function countToFive() {
  let firstFive = "12345";
  let len = firstFive.length;
  // Fix the line below
  for (let i = 0; i < len; i++) {
  // Do not alter code below this line
    console.log(firstFive[i]);
  }
}

countToFive();
```

## Use Caution When Reinitializing Variables Inside a Loop
```js
function zeroArray(m, n) {
  // Creates a 2-D array with m rows and n columns of zeroes
  let newArray = [];

  for (let i = 0; i < m; i++) {
    // Adds the m-th row into newArray
    let row = [];
    for (let j = 0; j < n; j++) {
      // Pushes n zeroes into the current row to create the columns
      row.push(0);
    }
    // Pushes the current row, which now has n zeroes in it, to the array
    newArray.push(row);
  }
  return newArray;
}

let matrix = zeroArray(3, 2);
console.log(matrix);
```

## Prevent Infinite Loops with a Valid Terminal Condition
```js
function myFunc() {
  for (let i = 1; i <= 4; i += 2) {
    console.log("Still going!");
  }
}
```
