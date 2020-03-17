<!-- .slide: id="lesson6" -->

# Basic Frontend - Spring 2020

Lesson 6, Thursday, 2020-03-19

---
<!-- .slide: id="lesson6:loops" -->

## Loops

---

### Loops

![loops](images/loop_js-02-farm.png)

<!-- from: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code -->

---

### While loop

A `while` loop repeats its body while its `condition` is `true`:

```js
while (condition) {
  // body is executed while "condition" is true
  console.log("Hello from while loop");
}
```

Example:

```js
while (isHungry) {
  eat();
}
```

While `isHungry` is `true`, the function `eat` is called.

---

### While loop 2

A while loop might execute zero to unlimited times:

```js
let isHungry = false; // we just ate
while (isHungry) {
  eat(); // this is never reached!
}
```

---

### While loop 3

Always make sure that a `while` loop's condition is eventually set to `false`:

```js
while (true) {
  console.log("Hello");
  // this code will print "Hello" until your laptop
  // runs out of battery, you kill the process
  // by closing the browser, you reboot or the universe ends
}

while (isHungry) {
  goRunning(); // going running makes us more hungry
               // loop won't terminate!!!
}
```

---

### Counting

Quiz: Let's `console.log` the numbers from 1 to 5 using a `while` loop.

---

### Counting - solution

Quiz: Let's `console.log` the numbers from 1 to 5 using a `while` loop.

```js
let i = 1;          // initialize i with 1
while (i < 6) {     // repeat this loop until we reach 6
  console.log(i);
  i++;              // increment i at every step
}
```

---

### Remainder Operator

* One useful operator is the [Remainder Operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Remainder): `%`
* It shows you what integer remains when you divide one number by another:

```js
6 % 3  // 6 / 3 is 2, an integer. remainder is 0
7 % 3  // 7 / 3 is not an integer. It is 2 with a remainder of 1
8 % 3  // 8 / 3 is not an integer, It is 2 with a remainder of 2
9 % 3  // 9 / 3 is 3, remainder 0
10 % 3 // remainder 1
11 % 3 // remainder 2
12 % 3 // remainder 0
```

---

### Exercises

* Write your name five times
* Write the squares of the first 10 numbers (1, 4, 9, 16, ...)
* Output the sum of the first 10 numbers
* Write out the first 10 numbers and write if a number is even or odd.
  * It's even if `i % 2 === 0`, odd otherwise

