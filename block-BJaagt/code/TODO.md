Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // `Reference Error username is not defined`.
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // `Reference Error username is not defined`.
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the scope and we can't access the variable defined inside a scope with `const` from outside.

The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username);// `Reference Error username is not defined`
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the scope and we can't access the variable defined inside a scope with `let` from outside.

The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // Arya
```
In above code we are looking for the variable named `username`. `var` is a function scope and in above code  var is not defined inside the function that's why we can access it from outside.


5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // `Syntax Error username has already been declared`
```
In above code we are looking for the variable named `username`.In above code same variable name i.e. `username` is defined two times, once using `let` and once using `var` and var is only function scope variable and it can access from scope that's why `Syntax Error username has already been declared` error is coming.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // John
```
In above code we are looking for the variable named `username`. first `username` is defined in global scope and second `username` is defined in scope that's why we are getting value from global scope.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // John
```
In above code we are calling the `sayHello()` function and then `consoling` variable named `username`. Here only `John` will be output because from function we are not accessing any value, we are just calling the function. 

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0-9
}
console.log(i, 'Second'); // 10
```
In above code we are consoling the `i` inside `loop` and also outside the `loop` and at both places it is accessing the value of `i`. For inside the loop `i` getting the value from `0-9` and for outside the loop `i` it getting the value from `0-10`.


9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0-9
}
console.log(i, 'Second'); // i is not defined
```
In above code we are consoling the `i` inside `loop` and also outside the `loop` and only inside the loop `i` is accessing but outside the loop `i` is not accessble because `i` is defined using block scope. 
