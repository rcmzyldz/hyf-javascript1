# First Part Homework Javascript1

[My FreeCodeCamp Portfolio](https://www.freecodecamp.org/alfiyusrina)
## 1. Comment Your Code

```
// this is my first comment
/* this is a multi line comment */
```

## 2. Declare Variables
```
var myName;
```

## 3.Storing Values with the Assignment Operator
```
a = 7;
b = a;
a = b;
```

## 4. Initializing Variables with the Assignment Operator
```
var a = 9;
```

## 5. Understanding Uninitialized Variables
```
var a = 5;
var b = 10;
var c = "I am a";
```
## 6. Understanding Case Sensitivity in Variables
```
// Declarations
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

// Assignments
studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;
```

## 7.Add Two Numbers (+)
```
var sum = 10 + 0;
sum = 10 + 10;
```
## 8. Subtract One Number from Another
```
var difference = 45 - 33;
```
## 9. Multiply Two Numbers
```
var product = 8 * 10;
```
## 10. Divide One Number by Another (/)
```
var quotient = 66 / 33;
```
## 11 .Increment a Number (i++)

```
var myVar = 87;
myVar++;
```

## 12. Decrement a Number (i--)
```
myVar--;
```


## 13. Create Decimal Numbers
```
var myDecimal = 8.8;
```

## 14. Multiply Two Decimals
```
var product = 2.0 * 2.5;
```

## 15. Divide One Decimal by Another
```
var quotient = 4.4 / 2.0;
```
## 16. Finding a Remainder
```
var remainder;
remainder = 11 % 3;
```
## 17. Compound Assignment With Augmented Addition (+=)
```
a += 12;
b += 9;
c += 7;
```
## 18. Compound Assignment With Augmented Subtraction (-=)

```
a -= 6;
b -= 15;
c -= 1;
```
## 19. Compound Assignment With Augmented Multiplication
```
a *= 5;
b *= 3;
c *= 10;
```
## 20. Compound Assignment With Augmented Division
```
a /= 12;
b /= 4;
c /= 11;
```

## 21. Declare String Variables
with  ``` " "  ```
```
var myFirstName = "Alfi";
var myLastName = "Yusrina";
```

## 22. Escaping Literal Quotes in Strings
Using *backlash* ```\``` in the beginning and in the end of your quotes.
```
var myStr = "I am a \"double quoted\" string inside \"double quotes\".";
```
## 23. Quoting Strings with Single Quotes
String values in JS may be written with single or double quotes.
```
var myStr = '<a href="http://www.example.com" target="_blank">Link</a>';
```

## 24. Escape Sequences in Strings
Reasons to use escaping characters:
- is to allow you to use characters you might not otherwise be able to type out, such as a backspace.
- is to allow you to represent multiple quotes in a string without JS misinterpreting what you mean.

```
var myStr = 'FirstLine\n\t\\SecondLine\nThirdLine';
```

## 25. Concatenating Strings with Plus Operator
```
var myStr = "This is the start. " +  "This is the end.";
```
## 26. Concatenating Strings with the Plus Equals Operator
```
var myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";
```
## 27. Constructing Strings with Variables
```
var myStr = "My name is " + myName + " and I am well!";
```
## 28. Appending Variables to Strings
```
var someAdjective = "boring";
var myStr = "Learning to code is ";
myStr += someAdjective;
```
## 29. Find the Length of a String
```
lastNameLength = lastName.length;
```
## 30. Use Bracket Notation to Find the First Character in a String
```
firstLetterOfLastName = lastName[0];
```
## 31. Understand String Immutability
String values are *immutable*, means that they cannot be altered once created.
```
myStr = "Hello World";
```
## 32. Use Bracket Notation to Find the Nth Character in a String
```
var thirdLetterOfLastName = lastName[2];
```
## 33. Use Bracket Notation to Find the Last Character in a String
Use  ```.length-1```
```
var lastLetterOfLastName = lastName[lastName.length-1];
```
## 34. Use Bracket Notation to Find the Nth-to-Last Character in a String
```
var secondToLastLetterOfLastName = lastName[lastName.length - 2];
```
## 35. Word Blanks
```
function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) {
  var result = "The " + myAdjective + " " + myNoun + " " + myVerb + " " + myAdverb + ".";
  return result;
}
wordBlanks("cat", "little", "hit", "slowly");
```
## 36. Store Multiple Values in one Variable using JavaScript Arrays
Array variables for storing several pieces of data in one place.
```
var myArray = ["Alfi", 28];
```
## 37. Nest one Array within Another Array
```
var myArray = [["Bulls", 23], ["White Sox", 45]];
```
## 38. Access Array Data with Indexes
```
var myData = myArray[0];
```
## 39. Modify Array Data With Indexes
```
myArray[0] = 45;
```
## 40. Access Multi-Dimensional Arrays With Indexes
```
var myData = myArray[2][1];
```
## 41. Manipulate Arrays With push()
Adding an extra to the last array.
```
myArray.push(["dog", 3]);
```
## 42. Manipulate Arrays With pop()
You can pop off the last array, and store it in a variable.
```
var removedFromMyArray = myArray.pop();
```
## 43. Manipulate Arrays With shift()
removing the first in the array
```
var removedFromMyArray = myArray.shift();
```
## 44. Manipulate Arrays With unshift()
Adding an extra to the first in the array.
```
var myArray = [["John", 23], ["dog", 3]];
myArray.shift();

myArray.unshift(["Paul",35]);
```
## 45. Shopping List
```
var myList = [["rice", 5] , ["bread", 6] , ["cake", 7], [ "quinoa", 9], ["potato", 20]];
```
## 46. Write Reusable JavaScript with Functions
```
function reusableFunction() {
  console.log("Hi World");
}

reusableFunction();
```
## 47. Passing Values to Functions with Arguments
```
function functionWithArgs (a , b) {
console.log(a + b);
}
functionWithArgs (1 , 2);
functionWithArgs (7 , 9);
```
## 48. Global Scope and Functions
Scope refers to the visibility of variables.
Variables which are defined **outside of a function block** have **Global scope**.
Variables which are used **without the ```var```** keyword are automatically created in the ```global``` scope. This can create unintended consequences elsewhere in your code or when running a function again. You should always declare your variables with ```var```.
```
var myGlobal = 10;
function fun1() {
  oopsGlobal = 5;
}
```
## 49. Local Scope and Functions
```
function myLocalScope() {
var myVar = 'use strict';
}
myLocalScope();
```
## 50. Global vs. Local Scope in Functions
```
var outerWear = "T-Shirt";
function myOutfit() {
  var outerWear = "sweater";
  return outerWear;
}
myOutfit();
```
## 51. Return a Value from a Function with Return
Use a ```return``` statement to send a value back out of a function.
```
function timesFive (num) {
  return num * 5;
}
timesFive(5);
timesFive(2);
timesFive(0);
```
## 52. Understanding Undefined Value returned from a Function
```
function addFive() {
  sum = sum + 5;
}
```
## 53. Assignment with a Returned Value
```
var processed = 0;
function processArg(num) {
  return (num + 3) / 5;
}
processed = processArg(7);
```
## 54. Stand in Line
 A **queue** is an abstract Data Structure where items are kept in order.
 New items can be added (```push```) at the back of the queue and old items are taken off (```shift```) from the front of the queue.

Add the number to the end of the array = ```push```
Remove the first element of the array = ```shift```
Then return the element that was removed = using ```return```.
```
function nextInLine(arr, item) {
  arr.push(item);
  return  arr.shift();
}
```
## 55. Understanding Boolean Values
```
function welcomeToBooleans() {
return true;
}
```
## 56. Use Conditional Logic with If Statements
```
function trueOrFalse(wasThatTrue) {
    if (wasThatTrue) {
    return "Yes, that was true";
  }
  return "No, that was false";
}
trueOrFalse(true);
```
## 57. Comparison with the Equality Operator
```
function testEqual(val) {
  if (val == 12) {
    return "Equal";
  }
  return "Not Equal";
}
testEqual(12);
```
## 58. Comparison with the Strict Equality Operator
However, unlike the equality operator, which attempts to convert both values being compared to a common type, the strict equality operator does not perform a type conversion.

If the values being compared have different types, they are considered unequal, and the strict equality operator will return false.
```
function testStrict(val) {
  if (val === 7) {
    return "Equal";
  }
  return "Not Equal";
}
testStrict(10);
```
## 59. Practice comparing different values
```
function compareEquality(a, b) {
  if (a === b) {
    return "Equal";
  }
  return "Not Equal";
}
compareEquality(10, "10");
```
## 60. Comparison with the Inequality Operator
```
function testNotEqual(val) {
  if (val != 99) {
    return "Not Equal";
  }
  return "Equal";
}
testNotEqual(10);
```
## 61. Comparison with the Strict Inequality Operator
```
function testStrictNotEqual(val) {
  if (val !== 17) {
    return "Not Equal";
  }
  return "Equal";
}

testStrictNotEqual(10);
```
## 62. Comparison with the Greater Than Operator
```
function testGreaterThan(val) {
  if (val > 100) {
    return "Over 100";
  }

  if (val > 10) {
    return "Over 10";
  }

  return "10 or Under";
}

testGreaterThan(10);
```
## 63. Comparison with the Greater Than Or Equal To Operator
```
function testGreaterOrEqual(val) {
  if (val >= 20) {
    return "20 or Over";
  }

  if (val >= 10) {
    return "10 or Over";
  }

  return "Less than 10";
}


testGreaterOrEqual(10);
```
## 64. Comparison with the Less Than Operator
```
function testLessThan(val) {
  if (val < 25) {
    return "Under 25";
  }

  if (val < 55) {
    return "Under 55";
  }

  return "55 or Over";
}

testLessThan(10);
```
## 65. Comparison with the Less Than Or Equal To Operator
```
function testLessOrEqual(val) {
  if (val <= 12) {
    return "Smaller Than or Equal to 12";
  }

  if (val <=24) {
    return "Smaller Than or Equal to 24";
  }

  return "More Than 24";
}

testLessOrEqual(10);

```
## 66. Comparison with the Logical And Operator
```
function testLogicalAnd(val) {

  if (val >= 25 && val <= 50) {
      return "Yes";
  }

  return "No";
}


testLogicalAnd(10);
```
## 67. Comparison with the Logical Or Operator
```
function testLogicalOr(val) {


  if (val < 10 || val > 20 ) {

    return "Outside";
  }

  return "Inside";
}


testLogicalOr(15);
```
## 68. Introducing Else Statements

```
function testElse(val) {
  var result = "";

  if (val > 5) {
    result = "Bigger than 5";
  }

  else {
    result = "5 or Smaller";
  }


  return result;
}


testElse(4);

```
## 69. Introducing Else If Statements
```
function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  }

  else if (val < 5) {
    return "Smaller than 5";
  }
  else {
      return "Between 5 and 10";
  }

}

testElseIf(7);

```
## 70. Logical Order in If Else Statements
```
function orderMyLogic(val) {
  if (val < 5) {
    return "Less than 5";
  } else if (val < 10) {
    return "Less than 10";
  } else {
    return "Greater than or equal to 10";
  }
}

orderMyLogic(7);
```
## 71. Chaining If Else Statements
```
function testSize(num) {
  if(num < 5) {
    return "Tiny";
  } else if (num < 10) {
 return "Small";
  } else if (num < 15) {
return "Medium";
  } else if (num < 20) {
return "Large";
  } else if ( num >= 20 ) {
    return "Huge";
    } else {
    return "Change Me"; }

}

testSize(7);
```
## 72. Golf Code
```
var names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];
function golfScore(par, strokes) {
  if (strokes == 1) {
return "Hole-in-one!";
  } else if (strokes <= par - 2) {
     return "Eagle" ;
  } else if (strokes == par - 1) {
     return "Birdie" ;
  } else if (strokes == par) {
     return "Par" ;
  } else if (strokes == par + 1) {
     return "Bogey" ;
  } else if (strokes == par + 2) {
     return "Double Bogey" ;
  } else if (strokes >= par + 3) {
     return "Go Home!" ;
  } else {
     return "Change Me";
  }
}

golfScore(5, 4);
```

Resource: [freeCodeCamp](https://www.freecodecamp.org/)
