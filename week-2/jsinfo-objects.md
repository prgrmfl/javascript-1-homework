> start (and try to finish) the [object tasks](https://javascript.info/object) from javascript.info and paste each of your solutions into this file.    
> Don't be afraid of peeking at the solutions!  Just be sure you study them well

## nice example
```js
let user = {
  name: "John",
  age: 30,
  isAdmin: true
};

for (let key in user) {
  // keys
  alert( key );  // name, age, isAdmin
  // values for the keys
  alert( user[key] ); // John, 30, true
}
```

## Summary

Objects are associative arrays with several special features.

They store properties (key-value pairs), where:

Property keys must be strings or symbols (usually strings).
Values can be of any type.
To access a property, we can use:

The dot notation: obj.property.
Square brackets notation obj["property"]. Square brackets allow to take the key from a variable, like obj[varWithKey].
Additional operators:

To delete a property: delete obj.prop.
To check if a property with the given key exists: "key" in obj.
To iterate over an object: for (let key in obj) loop.
Objects are assigned and copied by reference. In other words, a variable stores not the “object value”, but a “reference” (address in memory) for the value. So copying such a variable or passing it as a function argument copies that reference, not the object. All operations via copied references (like adding/removing properties) are performed on the same single object.

To make a “real copy” (a clone) we can use Object.assign or _.cloneDeep(obj).

What we’ve studied in this chapter is called a “plain object”, or just Object.

There are many other kinds of objects in JavaScript:

Array to store ordered data collections,
Date to store the information about the date and time,
Error to store the information about an error.
…And so on.
They have their special features that we’ll study later. Sometimes people say something like “Array type” or “Date type”, but formally they are not types of their own, but belong to a single “object” data type. And they extend it in various ways.

Objects in JavaScript are very powerful. Here we’ve just scratched the surface of a topic that is really huge. We’ll be closely working with objects and learning more about them in further parts of the tutorial.


## 1. Hello, object

```js
//Create an empty object user.
let user = {};
//Add the property name with the value John.
user.name = "John";
//Add the property surname with the value Smith.
user["surname"] = "Smith";
//Change the value of the name to Pete.
user.name = "Pete";
//Remove the property name from the object.
delete user.name;
```

## 2. Check for emptiness

```js
//isEmpty(obj) which returns true 
//if the object has no properties, false otherwise.
let obj = {};
function isEmpty(obj) {
  for (let key in obj) {
  return false;  
  } 
  return true;
};
alert(isEmpty(obj)); //false
```

## 3. Constant objects?

```js
const user = {
  name: "John"
};

// does it work?
user.name = "Pete"; //It works!
```

## 4. Sum object properties

```js
let salaries = {
  John: 100,
  Ann: 160,
  Pete: 130
}
//Write the code to sum all salaries and store in the variable sum. 
//Should be 390 in the example above. If salaries is empty, then the result must be 0.
let sum = 0; 
for (let key in salaries) {
  sum = sum + salaries[key]; //or sum += salaries[key]; 
}
console.log(sum);
```

## 5. Record Collection

```js

```

## 1. Record Collection

```js

```







Resource: [javascript.info](https://javascript.info/object)

