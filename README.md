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
SQL stands for "structured query language", and it's a programming language where we can go into a database and extract or manipulate information. With SQL you can make requests to return information using different keyword commands like ‘SELECT’, ‘FROM’, and ‘WHERE’.

16. What are SQL joins?
If you are using SQL, you have data organized in tables and these tables have relationships to each other (Relational databases). In order to make a query that requests data from two tables, we have to connect them with a ‘JOIN’ keyword. There are different types of JOINS: Inner, Left Join, Right Join, Full Join.

17. What is type-coercion?
It is the process of converting one value into another. The main three types of coercion are converting a value to a string, a boolean, or a number.

18. What is a closure?
Closures are created whenever a variable that is defined outside the current scope is accessed from within some inner scope. It gives you access to an outer function’s scope from an inner function. In JavaScript, closures are created every time a function is created. To use a closure, simply define a function inside another function and expose it.

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

