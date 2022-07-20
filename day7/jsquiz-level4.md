#### 1. What are anonymous functions in JavaScript?
Anonymous Function is a function that does not have any name associated with it.
An anonymous function is not accessible after its initial creation, it can only be accessed by a variable it is stored in as a function as a value. An anonymous function can also have multiple arguments, but only one expression. 
#### 2. Explain strict comparison and Abstract comparison in javascript?

|abstract comoarison | strict comarison|
|------|------|
|Abstract equality will attempt to resolve the data types via type coercion before making a comparison. |Strict equality will return false if the types are different.|
#### 3. Difference b/w arrow functions and regular functions?
1. arrow function are easier to write , there is a difference of syntax 
2. arrow function do not support argymrnt binding .
3. in normal function , fucntion get hoisted on top . 
In arrow function , fucntion get hoisted where you define . so ,if you call the function before initialisation you will get refrence error .
4. you can define methods in class using regular fucntions 


#### 4. What is Hoisting in JavaScript?

JavaScript Hoisting refers to the process whereby the interpreter appears to move the declaration of functions, variables or classes to the top of their scope, prior to execution of the code.

#### 5. JavaScript is a garbage collected programming language, explain how?
js support garbage collection by utilizing a form of automatic memory managment known as garbage collector ,The purpose of a garbage collector is to monitor memory allocation and determine when a block of allocated memory is no longer needed and reclaim it.

#### 6. Explain Shallow copy vs Deep copy in Javascript?

In Shallow copy, a copy of the original object is stored and only the reference address is finally copied. In Deep copy, the copy of the original object and the repetitive copies both are stored.

#### 7. What is Object.freeze?
The Object.freeze() method freezes an object .

## programs
1.Write a function that generates a random number between two ranges, -100 to 0 and800 - 900.


function radomInRange(min, max) {  
    return Math.floor(Math.random() * (max - min + 1) + min)
}

const rndNum1 = radomInRange(-100, 0);
const rndNum2 = radomInRange(800, 900);
console.log(rndNum1);
console.log(rndNum2);
