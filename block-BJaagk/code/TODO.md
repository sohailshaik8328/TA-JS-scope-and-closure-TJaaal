1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here

let percentage = function (marks, total) {
  return (marks * 100) / total;
}

let percentage =  (marks, total) => {
  return (marks * 100) / total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer

let percentage =  (marks, total) => {
  return (marks * 100) / total;
}
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

let percentage = function (marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => (marks * 100) / total;
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

```js
A function defination and an expression will be much easier to write and we can use it in multiple ways when compare to the normal function effectively by storing it in a variable.
```

4. Why is a function call an expression in JavaScript?
```js
A function call is used to execute the funtion either it is normal function or the function expression.
```

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer -  valid
// Because we are calling the function by storing it in a variable.

five = add; // Answer  - Invalid 
// Because we are not passing parameters to the function.

five = five(10, 11); // Answer - Invalid
// Because we are haven't define a function named five.

five = function () {
  return 'Hello';
}; // Answer - Invalid
// Because we are not calling the function
```

6. What is the difference between function definition and function call? Explain with an example.
```js
A function definition is declaring the function starts with a function object 
Example :-  
function add (a, b) {
  return a + b;
}

A function call is calling the function to execute it.
Example :-
add(2, 3) 
```

7. What is the similarities between function definition and function call?
```js
Similarities are like the name which we are using to define a function defination. We must call the function with the same name.
```

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid  
// valid 
Because a function is an object and it has an access to add the values to it by using  '.' 
```

9. What is higher order function explain with an example.
```js
A higher order function is a function which accepts the function definition as a parameter with the function rererence.

Example :- 
let add =  (a, b) => {
  return a + b;
}

function multiply (a, b, cb) {
  return (a * b), cb;
}

let addition = add(4, 5)
multiply((2, 3), addition)
```

10. Explain what is callback function. Why you can pass a function inside a function?
```js
A callback function can be used in multiple ways based on the requirement by passing a parameter or function reference. Based on the requierment we can pass the function inside a function
```
