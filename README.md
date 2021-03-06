Below are (my) answers to commonly asked JavaScript questions! I found these questions on a post on LinkedIn, and it's a way for me to keep track of my progress and to use as a study tool. 

---------------------------------------------------------------
What is Javascript?
JavaScript is a client-side and server-side scripting language inserted into HTML pages and is understood by web browsers. JavaScript is also an Object-based Programming language.

What are the Javascript data types?
Number, boolean, string, object, undefined, and null.

What is 'NaN'?
NaN gets returned when the return value is not a number. 

What are global variables?
Global variables are those assigned outside of the scope of functions, and can be accessed through functions 

What are Javascript Cookies?
Cookies are bits of data stored onto your computer that come from interactions you have with a website. These bits of data are used to contain data on a specific website (such as login data, items in a cart, visited pages, etc) in order to create an easier user experience. However, sometimes can be used maliciously in order to target users with specific advertisements based on data that they've consumed. 

What is a typeof operator?
Returns a string of what data type the variable is. 

What are the types of errors in Javascript?
Loadtime Errors: errors shown at the time of page load errors, usually due to incorrect syntax or creates loading issues.
Runtime Errors: errors that are shown while the page is already running. an example would be illegal operations caused by mathematical issues
Logic Errors: syntactically correct code that doesn't fulfill the task -- example, an infinite loop 

1. What's the difference between undefined and null?

undefined: nothing was assigned to the variable. whether intentional or accidental. 
null: it means nothing. it can be assigned the value of null, as well. 

2. What does the && operator do?

representative of the logical AND operator. if used with booleans, will return true if both sides are true/false. 


3. What does the || operator do?

representative of the logical OR operator.

4. Is using the + or unary plus operator the fastest way in turning a string into a number?


5. What is the DOM?

DOM stands for Document Object Model, and it is essentially the interface to webpages. it allows programs to read/manipulate the page's content, structure, and styles.


6. What is Event Propagation? 
It is a way to describe the "stack" of events that gets triggered when clicking on a specific part of the web browser. Most elements on a web page are nested, which is where the "stack" comes from. 

7. What's Event Bubbling?
The movement up of events within the stack.


8. What's Event Capturing?


9. What's the difference between event.preventDefault() and event.stopPropagating() methods?
event.stopPropagating() 

10. How to know if the event.preventDefault() method was used in an element?

It will prevent the page from refreshing.

11. What is event.target? 
"target" is a reference to the object onto which the event was dispatched. basically, what item you click on or are ineracting with. 

12. What are the falsy values in javascript?
- the number 0 
- the BigInt 0n 
- the keyword null
- the keyword undefined 
- the boolean false
- the number NaN
- the empty string -> ""

13. What are truthy falues in javascript?
Anything that is not falsy is truthy including the empty object {} and the empty array []

14. What is a database?
A database is a collection of structured information or data, which is made up of structured rows and columns, making data management easier. There are a lot of different examples of databases: objected-oriented, relational, or noSQL. PostgreSQL is an example of an object-oriented database that supports the storage of all data types, and they are stored as objects. MySQL is an example of a relational database where the database is in the form of a table, and NoSQL is good for large sets of unorganized data. 

15. What is SQL?
SQL stands for "structured query language", and it's a programming language where we can go into a database and extract or manipulate information. With SQL you can make requests to return information using different keyword commands like ???SELECT???, ???FROM???, and ???WHERE???.

16. What are SQL joins?
If you are using SQL, you have data organized in tables and these tables have relationships to each other (Relational databases). In order to make a query that requests data from two tables, we have to connect them with a ???JOIN??? keyword. There are different types of JOINS: Inner, Left Join, Right Join, Full Join.

17. What is type-coercion?
It is the process of converting one value into another. The main three types of coercion are converting a value to a string, a boolean, or a number.

18. What is a closure?
Closures are created whenever a variable that is defined outside the current scope is accessed from within some inner scope. It gives you access to an outer function???s scope from an inner function. In JavaScript, closures are created every time a function is created. To use a closure, simply define a function inside another function and expose it.

19. What is the difference between local storage and session storage?
Local storage data is not sent back to the server for each HTTP request, and this is in regards to HTML, any images, CSS, JS, etc. This way it will reduce the amount of traffic between the client and the server and it will stay until it is manually cleared. 
Session storage is similar to local storage, bu the main difference is that session storage will be cleared when the page session ends, aka when the browser is closed. 

20. How can you convert the string of any base to an integer in JavaScript?
parseInt() function is used to convert numbers between different bases. parseInt() takes the string to be converted as its first parameter. The second parameter is the base of the given string.
ex: parseInt("2F", 4)

21. What is the data type of variables in JavaScript?
All data types in JS are object data types. 

22. What is break and continue statements?
Break gets you out of a loop, while continue will continue the loop. 

In what order will the numbers 1-4 be logged to the console when the code below is executed? Why?

(function() {
    console.log(1); 
    setTimeout(function(){console.log(2)}, 1000); 
    setTimeout(function(){console.log(3)}, 0); 
    console.log(4);
})();
answer: 1, 4, 3, 2. 1 and 4 will log immediately since they are being returned with a simple console.log(). 3 will follow 4, and 2 will be last because of the setTimeout function requiring it to wait a second. 

23. What will the code below output to the console and why ?

console.log(1 +  "2" + "2");
console.log(1 +  +"2" + "2");
console.log(1 +  -"1" + "2");
console.log(+"1" +  "1" + "2");
console.log( "A" - "B" + "2");
console.log( "A" - "B" + 2);

- '122' -> JS is a loosely typed language, so it will just literally add up 1 and 2 and 2
- '32' -> the double plus converts the first string of 2 into a number and adds it 
- '02' -> same here butwith a negative
- '112'
- 'NaN2'
- NaN

24. What would following code return?

console.log(typeof typeof 1);

- it will return string. typeof 1 is "number", and typeof "number" is string. 

25. Consider the two functions below. Will they both return the same thing? Why or why not?

function foo1()
{
  return {
      bar: "hello"
  };
}

function foo2()
{
  return
  {
      bar: "hello"
  };
}


26. What will the code below output? Explain your answer.

console.log(0.1 + 0.2);
console.log(0.1 + 0.2 == 0.3);

- 0.30000000000000004
false

it may print out .3 and true, but it's unsure because of floating point precision in JS. 

27. What will be the output of this code?

var x = 21;
var girl = function () {
    console.log(x);
    var x = 20;
};
girl ();

- the result is undefined because Javascript initialization is unhoisted. when the function is executed, it wll look for a local x variable, but wont declare it yet, and then it won't go ahead and look for a global one. 

28. What will the following code output and why?

var b = 1;
function outer(){
   	var b = 2
    function inner(){
        b++;
        var b = 3;
        console.log(b)
    }
    inner();
}
outer();

Output to the console will be ???3???. There are three closures in the example, each with it???s own var b declaration. When a variable is invoked closures will be checked in order from local to global until an instance is found. Since the inner closure has a b variable of its own, that is what will be output.

29. What is the value of typeof undefined == typeof NULL?
The expression will be evaluated to true, since NULL will be treated as any other undefined variable. JavaScript is case-sensitive and here we are using NULL instead of null.

30. What is memoization?
Memoization is a programming technique which attempts to increase a function???s performance by caching its previously computed results. Each time a memoized function is called, its parameters are used to index the cache. If the data is present, then it can be returned, without executing the entire function. Otherwise the function is executed and then the result is added to the cache. 

31. What will the code below output to the console and why?

(function(){
  var a = b = 3;
})();

console.log("a defined? " + (typeof a !== 'undefined'));
console.log("b defined? " + (typeof b !== 'undefined'));

32. What is the difference between slice and splice? 
Slice does not modify the original array while splice does. (immutable vs mutable)
Slice returns the subset of the original array, while splice returns the deleted elements as an array. 
Slice picks elements from an array, while splice is used to insert/delete items to/from the array. 

33. What is a first class function
In Javascript, functions are first class objects. First-class functions means when functions in that language are treated like any other variable.

For example, in such a language, a function can be passed as an argument to other functions, can be returned by another function and can be assigned as a value to a variable. For example, in the below example, handler functions assigned to a listener

const handler = () => console.log ('This is a click handler function');
document.addEventListener ('click', handler);

34. What is a unary function
Unary function (i.e. monadic) is a function that accepts exactly one argument. It stands for a single argument accepted by a function.

Let us take an example of unary function,
const unaryFunction = a => console.log (a + 10)

35. What is a pure function?
- A pure function is a function where the return value is only determined by the arguments and not by any side effects. 

36. Difference between first order function and higher order function?
- A first order function is a function that does not take another function as an argument and doesn't return a function. A higher order function takes another function as an argument, or returns a return value as a function, or both. 

37. What is an undefined value in JavaScript?

Undefined value means the

Variable used in the code doesn't exist
Variable is not assigned to any value
Property does not exist.

38. What are all the types of Pop up boxes available in JavaScript?

Alert
Confirm and
Prompt

39. What is a window.onload and onDocumentReady?

The onload function is not run until all the information on the page is loaded. This leads to a substantial delay before any code is executed.

onDocumentReady loads the code just after the DOM is loaded. This allows early manipulation of the code.

40. What are the differences between Java and JavaScript?

Java is a complete programming language. In contrast, JavaScript is a coded program that can be introduced to HTML pages. These two languages are not at all inter-dependent and are designed for different intent. Java is an object-oriented programming (OOPS) or structured programming languages like C++ or C, whereas JavaScript is a client-side scripting language.

41. JavaScript timers?

Timers are used to execute a piece of code at a set time or repeat the code in a given interval. This is done by using the functions setTimeout, setInterval, and clearInterval.

The setTimeout(function, delay) function is used to start a timer that calls a particular function after the mentioned delay. The setInterval(function, delay) function repeatedly executes the given function in the mentioned delay and only halts when canceled. The clearInterval(id) function instructs the timer to stop.

Timers are operated within a single thread, and thus events might queue up, waiting to be executed.


42. What is the function of the delete operator?

The delete keyword is used to delete the property as well as its value.

Example

var student= {age:20, batch:"ABC"};
Delete student. age;

43. Does JavaScript has concept level scope?

No. JavaScript does not have concept-level scope. The variable declared inside the function has scope inside the function.

44. Why do you need web storage?
Web storage is more secure, and large amounts of data can be stored locally, without affecting website performance. Also, the information is never transferred to the server. Hence this is a more recommended approach than Cookies.

45. Why do you need a promise?
Promises are used to handle asynchronous operations. They provide an alternative approach for callbacks by reducing the callback hell and writing the cleaner code.

What are the three states of promise?
Promises have three states:

Pending: This is an initial state of the Promise before an operation begins
Fulfilled: This state indicates that the specified operation was completed.
Rejected: This state indicates that the operation did not complete. In this case an error value will be thrown.

46. When is prototypal inheritance an appropriate choice?

There is more than one type of prototypal inheritance:
Delegation (i.e., the prototype chain).
Concatenative (i.e. mixins, `Object.assign()`).
Functional (Not to be confused with functional programming. A function used to create a closure for private state/encapsulation).
Each type of prototypal inheritance has its own set of use-cases, but all of them are equally useful in their ability to enable composition, which creates has-a or uses-a or can-do relationships as opposed to the is-a relationship created with class inheritance.

47. What is AJAX?
AJAX stands for Asynchronous JavaScript and XML. It is a group of related technologies used to display data asynchronously. What this means is that we can send data to the server and get data from the server without reloading the web page.

Technologies use for AJAX.

HTML - web page structure
CSS - the styling for the webpage
JavaScript - the behaviour of the webpage and updates to the DOM
XMLHttpRequest API - used to send and retrieve data from the server
PHP,Python,Nodejs - Some Server-Side language

48. What are ES6 Modules?
Modules let us split our code base to multiple files for more maintainability and this lets us avoid putting all of our code in one big file (yucksss). Before ES6 has supported Modules there were two popular module systems that were used for Code Maintainability in JavaScript.

CommonJS - Nodejs
AMD (Asynchronous Module Definition) - Browsers
Basically, the sytanx for using modules are straightforward,
import is used for getting functionality from another file or several functionalities or values while
export is used for exposing functionality from a file or several functionalities or values.
