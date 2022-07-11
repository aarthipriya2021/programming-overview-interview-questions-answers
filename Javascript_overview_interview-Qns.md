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

### Data types

<details>
  <summary>:bulb:</summary>


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

#### <li>search()</li>

<li>The search() method searches a string for a specified value and returns the position of the match</li>

``` JS
<!-- search() -->
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Methods</h2>

<p>The search() method returns the position of the first occurrence of a specified text in a string:</p>

<p id="demo"></p>

<script>
let str = "Please locate where 'locate' occurs!";
document.getElementById("demo").innerHTML = str.search("locate");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178099923-0e2e8a0e-1e0c-4e99-9a37-8deb875cda63.png)

#### <li>match()</li>

<li>The match() method searches a string for a match against a regular expression, and returns the matches, as an Array object.</li>

``` JS
<!-- match() -->
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Search</h2>

<p>Search a string for "ain":</p>

<p id="demo"></p>

<script>
let text = "The rain in SPAIN stays mainly in the plain"; 
document.getElementById("demo").innerHTML = text.match(/ain/g);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178100530-ec38c854-a564-485c-ae67-3066589f5822.png)

#### <li>includes()</li>

<li>The includes() method searches a string for a match against a regular expression, and returns the matches, as an Array object.</li>

``` JS
<!-- includes() -->
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript String Search</h2>

<p>Check if a string includes "world":</p>

<p id="demo"></p>

<p>The includes() method is not supported in Internet Explorer.</p>

<script>
let text = "Hello world, welcome to the universe.";
document.getElementById("demo").innerHTML = text.includes("world");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178100706-8fd5ac68-a782-4dbd-8df5-c48fc88acb73.png)


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

#### <li> Number Methods </li>

#### <li>toString()</li>

<li>The toString() method returns a number as a string.</li>
<li>All number methods can be used on any type of numbers (literals, variables, or expressions)</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Number Methods</h2>

<p>The toString() method converts a number to a string.</p>

<p id="demo"></p>

<script>
let x = 123;
document.getElementById("demo").innerHTML =
  x.toString() + "<br>" +
   (123).toString() + "<br>" +
   (100 + 23).toString();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178102220-11728681-6117-4fb7-8dc9-b99a3e9730ce.png)

#### <li>toExponential()</li>

<li>The toString() method returns a number as a string.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Number Methods</h2>

<p>toExponential() returns a string, with a number rounded and written using exponential notation.</p>

<p>An optional parameter defines the number of digits behind the decimal point.</p>

<p id="demo"></p>

<script>
let x = 9.656;
document.getElementById("demo").innerHTML =
  x.toExponential() + "<br>" + 
  x.toExponential(2) + "<br>" + 
  x.toExponential(4) + "<br>" + 
  x.toExponential(6);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178102409-3926e4a9-18f8-4cc0-b7b3-764f4263283d.png)

#### <li>toFixed()</li>

<li>toFixed() returns a string, with the number written with a specified number of decimals</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Number Methods</h2>

<p>The toFixed() method rounds a number to a given number of digits.</p>
<p>For working with money, toFixed(2) is perfect.</p>

<p id="demo"></p>

<script>
let x = 9.656;
document.getElementById("demo").innerHTML =
  x.toFixed(0) + "<br>" +
  x.toFixed(2) + "<br>" +
  x.toFixed(4) + "<br>" +
  x.toFixed(6);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178102453-99205a98-f117-41e6-98ac-c57570474803.png)

#### <li>Converting Variables to Numbers</li>

<li>The Number() method</li>
<li>The parseInt() method</li>
<li>The parseFloat() method</li>

![image](https://user-images.githubusercontent.com/75599178/178102559-46a11067-da95-4728-9d35-1d689dd32538.png)

#### The Number() Method
> Example 1:

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Global Methods</h2>

<p>The Number() method converts variables to numbers:</p>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = 
  Number(true) + "<br>" +
  Number(false) + "<br>" +
  Number("10") + "<br>" + 
  Number("  10") + "<br>" +
  Number("10  ") + "<br>" +
  Number(" 10  ") + "<br>" +
  Number("10.33") + "<br>" + 
  Number("10,33") + "<br>" +
  Number("10 33") + "<br>" +
  Number("John");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178103960-cb631550-2780-43ec-8702-88770bef40c3.png)

#### The parseInt() Method

> Example 2:

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Global Functions</h2>
<h2>parseInt()</h2>
<p>The global JavaScript function parseInt() converts strings to numbers:</p>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = 
  parseInt("-10") + "<br>" +
  parseInt("-10.33") + "<br>" +
  parseInt("10") + "<br>" +
  parseInt("10.33") + "<br>" +
  parseInt("10 6") + "<br>" +  
  parseInt("10 years") + "<br>" +  
  parseInt("years 10");  
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178104645-92ed9a00-b50c-4c41-8b35-7ab7078e060c.png)

#### The parseFloat() Method

> Example 3:

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Global Methods</h2>

<p>The parseFloat() method converts strings to numbers:</p>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = 
  parseFloat("10") + "<br>" +
  parseFloat("10.33") + "<br>" +
  parseFloat("10 6") + "<br>" +  
  parseFloat("10 years") + "<br>" +
  parseFloat("years 10");    
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178104751-a61651d9-9dee-478f-9d6f-e7bf12d091f8.png)

#### <li> Arrays </li>
JavaScript arrays are written with square brackets.
Array items are separated by commas.

``` JS
const cars = ["Saab","Volvo","BMW"]  // cars is array
```

#### Creating an Array
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Arrays</h2>

<p id="demo"></p>

<script>
const cars = new Array("Saab", "Volvo", "BMW");
document.getElementById("demo").innerHTML = cars;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178105722-f016911f-133b-4ff3-8efe-3293ce1651bb.png)

#### Creating an Array
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Arrays</h2>

<p id="demo"></p>

<script>
const cars = new Array("Saab", "Volvo", "BMW");
document.getElementById("demo").innerHTML = cars;
</script>

</body>
</html>

```


#### <li> Array Methods </li>

#### toString()

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2> 
<h2>toString()</h2>
<p>The toString() method returns an array as a comma separated string:</p>

<p id="demo"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.toString();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178266325-14f2375c-0b47-4634-893d-155d4dbf7f93.png)

#### join()

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2> 
<h2>join()</h2> 
<p>The join() method joins array elements into a string.</p>
<p>It this example we have used " * " as a separator between the elements:</p>

<p id="demo"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.join(" * ");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178271178-f3015e17-d06a-4e09-acd0-a61031418fb2.png)


#### pop()

<li>Popping items out of an array, or pushing items into an array.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2>
<h2>pop()</h2>
<p>The pop() method removes the last element from an array.</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits;
fruits.pop();
document.getElementById("demo2").innerHTML = fruits;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178267408-2f52bea2-b76b-469a-aa5a-8240cd29f871.png)

#### push()

<li>The push() method adds a new element to an array (at the end)</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2> 
<h2>push()</h2>
<p>The push() method appends a new element to an array:</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits;
fruits.push("Kiwi");
document.getElementById("demo2").innerHTML = fruits;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178274531-3563124a-77e8-4493-8613-5f991a050278.png)

#### shift()

<li>The shift() method removes the first array element and "shifts" all other elements to a lower index.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2> 
<h2>shift()</h2>
<p>The shift() method removes the first element of an array (and "shifts" the other elements to the left):</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits;
fruits.shift();
document.getElementById("demo2").innerHTML = fruits;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178275051-5657a144-e525-4fc6-b771-48078302c22e.png)


#### unshift()

<li>The unshift() method adds a new element to an array (at the beginning), and "unshifts" older elements</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2> 
<h2>unshift()</h2>
<p>The unshift() method adds new elements to the beginning of an array:</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits;
fruits.unshift("Lemon");
document.getElementById("demo2").innerHTML = fruits;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178276283-f786b1d4-3995-4fc9-b74d-cedc2780861a.png)

#### Array length

<li>The length property provides an easy way to append new elements to an array without using the push() method.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2>
<p>The length property provides an easy way to append new elements to an array without using the push() method:</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits;
fruits[fruits.length] = "Kiwi";
document.getElementById("demo2").innerHTML = fruits;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178277027-0c29ecaf-8b2c-4126-9d6a-1cf0f3d0b2a5.png)

#### Array delete()

<li>The length property provides an easy way to append new elements to an array without using the push() method.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2>
<p>Deleting elements leaves undefined holes in an array:</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];

document.getElementById("demo1").innerHTML =
"The first fruit is: " + fruits[0];

delete fruits[0];

document.getElementById("demo2").innerHTML =
"The first fruit is: " + fruits[0];
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178277619-80c52fbb-cc6b-4141-a2b6-338089ba6ba1.png)

#### Merging (Concatenating) Arrays

<li>The concat() method creates a new array by merging (concatenating) existing arrays</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2>
<h2>concat()</h2>
<p>The concat() method merges (concatenates) arrays:</p>

<p id="demo"></p>

<script>
const myGirls = ["Cecilie", "Lone"];
const myBoys = ["Emil", "Tobias", "Linus"];
const myChildren = myGirls.concat(myBoys);

document.getElementById("demo").innerHTML = myChildren;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178277933-6f6ebfd8-400e-42a6-9047-d21071ee4676.png)

#### splice()

<li>The splice() method can be used to add new items to an array</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2>
<h2>splice()</h2>

<p>The splice() method adds new elements to an array, and returns an array with the deleted elements (if any):</p>

<p id="demo1"></p>
<p id="demo2"></p>
<p id="demo3"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = "Original Array:<br> " + fruits;
let removed = fruits.splice(2, 2, "Lemon", "Kiwi"); 
document.getElementById("demo2").innerHTML = "New Array:<br>" + fruits;
document.getElementById("demo3").innerHTML = "Removed Items:<br> " + removed; 
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178326065-c44bb714-b222-42ab-b192-cbe094b65bad.png)

![image](https://user-images.githubusercontent.com/75599178/178325956-0a438e94-76d6-4561-87ff-98e92aeeb1b5.png)

#### slice()

<li>The slice() method slices out a piece of an array into a new array.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Methods</h2>
<h2>slice()</h2>
<p>This example slices out a part of an array starting from array element 1 ("Orange"):</p>

<p id="demo"></p>

<script>
const fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
const citrus = fruits.slice(1);
document.getElementById("demo").innerHTML = fruits + "<br><br>" + citrus;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178326337-e214e5d4-2927-4232-97d8-31d11d611929.png)

#### sort()

<li>The sort() method sorts an array alphabetically</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Sort</h2>
<p>The sort() method sorts an array alphabetically:</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits;

fruits.sort();
document.getElementById("demo2").innerHTML = fruits;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178327234-c87a6f44-410a-4aea-942e-cfc66178f4f5.png)

#### reverse()

<li>The slice() method slices out a piece of an array into a new array.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Sort</h2>
<p>The sort() method sorts an array alphabetically:</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits;

fruits.sort();
document.getElementById("demo2").innerHTML = fruits;
</script>

</body>
</html>

```
</details>





