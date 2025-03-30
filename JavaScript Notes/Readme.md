<!-- 14/02/2025 -->
Javascript:-
 - Javascript is used for building logics of a web page.
 - Javascript is a high level programming language used in both client side as well as server side.
 - Javascript comes from ecam script so we see that latest version of javascript in the of ecma script.
 - Now we use javascript version 6 i.e ES6 (Ecma Script 6)
 - In another way we called ES6 as the vanilla javascript.
 - Node JS is the environment of javascript.
  
Variable :-
- variable is the container to store some data.
- In javascript there are 3 types of variable are there.

1. var:-
- Variable can be re-declared and update. A global scope variable.
- Var is a type of variable which is used for changing the variable in later stage.
- var is used in oldest browser so now days we are don't use var most of the cases.
syntax:-
var variableName =value of var;

2. let:-
- Variable can be re-declared and update. A block scope variable.
- let is a type of variable which is also used for changing the variable in later stage.
- Now these days, most of the cases we used for changing the variable.
- let is a block scope code so we have used most cases.
syntax:-
let variable_name=value:

3. const:-
- variable cannot be re-declared and updated. A block scope variable.
ex- for,while,var,let this,boolean its.
Syntax:-
const const_name;
const x:

Rules for creating variable name:-
- variable names are case sensitive "a"&"A" is different.
- Only letter, digits,underscore and special character is allowed.
  (dont keep white space over here)
- Only letter, digits,underscore and special character should be the 1st character only.
- Reserved words cannot be a variable name.

<!-- 17/02/2025 -->
Data type:-
- data types is a attribute associated a piece of data that tells a computer system how to interpret its value.
- in data type we used "typeof" opertor to know what  type of data is.
- mainly in java script there are two type of data types are there.

1. Primitive Data Type :-
- Data Type is an  attribute associated with a piece of data types are there.
  
* a. String - Used to represent  textual data. Enclosed in single('),double(") or  templete literals(`)
  ex :- let name = "john"
        let greeting = Hello , $ {name}!;

* b. Number - Represent both integers and floating point numbers.
  ex:- let age =35;
       let pi= 3.14;

* c. BigInt - for integers larger than  number MAX_SAFE_INTEGER.
  ex:- let big number = 8257927509n;

* d. Boolean - Represent Logical value : true or false.
  ex:-let isActive = true;
      let hasAccess = false;

* e. undefined - a variable that has been declared but not assigned a value.
  ex:-let x;
      console.log(x);// undefined

* f. Null - Represent the intentional absence of a value.
  ex:- let emptyValue = null;

* g. Symbol - Used to creat unique identifiers.
  ex:- let uniqueid = Symbol ("id");

2. Non primitive Data Types :-
- these are object and mutable data structure.

* a. object - A collection of key-value pairs.
  ex:- let student 

* b. Array :- An order list of values (can hold mixed types);
  ex:- let fruits = ["apple","banana","orange"]

* c. Function :- A block scope code designed to perform a perticular task.
  ex:- Function addNumbers (a,b) {
       return a+b;
    }
    let result  = addNumber (5,3);
    console.log(result); 8


QUESTIONS:-
-------------------
1. Create a const object called "product" to store information show in the picture?


Operator in Javascript :-
- operator are the key features to do some task or operate some task.
  ex. A + B
- in the above example A & B are the operands, "+" is our operator.
- in javascript, there are 5 types of operator re there..
* Arithmetic operator -> (+,-,,/), %(modulus), * (exponent)
* Assignment Operator -> (=,+=,-+,=,/=,%=,*=)
* compairision operator -> (==, !==, ===)
* Logical operator -> Logical AND (&&), Logical OR (||), Logical NOT (!)
* unary operator -> increament (++), decreament (--)
  logical AND (&&)
  A B AND(&&)
  T T T T F F F T F F F F
  Logical OR (||)
  A B OR(||)
  T T T T F T F T T F F F

conditional statement :-

to implement some condition in the code.
there are 3 types of conditional statements are there
if condition :-
if condition is true then statement is true.
syntax :- if (condition){ statement }
if-else condition :-
if condition is true then sttement is true otherwise false.
syntax :- if (condition){ statement } else { statement }
if-elif condition or switch condition
its check the comdition multiple times, where the condition is true, it returns the statement.

if else if case. else condition if the default condition so if the condition doesn't satisfy any of the case then he print the default condition.

syntax :- if (condition){ statement } else if(condition){ statement } else if(condition){ statement } else { statement }

practice task :-

write a code which can give grades to student according to their score.

80-100 (A)
70-79 (B)
60-69 (C)
50-59 (D)
0-49 (fail - go to aganwadi)


Loops in Javascript :-

loop are used to execute a piece of code again & again.
there are 5 types of loop are there..

For Loop :-
syntax :- for (initialization; condition; updation){ statement } ex. - we want to print "web Bocket" 5 times,
for (let i = 1; i <= 5; i++){ console.log("Web Bocket) }

working :-

i = 1 -> web bocket i = 2 -> web Bocket i = 3 -> Web Bocket i = 4 -> Web Bocket i = 5 -> Web Bocket

While Loop :-
syntax :-
initialize; while (condition){ statement; update; }

ex -> Print "GIFT" 5 times.. in while loop

let i = 1 while (i <= 5){ console.log("GIFT"); i++; }

Do-While Loop :-

syntax :-
initialize; do { statement; updation; } while (condition)

For-Of Loop :- it iterates on string & Array
For-In Loop :- it iterate on objects

String in Javascript :-

Basically String is a sequence of character used to represent text.
create a string -> let str = "web bocket".
we calculate the string length -> str.length property.
we calculate the string index -> str[0], str[1] ...etc
String Literals :-

its a way to have embedded expression in string.
its denoted by symbol ``.
String Interpolation :-

to create string by doing substitution of placeholder.
ex. -> string text ${expression} string text.
Escape symbol in String :-

\n -> new line
\t -> new tab
String Method in Javascript :-

str.toUpperCase()
str.toLowerCase()
str.trim()
str.slice(start,(end-1))
str1.concat(str2)
str.replace(oldVal, newVal) -> its checnge the 1st sequence
str.replaceAll(oldVal, newVal) -> its change all the old value
str.charAt(idx)


Array in Javascript :-

-Array is a collection of items.
ex. let heros = ["iron man", "bat man", "spyder man"]
-array index starts from "0".
-arr[0], arr[1] ....etc

looping over an Array :-
loop -> iteration
syntax -> for (let i = 0; i < arr.length; i++){ statement }
practice question :-

1.for a given array with marks of students -> [89,76,45,90,38,93]. find the average marks of the entire class.
2.for a given array with price of 5 items -> [768,987,456,765,345]. all items have an offer of 10% off of them. change the array to store final price after applying offer.

Array methods on javascript :-
1.push - add an element to the end
2.pop - remove from the end
3.toString - convert array to string
4.concat - join multiple array and return one result
5.unshift - add an element to the start
6.shift - remove an element to the first
7.slice() - return a piece of the array
8.splice() - change original array (add, remove, replace)


Function in Javascript :-
  - it is a block of code that perform a specific task, can be invoked(called) whenever we need.
-ex. (in-build function)
  - console.log("hello world") -> in that code log() is a function
  -"abc".toUpperCase() -> in this code toUpperCase() is a function
  - [1,2,3].push(4) -> in this code push() is a function.
  - there are two types of function in javascript.

Normal Function :-
-> Type A function // function creation function functionName(){ // do some task }

// function calling functionName()

-> Type B function // function creation function functionName(parameter){ 
  // do some task
  }

// function calling functionName(arguments)

Arrow Function :-
Its a compact way of writing a function.
it uses map function to retrive the backend data, filter function for filterise our data...
// function creation const functionName = (parameter..) => { // do some task }

// function calling fuctionName()

Normal function ->
function sum(a,b){ return a + b; } sum(2,3);

Arrow Function -> const sum = (a,b) => { return a + b; } sum(2,3);

practice task :-

1.create a function using the "function" keyword that takes a string as an argument & returns the number of vowels in that string. (TCS Interview Question)

For Each Loop in Array :-

arr.forEach(callBackFunction)
callBackFunction :- it is a function to execute for each element in the array.
a callback is a function passed as an argument to another function.
ex. arr.forEach((val) => { console.log(val) })

practice task :-

1. create a function that reverse an array.
2. create a function that filter out negative numbers.
3. check if a string is a palindrome or not.


Map Method/function :-

create a new array with the result of some operation. The value its callback returns are used to form a new array. Normally we can say, we create a new array by calling the function in every array element.
map does not change the original array.
it does not executte the function for empty array.
syntax :- arr.map(callBackFnx (value,index,array)).
ex. let newArr = arr.map((val) => { returns val * 2; })

Filter Method / function :-

create a new array of element that gives true for a filteration.
ex. all even numbers..
let newArr = arr.filter((val) => { return val % 2 === 0; })

Practice set:-
1. Write a program to print numbers from 1 to 100 using a for loop.
2. Print all even numbers from 1 to 50 using a while loop.
3. Find the sum of the first 10 natural numbers using a do-while loop.
4. Write a program to check whether a number is prime or not up to n terms using for loop.
5. Print the Fibonacci series up to n terms using a loop.
6. Reverse a given number using a loop.
7. Count the number of digits in a given number using a while loop.
8. Print numbers from 10 to 1 using a for loop.
9. Count the number of vowels in a string.
10. Convert a given string to uppercase.
11. Reverse a string without using the built-in reverse() method.
12. Write a program to count the occurrences of a given character in a string.
13. Remove all spaces from a given string.
14. Replace all occurrences of a word in a string with another word.
15. Extract the first 5 characters from a string.
16. Reverse an array.
17. Find the sum of all elements in an array using reduce().
18. Filter out even numbers from an array using filter().
19. Write a function that returns the factorial of a given number.
20. Implement a function that takes a number and returns true if it's even, false otherwise.
21. Iterate over an object and print all its key-value pairs.

DOM IN JAVASCRIPT 

-   DOM stands for -> Document Object Model.
-   Whan a web page is loaded, the browser create a document object model of that page.
-   The HTML DOM model is constructed as a tree structure.

WHY WE USED DOM IN JAVASCRIPT 

-   Javascript can change all the HTML element in the page.
-   Javascript can create, delet or edit any HTML page directly.
-   Javascript can also access CSS styling directly.

WINDOW OBJECT 

-   The window object represents an open window in a browser. it is a browser object & it automatically created by browser.
-   It is also a global object with lots of properties & method.

DOM MANIPULATION

-   Selecting with Id -> document.getElementById("myId")
-   Selecting with Class -> document.getElementsByClassName("myClass")
-   Selecting with Tag -> document.getElementsByTagName("p")

      Program
      javascript
            let heading = document.getElementById("heading")
            console.log(heading);

            let paragraphs = document.getElementsByClassName("para")
            console.log(paragraphs);

            let head1 = document.getElementsByClassName("head")
            console.log(head1);

            let para = document.getElementsByTagName("p")
            console.log(para);
        


QUERY SELECTOR 

-   document.querySelector("id/class/tag")
-   document.querySelectorAll("id/class/tag")

      javascript
      let heading1 = document.querySelector("#heading")
      console.log(heading1);   

      let para1 = document.querySelector(".para")
      console.log(para1);

      let allpara = document.querySelectorAll(".para")
      console.log(allpara);
      

ATTRIBUTES

-   getAttribute(attr) -> to get the attribute value
-   setAttribute(attr, value) -> to set the attribute value

      javascript
      let headattr = heading1.getAttribute("id")
      heading1.setAttribute("class","heading")
      console.log(heading1);
      console.log(headattr);

      let attr = para1.getAttribute("class")
      console.log(attr);
      
INSERT ELEMENT

-   node.append(ele) -> adds at the end of node (inside)
-   node.prepend(ele) -> adds at the start of node (inside)
-   node.after(ele) -> adds after the node (outside)
-   node.before(ele) -> adds before the node (outside)

      javascript
      let boxEl = document.querySelector(".box")
      console.log(boxEl);

      let paraEl = document.createElement("p")
      paraEl.innerText = "Hello this is not me"
      boxEl.before(paraEl)
      boxEl.after(paraEl)
      boxEl.append(paraEl)
      boxEl.prepend(paraEl)

      function AppentChild() {
          boxEl.prepend(paraEl)
      }
      

DELETE ELEMENT
-   node.remove() -> remove the node

      javascript
      let removeEl = document.querySelector(".head")
      removeEl.remove()

      let dltpara = document.getElementsByClassName("para")
      console.log(dltpara);
      for(let i=0;i<dltpara.length;i++){
          dltpara[i].remove()
      }
      

EVENT IN JAVASCRIPT
-   The change in the state of an object is known as event.

      javascript
      function printHello() {
        console.log("Hello Everyone");
      }

      let head1El = document.getElementById("head1")
      console.log(head1El);

      function hoverData() {
        head1El.style.color = 'red'
        head1El.innerHTML = "Hello"
      }
      

SOME FAMOUS EVENTS ARE

-   Mouse event (click, double click)
-   Keyboard Event (keypress, keydown, keyup)
-   Form Events (submit)
-   Print Event ....etc..

EVENT HANDLING
-   syntax -> node.event = () => { // handle here }

EVENT OBJECT 

-   The Event Object is a special object in JavaScript that contains details about an event that occurs, such as a button click, mouse movement, or keyboard press. All event handlers have access to the event object, which provides various properties and methods.
-   Syntax:
    node.event = (e) => {
    // handle event here
    }

COMMON PROPERTIES OF EVENT OBJECT (e)

-   e.target → Refers to the element that triggered the event.
-   e.type → Returns the type of the event (e.g., "click", "keydown").

    Example:
    document.getElementById("myButton").onclick = (e) => {
    console.log("Event Type:", e.type); // Output: "click"
    console.log("Target Element:", e.target); // Output: <button id="myButton">Click Me</button>
    };

EVENT LISTENER 

-   The Event Listener is a method used to listen for an event on an element and execute a callback function when the event occurs.

-   Syntax:
    node.addEventListener(event, callback);
    node.removeEventListener(event, callback);

> Note: When removing an event listener, the callback function reference must be the same as when it was added.

KEY POINTS

-   addEventListener() allows adding multiple events on the same element without overwriting previous ones.
-   removeEventListener() requires the exact same function reference that was used in addEventListener().

PROTOTYPE (SPECIAL OBJECT) IN JAVASCRIPT

-   In JavaScript, every object has an internal property called prototype, which acts as a blueprint for other objects. 
-   Prototypes allow objects to inherit properties and methods from other objects, promoting code reusability.

KEY POINTS

1.  Prototype Chain: If a property/method is not found in an object, JavaScript looks for it in the prototype chain.
2.  Setting Prototype: We can set the prototype using __proto__ or Object.create().
3.  Method Overriding: If an object and its prototype have the same method, the object's method takes precedence.

      EXAMPLE 1: UNDERSTANDING PROTOTYPE INHERITANCE

      javascript
      // Creating a prototype object
      const animal = {
        makeSound: function () {
          console.log("Some generic sound...");
        },
      };
      // Creating an object and setting its prototype
      const dog = {
        __proto__: animal, // Inheriting from 'animal'
        makeSound: function () {
          console.log("Bark! Bark!");
        },
      };
      // Calling method
      dog.makeSound(); // Output: "Bark! Bark!"
      

      > Explanation: The dog object overrides the makeSound() method from the prototype.

      Example 2: Using Object.create()

      javascript
      const person = {
        greet: function () {
          console.log("Hello!");
        },
      };
      const student = Object.create(person); // student inherits from person
      student.study = function () {
        console.log("Studying...");
      };
      student.greet(); // Output: "Hello!" (Inherited from person)
      student.study(); // Output: "Studying..."
      

      > Explanation: student doesn't have greet(), so it is inherited from person.

      EXAMPLE 3: ADDING METHODS TO PROTOTYPE

      javascript
      function Person(name) {
        this.name = name;
      }
      // Adding a method to prototype
      Person.prototype.sayHello = function () {
        console.log(`Hello, my name is ${this.name}`);
      };
      const user = new Person("Alice");
      user.sayHello(); // Output: "Hello, my name is Alice"
      

      > Explanation: sayHello() is added to Person.prototype, making it available to all instances.

CLASSES IN JAVASCRIPT

- A class in JavaScript is a template for creating objects. It allows defining properties (state) and methods (behavior) that objects created from the class will have.

      Syntax:
      javascript
      class MyClass {
        constructor() {
          // Initialization code
        }
        method1() {
          // Method definition
        }
      }
      let myObj = new MyClass(); // Creating an object
      

CONSTRUCTOR IN JAVASCRIPT

- A constructor is a special method inside a class that is automatically called when an object is created using the new keyword. It is used to initialize object properties.

      Example:
      javascript
      class Person {
        constructor(name, age) {
          this.name = name;
          this.age = age;
        }
        introduce() {
          console.log(
            `Hello, my name is ${this.name} and I am ${this.age} years old.`
          );
        }
      }
      const user = new Person("Alice", 25);
      user.introduce(); // Output: "Hello, my name is Alice and I am 25 years old."
      

      > Explanation: The constructor(name, age) initializes the name and age properties when an object is created.

INHERITANCE IN JAVASCRIPT

- Inheritance allows a child class to inherit properties and methods from a parent class. This avoids code duplication and promotes reusability.

      Syntax:

      javascript
      class Parent {
        // Properties & methods
      }
      class Child extends Parent {
        // Properties & methods
      }
      

      Example:

      javascript
      class Animal {
        constructor(name) {
          this.name = name;
        }
        speak() {
          console.log(`${this.name} makes a sound.`);
        }
      }
      // Child class inheriting from Animal
      class Dog extends Animal {
        speak() {
          console.log(`${this.name} barks!`);
        }
      }
      const dog = new Dog("Buddy");
      dog.speak(); // Output: "Buddy barks!"
      

      > Explanation: The Dog class overrides the speak() method from Animal.

      Note :- if child & parent have same property , child methods will be used(method overiding)

STATUS CODE 

200 -> ok
201 -> created
202 -> accepted
300 -> multiple choice
302 -> found
400 -> bad request
402 -> payment required
404 -> Not found
406 -> not accepted
408 -> request timeout
500 -> internal server error
502 -> bad gateway
504 -> gateway timeout

SYNC IN JAVASCRIPT 
SYNCHRONOUS 

-   synchronous means the code runs in a particular sequence of instruction given in the program.
Each instruction waits for the previous instruction to complete its execution.
-   EX - console.log("one") console.log("two") console.log("three")
-   output -> one, two , three

ASYNCHRONOUS 

-   Due to synchronous programming , sometimes imp. instruction get blocked due to some previous instruction, which couses a delay in the UI.
-   Asynchronous code execution allows to execute next instruction immediatelly and doesn't block the flow
-   EX - console.log("one") console.log("two") setTimeout(() => { console.log("three") }, 3000) // 3s = 3000 ms console.log("four") console.log("five")
-   output -> one, two, four, five, three


CALLBACKS IN JAVASCRIPT 

- A callback is a function which passed as an argument of another function.

CALLBACK HELL 

-   Its a nested callback stacked below one another forming a pyramid structure.
-   This style of programming becomes difficult to understand & manage.

PROMISE 

-   It is a solution of callback hell.
-   syntax :- let promise = new Promise((resolve, reject) => { // statement })
a javascript promise objects can be ->>

pending - the result is undefined
resolved - the rsult is a value (fulfilled)
rejected - the result is an error
promise.then((res) => {......})
promise.catch((err) => {......})

ASYNC & AWAIT IN JAVASCRIPT 

-   async function always returns a promise.
-   syntax :- async function myFunc(){ // statement }
-   Note :- await pauses the execution of its surrounding async function until the promise is settled.

FETCH-API 

-   The fetch API provides an interface for fetching data.
-   It uses Request & Response objects.
-   The Fetch() method is used to fetch a data.
-   syntax :- let promise = fetch(URL)