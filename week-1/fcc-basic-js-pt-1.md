> complete [the basic JS exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript) through _Counting Cards_ & paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD) 

## 1. Comment Your Code

```js
//This is a comment.
/*This is a possibly multiline
comment.*/
```

## 2. Declare JavaScript Variables

```js
var myName;
```

## 3. Storing Values with the Assignment Operator

```js
var a;
var b = 2;

a=7;
b=a;
```

## 4. Initializing Variables with the Assignment Operator

```js
var a=9;
```

## 5. Understanding Uninitialized Variables

```js
var a=5;
var b=10;
var c="I am a";

// Do not change code below this line

a = a + 1;
b = b + 5;
c = c + " String!";
```

## 6. Understanding Case Sensitivity in Variables

```js
var studlyCapVar;
var properCamelCase;
var titleCaseOver;
```

## 7. Add Two Numbers with JavaScript

```js
var sum = 10 + 10;
```

## 8. Subtract One Number from Another with JavaScript

```js
var difference = 45 - 33;
```

## 9. Multiply Two Numbers with JavaScript

```js
var product = 8 * 10;
```

## 10. Divide One Number by Another with JavaScript

```js
var quotient = 66 / 33;
```

## 11. Increment a Number with JavaScript

```js
var myVar = 87;
myVar++;
```

## 12. Decrement a Number with JavaScript

```js
var myVar = 11;
myVar--;
```

## 13. Create Decimal Numbers with JavaScript

```js
var myDecimal=8.7;
```

## 14. Multiply Two Decimals with JavaScript

```js
var product = 2.0 * 2.5;
```

## 15. Divide One Decimal by Another with JavaScript

```js
var quotient = 4.4 / 2.0;
```

## 16. Finding a Remainder in JavaScript

```js
var remainder = 11 % 3;
// remainder is equal to 2
```

## 17. Compound Assignment With Augmented Addition

```js
var a = 3;
var b = 17;
var c = 12;

// Only modify code below this line

a += 12;
b += 9;
c += 7;

// a is equal 15
// b is equal 26
// c is equal 19

```

## 18. Compound Assignment With Augmented Subtraction

```js
a -= 6;
b -= 15;
c -= 1;
```

## 19. Compound Assignment With Augmented Multiplication

```js
a *= 5;
b *= 3;
c *= 10;
```

## 20. Compound Assignment With Augmented Division

```js
var a = 48;
var b = 108;
var c = 33;

// Only modify code below this line

a /= 12;
b /= 4;
c /= 11;
```

## 21. Declare String Variables

```js
var myFirstName = "prgrm";
var myLastName = "fl";
```

## 22. Escaping Literal Quotes in Strings

```js
var myStr = "I am a \"double quoted\" string inside \"double quotes\".";
// output is: I am a "double quoted" string inside "double quotes".
```

## 23. Quoting Strings with Single Quotes

```js
var myStr = '<a href="http://www.example.com" target="_blank">Link</a>';
```

## 24. Escape Sequences in Strings

```js
var myStr = "FirstLine\n\t\\SecondLine\nThirdLine";

// FirstLine
//    \SecondLine
// ThirdLine
```

## 25. Concatenating Strings with Plus Operator

```js
var myStr = "This is the start. " + "This is the end.";
```

## 26. Concatenating Strings with the Plus Equals Operator

```js
var myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";
```

## 27. Constructing Strings with Variables

```js
var myName = "prgrmfl";
var myStr = "My name is " + myName + " and I am well!";
```

## 28. Appending Variables to Strings

```js
var someAdjective = "enjoying";
var myStr = "Learning to code is ";
myStr += someAdjective;
```

## 29. Find the Length of a String

```js
// Setup
var lastNameLength = 0;
var lastName = "Lovelace";

lastNameLength = lastName.length;
//8
```

## 30. Use Bracket Notation to Find the First Character in a String

```js
var firstLetterOfLastName = "";
var lastName = "Lovelace";

firstLetterOfLastName = lastName[0];
```

## 31. Understand String Immutability

```js
var myStr = "Jello World";

myStr = "Hello World";
```
## Comment: 
The individual characters of a string literal cannot be changed. The only way to change myStr would be to assign it with a new string.
-This (myStr[0] = "H") doesn't work.

## 32. Use Bracket Notation to Find the Nth Character in a String

```js
var lastName = "Lovelace";

var thirdLetterOfLastName = lastName[2];
```

## 33. Use Bracket Notation to Find the Last Character in a String

```js
var lastName = "Lovelace";

var lastLetterOfLastName = lastName[lastName.length - 1];
```

## 34. Use Bracket Notation to Find the Nth-to-Last Character in a String

```js
var lastName = "Lovelace";

var secondToLastLetterOfLastName = lastName[lastName.length - 2];
```

## 35. Word Blanks

```js
function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) {
  var result = "If I had a " + myAdjective + " " + myNoun + ", crazy people would have " + myVerb + " it " + myAdverb + "!";
  return result;
}

wordBlanks("hummer", "fancy", "adore", "much");
```

## 36. Store Multiple Values in one Variable using JavaScript Arrays

```js
var myArray = ["The price of butter", 2.5];
```

## 37. Nest one Array within Another Array

```js
var myArray = [["Galatasaray", 69], ["All others", "in dream"]];
```

## 38. Access Array Data with Indexes

```js
var myArray = [50,60,70];

var myData = myArray[0]; // equals 50
```

## 39. Modify Array Data With Indexes

```js
var myArray = [18,64,99];

myArray[0] = 45;
```

## 40. Access Multi-Dimensional Arrays With Indexes

```js
var myArray = [[1,2,3], [4,5,6], [7,8,9], [[10,11,12], 13, 14]];

var myData = myArray[0][0];
myData = myArray[2][1]; // equals 8
```
## Note: 
There shouldn't be any spaces between the array name and the square brackets, like array [0][0] and even this array [0] [0] is not allowed. Although JavaScript is able to process this correctly, this may confuse other programmers reading your code.

## 41. Manipulate Arrays With push()

```js
var myArray = [["John", 23], ["cat", 2]];

myArray.push(["dog", 3]);
```

## 42. Manipulate Arrays With pop()

```js
var myArray = [["John", 23], ["cat", 2]];

var removedFromMyArray = myArray.pop(1);
console.log(removedFromMyArray); // Returns ["cat", 2]
console.log(myArray); // Returns ["John", 23]
```

## 43. Manipulate Arrays With shift()

```js
var myArray = [["John", 23], ["dog", 3]];

var removedFromMyArray = myArray.shift(0);
```

## 44. Manipulate Arrays With unshift()

```js
var myArray = [["John", 23], ["dog", 3]];
myArray.shift();

myArray.unshift(["Paul",35]);
```

## 45. Shopping List

```js
var myList = [["milk", 5], ["banana", 6], ["eggs", 12],
["orange juice", 3], ["bread", 2]];
```

## 46. Write Reusable JavaScript with Functions

```js
function reusableFunction() {
    console.log("Hi World");
}
reusableFunction();
```

## 47. Passing Values to Functions with Arguments

```js
function functionWithArgs(x, y) {
  console.log(x + y);
}
functionWithArgs(7835, 4894);
```

## 48. Global Scope and Functions

```js
var myGlobal = 10;

function fun1() {
  oopsGlobal = 5;
}

```

## 49. Local Scope and Functions

```js
function myLocalScope() {
  var myVar = "This is a local var";
  console.log(myVar);
}
myLocalScope();
```

## 50. Global vs. Local Scope in Functions

```js
var outerWear = "T-Shirt";

function myOutfit() {
 
  var outerWear = "sweater";
  return outerWear;
}

myOutfit();
```

## 51. Return a Value from a Function with Return

```js
function timesFive(arg) {
  return arg * 5;
}

console.log(timesFive(10));
```

## 52. Understanding Undefined Value returned from a Function

```js
var sum = 3;
function addFive() {
  sum = sum + 5;
}
var returnedValue = addFive();
```

## 53. Assignment with a Returned Value

```js
var processed = 0;

function processArg(num) {
  return (num + 3) / 5;
}
processed = processArg(7);
```

## 54. Stand in Line

```js
function nextInLine(arr, item) {
  arr.push(item);
  return arr.shift();
}

// Test Setup
var testArr = [1,2,3,4,5];

// Display Code
console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 10)); // Modify this line to test
console.log("After: " + JSON.stringify(testArr));

//Before: [1,2,3,4,5]
//1
//After: [2,3,4,5,10]
```

## 55. Understanding Boolean Values

```js
function welcomeToBooleans() {
return true; 
}
```

## 56. Use Conditional Logic with If Statements

```js
function trueOrFalse(wasThatTrue) {

  if (wasThatTrue) {
      return "Yes, that was true";
  }
  return "No, that was false";
}

console.log(trueOrFalse(true)); //Yes, that was true
```

## 57. Comparison with the Equality Operator

```js
function testEqual(val) {
  if (val == 12) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

// Change this value to test
console.log(testEqual(10)); //Not Equal
```

## 58. Comparison with the Strict Equality Operator

```js
function testStrict(val) {
  if (val === 7) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

console.log(testStrict(7)); //Equal
```
## Comment:
As a difference from 'the Equality Operator'; If the values being compared have different types, 
/n they are considered unequal, and the strict equality operator will return false.

## 59. Practice comparing different values

```js
function compareEquality(a, b) {
  if (a === b) {
    return "Equal";
  }
  return "Not Equal";
}

console.log(compareEquality(10, "10")); //Not Equal
```
## Note:
If the values being compared are not of the same type, the equality operator will perform a type conversion, 
/n and then evaluate the values. However, the strict equality operator will compare both the data type and 
/n value as-is, without converting one type to the other.

## 60. Comparison with the Inequality Operator

```js
function testNotEqual(val) {
  if (val != 99) { 
    return "Not Equal";
  }
  return "Equal";
}

console.log(testNotEqual(10)); //Not Equal
```
##Note:
Like the equality operator, the inequality operator will convert data types of values while comparing.

## 61. Comparison with the Strict Inequality Operator

```js
function testStrictNotEqual(val) {

  if (val !== 17) {

    return "Not Equal";
  }
  return "Equal";
}

testStrictNotEqual(10); //Not Equal
```
##Note:
(!==) is the logical opposite of the strict equality operator. It means "Strictly Not Equal" and returns false.

## 62. Comparison with the Greater Than Operator

```js
function testGreaterThan(val) {
  if (val > 100) { 
    return "Over 100";
  }
  
  if (val > 10) {  
    return "Over 10";
  }

  return "10 or Under";
}

console.log(testGreaterThan(10));  //10 or Under
```
##Note:
Like the equality operator, greater than operator will convert data types of values while comparing.

## 63. Comparison with the Greater Than Or Equal To Operator

```js
function testGreaterOrEqual(val) {
  if (val >= 20) { 
    return "20 or Over";
  }
  
  if (val >= 10) {  // Change this line
    return "10 or Over";
  }

  return "Less than 10";
}

testGreaterOrEqual(100); //20 or Over
```

## 64. Comparison with the Less Than Operator

```js
function testLessThan(val) {
  if (val < 25) {  
    return "Under 25";
  }
  
  if (val < 55) { 
    return "Under 55";
  }

  return "55 or Over";
}


testLessThan(10); //Under 25
```

## 65. Comparison with the Less Than Or Equal To Operator

```js
function testLessOrEqual(val) {
  if (val <= 12) {
    return "Smaller Than or Equal to 12";
  }
  
  if (val <= 24) {  
    return "Smaller Than or Equal to 24";
  }

  return "More Than 24";
}


console.log(testLessOrEqual(10)); //Smaller Than or Equal to 12
```

## 66. Comparisons with the Logical And Operator (&&)

```js
function testLogicalAnd(val) {

  if (val <= 50 && val >= 25) {
    return "Yes";
  }
  return "No";

}

console.log(testLogicalAnd(10)); //No
```

## 67. Comparisons with the Logical Or Operator  (||)

```js
function testLogicalOr(val) {

  if (val > 20 || val < 10) {
    return "Outside";
  }

  return "Inside";
}


console.log(testLogicalOr(15)); //Inside
```

## 68. Introducing Else Statements

```js
function testElse(val) {
  var result = "";
  
  if (val > 5) {
    result = "Bigger than 5";
  } else {
    result = "5 or Smaller";
  }
 
  return result;
}

console.log(testElse(4)); //5 or Smaller
```

## 69. Introducing Else If Statements

```js
function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  } else if (val < 5) {
    return "Smaller than 5";
  } else {
    return "Between 5 and 10";
  }
}

console.log(testElseIf(7)); //Between 5 and 10
```

## 70. Logical Order in If Else Statements

```js
function orderMyLogic(val) {
  if (val < 5) {
    return "Less than 5";
  } else if (val < 10) {
    return "Less than 10";
  } else {
    return "Greater than or equal to 10";
  }
}

console.log(orderMyLogic(7)); //Less than 10
```
##Note:
The function is executed from top to bottom so you will want to be careful of what statement comes first.

## 71. Chaining If Else Statements

```js
function testSize(num) {
  
  if (num < 5) {
  return "Tiny";
  } else if (num < 10) {
  return "Small";
  } else if (num < 15) {
  return "Medium";
  } else if (num < 20) {
  return "Large";
  } else {
  return "Huge";
  }

}


console.log(testSize(37)); //Huge
```

## 72. Golf Code

```js
var names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];
function golfScore(par, strokes) {
  
  if (strokes == 1) {
  return names[0];
  } else if (strokes <= par - 2) {
  return names[1];
  } else if (strokes == par - 1) {
  return names[2];
  } else if (strokes == par) {
  return names[3];
  } else if (strokes == par + 1) {
  return names[4]; 
  } else if (strokes == par + 2) {
  return names[5];
  } else if (strokes >= par + 3) {
  return names[6];
  }
}

console.log(golfScore(4, 7)); //Double Bogey
console.log(golfScore(4, 7)); //Go Home!
console.log(golfScore(5, 2)); //Eagle
```
## 73. Selecting from Many Options with Switch Statements

```js
function caseInSwitch(val) {
  var answer = "";

  switch(val) {
    case 1:
      return answer = "alpha";
      break;
    case 2:
      return answer = "beta";
      break;
    case 3:
      return answer = "gamma";
      break; 
    case 4:
      return answer = "delta";
      break;  
  }
  
  return answer;  
}

console.log(caseInSwitch(3)); //gamma
```

## 74. Adding a Default Option in Switch Statements

```js
function switchOfStuff(val) {
  var answer = "";

  switch(val) {
    case "a":
      return answer = "apple";
      break;
    case "b":
      return answer = "bird";
      break;
    case "c":
      return answer = "cat";
      break; 
    default:
      return answer = "stuff";
      break;  
  }
  

  return answer;  
}

console.log(switchOfStuff(4)); //stuff
```

## 75. Multiple Identical Options in Switch Statements

```js
function sequentialSizes(val) {
  var answer = "";

  switch(val) {
    case 1:
    case 2:
    case 3:
      return answer = "Low";
      break;
    case 4:
    case 5:
    case 6:
      return answer = "Mid";
      break;
    case 7:
    case 8:
    case 9:
      return answer = "High";
      break;
  }
  
  return answer;  
}

// Change this value to test
console.log(sequentialSizes(5)); //Mid
```

Resource: [freeCodeCamp](https://www.freecodecamp.org/)
