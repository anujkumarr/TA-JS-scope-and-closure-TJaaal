1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage= function(marks, total){
   return (marks * 100) / total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
```
```js
let percentage= function(marks, total){
   return (marks * 100) / total;
}
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```
```js
 function percentage(marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};

```
```js
 function percentage(marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```
```js
 function percentage(marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => (marks * 100) / total;
```
```js
 function percentage(marks, total) {
  return (marks * 100) / total;
};
```
3. Why is a function definition an expression in JavaScript? Give one example of function expression.

Answer: When any function stored in a variable, it called as function expression. It is easy to accesible anywhere by variable name. 

Example:
```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```

4. Why is a function call an expression in JavaScript?

Anwer: Functions are values. They can be assigned, copied or declared in any place of the code. If the function is created as a part of an expression, it's called a “Function Expression”.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Valid, beacuse the value which return by the function get stored in variable. 
five = add; // valid, but when we access the variable, it will return only fuction body.
five = five(10, 11); // valid;
five = function () {
  return 'Hello';
}; // "Hello
```

6. What is the difference between function definition and function call? Explain with an example.

Answer: When we write any function name which starts with function keyword it is known as function definition ,and when we call any function with parentheses with arguments or without arguments its known as function call.

Example of function definition.
```js
function add(a, b) {
  return a + b;
}
```

Example of function call
```js

add(4, 10);

```


7. What is the similarities between function definition and function call?

Answer: A function definition is procedure or steps to achieve a particular result while function call is using this function name to achive that task.

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}// valid because it will return Hello World, when we call the fuction.


hello.user = 'Sam'; // valid beacuse when we access the value of hello.user it will give the value .
```

9. What is higher order function explain with an example.

Answer: Higher order functions are functions that operate on other functions, either by taking them as arguments as reference or by returning them.

```js
let number = [2,4,6,11];

let evenNum(num) =>{
if(num % 2 ===0 ){
return num} else{
return "number is not even"};
}

number.map(evenNum) 
```

10. Explain what is callback function. Why you can pass a function inside a function?

Answer: A callback function is a function passed into another function as an argument, which is then go inside the outer function to complete operation.We can pass a function inside a function because function is a object and object is an expression.

```js

function userName(name) {
  alert('Hello ' + name);
}

function userInput(input) {
  var user = prompt('Please enter your name.');
  input(user);
}

userInput(userName);
```
