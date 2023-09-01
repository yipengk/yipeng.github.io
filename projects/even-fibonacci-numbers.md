---
layout: project
type: project
image: https://logos-world.net/wp-content/uploads/2023/02/JavaScript-Symbol.png
title: "Even Fibonacci Numbers"
date: 2023-08-31
published: true
labels:
  - Software engineering
  - Javascript
  - Technology
summary: "Take the items in the Fibonacci sequence that are no more than four million and add up the even numbers."
---
 

<div class="text-center p-4">
  <img width="200px" src="https://logos-world.net/wp-content/uploads/2023/02/JavaScript-Symbol.png" class="img-thumbnail" >
 
</div>
  This is the second problem I have been practicing on projecteuler. The question asks us take the items in the Fibonacci sequence that are no more than four million and add up the even numbers. My code is as follows:

```javascript
let num1 = 1;
let num2 = 2;
let sum = 0;  

while (num2 < 4000000) {
  if (num2 % 2 === 0) {  
    sum+=num2;
    }
  let nextNum = num1 + num2;
  num1 = num2;
  num2 = nextNum
}

console.log(sum);
```
