> complete the rest of [basic JS exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript) on FCC and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD) 

## 76. Replacing If Else Chains with Switch

```js
function chainToSwitch(val) {
  var answer = "";
  // Only change code below this line
  
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
  }
  
  // Only change code above this line  
  return answer;  
}

// Change this value to test
chainToSwitch(99); //Missed me by this much!
```

## 77. Returning Boolean Values from Functions

```js
function isLess(a, b) {
  // Fix this code
  return a < b;
}

console.log(isLess(100, 15)); //false
```

## 78. Return Early Pattern for Functions

```js
// Setup
function abTest(a, b) {
  // Only change code below this line
  if (a < 0 || b < 0) {
    return undefined;
  }
  // Only change code above this line

  return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}

// Change values below to test your code
console.log(abTest(2,-10));
```

## 79. Counting Cards

```js
var count = 0;

function cc(card) {
  // Only change code below this line
  switch(card){
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
      count++;
      break;
    case 10:
    case "J":
    case "Q":
    case "K":
    case "A":
      count--;
      break;
  }
  if(count > 0) {
    return count + " " + "Bet";
  } else {
    return count + " " + "Hold";
  }
  
  // Only change code above this line
}

// Add/remove calls to test your function.
// Note: Only the last will display
console.log(cc("Q")); //-1 Hold
console.log(cc(3)); //0 Hold
console.log(cc(7)); //0 Hold
console.log(cc('K')); //-1 Hold
console.log(cc('A')); //-2 Hold
```

## 80. Build JavaScript Objects

```js

```










Resource: [freeCodeCamp](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript)
