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
var myDog = {
  name : "Johnny",
  legs: 3,
  tails: 2,
  friends: ["Pelush", "Koko"]  
};
```

## 81. Accessing Object Properties with Dot Notation

```js
// Setup
var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

// Only change code below this line

var hatValue = testObj.hat;      
var shirtValue = testObj.shirt;
```


## 82. Accessing Object Properties with Bracket Notation

```js
// Setup
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};

// Only change code below this line

var entreeValue = testObj["an entree"];   
var drinkValue = testObj["the drink"];   
```


## 83. Accessing Object Properties with Variables

```js
// Setup
var testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};

// Only change code below this line;

var playerNumber = 16;       
var player = testObj[playerNumber];  
console.log(player);  //Montana
```


## 84. Updating Object Properties

```js
var myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

// Only change code below this line.
myDog.name = "Happy Coder"; //or myDog["name"] = "Happy Coder";
```


## 85. Add New Properties to a JavaScript Object

```js
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

// Only change code below this line.
myDog.bark = "wooof";
console.log(myDog.bark); //wooof
```


## 86. Delete Properties from a JavaScript Object

```js
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

// Only change code below this line.
delete myDog["tails"];
```

## 87. Using Objects for Lookups

```js
// Setup
function phoneticLookup(val) {
  var result = "";

  var lookup = {
    "alpha": "Adams",
    "bravo": "Boston",
    "charlie":"Chicago",
    "delta": "Denver",
    "echo": "Easy",
    "foxtrot": "Frank"
  };
  result = lookup[val];

  return result;
}

// Change this value to test
console.log(phoneticLookup("charlie")); //Chicago
```

## 88. Testing Objects for Properties

```js
// Setup
var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};

function checkObj(checkProp) {

  if(myObj.hasOwnProperty(checkProp)) {
    return myObj[checkProp];
  } else {
    return "Not Found";
  }  

}

// Test your code by modifying these values
checkObj("gift");
console.log(checkObj("gift")); //pony
console.log(checkObj("bed")); //sleigh
console.log(checkObj("mind")); //Not Found
```

## 89. Manipulating Complex Objects

```js
var myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [ 
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  },
  // Add record here
  {
    "artist": "Barış Manço",
    "title": "Sen Gelmez Oldun",
    "release_year": 1990,
    "formats": [
      "DVD",
      "mp3",
      "avi"
    ]
  }
];

console.log(myMusic[1]["formats"][0]); //DVD
console.log(myMusic[1]["artist"]); //Barış Manço
```


## 90. Accessing Nested Objects

```js
var myStorage = {
  "car": {
    "inside": {
      "glove box": "maps",
      "passenger seat": "crumbs"
     },
    "outside": {
      "trunk": "jack"
    }
  }
};

var gloveBoxContents = myStorage.car.inside["glove box"];
console.log(gloveBoxContents); //maps
var content = myStorage.car.outside.trunk;
console.log(content); //jack
```

## 91. Accessing Nested Arrays

```js
var myPlants = [
  { 
    type: "flowers",
    list: [
      "rose",
      "tulip",
      "dandelion"
    ]
  },
  {
    type: "trees",
    list: [
      "fir",
      "pine",
      "birch"
    ]
  }  
];

var secondTree = myPlants[1].list[1]; 
console.log(secondTree); // pine
```

## 92. Record Collection

```js
// Setup
var collection = {
    "2548": {
      "album": "Slippery When Wet",
      "artist": "Bon Jovi",
      "tracks": [ 
        "Let It Rock", 
        "You Give Love a Bad Name" 
      ]
    },
    "2468": {
      "album": "1999",
      "artist": "Prince",
      "tracks": [ 
        "1999", 
        "Little Red Corvette" 
      ]
    },
    "1245": {
      "artist": "Robert Palmer",
      "tracks": [ ]
    },
    "5439": {
      "album": "ABBA Gold"
    }
};
// Keep a copy of the collection for tests
var collectionCopy = JSON.parse(JSON.stringify(collection));

// Only change code below this line
function updateRecords(id, prop, value) {
  if (prop != "tracks" && value != "") {
    collection[id][prop] = value;
  } else if (prop === "tracks" && value != "") {
    if (collection[id][prop]) {
      collection[id][prop].push(value);
    } else {
      collection[id][prop]=[value];
    }    
  } else if (value == "") {
    delete collection[id][prop];
  };
  
  return collection;
}

// Alter values below to test your code
updateRecords(5439, "artist", "ABBA");

```

## 93. Iterate with JavaScript While Loops 

```js
// Setup
var myArray = [];

// Only change code below this line.
let i = 0;
while (i <= 4) {
  myArray.push(i);
  i++;
} 

alert(myArray); //0,1,2,3,4
```

## 94. Iterate with JavaScript For Loops

```js
// Setup
var myArray = [];

// Only change code below this line.
for  (var i = 1 ;i <= 5; i++) {
  myArray.push(i);
}
console.log(myArray); //1,2,3,4,5
```

## 95. Iterate Odd Numbers With a For Loop

```js
// Setup
var myArray = [];

// Only change code below this line.
for (var i = 1; i <= 9; i += 2) {
  myArray.push(i);
}
console.log(myArray); //1,3,5,7,9
```

## 96. Count Backwards With a For Loop

```js
// Setup
var myArray = [];

// Only change code below this line.
for (let i = 9; i > 0; i -= 2) {
  myArray.push(i);
}
console.log(myArray); //9,7,5,3,1
```

## 97. Iterate Through an Array with a For Loop

```js
// Setup
var myArr = [ 2, 3, 4, 5, 6];

// Only change code below this line
var total = 0;
for (i = 0; i < myArr.length; i++) {
  total += myArr[i];
}
console.log(total); //20
```

## 98. Nesting For Loops

```js
function multiplyAll(arr) {
  var product = 1;
  // Only change code below this line
  for (var i = 0; i < arr.length; i++) {
    for (var j = 0; j < arr[i].length; j++) {
      product *= arr[i][j];
    }
  }
  
  // Only change code above this line
  return product;
}

// Modify values below to test your code
multiplyAll([[1,2],[3,4],[5,6,7]]);
console.log(multiplyAll([[1,2],[3,4],[5,6,7]])); //5040

```

## 99. Iterate with JavaScript Do...While Loops
Essentially, a do...while loop ensures that the code inside the loop will run at least once.

```js
// Setup
var myArray = [];
var i = 10;

// Only change code below this line.

do {
  myArray.push(i);
  i++;
} while (i < 10);

console.log(myArray); //10
```

## 100. Profile Lookup

```js
//Setup
var contacts = [
    {
        "firstName": "Akira",
        "lastName": "Laine",
        "number": "0543236543",
        "likes": ["Pizza", "Coding", "Brownie Points"]
    },
    {
        "firstName": "Harry",
        "lastName": "Potter",
        "number": "0994372684",
        "likes": ["Hogwarts", "Magic", "Hagrid"]
    },
    {
        "firstName": "Sherlock",
        "lastName": "Holmes",
        "number": "0487345643",
        "likes": ["Intriguing Cases", "Violin"]
    },
    {
        "firstName": "Kristian",
        "lastName": "Vos",
        "number": "unknown",
        "likes": ["JavaScript", "Gaming", "Foxes"]
    }
];


function lookUpProfile(name, prop) {
// Only change code below this line
  for (var i = 0; i < contacts.length; i++) {
    if (name === contacts[i].firstName) {
      if (contacts[i].hasOwnProperty(prop)) {
        return contacts[i][prop];
      } else {
        return "No such property";
      }
    } 
  }
  return "No such contact";
// Only change code above this line
};

// Change these values to test your function
console.log(lookUpProfile("Akira", "likes")); //Pizza,Coding,Brownie Points

console.log(lookUpProfile("Kristian", "lastName")); //Vos
```

## 101. Generate Random Fractions with JavaScript

```js
function randomFraction() {

  // Only change code below this line.

  return Math.random();

  // Only change code above this line.
}
alert(randomFraction()); //0.93789...

```

## 102. Generate Random Whole Numbers with JavaScript

```js
function randomWholeNum() {

  // Only change code below this line.

  return Math.floor(Math.random() * 10);
}
console.log(randomWholeNum());
```

## 103. Generate Random Whole Numbers within a Range

Math.floor(Math.random() * (max - min + 1)) + min

```js
function randomRange(myMin, myMax) {

  return Math.floor(Math.random() * (myMax - myMin + 1)) + myMin; // Change this line

}

// Change these values to test your function
var myRandom = randomRange(5, 215);
console.log(myRandom); //79 //51 //13 //157...
```

## 104. Use the parseInt Function

```js
function convertToInteger(str) {
  return parseInt(str);
}

convertToInteger("56");
console.log(convertToInteger("002399.344")); //2399
console.log(convertToInteger("Hey12 15li")); //NaN

```

## 105. Use the parseInt Function with a Radix !

The parseInt() function parses a string and returns an integer. It takes a second argument for the radix, which specifies the base of the number in the string. The radix can be an integer between 2 and 36.

The function call looks like:

parseInt(string, radix);

And here's an example:

var a = parseInt("11", 2);

```js
function convertToInteger(str) {
  return parseInt(str, 2);
}

console.log(convertToInteger("10011")); //19
```

## 106. Use the Conditional (Ternary) Operator

condition ? statement-if-true : statement-if-false;


```js
function checkEqual(a, b) {
  return a === b ? true : false;
}

checkEqual(1, 2);
console.log(checkEqual(1, 2)); //false
console.log(checkEqual(22, 22)); //true
```

## 107. Use Multiple Conditional (Ternary) Operators 

```js
function checkSign(num) {
  return (num === 0) ? "zero" : (num > 0) ? "positive" : "negative";
}

checkSign(10);
console.log(checkSign(10)); //positive
console.log(checkSign(-6586)); //negative
console.log(checkSign(0)); //zero
```








Resource: [freeCodeCamp](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript)
