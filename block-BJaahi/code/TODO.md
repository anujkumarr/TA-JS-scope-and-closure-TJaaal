For the given code below:

- re-write the code in ways that system will understand

For Example:

1.

```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->
```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
console.log(username, brothers[0]);

```

```js
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);// Arya, John

message = sayHello(username); // Hello Arya
nextMessage = sayHello('Test'); // Hello Test
```

2.

```js
console.log(username, number);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->
```js
var username = 'Arya';
let number = 21;
function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
console.log(username, number);
```

```js
// Declaration Phase

var username = undefined;
let number;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;

var nextMessage = undefined;

// Execution Phase

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message= sayHello(username);;

var nextMessage = sayHello('Test');
console.log(username, number);

```

3.

```js
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->
```js

let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
console.log(username, number);
```

```js
// Declaration Phase

var username = undefined;
let number;

let sayHello;

let message;

var nextMessage = undefined;

// Execution Phase

var username = 'Arya';
let number = 21;
let sayHello = function sayHello(name) {
  return `Hello ${name}`;
};

let message = sayHello(username);

var nextMessage = sayHello('Test');
console.log(username, number);
```

4.

```js
let username = 'Arya';
console.log(username, number);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
```

<!-- Answer -->
```js

let username = 'Arya';
let number = 21;
let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
console.log(username, number);
```

```js
// Declaration Phase

let username;
let number;

let sayHello;

let message;

var nextMessage = undefined;

// Execution Phase

let username = 'Arya';
let number = 21;
let sayHello = function sayHello(name) {
  return `Hello ${name}`;
};

let message = sayHello(username);

var nextMessage = sayHello('Test');
console.log(username, number);
```

5.

```js
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
```

<!-- Answer -->
```js
var name = 'Lydia';
let age = 21;
console.log(name);
console.log(age);
```

```js
//Declaration Phase
var name = undefined;
let age;

//Execution Phase
var name = 'Lydia';
let age = 21;
console.log(name);
console.log(age);
```

6.

```js
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
```

<!-- Answer -->
```js
var name = 'Lydia';
let age = 21;
function sayHi() {
  console.log(name);
  console.log(age);
}
sayHi();
```
```js
//Declaration phase

var name = undefined;
let age;
function sayHi() {
  console.log(name);
  console.log(age);
}

//Execution phase
var name = 'Lydia';
let age = 21;
function sayHi() {
  console.log(name);
  console.log(age);
}
sayHi();

```

7.

```js
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
```

<!-- Answer -->
```js
var name = 'Lydia';
let age = 21;
function sayHi() {
  console.log(name);
  console.log(age);
}
sayHi();

```

```js
//Declaration phase

var name = undefined;
let age;
function sayHi() {
  console.log(name);
  console.log(age);
}

//Execution phase
var name = 'Lydia';
let age = 21;
function sayHi() {
  console.log(name);
  console.log(age);
}
sayHi();

```

8.

```js
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
```

<!-- Answer -->
```js
var name = 'Lydia';
let age = 21;
let sayHi = function sayHi() {
  console.log(name);
  console.log(age);
};
sayHi();
```

```js
//Declaration phase

var name = undefined;
let age;
function sayHi() {
  console.log(name);
  console.log(age);
}

//Execution phase
var name = 'Lydia';
let age = 21;
function sayHi() {
  console.log(name);
  console.log(age);
}
sayHi();
```

9.

```js
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
```

<!-- Answer -->
```js
let num1 = 21;
let num2 = 30;
var sum = num1 + num2;
console.log(sum);
```

```js
// Declaration Phase
let num1
let num2
var sum = undefined;

// Execution Phase

let num1 = 21;
let num2 = 30;
var sum = num1 + num2;
console.log(sum);

```

10.

```js
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
```

<!-- Answer -->
```js
var num1 = 21;
let num2 = 200;
let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgain(a, b) {
  return a + b;
}
let sum = add(num1, num2, 4, 5, 6);
let sum2 = addAgain(num1, num2, 4, 5, 6);
```

```js
// Declaration Phase

var num1 = undefined;

let num2;

let add;

function addAgian(a, b) {
  return a + b;
}
let sum;
let sum2;

// Execution Phase

var num1 = 21;
let num2 = 200;
let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let sum = add(num1, num2, 4, 5, 6);
let sum2 = addAgain(num1, num2, 4, 5, 6);

```

11.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
```

<!-- Answer -->
```js
function test(a) {
  let num1 = 21;
  return (a, b) => {
  return a + b;
};
  return add(a, num1);
}

let sum = test(100);


```

```js
// Your code goes here
```

12.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
```

<!-- Answer -->

```js
// Your code goes here
```
