1. What does thread of execution means in JavaScript?

Answer: In JavaScript code execution done by single line by line, and this execution of the code called thread of execution.

2. Where the JavaScript code gets executed?

Answer: JavaScript code gets executed in JavaScript engine. As soon as we execute the code snippet, the JS engine creates a global execution context and store the data , also known as memory. 

3. What does context means in Global Execution Context?

Answer: Context means the environment , in which we are executing the code. It is created when our code is executed.

4. When do you create a global execution context.

Answer: It is the first execution context that gets created by JS engeine whenever we are running any peice of code for the first time.

5. Execution context consists of what all things?

Answer: It consist of two things i.e. Global execution context and function execution context.

6. What are the different types of execution context?

Answer : Global execution context and function execution context.

7. When global and function execution context gets created?

Answer : When the JS page run for the first time on JS engeine the global execution context gets created and they can be multiple function execution context inside one single global execution context, and whenever we are executing any function, It will create function execution context.

8. Function execution gets created during function execution or while declaring a function.

Answer : Its created during function execution.

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)