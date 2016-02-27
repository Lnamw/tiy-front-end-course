##Problem 0.1

/*
Write a function mergeArrays that takes two arrays as parameters and returns a new array that is made of two arrays merged together.

Example:

mergeArrays([1, 2, 3], [4, 5, 6]); // returns [1, 2, 3, 4, 5, 6]
*/


```js
function mergeArrays(list1, list2) {
  var listsMerged = [];
  
  for (var iterator1 = 0; iterator1 <= list1.length -1; iterator1 = iterator1 +1){
    listsMerged[listsMerged.length] = list1[iterator1]; 
  }
  for (var iterator2 = 0; iterator2 <= list2.length -1; iterator2 = iterator2 +1){
    listsMerged[listsMerged.length] = list2[iterator2]; 
  }

  return listsMerged;
}

console.log(mergeArrays([1, 2, 3], [4, 5, 6]));
```


##Problem 0.2

/*
Write a function updateObjects that takes an array of objects where each object has a message key and a string value.

For each object updateObjects must add another key getMessage with a value of a function that returns the message in that object.

Example:

```js 
var objects = [
  {
    message: 'Please enter your email address.'
  },
  {
    message: 'Please log in.'
  }
];

var updatedObjects = updateObjects(objects);

updatedObjects[0].getMessage(); // 'Please enter your email address.' 
*/
```

```js
function updateObjects() {
  var objects = [
  {
    message: 'Please enter your email address.'
  },
  {
    message: 'Please log in.'
  },
  {
    message: 'Please type your password.'
  }  
  ];
      
  
  function getMessage() {
  for (var iterator = 0; iterator <= message.length -1; iterator = iterator + 1) {
      return objects;
    }
  }
  var updatedObjects = updateObjects(objects);


}

updatedObjects[0].getMessage();
```


##Problem 1

How many lexical scopes you can see here:

```js 
function printMessage(message) {
  console.log(message);  
}

function getMessageLength(message) {
  return message.length;
}
```

- 3 scopes : global, printMessage, getMessageLength.


##Problem 2

Fix `ReferenceError: askForAddress` error:

```js
deliverProduct();

function deliverProduct() {
  var address = askForAddress();
}

function takeOrder() {
  function askForAddress() {
    var address = {
      houseNumber: '20',
      street: 'Bond Street',
      city: 'London',
      country: 'United Kingdom'
    };

    return address;
  }
}
```

```js
//Fix ReferenceError: askForAddress error:

deliverProduct();

function deliverProduct() {
  var address = askForAddress();
}

  function askForAddress() {
    var address = {
      houseNumber: '20',
      street: 'Bond Street',
      city: 'London',
      country: 'United Kingdom'
    };

    return address;
  }

console.log(askForAddress());
```


##Problem 3

Convert this named function into annonymous function:

```js 
function sum(a, b) {
  return a + b;
}
```

```js 
	function (a, b) {
  return a + b;
	}
```


##Problem 4
Convert this function into Immediately Invoked Function Expression (IIFE):

```js
function getMessageLength(message) {
  return message.length;
}
```

```js
	(function getMessageLength(message) {
  return message.length;
	})();
```

##Problem 5


##Problem 6

/*
Write a function that: 
1. Takes an array as a parameter 
2. Iterates over each value in that array 
3. Checks if the value's type is number 
4. If it is - calculate the sum of all numbers
*/

```js
function calculateNumbers(list) {
  var sumNumbers = 0;
  
  for (var iterator= 0; iterator <= list.length -1; iterator = iterator +1) {
    if(typeof(list[iterator]) == 'number'){
      sumNumbers = sumNumbers + list[iterator];
    }
  }
  return sumNumbers;
    
}

console.log(calculateNumbers([1, 2, 'Hello', 10, 'Elena', 7]));
```


##Problem 7  - to finish...

/*
Write an algorithm in JavaScript that sorts and returns an array of 3 numbers, e.g.:


To test:

sortArray([2, 12, 7]); // returns: `[2, 7, 12]`
sortArray([1, 34, -27]); // returns: `[-27, 1, 34]`
*/

```js
function sortArray(unsortedArray) {
  var sortedArrey = [];
  
  for (var iterator= 0; iterator <= unsortedArray.length -1; iterator = iterator +1) {
    if(unsortedArray[iterator] > unsortedArray[iterator + 1]){
      sortedArrey = sortedArrey.length + unsortedArray[iterator + 1]  ;}
    else {
        sortedArrey = sortedArrey.length + unsortedArray[iterator];
      }
  }  
  
}

console.log(sortArray([2, 7, 12]));
```






