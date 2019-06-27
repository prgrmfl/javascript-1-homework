> begin [the basic data structure exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-data-structures) and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  

## 1. Use an Array to Store a Collection of Data

```js
let yourArray = [
    "let's",
    "fly",
    5,
    true,
    "good to go"
]; 
```

## 2. Access an Array's Contents Using Bracket Notation

```js
let myArray = ["a", "b", "c", "d"];
myArray[1] = 79;

console.log(myArray);
```

## 3. Add Items to an Array with push() and unshift()

```js
function mixedNumbers(arr) {
  // change code below this line
  arr.unshift('I', 2, 'three');
  arr.push(7, 'VIII', 9);
  // change code above this line
  return arr;
}

// do not change code below this line
console.log(mixedNumbers(['IV', 5, 'six'])); //I,2,three,IV,5,six,7,VIII,9
```

## 4. Remove Items from an Array with .pop() and .shift()

```js
function popShift(arr) {
  let popped = arr.pop(); // change this line
  let shifted = arr.shift(); // change this line
  return [shifted, popped];
}
console.log(popShift(['challenge', 'is', 'not', 'complete'])); //challenge,complete
```

## 5. Remove Items Using splice()

```js
function sumOfTen(arr) {

  arr.splice(2, 2);

  return arr.reduce((a, b) => a + b);
}

console.log(sumOfTen([2, 5, 1, 5, 2, 1])); //10
```

## 6. Add Items Using splice()

```js
function htmlColorNames(arr) {

  arr.splice(0, 2, 'DarkSalmon', 'BlanchedAlmond');

  return arr;
} 

console.log(htmlColorNames(['DarkGoldenRod', 'WhiteSmoke', 'LavenderBlush', 'PaleTurqoise', 'FireBrick'])); //DarkSalmon,BlanchedAlmond,LavenderBlush,PaleTurqoise,FireBrick
```

## 7. Copy Array Items Using slice()

```js
function forecast(arr) {
  
  arr = arr.slice(2,4);
  return arr;
}

console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
//warm,sunny
```

## 8. Copy an Array with the Spread Operator

```js
function copyMachine(arr, num) {
  let newArr = [];

  while (num >= 1) {
    newArr.push([...arr]);
    num--;
  }
  return newArr;
}

// change code here to test different cases:
console.log(copyMachine([true, false, true], 2)); //true,false,true,true,false,true

console.log(copyMachine(["yes", "ok", "hoi"], 3)); //yes,ok,hoi,yes,ok,hoi,yes,ok,hoi
```

## 9. Combine Arrays with the Spread Operator

```js
function spreadOut() {
  let fragment = ['to', 'code'];
  let sentence = ['learning', ...fragment, 'is', 'fun'];
  return sentence;
}

console.log(spreadOut()); //learning,to,code,is,fun
```

## 10. Check For The Presence of an Element With indexOf()

```js
function quickCheck(arr, elem) {

  let num = arr.indexOf(elem);
  if (num >= 0)  {
    return num + ' true';

  } else {
    return num + ' false';
  }

}

console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms')); //-1 false
console.log(quickCheck(['squash', 'onions', 'shallots', 'carrot', 'onions'], 'onions')); //1 true
console.log(quickCheck(['squash', 'onions', 'banana', 'shallots'], 'banana')); //2 true

function quickCheck(arr, elem) {

  let num = arr.indexOf(elem);
  if (num >= 0)  {
    return true;

  } else {
    return false;
  }

}

console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms')); //false
console.log(quickCheck(['squash', 'onions', 'shallots', 'carrot', 'onions'], 'onions')); //true
console.log(quickCheck(['squash', 'onions', 'banana', 'shallots'], 'banana')); //true

```

## 11. Iterate Through All an Array's Items Using For Loops

```js
function filteredArray(arr, elem) {
  let newArr = [];

  for (let i = 0; i < arr.length; i++) {
    if (arr[i].indexOf(elem) === -1) {
        newArr.push(arr[i]);
    }
  }
  return newArr;
}

// change code here to test different cases:
console.log(filteredArray([[3, 2, 3], [1, 6, 3], [3, 13, 26], [19, 3, 9]], 3)); //
console.log(filteredArray([[3, 2, 3], [1, 6, 3], [3, 13, 26], [19, 3, 9]], 9)); //3,2,3,1,6,3,3,13,26
console.log(filteredArray([[3, 2, 3], [1, 6, 3, 4], [3, 13, 26], [19, 2, 3, 9]], 2)); //1,6,3,4,3,13,26
```

## 12. Create complex multi-dimensional arrays

```js
let myNestedArray = [
 
  ['unshift', false, 1, 2, 3, 'complex', 'nested'],
  ['loop', 'shift', 6, 7, 1000, 'method',
    ['deep'] 
  ],
  [false, 'concat', true, 'spread', 'array',
    [
      ['deeper'] 
    ]
  ],

  ['mutate', 1327, 'splice', 'slice', 'push', 'iterate', 13849, 7, 4876, 'arbitrary',
    [
      [
        ['deepest']
      ] 
    ]
  ]

];
```

## 13. Add Key-Value Pairs to JavaScript Objects

```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28
};

foods.bananas = 13;
foods.grapes = 35;
foods.strawberries = 27;

console.log(foods); //{ apples: 25, oranges: 32, plums: 28, bananas: 13, grapes: 35, strawberries: 27 }
```

## 14. Modify an Object Nested Within an Object

```js
let userActivity = {
  id: 23894201352,
  date: 'January 1, 2017',
  data: {
    totalUsers: 51,
    online: 42
  }
};

userActivity.data.online = 45;

console.log(userActivity);
```

## 15. Access Property Names with Bracket Notation

```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};
// do not change code above this line

function checkInventory(scannedItem) {
  return foods[scannedItem];
}

console.log(checkInventory("apples")); //25
console.log(checkInventory("grapes")); //35
```

## 16. Use the delete Keyword to Remove Object Properties

```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};

delete foods.oranges;
delete foods.plums;
delete foods.strawberries;

console.log(foods.oranges); //
```

## 17. Check if an Object has a Property

```js
let users = {
  Alan: {
    age: 27,
    online: true
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: true
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function isEveryoneHere(obj) {
  if(obj.hasOwnProperty('Alan', 'Jeff', 'Sarah', 'Ryan')) {
    return true;
  }
  return false;  
}

console.log(isEveryoneHere(users)); //true
```

## 18. Iterate Through the Keys of an Object with a for...in Statement

```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function countOnline(obj) {

  let i = 0;
  for (let num in obj) {
    if(obj[num].online == true) {
      i++;
    };    
  };
  return i;

}

console.log(countOnline(users)); //2
```

## 19. Generate an Array of All Object Keys with Object.keys()

```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function getArrayOfUsers(obj) {
  return Object.keys(obj);
};

console.log(getArrayOfUsers(users)); //[ 'Alan', 'Jeff', 'Sarah', 'Ryan' ]
```

## 20. Modify an Array Stored in an Object

```js
let user = {
  name: 'Kenneth',
  age: 28,
  data: {
    username: 'kennethCodesAllDay',
    joinDate: 'March 26, 2016',
    organization: 'freeCodeCamp',
    friends: [
      'Sam',
      'Kira',
      'Tomo'
    ],
    location: {
      city: 'San Francisco',
      state: 'CA',
      country: 'USA'
    }
  }
};

function addFriend(userObj, friend) {
  userObj.data.friends.push(friend);
  return userObj.data.friends;
}

console.log(addFriend(user, 'Pete')); //Sam,Kira,Tomo,Pete
```



Resource: [freeCodeCamp](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-data-structures)
