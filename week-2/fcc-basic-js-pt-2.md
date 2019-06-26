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

```







Resource: [freeCodeCamp](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript)
