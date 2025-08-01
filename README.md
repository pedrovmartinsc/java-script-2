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
## Arithmetic operators
~~~ javascript
/*arithmetic operators= operands (values, variables, etc.)
                        operators (+ - * /)
                        ex. 11 = x + 5;
*/
let students = 30;

//students = students + 1;

//students = students - 1;

//students = students * 2;  -> multiplication

//students = students / 2;  -> division

//students = students ** 2; -> the (variable) is multiply by itself the amount of times that is define by the number after the "**"

//let extraStudents = students % 2; -> the module, the rest of the division

//students += 1; -> students = 31

//students -= 1; -> students = 29

//students *= 2; -> students = 60

//students /= 2; -> students = 15

//students **= 2; -> students = 900

//students %= 2; -> students = 0

//students++; -> students = 31

//students--; -> students = 29
~~~ 

## Operator precedence 

~~~ javascript
/*

    operator precedence 
    1. parenthesis ()
    2. exponents
    3. multiplication & division & modulo
    4. addition & subtraction
*/

let result = 1 + 2*3 + 4**2; // the result is 23                          
~~~
## How to accept user input 

### 1. EASY WAY = window prompt
~~~ javascript 

let username;

username = window.prompt("What's your username?")

console.log(username)

document.getElementById("p1").textContent = username

~~~

### 2. PROFESSIONAL WAY = HTML textbox

~~~ javascript 

let username;

document.getElementById("mySubmit").onclick = function(){
    username =  document.getElementById("myText").value;
    document.getElementById("myH1").textContent = `Hello ${username}`
}

~~~ 

~~~ javascript
let age = window.prompt("How old are you?");

age = Number(age);

age+=1;

console.log(age, typeof age)
~~~

## Type conversion

- Change the datatype of a value to another (strings, numbers, booleans)

~~~ javascript
let x = "pizza";
let y = "pizza";
let z = "pizza";

x = Number(x);
y = String(y);

z =  Boolean(z);

console.log(x, typeof x)
console.log(y, typeof y)
console.log(z, typeof z)
~~~

## Const

- A variable that can't be changed

~~~ javascript
//const = a variable that can't be changed

const pi = 3.14159;
let radius;
let circumference;



radius = window.prompt('Enter the radius of a circle')
radius = Number(radius);

circumference = 2 * pi * radius;

console.log(circumference)
~~~

~~~ javascript
const pi = 3.14159;
let radius;
let circumference;


console.log(circumference)

document.getElementById("mySubmit").onclick = function(){
    radius = document.getElementById("myText").value 
    radius = Number(radius);
    circumference = 2 * pi * radius;
    document.getElementById("myH3").textContent = circumference + "cm";
}
~~~