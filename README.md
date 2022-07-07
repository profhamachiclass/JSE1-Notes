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

The number `2` is stored in the variable `n (let n = 2;)`. The command `n = n*n*n` is the called. This last command can be replaced by: `n **= 3;`

Which operator do we use if we want to check if two variables store the same values of exactly the same type? `===`

The string `"12"` has been written into the `str` variable: (`let str = "12";`). Then the operation `str = +str` is performed. As a result, the variable `str` will contain `12`

