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
The msg variable contains a String type value. Information about the number of characters of this string can be obtained using:


Analyze the code snippet:
```js
let counter = 0;
let userName = “John”;
```

After declaring a counter variable, we want to put a short comment with information about what the variable is used for. To do this, we modify the line with the declaration to the form:

In the daysOfWeek variable, we place an array with the names of the days of dthe week. To reverse the order of the array elements, we should call:

We want to declare a distance constant and initialize it with the value 120. What should such a declaration look like?

Performing the operation: `let x = 100 / 0;` will result in:

We have declared an array of selected month names `let summer = [ “June”, “July”, “August”];` We want to change the value `“July”` stored in the array to the number `7`

We perform the operation: `let x = “abcdefg”.slice(2, 4)` . As a result, the value:

Analyze the following code:

```
let x = 10 / 100;
console.log(typeof (x))
```

As a result of its execution:

Analyze the following code:
```js
let height = 180;
{
    let heigh = 200;
    height = height + 10;
}
console.log(height);
```
Point out the correct declaration of the height variable:

Complex (or composite) data types:

We have declared an array of animals `let animals = [“dog”, “cat”, “hamster”]` . Then we call the method `animals.push(“canary”);` . As a result, the animals array will look like this:


Analyze the code snippet:
```js
let summer = [“June”, “July”, “August”];
let index = summer.indexOf(“June”);
```
The index variable will have the value:


Analyze the code snippet:
```js
let name;
let age;
{
let height;					    // 2
{							    // 2
	let weight:	        // 1	// 2
	console.log(name);
}							    // 2
console.log(name);		// 2
}
```
We have access to the weight variable:

What does **shadowing** mean?

We can replace the declaration `let x = 0x21;` with:

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
name =
profession =
age =
height =
weight =

We have declared an array of animals `let animals = [“dog”, “cat”, “hamster”]` . Then we call the method `animals.pop();`. As a result, the animals array will look like this:

In order to check the number of elements of the array stored in the `names` variable, we call:

Performing the operation: `let x = 20n + 10;` will result in:

Performing the operation: `let x = "Alice" + 10;` will result in:

We want to convert the string `"1024"` to type **Number** and store the result in variable `n`. Point out the correct statement:

We declare an object called `dog`, with two fields: `age` and `name`:
```js
let dog = {
    age: 5.
    name: "Axel"
};
```
To change the value of the `age` field to `6`, we need to perform:

Review the following code (note the variable name):
```js
let age = 32;
age = age + 1;
console.log(Age);
```
As a result of its execution, the following should appear in the console:

If a variable stores the value `false`, then the variable:

We have declared an array `let animals = [“dog”, “cat”, “hamster”]` . We want to temporarily comment out the element `"cat"`, and to do this, we can modify the declaration as follows:

We need to come up with a name for a variable where we will store **the age of a user**. All of the following variable names are formally correct, but one of them is the most readable, indicate which one:

By default, JavaScript allows us to write to an undeclared variable (it declares it implicitly for us). If we want the interpreter to treat such a situation as an error, we have to:

Analyze the following code:
```js
let counter = 100;
let counter = 200;
counter = 300;
```
As a result of its execution:

