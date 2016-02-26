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
``

##Problem 5
##Problem 6
##Problem 7






