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

#### <li>Slice()</li>
<li>slice() extracts a part of a string and returns the extracted part in a new string.</li>
<li>The method takes 2 parameters: the start position, and the end position (end not included).</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Methods</h2>

<p>The slice() method extract a part of a string
and returns the extracted parts in a new string:</p>

<p id="demo"></p>

<script>
let str = "Apple, Banana, Kiwi";
document.getElementById("demo").innerHTML = str.slice(7,13); 
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/177770021-8aff74be-dd26-4419-a97a-dbf074fdf994.png)

<li>If a parameter is negative, the position is counted from the end of the string.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Methods</h2>

<p>The slice() method extract a part of a string
and returns the extracted parts in a new string:</p>

<p id="demo"></p>

<script>
let str = "Apple, Banana, Kiwi";
document.getElementById("demo").innerHTML = str.slice(-12,-6);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/177770851-47a65955-0338-4536-a1f8-948ecb6e4569.png)

<li>If you omit the second parameter, the method will slice out the rest of the string.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Methods</h2>

<p>The slice() method extract a part of a string
and returns the extracted parts in a new string:</p>

<p id="demo"></p>

<script>
let str = "Apple, Banana, Kiwi";
document.getElementById("demo").innerHTML = str.slice(7);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/177771563-d2efacc4-49b8-4d5e-b9b7-998b51c84013.png)

#### <li>substr()</li>
<li>substr() is similar to slice().</li>
<li>The difference is that the second parameter specifies the length of the extracted part.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Methods</h2>

<p>The substr() method extract a part of a string
and returns the extracted parts in a new string:</p>

<p id="demo"></p>

<script>
let str = "Apple, Banana, Kiwi";
document.getElementById("demo").innerHTML = str.substr(7,6);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/177947955-f1a22229-15c1-41d3-90c9-76ffa1eac2d3.png)

#### <li>Replacing String Content</li>

<li>The replace() method does not change the string it is called on.</li>
<li>The replace() method returns a new string.</li>
<li>he replace() method replaces only the first match</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Methods</h2>

<p>Replace "Microsoft" with "W3Schools" in the paragraph below:</p>

<button onclick="myFunction()">Try it</button>

<p id="demo">Please visit Microsoft and Microsoft!</p>

<script>
function myFunction() {
  let text = document.getElementById("demo").innerHTML; 
  document.getElementById("demo").innerHTML =
  text.replace("Microsoft","W3Schools");
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/177958396-ff5fcdc8-9c28-4017-a2f5-aaa2363415d9.png)

#### <li>Converting to Upper and Lower Case</li>

<li>A string is converted to upper case with toUpperCase()</li>
<li>A string is converted to lower case with toLowerCase()</li>

``` JS
<!-- Uppercase -->
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

<button onclick="myFunction()">Replace it</button>

<p id="upper">Can you open chrome browser?</p>

<script>
    function myFunction(){
        let text1 = document.getElementById("upper").innerHTML;
        document.getElementById("upper").innerHTML = text1.toUpperCase()
    }

</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/177996365-1c632f90-340c-4746-99ff-41ff006ed46f.png)

``` JS
<!-- Smallcase -->
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

<button onclick="myFunction()">Replace it</button>

<p id="lower">Can you open chrome browser?</p>

<script>
    function myFunction(){
        let text1 = document.getElementById("lower").innerHTML;
        document.getElementById("lower").innerHTML = text1.toLowerCase()
    }

</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/177996633-da81fef6-74ae-4044-8977-ee59ed79a33c.png)

> Strings are immutable: Strings cannot be changed, only replaced.

#### <li>concat</li>

<li>The concat() method can be used instead of the plus operator.</li>

``` JS
<!-- concat -->
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Methods</h2>

<p>The concat() method joins two or more strings:</p>

<p id="demo"></p>

<script>
let text1 = "Hello";
let text2 = "World!";
let text3 = text1.concat(" ",text2);
document.getElementById("demo").innerHTML = text3;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/177998979-03669755-e8ff-4493-8048-874ffc3f6575.png)

#### <li>trim</li>

<li>The trim() method removes whitespace from both sides of a string.</li>

``` JS
<!-- trim -->
<!DOCTYPE html>
<html>
<body>

<h1>JavaScript Strings</h1>
<h2>The trim() Method</h2>
<p>The trim() method removes whitespace from both sides of a string.</p>

<p id="demo"></p>

<script>
let text1 = "     Hello World!     ";
let text2 = text1.trim();

document.getElementById("demo").innerHTML =
"Length text1=" + text1.length + "<br>Length2 text2=" + text2.length;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178003016-aa3add38-af2a-4120-b5ea-42968bf0b864.png)

#### String Search Methods

<h4>JavaScript Search Methods</h4>
<li>String indexOf()</li>
<li>String lastIndexOf()</li>
<li>String startsWith()</li>
<li>String endsWith()</li>

#### <li>indexOf()</li>

<li>The indexOf() method returns the index of (the position of) the first occurrence of a specified text in a string</li>

``` JS
<!-- indexOf() -->
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Methods</h2>

<p>The indexOf() method returns the position of the first occurrence of a specified text:</p>

<p id="demo"></p>

<script>
let str = "Please locate where 'locate' occurs!";
document.getElementById("demo").innerHTML = str.indexOf("locate");
</script>

</body>
</html>


```
![image](https://user-images.githubusercontent.com/75599178/178013526-7c5219d2-2c19-4fd4-9f28-1afe1054079a.png)



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




