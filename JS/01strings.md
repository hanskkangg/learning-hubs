📘 JavaScript Fundamentals: Strings & Numbers
📌 String Basics
A string is a sequence of characters wrapped in:

'single quotes'

"double quotes"

backticks

Strings are primitive data types and immutable — once created, they cannot be changed.

🎯 Accessing Characters
js
Copy
Edit
let text = "JavaScript";
console.log(text[0]); // J
console.log(text[4]); // S
🧾 prompt()
js
Copy
Edit
let name = prompt("What's your name?");
console.log(name);
🔍 indexOf()
js
Copy
Edit
const str = "LoveIsAwesome";
console.log(str.indexOf("Awesome")); // 6
console.log(str.indexOf("Hate"));    // -1
🔍 includes()
js
Copy
Edit
let phrase = "javascript is awesome!";
console.log(phrase.includes("awesome"));       // true
console.log(phrase.includes("Awesome"));       // false
console.log("Hello, Javascript world!".includes("Javascript", 7)); // true
✂️ slice()
js
Copy
Edit
let msg = "Hello,World!";
console.log(msg.slice(0, 5));   // "Hello"
console.log(msg.slice(7));      // "World!"
console.log("JavaScript is fun!".slice(-4));  // "fun!"
🔠 toUpperCase() / toLowerCase()
js
Copy
Edit
let greeting = "Hello World!";
console.log(greeting.toUpperCase()); // "HELLO WORLD!"
console.log(greeting.toLowerCase()); // "hello world!"
🔁 repeat()
js
Copy
Edit
let word = "hello!";
console.log(word.repeat(5)); // hello!hello!hello!hello!hello!
Negative or Infinity → RangeError

Decimal → Rounded down

✂️ trim(), trimStart(), trimEnd()
js
Copy
Edit
let msg = "   Hello!   ";
console.log(msg.trim());       // "Hello!"
console.log(msg.trimStart());  // "Hello!   "
console.log(msg.trimEnd());    // "   Hello!"
🔡 charCodeAt() / fromCharCode()
js
Copy
Edit
console.log("A".charCodeAt(0));       // 65
console.log(String.fromCharCode(66)); // "B"
ASCII: A = 65, B = 66, a = 97

🔁 replace()
js
Copy
Edit
let text = "I love javascript!";
let newText = text.replace("javascript", "coding");
console.log(newText); // "I love coding"
💬 Template Literals (Interpolation)
js
Copy
Edit
let user = "Hans";
console.log(`Hello, ${user}!`); // "Hello, Hans!"
➕ String Concatenation
js
Copy
Edit
let first = "Hello";
let second = "World";
console.log(first + " " + second); // "Hello World"
➗ Arithmetic Operators
markdown
Copy
Edit
+ : Addition  
- : Subtraction  
* : Multiplication  
/ : Division  
% : Remainder (Modulo)
🔁 Type Coercion
js
Copy
Edit
console.log('10' - 5);    // 5
console.log('10' * 2);    // 20
console.log('20' / 2);    // 10
console.log(5 + '10');    // "510"
console.log('hello' + true); // "hellotrue"
🧠 Booleans in Math
js
Copy
Edit
console.log(false + 1); // 1
console.log(true + 1);  // 2
🧮 Operator Precedence
js
Copy
Edit
console.log(2 + 3 * 4);     // 14
console.log((2 + 3) * 4);   // 20
🌀 NaN and Infinity
js
Copy
Edit
console.log(1 / 0);      // Infinity
console.log('hi' / 2);   // NaN
📌 Bonus Notes

null is treated as 0 in arithmetic

undefined is treated as NaN

JavaScript uses one unified Number type for both integers and floats

Binary: base 2 → 0b1010

Octal: base 8 → 0o12

Hexadecimal: base 16 → 0xA

📝 Last Updated: April 2025
📂 You can paste this into: 01-strings.md, notes.txt, Word doc, or any dev wiki
