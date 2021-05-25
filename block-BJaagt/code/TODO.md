Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // Reference Error username is not defined
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // Reference Error username is not defined
```
In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the curly braces has an function scope and we can't access the variable defined inside a function scope from outside.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); // Reference Error username is not defined
```
In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the if condition has an function scope and we can't access the variable defined inside a function scope from outside.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // Reference Error username is not defined
```
In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the if condition has an function scope and we can't access the variable defined inside a function scope from outside.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // Uncaught SyntaxError: Identifier 'username' has already been declared
```
In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope. But we know that 'let' has a rule of creating a same variable name has not an access and we are defining the same variable 'username' with 'var' but it is already declared.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(useranme); // John
```
In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope. Since let has an functional scope and the username we are consoling will take the access of the global username and it will console John.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); // John
```
In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope. Since let has an functional scope and the username we are consoling will take the access of the global username and it will console John. Whether another username inside the function, we are not returning it.

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 "First"
                          //  1 "First"
                          //  2 "First"
                          //  3 "First"
                          //  4 "First"
                          //  5 "First"
                          //  6 "First"
                          //  7 "First"
                          //  8 "First"
                          //  9 "First"
}
console.log(i, 'Second'); // 10 "Second"
```
Here, the for loop will loop through the condition and it will return the values of 'i' with 'First' until the condition satisfies till '10' times it will return 'First'. And the console outside the for loop will take only one 'i' and it will print the 'Second' for once at 11th time. Because it has defined with 'var'.

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 "First"
                          //  1 "First"
                          //  2 "First"
                          //  3 "First"
                          //  4 "First"
                          //  5 "First"
                          //  6 "First"
                          //  7 "First"
                          //  8 "First"
                          //  9 "First"
}
console.log(i, 'Second'); // 10 "Second"
```
```
Here, the for loop will loop through the condition and it will return the values of 'i' with 'First' until the condition satisfies till '10' times it will return 'First'. And it will through an error at 11th time because the loop has been defined with 'let' and it doesn't has an golobal scope.

