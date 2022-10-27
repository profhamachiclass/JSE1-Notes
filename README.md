# JSE1-Notes

## Module 1 Notes
JavaScript is an interpreted language

What is the basic difference between compiled and interpreted languages? 
In compiled languages, unlike in interpreted languages, all the program code must be transformed into the target form before it can be run.

The basic online dev environment will consist of:
At least a code editor and a runtime environment.

What is not the task of the debugger?
Transforming the source code of the program into the target form.

Using JS, we want to display the word “hello” in the console. What statement do we use to do this?
console.log(“hello”);

A client-side JS program:
Should be embedded inside an HTML document.

HTML is:
A language for describing the structure of a web page.

The `<html>` tag indicates the start of the actual HTML document. What tag should appear at the end of the document? 
`</html>`

What tag do we use in HTML to denote the main part of the document inside which we define the page elements? `<body>`


What HTML tag is used to indicate that we are embedding JS code? `<script>`

In a browser, we want to open a local file by typing the path to it in the address bar. The path must be preceded by:
```
file:///
```

In the browser, we type into the address bar a string starting with `file:///`.  This means that:
- The rest of the string is the path to the file on our local computer that we want to open in the browser.

Entering `about:blank` in the address bar of your browser will:
- Generate and load a minimal blank HTML page into the current tab.

The JS code includes the 
`console.log(“http://test.org”);` command. Its execution will Display the following message on the console: `“http://test.org”`

## Module 2 Notes
The msg variable contains a String type value. Information about the number of characters of this string can be obtained using: `msg.length`


Analyze the code snippet:
```js
let counter = 0;
let userName = “John”;
```

After declaring a counter variable, we want to put a short comment with information about what the variable is used for. To do this, we modify the line with the declaration to the form: `let counter = 0; // user visit counter`

In the daysOfWeek variable, we place an array with the names of the days of dthe week. To reverse the order of the array elements, we should call: `daysOfWeek.reverse();`

We want to declare a distance constant and initialize it with the value 120. What should such a declaration look like?
```js
const distance = 120;
```

Performing the operation: `let x = 100 / 0;` will result in an `Infinity` value being stored in the variable `x`.

We have declared an array of selected month names `let summer = [ “June”, “July”, “August”];` We want to change the value `“July”` stored in the array to the number `7`
```js
summer[1] = 7;
```

We perform the operation: `let x = “abcdefg”.slice(2, 4)` . As a result, the value `"cd"` will be written to the variable `x`.

Analyze the following code:

```
let x = 10 / 100;
console.log(typeof (x))
```

As a result of its execution, it will display `"Number"` in the console.

Analyze the following code:
```js
let height = 180;
{
    let height = 200;
    height = height + 10;
}
console.log(height);
```
A value of `180` will be displayed in the console.

Point out the correct declaration of the height variable:

Complex (or composite) data types: may consist of multiple elements, each of which may be of a primitive or composite type.

We have declared an array of animals `let animals = [“dog”, “cat”, “hamster”]` . Then we call the method `animals.push(“canary”);` . As a result, the animals array will look like this:
```js
['dog', 'cat', 'hamster', 'canary']
```

Analyze the code snippet:
```js
let summer = [“June”, “July”, “August”];
let index = summer.indexOf(“June”);
```
The index variable will have the value `0`


Analyze the code snippet:
```js
let name;
let age;
{
let height;				// 2
{					// 2
	let weight:	        // 1	// 2
	console.log(name);	// 1	// 2
}					// 2
console.log(name);		// 2
}
```
We have access to the weight variable in the part marked **1**.

What does **shadowing** mean? Declaring a local variable with the same name as a previously declared global variable.

We can replace the declaration `let x = 0x21;` with `let x = 33;`

Analyze the code snippet. Identify which variables are **local** and which are **global**:
```js
let name;
let age;
{
    let profession;
    {
        let height;
        let weight;
    }
}
```
name = global
profession = local
age = global
height = local
weight = local

We have declared an array of animals `let animals = [“dog”, “cat”, “hamster”]` . Then we call the method `animals.pop();`. As a result, the animals array will look like this: `"[ 'dog', 'cat' ]"`

In order to check the number of elements of the array stored in the `names` variable, we call: `names.length`

Performing the operation: `let x = 20n + 10;` will result in: the program to abort due to an error

Performing the operation: `let x = "Alice" + 10;` will result in the value `"Alice10"` of **String** type to be stored in the variable `x`.

We want to convert the string `"1024"` to type **Number** and store the result in variable `n`. Point out the correct statement: `let n = Number("1024");`

We declare an object called `dog`, with two fields: `age` and `name`:
```js
let dog = {
    age: 5,
    name: "Axel"
};
```
To change the value of the `age` field to `6`, we need to perform `dog.age = 6;`

Review the following code (note the variable name):
```js
let age = 32;
age = age + 1;
console.log(Age);
```
As a result of its execution, the following should appear in the console:

If a variable stores the value `false`, then the variable is of the **Boolean** type.

We have declared an array `let animals = [“dog”, “cat”, “hamster”]` . We want to temporarily comment out the element `"cat"`, and to do this, we can modify the declaration as follows:
`let animals = ["dog",/*"cat",*/"hamster"];`

We need to come up with a name for a variable where we will store * *the age of a user**. All of the following variable names are formally correct, but one of them is the most readable, indicate which one: `userAge`

By default, JavaScript allows us to write to an undeclared variable (it declares it implicitly for us). If we want the interpreter to treat such a situation as an error, we have to place the `"use strict";` directive at the beginning of the script.
Analyze the following code:
```js
let counter = 100;
let counter = 200;
counter = 300;
```
As a result of its execution, the program will be aborted ue to an error (redeclaration of a variable).

## Module 3 Notes
The result of the operation `false || "false"` will be `false`

Analyze the following code:
```js
let test = prompt("Hello", "World");
```
What value will the `test` variable have if, after running the code, we immediately press the **OK** button on the newly created dialog? `"World"`

The methods `window.alert`, `window.confirm`, and `window.prompt` are methods of the `window` object. Which of the following is **not true?**. the `alert`, `confirm`, and `prompt` methods require an argument specifying the position of the dialog box in which the information will be displayed.

The `confirm` method allows you to create a dialog box. What value does this method return when the user closes the window? It depends on the option selected by the user.

Analyze the code snippet:
```js
let n = 2 * 3 ** 3 - 1;
```
The result stored in the variable `n` is `53`

Analyze the code snippet:
```js
let n = 10;
let m = ++n;
```
Its execution will result in the following values in the variables `n` and `m`: n:`11`, m:`11`

The result of the comparison `"abcd" > "Abcd"` will be `true`

The result of the operation `!(true && false || true)` will be `false`

The result of the operation `3 * 4 > 20 - 15` will be `true`

Analyze the code snippet:
```js
let nr = 1;
let x = (nr === 1);
let y = (nr == 1);
let z = (nr = 1);
```
After its execution, the variables `x`, `y`, and `z` will have the values: x:`false`, y:`true`, z:`1`

The result of the operation `20 || 5` will be `20`

The number `2` is stored in the variable `n (let n = 2;)`. The command `n = n*n*n` is then called. This last command can be replaced by: `n **= 3;`

Which operator do we use if we want to check if two variables store the same values of exactly the same type? `===`

The string `"12"` has been written into the `str` variable: (`let str = "12";`). Then the operation `str = +str` is performed. As a result, the variable `str` will contain `12`

## Module 4 Notes
If we want to display all the elements of the `days` array in reverse order (starting from the last element) then we can do this using the statement: `for(let i = days.length -1; i >= 0; i--) console.log(days[i]);`

Examine the following code:
```js
for (let a = 5; a > 1; a--) {
    console.log(a);
}
;
```
`let a = 5; while (a > 1) console.log(a--);`

Review the following code snippet:
```js
if (counter <= 10 && confirm === false) {
    console.log("test");
}
```
What values can the `counter` and `confirm` variables have so that the console displays `"test"` as a result of code execution?

counter: `10`, show: `false`

Review the following code:
```js
let x = 100;
if (x < 100)
    x = 20;
console.log(x)
```
What will be displayed in the console as a result of its execution?
`100`

Which of the following is **not a loop** instruction in JavaScript?

`if ... else`

Examine the following code:
```js
let car = {make: "Citroen", model: "DS"};
for (let f in car) console.log(f);
```
What will appear on the console as a result?
`"make""model"`

Analyze the following code:
```js
for (let x = 10; x > 1; x -=2) console.log("hello");
```

How many times will "hello" be displayed in the console as a result of its execution? **5**

Analyze the following code:
```js
let a = 10;
do {
    console.log(a--);
} while (a > 3);
```
Which statement can replace the `do ... while` from the example above?
`while (a > 3) console.log(a--);`

The `switch` statement:
**is a conditional statement that allows different actions to be taken depending on the value stored in the indicated variable.**


Which of the following operators is a **ternary** one?

**A **conditional** operator `? :`**

We want to rewrite the following code snippet using the conditional operator:
```js
let name;
if (test) {
    name = 10;
} else {
    name = 20;
}
```
Which notation is correct?
`let name = test ? "Alice" : "Bob";`

The condition `if (!a)` can be replaced by the condition:
`if (a == false);`

Which of the following loop instructions is intended only to loop through all the keys of the indicated **object**?
`for ... in`

which sequence of `if ... else` statements is **incorrect**?

`if ... else ... else if ...`

Examine the following code:
```js
for (let a = 4; a < 4; a++) {
    console.log("test");
}
```
How many times will `"test"` be displayed in the console as a result of its execution?
**It will not be displayed at all**

We store an array of animal names in the `animals` variable (e.g. `let animals = ["dog", "cat", "hamster", "rabbit"];`). Which of the following statements will display **exactly two** names from the array?

`for (let i = 0; i < animals.length; i+=2) console.log(animals[i]);`

The condition `if( a >= 0 )` can be replaced by the condition:
`if (a > 0 || a == 0);`

Examine the following code:
```js
let steps = [3, 2, 1];
for (let n of steps) console.log(n);
```
What will appear on the console as a result?

`3 2 1`

Review the following code:
```js
if (counter <= 10) {
    if (counter >= 10) {
        console.log(1);
    }
}
```
We can replace it using:
`if (counter == 10) console.log(1);`

Analyze the following code:
```js
if (counter === 10) {
    console.log("abc");
}
```
How can we write the same condition using the `switch` statement?

`switch(counter) {case 10 : console.log("abc")};`

## Module 5 Notes
If the function is to return some calculated value on completion, we use the following keyword to do so:
`return;`

We define a function using the following function expression:

```js
let sum = function (a, b) {
    return (a + b);
}
```
What could the definition of the corresponding arrow function look like?
`let sum = (a, b) => a + b;`

Analyze the code below:
```js
function test(counter) {
    console.log("test");
    if (counter > 0)
        test (--counter);
}

test(3)
```
How many times will the word "test" be displayed in the console? `4`

Review the following code:
```js
let x = 10;

function test(x) {
    console.log(x);
}

test(20);
```
What will be displayed in the console as a result of its execution? `20`

Analyze the following code:
```js
let show = function () {
    console.log(test);
}
setTimeout(show, 2000);
```
Its execution will cause:
`the console to display "test" after a 2 second delay`

Analyze the following code:
```js
let x = 10;

function test() {
    let x = 20;
    console.log(x);
}
```
What will be displayed in the console as a result of its execution? `Nothing will show up`

We have defined an arrow function:
```js
let multiply = (m, n) => m * n;
```
We will try to write it in a slightly modified form, but without changing what it is supposed to do. Point out the correct definition:
```js
let multiply = (m, n) => return (m * n);
```
[let multiply = (m, n) => return (m * n);]
[let multiply = (m, n) => { m * n;}]
(yes)[let multiply = (m, n) => {return (m * n)};]
(no)let multiply = (m, n) => {console.log(m * n)};


The code snippet:
```js
function test() {

}
```
is:
the declaration of an empty `test` function.

Review the following code:
```js
let x = 10;
let y = 20;
function test(y) {
    console.log(y);
}

test(x);
```
What will be displayed in the console as a result of its execution?
`10`

We can use the `forEach` method to pass through the elements of an array. Which of the following code snippets will display all consecutive elements of the animals array in the console?
`animals.forEach(a => {console.log(a);})`

A `callback` function is a function that is passed to another function as an argument and only called in its code.

Logical errors that we make while writing a program are not indicated by the interpreter. Why?
The interpreter is unable to identify logical errors because they are not related to either the syntax or the semantics of the JavaScript language.

Analyze the following code:
```js
try {
	ocnsole.log("start");
} catch (error) {
	console.log("error");
} finally {
	console.log("end");
}
```
What will hapen as a result of its execution?

Analyze the following code:
```js
let x 10;
console.log(x);
```
What exception will be thrown as a result of its execution attempt?

Which of the following is a **syntax** error?
- Missing parenthesis ending in a condition in an `if` statement.
- Attempting to call a non-existent function.
- Attempting to modify the value of a constant.
- Attempting to read a value from a variable that we have not previously declared

## Module 6 Notes
Analyze the following code:
```js
try {
    console.log("start");
} catch (error) {
    console.log("error");
} finally {
    console.log("end");
}
```
What will happen as a result of its execution?
The following words will appear in the console: `"start"`, `"end"`.

Analyze the following code:
```js
let x = 10;
ocnsole.log(x);
```
What exception will be thrown as a result of its execution attempt?
**ReferenceError**

Using the debugger, we insert a breakpoint in the code at which, after running the program, we stop. In the debugger, we find a `Step` button among the step-by-step operation options. What does pressing it do? **Exactly one instruction immediately after the breakpoint will be executed and the program will be paused again**

```js
try {
    ocnsole.log("start");
} catch (error) {
    console.log("error");
} finally {
    console.log("end");}
```
What will happen as a result of its execution?
The following words will appear in the console `"error"` `"end"`.

Analyze the following code:
```js
"let x = 10;"
console.log(x);
```
What exception will be thrown as a result of its execution attempt?
**ReferenceError**

Analyze the following code:
```js
try {
    ocnsole.log("start");
} catch (error) {
    console.log("error");
} 
```
What will happen as a result of its execution?
In the console, there will appear in successive lines the words `"error"`, `"end"`.

Which of the following is a **syntax** error? Missing parenthesis ending a condition in an `if` statement.

Analyze the following code:
```js
const x = 10;
onsole.log(x);
x += 10;
```
What exception will be thrown as a result of its execution attempt?
**ReferenceError**

Where can we find in the debugger the information about currently called functions in our program? In the **call stack** window.

Analyze the following code:
```js
let x 10;
console.log(x);
```
What exception will be thrown as a result of its execution attempt? **SyntaxError**

What is the name of the place where program code execution is halted? breakpoint

Logical errors that we make while writing a program are not indicated by the interpreter. Why? **The interpreter is unable to identify logical errors because they are not related to either the syntax or the semantics of the JavaScript language.**

We want to measure how long a certain piece of code executes. In order to do so, it is enough to:
aprecede the fragment with the command `console.time("counter")` and end with `console.timeEnd("counter")`.

Analyze the following code:
```js
const x = 10;
x = 20;
```
What exception will be thrown as a result of its execution attempt? 
**TypeError**

## Final
We can replace the declaration `let x = 3e-3;` with:
'let x = 0.003;'
