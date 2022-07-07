# Overview

### What is javascript?
<details>
  <summary>:bulb:</summary>
    JavaScript, often abbreviated JS, is a programming language that is one of the core technologies of the World Wide Web, alongside HTML and CSS. As of 2022, 98% of websites use JavaScript on the client side for web page behavior, often incorporating third-party libraries.
</details>

### What makes JavaScript unique?
<details>
  <summary>:bulb:</summary>
    <li>Full integration with HTML/CSS.</li>
    <li>Simple things are done simply.</li>
    <li>Supported by all major browsers and enabled by default.</li>
</details>

# Topics

### Variables
<details>
  <summary>:bulb:</summary>
  A variable is a “named storage” for data. We can use variables to store goodies, visitors, and other data.

```JS
let message;
message = 'Hello!';

alert(message); // shows the variable content
```
</details>

### Difference between var - let - const:

<details>
  <summary>:bulb:</summary>

Props | var | let | const
------------ | ------------- | ------------ | ------------
Scope | Variables declared with var are in the function scope.(var variables are only accessible in the function scope) | Variables declared as let are in the block scope (let variables are only accessible within the block they are declared) | Variables declared as const are in the block scope(const variables under the block was accessible, but when you try to access x outside that block, you will get an error)
Hoisting (Hoisting means that you can define a variable before its declaration.) | Allowed | Not allowed | Not allowed
Reassign the value | Allowed | Allowed | Not allowed 
Redeclaration of the variable | Allowed | Not allowed | Not allowed

</details>

### Primitives

<details>
  <summary>:bulb:</summary>
A primitive
  <li>Is a value of a primitive type.</li>
  <li>There are 7 primitive types: string, number, bigint, boolean, symbol, null and undefined.</li>

#### <li> Strings </li>
A string (or a text string) is a series of characters like "John Doe".
Strings are written with quotes. You can use single or double quotes.

``` JS
let carName1 = "Volvo XC60";   // Using double quotes
let carName2 = 'Volvo XC60';   // Using single quotes
```
``` JS
let answer1 = "It's alright";
let answer2 = "He is called 'Johnny'";
let answer3 = "He is called Johnny"";
```
#### <li> String Methods </li>

 ``` JS
<li>Length</li>
<!DOCTYPE html>
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Javascript</title>
</head>
<html>
<body>
<h1>Strings</h1>

<p>The length property returns the length of a string:</p>

<p id="demo"></p>

<script>
let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
document.getElementById("demo").innerHTML = text.length;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/177744213-023f7ead-8ee4-4a2f-9410-03ee6c0c60f0.png)

#### <li>Extracting String Parts</li>
There are 3 methods for extracting a part of a string:

slice(start, end)
substring(start, end)
substr(start, length)
#### <li> Numbers </li>
JavaScript has only one type of numbers.
Numbers can be written with, or without decimals.

``` JS
let x1 = 34.00;
let x2 = 34;
let x3 = 3.14;
```
``` JS
let y = 123e5;      // 12300000
let z = 123e-5;     // 0.00123
```
#### <li> Arrays </li>
JavaScript arrays are written with square brackets.
Array items are separated by commas.

``` JS
const cars = ["Saab","Volvo","BMW"]  // cars is array
```

</details>




