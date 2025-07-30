~~~ javascript

//console.log("Hello, World!");

//console.log("I like pizza");

//window.alert("This is an aleart")
//window.alert("I like pizza!");

document.getElementById("myH1").textContent= "Hello";
document.getElementById("myP").textContent= "I like pizza";

//This is a comment
~~~ 

~~~ javascript
/* variable = A container that stores a value
              Behaves as if it were the value it contains
1. declaration   let x;
2. assigment x = 100;

You can only declare a variable one time, you can't declare more than one variable of same name

*/
let age = 25;
console.log(`you are ${age} years old`)
// This console command will show "you are 25 years old" on the console -> IT NEEDS TO START AND END WITH "`"//
let price = 10.99
console.log(`The price is $${price}`);

let favFood = prompt("What is your favorite food?");
console.log(`You favorite food is ${favFood}!`)

~~~

~~~ javascript
let online = true

console.log( typeof online)
//This a *boolean*, is used to verify something//
~~~ 

~~~ javascript
let fullName = "Pedro Victor Martins Câmara";
let age = 21;
let student = true;

document.getElementById("p1").textContent = `Your namew is ${fullName}`;
document.getElementById("p2").textContent = `You are ${age} years old`;
document.getElementById("p3").textContent = `Enrolled: ${student}`;
~~~