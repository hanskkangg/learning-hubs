<div align="center">
  <h1>JavaScript Fundamentals: Strings & Numbers</h1>
  <sub>Author: <b>You!</b> | <small>Last updated: April 2025</small></sub>
</div>

---

## 📌 Overview

This guide covers the **fundamentals of working with strings and numbers in JavaScript**, including methods, operators, and common concepts like type coercion and ASCII.

---

## 🔤 String Basics

### ✅ What is a String?

- A **string** is a sequence of characters wrapped in:
  - `'single quotes'`
  - `"double quotes"`
  - `` `backticks` `` (for template literals)

- Strings are **immutable** and **primitive data types**.

---

### 🎯 Accessing Characters

```js
let text = "JavaScript";
console.log(text[0]); // J
console.log(text[4]); // S
🧰 String Methods
🪟 prompt()
js
Copy
Edit
let name = prompt("Enter your name:");
console.log(name);
🔍 indexOf()
js
Copy
Edit
const str = "LoveIsAwesome";
console.log(str.indexOf("Awesome")); // 6
console.log(str.indexOf("Hate"));    // -1
🔎 includes()
js
Copy
Edit
let phrase = "javascript is awesome!";
console.log(phrase.includes("awesome"));        // true
console.log(phrase.includes("Awesome"));        // false (case-sensitive)
console.log("Hello, Javascript world!".includes("Javascript", 7)); // true
✂️ slice(start, end)
js
Copy
Edit
let message = "Hello,World!";
console.log(message.slice(0, 5));  // Hello
console.log(message.slice(7));     // World!

console.log("JavaScript is fun!".slice(-4)); // fun!
🔠 toUpperCase() / toLowerCase()
js
Copy
Edit
let greeting = "Hello World!";
console.log(greeting.toUpperCase()); // HELLO WORLD!
console.log(greeting.toLowerCase()); // hello world!
🔁 repeat()
js
Copy
Edit
let word = "hello!";
console.log(word.repeat(5)); // hello!hello!hello!hello!hello!
⚠️ Negative or Infinity → RangeError

Decimals are rounded down

✂️ trim(), trimStart(), trimEnd()
js
Copy
Edit
let message = "   Hello!   ";
console.log(message.trim());       // "Hello!"
console.log(message.trimStart());  // "Hello!   "
console.log(message.trimEnd());    // "   Hello!"
🔤 charCodeAt() / fromCharCode()
js
Copy
Edit
console.log("A".charCodeAt(0));       // 65
console.log(String.fromCharCode(66)); // B
A = 65, a = 97

Covers 128 ASCII characters

♻️ replace()
js
Copy
Edit
let text = "I love javascript!";
let newText = text.replace("javascript", "coding");
console.log(newText); // I love coding
Only the first match is replaced unless using a global regex.

💡 Template Literals
js
Copy
Edit
let user = "Dana";
console.log(`Hello, ${user}!`); // Hello, Dana!
➕ String Concatenation
js
Copy
Edit
let first = "Hello";
let second = "World";
console.log(first + " " + second); // Hello World
🧮 Arithmetic Operators
Operator	Description	Example	Result
+	Addition	5 + 2	7
-	Subtraction	5 - 2	3
*	Multiplication	5 * 2	10
/	Division	10 / 2	5
%	Modulus (Remainder)	5 % 2	1
📊 Number Concepts
JavaScript uses one number type for all numbers (integers, floats, etc.)

Infinity occurs when dividing by zero or exceeding max value

NaN = Not a Number ('hi' / 2)

js
Copy
Edit
console.log(1 / 0);        // Infinity
console.log('hi' / 2);     // NaN
⚙️ Type Coercion
Automatically converts values between types:

js
Copy
Edit
console.log('10' - 5);   // 5
console.log('10' * 2);   // 20
console.log('20' / 2);   // 10
console.log(5 + '10');   // "510"
console.log('hello' + true); // "hellotrue"
Booleans:

js
Copy
Edit
console.log(false + 1);  // 1
console.log(true + 1);   // 2
📈 Operator Precedence
Order in which operations are evaluated:

js
Copy
Edit
console.log(2 + 3 * 4);      // 14
console.log((2 + 3) * 4);    // 20
⚠️ Edge Cases
js
Copy
Edit
let result = "Hi!".repeat(-1);    // ❌ RangeError
let result2 = "Hi!".repeat(0);    // "" (empty string)
let result3 = "Hi!".repeat(2.9);  // "Hi!Hi!" (rounded down)
✅ Summary
Concept	Example	Result
indexOf()	"hello".indexOf("e")	1
includes()	"hello".includes("l")	true
slice()	"hello".slice(1, 4)	"ell"
toUpperCase()	"hi".toUpperCase()	"HI"
toLowerCase()	"HI".toLowerCase()	"hi"
repeat()	"ho!".repeat(3)	"ho!ho!ho!"
trim()	" hi ".trim()	"hi"
charCodeAt()	"A".charCodeAt(0)	65
fromCharCode()	String.fromCharCode(65)	"A"
replace()	"hi world".replace("world", "there")	"hi there"
Made with ❤️ for learning JavaScript.

yaml
Copy
Edit

---

✅ **Now you can copy and paste that entire file** into:

- GitHub as a `README.md` or `01-strings-numbers.md`
- Word or Notion (it'll retain formatting)
- Any Markdown-supported platform

If you want a downloadable `.md` file or want this split into sections like "Day 1", "Day 2", etc., let me know — I can generate it for you in seconds.







