
# [freeCodeCamp](https://www.freecodecamp.org/) Javascript Exercise Part 2

My JavaScript Exercise part 1 is [here](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD).

### Index
1. [Selecting from Many Options with Switch Statements](#Selecting-from-Many-Options-with-Switch-Statements)
1. [Adding a Default Option in Switch Statements](#adding-a-default-option-in-switch-statements)
1. [Multiple Identical Options in Switch Statements](#multiple-identical-options-in-switch-statements)
1. [Replacing If Else Chains with Switch](#replacing-if-else-chains-with-switch)
1. [Returning Boolean Values from Functions](#returning-boolean-values-from-functions)
1. [Return Early Pattern for Functions](#return-early-pattern-for-functions)
1. [Counting Cards](#counting-cards)
1. [Build JavaScript Objects](#build-javaScript-objects)
1. [Accessing Object Properties with Dot Notation](#accessing-object-properties-with-dot-notation)
1. [Accessing Object Properties with Bracket Notation](#accessing-object-properties-with-bracket-notation)
1. [Accessing Object Properties with Variables](#accessing-object-properties-with-variables)
1. [Updating Object Properties](#updating-object-properties)
1. [Add New Properties to a JavaScript Object](#add-new-properties-to-a-javaScript-object)
1. [Delete Properties from a JavaScript Object](#delete-properties-from-a-javaScript-object)
1. [Using Objects for Lookups](#using-objects-for-lookups)
1. [Testing Objects for Properties](#Testing-Objects-for-Properties)
1. [Manipulating Complex Objects](#Manipulating-Complex-Objects)
1. [Accessing Nested Objects](#Accessing-Nested-Objects)
1. [Accessing Nested Arrays](#Accessing-Nested-Arrays)
1. [Record Collection](#Record-Collection)
1. [Iterate with JavaScript While Loops](#Iterate-with-JavaScript-While-Loops)
1. [Iterate with JavaScript For Loops](#Iterate-with-JavaScript-For-Loops)
1. [Iterate Odd Numbers With a For Loop](#Iterate-Odd-Numbers-With-a-For-Loop)
1. [Count Backwards With a For Loop](#Count-Backwards-With-a-For-Loop)
1. [Iterate Through an Array with a For Loop](#Iterate-Through-an-Array-with-a-For-Loop)
1. [Nesting For Loops](#Nesting-For-Loops)
1. [Iterate with JavaScript Do...While Loops](#Iterate-with-JavaScript-Do-While-Loops)
1. [Profile Lookup](#Profile-Lookup)
1. [Generate Random Fractions with JavaScript](#Generate-Random-Fractions-with-JavaScript)
1. [Generate Random Whole Numbers with JavaScript](#Generate-Random-Whole-Numbers-with-JavaScript)
1. [Generate Random Whole Numbers within a Range](#Generate-Random-Whole-Numbers-within-a-Range)
1. [Use the parseInt Function](#Use-the-parseInt-Function)
1. [Use the parseInt Function with a Radix](#Use-the-parseInt-Function-with-a-Radix)
1. [Use the Conditional (Ternary) Operator](#Use-the-Conditional-Ternary-Operator)
1. [Use Multiple Conditional (Ternary) Operators](#Use-Multiple-Conditional-Ternary-Operators)

### Exercise
## Selecting from Many Options with Switch Statements
```js
function caseInSwitch(val) {
  var answer = "";
  switch(val) {
  case 1:
    return "alpha";
    break;
  case 2:
    return "beta";
    break;
  case 3:
    return "gamma";
    break;
     case 4:
   return "delta";
    break;
}

  return answer;
}

caseInSwitch(1);
caseInSwitch(2);
caseInSwitch(3);
caseInSwitch(4);
```

## Adding a Default Option in Switch Statements
```js
function switchOfStuff(val) {
  var answer = "";
    switch(val) {
  case "a":
    answer = "apple";
    break;
  case "b":
    answer = "bird";
    break;
  case "c":
    answer = "cat";
    break;
  default:
   answer = "stuff";
}

  return answer;
}

switchOfStuff(1);
```

## Multiple Identical Options in Switch Statements
```js
function sequentialSizes(val) {
  var answer = "";
  switch(val) {
  case 1:
  case 2:
  case 3:
    answer = "Low";
    break;
  case 4:
  case 5:
  case 6:
    answer = "Mid";
    break;
  case 7:
  case 8:
  case 9:
    answer = "High";
}
  return answer;
}

sequentialSizes(1);

```

## Replacing If Else Chains with Switch
```js
function chainToSwitch(val) {
  var answer = "";

  switch(val) {
  case "bob":
    answer = "Marley";
    break;
  case 42:
    answer = "The Answer";
    break;
  case 1:
    answer = "There is no #1";
    break;
  case 99:
    answer = "Missed me by this much!";
    break;
  case 7:
    answer = "Ate Nine";
    break;
  default:
    answer = "";
    break;
}

  return answer;
}

chainToSwitch(7);

```

## Returning Boolean Values from Functions
```js
{
}
```

## Return Early Pattern for Functions
```js
{
}
```

## Counting Cards
```js
{
}
```

## Build JavaScript Objects
```js
{  // completed example
  function f(param_1, param_2, param_3) {
    var result = param_2 + param_3 + param_1;
    return result;
  };

  // set values in the args to pass the assert
  let arg_1 = "x", arg_2 = "z", arg_3 = "y";
  let return_val = f(arg_1, arg_2, arg_3);

  console.assert(return_val === "zyx", "example: return_val === " + return_val);
}
```

## Accessing Object Properties with Dot Notation
## Accessing Object Properties with Bracket Notation
## Accessing Object Properties with Variables
## Updating Object Properties
## Add New Properties to a JavaScript Object
## Delete Properties from a JavaScript Object
## Using Objects for Lookups
## Testing Objects for Properties
## Manipulating Complex Objects
## Accessing Nested Objects
## Accessing Nested Arrays
## Record Collection
## Iterate with JavaScript While Loops
## Iterate with JavaScript For Loops
## Iterate Odd Numbers With a For Loop
## Count Backwards With a For Loop
## Iterate Through an Array with a For Loop
## Nesting For Loops
## Iterate with JavaScript Do While Loops
## Profile Lookup
## Generate Random Fractions with JavaScript
## Generate Random Whole Numbers with JavaScript
## Generate Random Whole Numbers within a Range
## Use the parseInt Function
## Use the parseInt Function with a Radix
## Use the Conditional Ternary Operator
## Use Multiple Conditional Ternary Operators
