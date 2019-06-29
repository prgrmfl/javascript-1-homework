> start (and try to finish) the [loop tasks](https://javascript.info/while-for) from javascript.info and paste each of your solutions into this file.  
> Don't be afraid of peeking at the solutions!  Just be sure you study them well

## Summary
We covered 3 types of loops:

while – The condition is checked before each iteration.
do..while – The condition is checked after each iteration.
for (;;) – The condition is checked before each iteration, additional settings available.
To make an “infinite” loop, usually the while(true) construct is used. Such a loop, just like any other, can be stopped with the break directive.

If we don’t want to do anything in the current iteration and would like to forward to the next one, we can use the continue directive.

break/continue support labels before the loop. A label is the only way for break/continue to escape a nested loop to go to an outer one.

## 1. Last loop value

```js
What is the last value alerted by this code? Why?

let i = 3;

while (i) {
  alert( i-- );
}

The answer: 1.
let i = 3;

alert(i--); // shows 3, decreases i to 2

alert(i--) // shows 2, decreases i to 1

alert(i--) // shows 1, decreases i to 0
```

## 2. Which values does the while loop show? (difference between i++ and ++i)

```js
1.The prefix form ++i:

let i = 0;
while (++i < 5) alert( i );
//i=1, 2, 3, 4

2.The postfix form i++

let i = 0;
while (i++ < 5) alert( i );
//i=1, 2, 3, 4, 5

```

## 3. Which values get shown by the "for" loop?

```js
1.The postfix form:

for (let i = 0; i < 5; i++) alert( i );
//0, 1, 2, 3, 4

2.The prefix form:

for (let i = 0; i < 5; ++i) alert( i );
//0, 1, 2, 3, 4
```

## 4. Output even numbers in the loop

```js
for (let i = 2; i < 11 ; i++) {
  if (i % 2 == 1) continue;              
  alert( i );
} 

or 

for (let i = 2; i <= 10; i++) {
  if (i % 2 == 0) {
    alert( i );
  }
}
```

## 5. Replace "for" with "while"

```js
for (let i = 0; i < 3; i++) {
  alert( `number ${i}!` );
}

==
 
let i = 0;
while (i < 3) {
  alert( `number ${i}!` );
  i++;
}
```

## 6. Repeat until the input is correct

```js
while (true) {

  let value = +prompt("Enter a number greater than 100 please", '');

  if (value > 100) break; // (*)
}

or 

let num;

do {
  num = prompt("Enter a number greater than 100?", 0);
} while (num <= 100 && num);
```

## 7. Output prime numbers ****

```js
function primeNumbers(n) {
  volgendepremier:
  for (let i = 2; i <= n; i++) {
    for (let j = 2; j < i; j++) {
      if (i % j == 0) continue volgendepremier;
    }
    
    alert( i );      
  }
};
primeNumbers(99);

```

Resource: [javascript.info](https://javascript.info/while-for#tasks)
