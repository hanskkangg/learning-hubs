# 📘 JavaScript Fundamentals: Strings & Numbers

## 📌 String Basics
- **Definition**: A string is a sequence of characters wrapped in `'single'`, `"double"`, or \`backticks\`.  
- Strings are **primitive data types** and **immutable** (cannot be changed once created).
- **Accessing characters**: Use bracket notation with zero-based index  
  ```js
  let text = "JavaScript";
  console.log(text[0]); // J
  console.log(text[4]); // S
  ```

---

## 🔍 Common String Methods

### `prompt()`
Prompts the user to input something:
```js
let name = prompt("What's your name?");
console.log(name);
```

### `indexOf()`
Finds the index of a substring. Returns -1 if not found.
```js
const str = "LoveIsAwesome";
console.log(str.indexOf("Awesome")); // 6
console.log(str.indexOf("Hate"));    // -1
```

### `includes()`
Checks if a substring exists in a string (case-sensitive).
```js
let phrase = "javascript is awesome!";
console.log(phrase.includes("awesome")); // true
console.log(phrase.includes("Awesome")); // false
console.log("Hello, Javascript world!".includes("Javascript", 7)); // true
```

### `charCodeAt()` and `fromCharCode()`
Interacts with ASCII codes.
```js
console.log("A".charCodeAt(0));       // 65
console.log(String.fromCharCode(66)); // B
```

### `slice(start, end?)`
Extracts a portion of a string. If `end` is omitted, slices to the end.
```js
let msg = "Hello, World!";
console.log(msg.slice(0, 5));   // Hello
console.log(msg.slice(7));      // World!
console.log(msg.slice(-4));     // rld!
```

### `toUpperCase()` / `toLowerCase()`
Changes case of all characters.
```js
let greeting = "Hello World!";
console.log(greeting.toUpperCase()); // HELLO WORLD
console.log(greeting.toLowerCase()); // hello world
```

### `replace(old, new)`
Replaces the first match of a string.
```js
let text = "I love javascript!";
let newText = text.replace("javascript", "coding");
console.log(newText); // I love coding
```

### `repeat(count)`
Repeats a string `count` times.
```js
let word = "hello!";
console.log(word.repeat(5)); // hello!hello!hello!hello!hello!
```

- Negative or infinite values = ❌ `RangeError`
- Decimal = rounded down
- 0 = returns an empty string

### `trim()`, `trimStart()`, `trimEnd()`
Removes whitespace.
```js
let message = "   Hello!   ";
console.log(message.trim());      // "Hello!"
console.log(message.trimStart()); // "Hello!   "
console.log(message.trimEnd());   // "   Hello!"
```

---

## 💡 Concepts & Operators

### String Interpolation
```js
const user = "Dana";
console.log(`Hello, ${user}!`);
```

### String Concatenation
```js
console.log("Hello" + " " + "World"); // Hello World
```

### Type Coercion
JavaScript automatically converts types:
```js
console.log('10' - 5); // 5
console.log('10' * 2); // 20
console.log('20' / 2); // 10
```

### Mixing Types
```js
console.log(5 + '10');      // "510" (string)
console.log('hello' + true); // "hellotrue"
console.log(false + 1);      // 1
console.log(true + 1);       // 2
```

- `null` is coerced to `0`
- `undefined` is coerced to `NaN`

---

## 🔢 Numbers in JavaScript

### Basics
- JavaScript has a single `Number` type for both **integers** and **floats**
- Special values: `Infinity`, `-Infinity`, `NaN`

### Examples
```js
console.log(1 / 0);         // Infinity
console.log('hi' / 2);      // NaN
```

### Arithmetic Operators
- `+` Addition  
- `-` Subtraction  
- `*` Multiplication  
- `/` Division  
- `%` Modulo (remainder)

```js
console.log(10 % 3); // 1
```

### Exponentiation
```js
console.log(2 ** 3); // 8 (instead of 2^3)
```

### Operator Precedence
- Parentheses first
- Then exponents
- Then multiplication/division/modulo
- Lastly addition/subtraction

---

## 🧠 ASCII Basics
- ASCII assigns numbers to characters:
  - A = 65
  - a = 97
- Covers 128 characters

Use:
```js
console.log("Z".charCodeAt(0)); // 90
console.log(String.fromCharCode(90)); // Z
```

---

## 🗒 Summary
JavaScript string and number methods are essential tools:
- Understand immutability
- Extract and modify strings using `slice()`, `replace()`, `repeat()`
- Convert case with `toUpperCase()`/`toLowerCase()`
- Handle whitespace with `trim()`
- Work with ASCII via `charCodeAt()` and `fromCharCode()`
- Practice type coercion and arithmetic operations for full control over data!

---

Happy coding! 🚀
