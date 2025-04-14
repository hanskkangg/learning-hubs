# 01 – JavaScript Strings 📘

## 🧠 Definition
A **string** is a sequence of characters wrapped in:
- Single quotes `'Hello'`
- Double quotes `"Hello"`
- Backticks `` `Hello` `` (used for template literals)

Strings are **primitive data types** and are **immutable**, meaning once created, their content can't be changed directly.

---

## 🎯 Accessing Characters
Use bracket notation with an **index** (starting at 0):

js
let word = "JavaScript";
console.log(word[0]); // J
console.log(word[4]); // S


🔤 Common String Methods
1. indexOf()
Finds the position of a substring. Returns -1 if not found.

js
Copy
Edit
const text = "LoveIsAwesome";
console.log(text.indexOf("Awesome")); // 6
console.log(text.indexOf("Hate"));    // -1


2. includes(substring, startIndex?)
Checks if the string contains a substring. Returns true or false.

js
Copy
Edit
let phrase = "JavaScript is awesome!";
console.log(phrase.includes("awesome"));       // true
console.log(phrase.includes("Awesome"));       // false (case-sensitive)
console.log(phrase.includes("JavaScript", 7)); // true

3. slice(start, end?)
Extracts a part of the string from start to end - 1.

js
Copy
Edit
let msg = "Hello, World!";
console.log(msg.slice(0, 5));   // "Hello"
console.log(msg.slice(7));      // "World!"
console.log(msg.slice(-6));     // "World!"
4. toUpperCase() / toLowerCase()
Converts the entire string to uppercase or lowercase.

js
Copy
Edit
let greeting = "Hello World!";
console.log(greeting.toUpperCase()); // "HELLO WORLD!"
console.log(greeting.toLowerCase()); // "hello world!"
5. repeat(count)
Repeats the string count times.

js
Copy
Edit
let word = "Hi!";
console.log(word.repeat(3)); // "Hi!Hi!Hi!"
⚠️ Note: Negative or Infinity will throw a RangeError. Decimal numbers are rounded down.

6. trim(), trimStart(), trimEnd()
Removes whitespace from both ends, the start only, or the end only.

js
Copy
Edit
let msg = "   Hello!   ";
console.log(msg.trim());       // "Hello!"
console.log(msg.trimStart());  // "Hello!   "
console.log(msg.trimEnd());    // "   Hello!"
7. charCodeAt(index) and fromCharCode(number)
Used to work with ASCII values.

js
Copy
Edit
console.log("A".charCodeAt(0));       // 65
console.log(String.fromCharCode(66)); // "B"
ASCII codes: A = 65, B = 66, a = 97, etc.

8. replace()
Replaces part of a string with something else.

js
Copy
Edit
let text = "I love JavaScript!";
let newText = text.replace("JavaScript", "coding");
console.log(newText); // "I love coding"
Only the first occurrence is replaced unless you use a global regular expression.

🔧 Extra Concepts
🧩 String Interpolation (Template Literals)
Use backticks ` ` and ${} to embed variables.

js
Copy
Edit
let user = "Hans";
console.log(`Hello, ${user}!`); // "Hello, Hans!"
➕ String Concatenation
Use + to join strings.

js
Copy
Edit
let first = "Hello";
let second = "World";
console.log(first + " " + second); // "Hello World"
💡 Notes
Strings are immutable — any method returns a new string, not a modified original.

Strings are widely used for:

Outputting text

Taking user input

Building HTML

API data handling

Logging and debugging

✅ Summary Table
Method	Description	Example Output
indexOf()	Finds position of substring	6, -1
includes()	Checks if substring exists	true, false
slice()	Extracts part of string	"Hello"
toUpperCase()	Converts to uppercase	"HELLO WORLD!"
toLowerCase()	Converts to lowercase	"hello world!"
repeat()	Repeats the string	"Hi!Hi!Hi!"
trim()	Removes whitespace	"Hello!"
trimStart()	Removes whitespace from the start	"Hello! "
trimEnd()	Removes whitespace from the end	" Hello!"
charCodeAt()	Gets ASCII code of a character	65
fromCharCode()	Converts ASCII code to character	"B"
replace()	Replaces first match in a string	"I love coding"
📝 Last updated: April 2025

vbnet
Copy
Edit

Let me know if you'd like the same format for:
- `02-boolean.md`
- `03-numbers.md`
- or a `string-playground.js` to practice all these in one file!











Search

Deep research
