Promp() = 
indexOf = 
charCodeAt() = 
fromCharCode() = 
slice() = 
toUpperCase() =
toLowerCase() =
repeat() = 
range error = 
trim() = 
trimStart() = 
trimEnd() = 
String Basics
•	Definition: A string is a sequence of characters wrapped in either single quotes, double quotes or backticks. Strings are primitive data types and they are immutable. Immutability means that once a string is created, is cannot be changed.
•	Accessing Characters from a String: To access a character from a string you can use bracket notation and pass in the index number. An index is the position of a character within a string, and it is zero-based.

string interpolation = ${user}
Arithmetic operators = 
OPERATOR PRECEDENT = order of the operator 
String concatenation = 

Type Coercion = when a value from one data type is converted into another data type.




 
Javascritp things I learned to day

indexOf = finds “words” in the string.  And gives the index number.
const loveIsAwesome = "LoveIsAwesome";
console.log(loveIsAwesome.indexOf("Awesome"));
Output =  6

If console loveIsAwesome = “LoveIsAwesome”
Console.log(loveIsAwesome.indexOf(“Hate”)) = which hate doesn’t exist
Output = -1

What is ASCII and how does it work with charCodeAt() ?? 
Understanding how characters are represented as numbers is fundamental 
charCodeAt()
fromCharCode()
to interact with ASCII value 
it’s like A = 65 a = 97 it covers 128 characters 
console.log(String.fromCharCode(66));
Output = B


Include()
Let phrase = “javascript is awesome!”
Let result = phrase.includes(“awesome”)
Console.log(result)

Output = TRUE

Includes check if the string has substring inside the string 
Its case sensitive.

If its Awesome and awesome = result will be false 

We can also do 
Let text = “Hello, Javascript world!”;
Let result = text.includes(“Javascript”,7);
Console.log(result) will be TRUE.
Because JAVASCRIPT exist in index of 7 in the string 

It only gives true and false results 


How to EXTRACT substring from a string?
Working in javascript, we often have to extract some portion of the string from a long string.

Slice() method = allows user to extract a portion of a string giving a new string without modifying original string. It takes two parameters
STARTING index and OPTIONAL ending index 
IF ENDING INDEX isn’t there, it extract from STARTING index to ending index

Let message = “Hello,World!”;
Let greeting = message.slice(0.5);
Console.log(greeting)
Output will be Hello

Let message = “Hello, world!”;
Let greeting = message.slice(7);
Console.log(greeting)
Output will be world!

We can also use NEGATIVE NUMBER

Let message = “Javsascript is fun!”;
Let lastWord = message.slice(-4);
Console.log(lastWord);
Will be fun!
It counts from the backward
 
It starts at index 7 and ends right before index 17. 
Slice() is powerful tool for extracting parts of a string in javascript 


Can you change the case of string? For example
Making all heading to upper case 
Javascript has two built in method

toUpperCase()
toLowerCase()

let greeting = “Hello World!”;
let upperCaseGreeting = greeting.toUpperCase();
console.log(upperCaseGreeting); 
will be HELLO WORLD!
It gives a new string. It doesn’t modity the original string 


How can we replace the portion of the string with another string?
For example, we might need to update the user informaiton of URL 
Or change the formatting of the dates or correct errors
Replace() method
 
Let text = “I love javascript!”
Let newText = text.replace(“javascript”, “coding”);
Console.log (newText)
Output I love coding

 
If there are a lot of world, only the first one will be replaced
 


How can you repeat the string x number of time?
In javascript, there will be a situation where we need to repeat the string multiple times.
Whether youre generated pattern or duplicating string.
String.repeat(count);

Let word = “hello!”;
Let repeatWord = word.repeat(5);
Console.log(repeatWord)
We will get hello! 5 times  

 
If its negative number it will give error.

 
Infinity = infinite QUANTITY 
 
If its decimal, it will round down to the nearest integer

 
It returns empty string 


How to trim white space? Its common to have unwanted white space in the beginning

Trim method is commonly used to get rid of white space

Let message = “   Hello!     “;
Let trimmedMessage = message.trim();
Console.log(trimmedMessage);
Output : Hello! 

Let message = “   Hello!   “
Let trimmedMessage = message.trimStart();
Console.log(trimmedMessage)
Output: “Hello!     “;

trimEnd()
trim end

trim()
trimStart()
trimEnd()

JavaScript uses one unified number type to account for numbers
 
 
 
All floats are juts number, positive negative numbers are just number

Infinity = used to represent numbers that are beyond the maximum limit.

 
Const notANumber = ‘hi’ / 2;
Console.log(notANumber); = NaN

Binary = a base 2 systems that uses only digits 1 and 0s
Octal = a base 8 systems.
Hexadecima = a base 16 that uses digits 0 to 9 and letters a to f 

Number = 
It covers both integers and floating-point numbers, as well as special cases like infinity and NaN.



When are floating point numbers most useful in JavaScript?
When you need more precision, such as in measurements or currencies.

When might you encounter the value Infinity in JavaScript?
When dividing a number by zero or exceeding the upper boundary of the Number type.

What are the different arithmetric operators in javascript?
Arithmetic operators = such as addition substraction multiplication such as remainder 
 
Divide by 0 we get infinity 
 
Remainder operator = modulo = left over value.

 
2^3  
In javascript there’s no 2^3 
 
OPERATOR PRECEDENT = order of the operator 


What happens when you mix string and number 
 
Javascript thinks 5 + stirng ‘10’ and string concanteration occurs so it becomes 510
 

Type Coercion = when a value from one data type is converted into another data type.
 
‘10’-5 = 5 
‘10’* 2 = 20 
‘20’/2 = 10
 

 

 
Javascript treats Boolean as numbers true = 1 false = 1
So 
False + 1 = 1 
True + 1 = 2
‘hello’ + true; 
= hellotrue (string)
 
Null = Number
Undefined = NaN



