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

<li>The reverse() method reverses the elements in an array.</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Sort Reverse</h2>

<p>The reverse() method reverses the elements in an array.</p>
<p>By combining sort() and reverse() you can sort an array in descending order:</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
// Create and display an array:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo1").innerHTML = fruits;

// First sort the array
fruits.sort();

// Then reverse it:
fruits.reverse();

document.getElementById("demo2").innerHTML = fruits;
</script>

</body>
</html>


```
![image](https://user-images.githubusercontent.com/75599178/179484922-7ffe146f-d4b9-4375-9b73-219f4d3e5063.png)

#### Numeric Sort

<li>Ascending order</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Sort</h2>
<p>Sort the array in ascending order:</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const points = [40, 100, 1, 5, 25, 10];
document.getElementById("demo1").innerHTML = points;  

points.sort(function(a, b){return a - b});
document.getElementById("demo2").innerHTML = points;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178328161-6a60d477-c121-4837-8edd-b4779be5b2ba.png)

#### Numeric Sort

<li>Desscending order</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Sort</h2>
<p>Sort the array in descending order:</p>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
const points = [40, 100, 1, 5, 25, 10];
document.getElementById("demo1").innerHTML = points;

points.sort(function(a, b){return b - a});
document.getElementById("demo2").innerHTML = points;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178328666-75b9f8ba-8574-4178-96e2-8da48a3c9925.png)

#### Sorting an Array in Random Order

<li>Sorting an Array in Random Order</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array Sort</h2>
<p>Click the button (again and again) to sort the array in random order.</p>

<button onclick="myFunction()">Try it</button>
<p id="demo"></p>

<script>
const points = [40, 100, 1, 5, 25, 10];
document.getElementById("demo").innerHTML = points;  

function myFunction() {
  points.sort(function(a, b){return 0.5 - Math.random()});
  document.getElementById("demo").innerHTML = points;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178328937-19b7086b-4cf8-4682-ae15-34932cf68236.png)

#### <li>Date and Time</li>

#### <li>JavaScript new Date()</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript new Date()</h2>
<p>Using new Date(milliseconds), creates a new date object as January 1, 1970, 00:00:00 Universal Time (UTC) plus the milliseconds:</p>

<p id="demo"></p>

<script>
const d = new Date();
document.getElementById("demo").innerHTML = d;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178442188-a0daf489-bdc2-4307-825f-8966b86ad697.png)

#### <li>JavaScript toString()</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript toString()</h2>
<p>The toString() method converts a date to a string:</p>

<p id="demo"></p>

<script>
const d = new Date();
document.getElementById("demo").innerHTML = d.toString();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178443069-2d958c2e-6d59-43b7-98d9-0115f1407e49.png)

#### <li>JavaScript toUTCString()</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Date()</h2>
<p>The toUTCString() method converts a date to a UTC string (a date display standard):</p>

<p id="demo"></p>

<script>
const d = new Date();
document.getElementById("demo").innerHTML = d.toUTCString();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178443297-fa37efa5-ce60-4275-8f9e-cc57bf55e980.png)

#### <li>JavaScript toUTCString()</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript toDateString()</h2>
<p>The toDateString() method converts a date to a date string:</p>

<p id="demo"></p>

<script>
const d = new Date();
document.getElementById("demo").innerHTML = d.toDateString();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178443456-7f362eb0-5fba-4d8c-b234-6ddbe826cf95.png)

#### <li>JavaScript toUTCString()</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript toISOString()</h2>
<p>The toISOString() method converts a date to a date string, using the ISO standard format:</p>

<p id="demo"></p>

<script>
const d = new Date();
document.getElementById("demo").innerHTML = d.toISOString();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178443597-c88d020c-e663-48ab-8c0d-07beb2fe7c64.png)

#### <li>Booleans</li>

![image](https://user-images.githubusercontent.com/75599178/178444096-e3503e47-bf3b-49bf-97e1-9fb5b040c1fb.png)

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Booleans</h2>
<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML =
"100 is " + Boolean(100) + "<br>" +
"3.14 is " + Boolean(3.14) + "<br>" +
"-15 is " + Boolean(-15) + "<br>" +
"Any (not empty) string is " + Boolean("Hello") + "<br>" +
"Even the string 'false' is " + Boolean('false') + "<br>" +
"Any expression (except zero) is " + Boolean(1 + 7 + 3.14);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178444404-95b5a775-6b71-4d5d-bd33-6d324deb01ab.png)

#### <li>Objects</li>
> A JavaScript object is a collection of named values
#### <li>Creating a JavaScript Object</li>
  With JavaScript, you can define and create your own objects.

  There are different ways to create new objects:

  <li>Create a single object, using an object literal.</li>
  <li>Create a single object, with the keyword new.</li>
  <li>Define an object constructor, and then create objects of the constructed type.</li>
  <li>Create an object using Object.create().</li>

#### <li>Using an Object Literal</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Objects</h2>
<p>Creating a JavaScript Object:</p>

<p id="demo"></p>

<script>
const person = {};
person.firstName = "John";
person.lastName = "Doe";
person.age = 50;
person.eyeColor = "blue"; 

document.getElementById("demo").innerHTML =
person.firstName + " is " + person.age + " years old.";
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179585016-24d5449f-0187-408a-b3b5-fd387489667d.png)

#### <li>JavaScript Keyword new</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Objects</h2>
<p>Creating a JavaScript Object:</p>

<p id="demo"></p>

<script>
const person = new Object();
person.firstName = "John";
person.lastName = "Doe";
person.age = 50;
person.eyeColor = "blue"; 

document.getElementById("demo").innerHTML =
person.firstName + " is " + person.age + " years old.";
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179586964-9784148d-e6b1-442b-b7ef-6e1901d92644.png)


</details>

### Math, random,comparison

<details>
  <summary>:bulb:</summary>

### Math

> The Math object is static.

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Math Constants</h2>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = 
"<p><b>Math.E:</b> " + Math.E + "</p>" +
"<p><b>Math.PI:</b> " + Math.PI + "</p>" +
"<p><b>Math.SQRT2:</b> " + Math.SQRT2 + "</p>" +
"<p><b>Math.SQRT1_2:</b> " + Math.SQRT1_2 + "</p>" +
"<p><b>Math.LN2:</b> " + Math.LN2 + "</p>" +
"<p><b>Math.LN10:</b> " + Math.LN10 + "</p>" +
"<p><b>Math.LOG2E:</b> " + Math.LOG2E + "</p>" +
"<p><b>Math.Log10E:</b> " + Math.LOG10E + "</p>";
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178453331-600e8e25-e3d4-4bf6-a340-c75d16b04058.png)

#### <li>Math</li>

> The Math object is static.

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Math.ceil()</h2>

<p>Math.round(x) returns the value of x rounded to its nearest integer:</p>
<p>Math.ceil() rounds a number <strong>up</strong> to its nearest integer:</p>
<p>Math.floor(x) returns the value of x rounded <strong>down</strong> to its nearest integer:</p>
<p>Math.trunc(x) returns the integer part of x:</p>
<p>Math.random() returns a random number between 0 and 1:</p>
<p>Math.min() returns the lowest value in a list of arguments:</p>
<p>Math.abs(x) returns the absolute (positive) value of x:</p>
<p>Math.sqrt(x) returns the square root of x:</p>
<p>Math.pow(x,y) returns the value of x to the power of y:</p>

<p id="demo_1"></p>
<p id="demo_2"></p>
<p id="demo_3"></p>
<p id="demo_4"></p>
<p id="demo_5"></p>
<p id="demo_6"></p>
<p id="demo_7"></p>
<p id="demo_8"></p>


<script>
document.getElementById("demo_1").innerHTML = Math.round(4.4);
document.getElementById("demo_2").innerHTML = Math.ceil(4.4);
document.getElementById("demo_3").innerHTML = Math.floor(4.7);
document.getElementById("demo_4").innerHTML = Math.trunc(4.7);
document.getElementById("demo_5").innerHTML = Math.min(0, 150, 30, 20, -8, -200);
document.getElementById("demo_6").innerHTML = Math.abs(-4.7);
document.getElementById("demo_7").innerHTML = Math.sqrt(64);
document.getElementById("demo_8").innerHTML = Math.pow(8,2);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178455359-62defeb7-1dc0-47b8-84c3-ad3b4ecbb9cf.png)


</details>

### if, else, and else if

<details>
  <summary>:bulb:</summary>

![image](https://user-images.githubusercontent.com/75599178/178487683-5ee72db5-1e41-407e-9ee3-467c6b8f4226.png)

#### Syntax

``` JS
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}

```
#### Example:-

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript if .. else</h2>

<p>A time-based greeting:</p>

<p id="demo"></p>

<script>
const time = new Date().getHours();
let greeting;
if (time < 10) {
  greeting = "Good morning";
} else if (time < 20) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
document.getElementById("demo").innerHTML = greeting;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178488628-35419b90-201f-4870-8c8c-72f78d5de6f6.png)

#### Switch 

##### Syntax

``` JS
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}

```
![image](https://user-images.githubusercontent.com/75599178/178489544-00327d83-0acc-496d-a2f9-fe196c1da97c.png)

#### Example

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript switch</h2>

<p id="demo"></p>

<script>
let day;
switch (new Date().getDay()) {
  case 0:
    day = "Sunday";
    break;
  case 1:
    day = "Monday";
    break;
  case 2:
    day = "Tuesday";
    break;
  case 3:
    day = "Wednesday";
    break;
  case 4:
    day = "Thursday";
    break;
  case 5:
    day = "Friday";
    break;
  case  6:
    day = "Saturday";
}
document.getElementById("demo").innerHTML = "Today is " + day;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178489776-ba103df6-6006-40de-bf4c-dbfbedb42c11.png)

#### the break keyword

> When JavaScript reaches a break keyword, it breaks out of the switch block.

> This will stop the execution inside the switch block.

> It is not necessary to break the last case in a switch block. The block breaks (ends) there anyway.

#### The default Keyword

> he default keyword specifies the code to run if there is no case match.

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript switch</h2>

<p id="demo"></p>

<script>
let text;
switch (new Date().getDay()) {
  case 6:
    text = "Today is Saturday";
    break;
  case 0:
    text = "Today is Sunday";
    break;
  default:
    text = "Looking forward to the Weekend";
}
document.getElementById("demo").innerHTML = text;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178491144-6c4d1ab2-e8e6-4b2e-b0d3-b51c0300471d.png)

#### Strict Comparison

> Switch cases use strict comparison (===).

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript switch</h2>

<p id="demo"></p>

<script>
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript switch</h2>

<p id="demo"></p>

<script>
let x = "0";

switch (x) {
  case 0:
    text = "Off";
    break;
  case 1:
    text = "On";
    break;
  default:
    text = "No value found";
}
document.getElementById("demo").innerHTML = text;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178491558-a8078e77-48fa-4a91-b2a9-3d1a46b3f3ff.png)

</details>

### Loops

<details>
  <summary>:bulb:</summary>
<li>Loops can execute a block of code a number of times.</li>

![image](https://user-images.githubusercontent.com/75599178/178744644-f0f7d302-a9a8-49bb-b018-93fbce6680f3.png)

#### The For Loop

#### <li>Syntax</li>

``` JS
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```
**Statement 1** is executed (one time) before the execution of the code block.<br>
**Statement 2**defines the condition for executing the code block.<br>
**Statement 3** is executed (every time) after the code block has been executed.<br>

#### <li>Example</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript For Loop</h2>

<p id="demo"></p>

<script>
let text = "";

for (let i = 0; i < 5; i++) {
  text += "The number is " + i + "<br>";
}

document.getElementById("demo").innerHTML = text;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178748468-654e08b3-37f4-464e-b8a6-1cc691ead3a1.png)

#### The For In Loop
#### <li>Syntax</li>

``` JS
for (key in object) {
  // code block to be executed
}
```
#### Example
``` JS

<!DOCTYPE html>
<html>
<body>

<h2>JavaScript For In Loop</h2>
<p>The for in statement loops through the properties of an object:</p>

<p id="demo"></p>

<script>
const person = {fname:"John", lname:"Doe", age:25}; 

let txt = "";
for (let x in person) {
  txt += person[x] + " ";
}

document.getElementById("demo").innerHTML = txt;
</script>

</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/178794759-9a13da85-7629-45bc-ba08-967cb3c37c7e.png)

Example Explanation:<br>
![image](https://user-images.githubusercontent.com/75599178/178794861-742f95a6-d619-45f1-974a-3131842f7fff.png)

#### For In Over Arrays
#### <li>Syntax</li>

``` JS
for (variable in array) {
  code
}
```
#### Example

``` JS

<!DOCTYPE html>
<html>
<body>

<h2>JavaScript For In</h2>
<p>The for in statement can loops over array values:</p>

<p id="demo"></p>

<script>
const numbers = [45, 4, 9, 16, 25];

let txt = "";
for (let x in numbers) {
  txt += numbers[x] + "<br>"; 
}

document.getElementById("demo").innerHTML = txt;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178795213-e7e356ee-d4b8-482a-be7d-1b5653a29ab5.png)

> It is better to use a for loop, a for of loop, or Array.forEach() when the order is important.

#### Array.forEach()
#### <li>Syntax</li>

``` JS
for (variable in array) {
  code
}
```
#### Example

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Array.forEach()</h2>
<p>Calls a function once for each array element.</p>

<p id="demo"></p>

<script>
const numbers = [45, 4, 9, 16, 25];

let txt = "";
numbers.forEach(myFunction);
document.getElementById("demo").innerHTML = txt;

function myFunction(value) {
  txt += value + "<br>"; 
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178795612-cc3a75ff-45a6-4e60-8963-3fd827ab968e.png)

#### The While Loop
> Loops can execute a block of code as long as a specified condition is true.

#### <li>Syntax</li>

``` JS
while (condition) {
  // code block to be executed
}
```
#### Example

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript While Loop</h2>

<p id="demo"></p>

<script>
let text = "";
let i = 0;
while (i < 10) {
  text += "<br>The number is " + i;
  i++;
}
document.getElementById("demo").innerHTML = text;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178796184-436ae138-7891-4048-8c43-9cf916512686.png)

#### The Do While Loop
#### <li>Syntax</li>

``` JS
do {
  // code block to be executed
}
while (condition);
```
#### Example
> The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Do While Loop</h2>

<p id="demo"></p>

<script>
let text = ""
let i = 0;

do {
  text += "<br>The number is " + i;
  i++;
}
while (i < 10);  

document.getElementById("demo").innerHTML = text;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178796541-5d0c7c13-ca88-4dc2-971c-d92890f0a1ef.png)

</details>

### Sets

<details>
  <summary>:bulb:</summary>

> A JavaScript Set is a collection of unique values.

> Each value can only occur once in a Set.

#### Essential Set Methods
![image](https://user-images.githubusercontent.com/75599178/178798670-aa0227a4-5843-405a-97eb-5c80ab42aeb4.png)

#### How to create new set
You can create a JavaScript Set by:
<li>Passing an Array to new Set()</li>
<li>Create a new Set and use add() to add values</li>
<li>Create a new Set and use add() to add variables</li>

#### <li>The new Set() Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Sets</h2>
<p>Create a Set from an Array:</p>

<p id="demo"></p>

<script>
// Create a Set
const letters = new Set(["a","b","c","d"]);

// Display set.size
document.getElementById("demo").innerHTML = letters.size;
</script>

</body>
</html>

```

#### <li>The add() Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Sets</h2>
<p>Adding equal elements to a Set:</p>

<p id="demo"></p>

<script>
// Create a Set
const letters = new Set();

// Add values to the Set
letters.add("a");
letters.add("b");
letters.add("c");
letters.add("c");
letters.add("c");
letters.add("c");
letters.add("c");
letters.add("c");

// Display set.size
document.getElementById("demo").innerHTML = letters.size;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178801261-a7daf0b2-f1c7-4c04-aa8a-0d4c0040f76f.png)

#### <li>The values() Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Sets</h2>
<p>Set.values() returns a Set Iterator:</p>

<p id="demo"></p>

<script>
// Create a Set
const letters = new Set(["a","b","c"]);

// Display set.size
document.getElementById("demo").innerHTML = letters.values();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178801485-97389db4-ae3a-40bd-923d-3210a206f411.png)

</details>

### Maps

<details>
  <summary>:bulb:</summary>

> A Map holds key-value pairs where the keys can be any datatype.

> A Map remembers the original insertion order of the keys.

#### Essential Set Methods
![image](https://user-images.githubusercontent.com/75599178/178803671-eedf25d9-a07d-4c9c-8a3b-18b8a1f9172e.png)

#### How to create new map
You can create a JavaScript Map by:
<li>Passing an Array to new Map()</li>
<li>Create a Map and use Map.set()</li>

#### <li>The add() Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Map Objects</h2>
<p>Creating a Map from an Array:</p>

<p id="demo"></p>

<script>
// Create a Map
const fruits = new Map([
  ["apples", 500],
  ["bananas", 300],
  ["oranges", 200]
]);

document.getElementById("demo").innerHTML = fruits.get("apples");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178803825-2a51f03a-f278-4a09-a44e-3efcf32aacbc.png)

#### <li>The new Map() Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Map Objects</h2>
<p>Creating a Map from an Array:</p>

<p id="demo"></p>

<script>
// Create a Map
const fruits = new Map([
  ["apples", 500],
  ["bananas", 300],
  ["oranges", 200]
]);

document.getElementById("demo").innerHTML = fruits.get("apples");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178950904-152c5ac6-cb64-4c69-8cc4-37f59abaff77.png)

#### <li>The set() Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Map Objects</h2>
<p>Using Map.set():</p>

<p id="demo"></p>

<script>
// Create a Map
const fruits = new Map();

// Set Map Values
fruits.set("apples", 500);
fruits.set("bananas", 300);
fruits.set("oranges", 200);

document.getElementById("demo").innerHTML = fruits.get("apples");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178945539-83a7c58f-40bc-40f0-b447-822229f6c5ab.png)

#### <li>The get() Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Map Objects</h2>
<p>Using Map.set():</p>

<p id="demo"></p>

<script>
// Create a Map
const fruits = new Map();

// Set Map Values
fruits.set("apples", 500);
fruits.set("bananas", 300);
fruits.set("oranges", 200);

document.getElementById("demo").innerHTML = fruits.get("apples");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178949601-b0d9890c-2861-42b3-8b42-b955a6274aa0.png)

#### <li>The size Property</li>

``` JS
<!DOCTYPE html>
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Maps</h2>
<p>Using Map.size:</p>

<p id="demo"></p>

<script>
// Create a Map
const fruits = new Map([
  ["apples", 500],
  ["bananas", 300],
  ["oranges", 200]
]);

document.getElementById("demo").innerHTML = fruits.size;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178949659-5c59d30e-f02f-4be3-b952-c9cdd78642e8.png)

#### <li>The delete() Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Maps</h2>
<p>Deleting Map elements:</p>

<p id="demo"></p>

<script>
// Create a Map
const fruits = new Map([
  ["apples", 500],
  ["bananas", 300],
  ["oranges", 200]
]);

// Delete an Element
fruits.delete("apples");

document.getElementById("demo").innerHTML = fruits.size;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178949923-d83100d2-476b-43d3-ad26-efbc7a314f0f.png)

#### <li>The has() Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Maps</h2>
<p>Using Map.has():</p>

<p id="demo"></p>

<script>
// Create a Map
const fruits = new Map([
  ["apples", 500],
  ["bananas", 300],
  ["oranges", 200]
]);

document.getElementById("demo").innerHTML = fruits.has("apples");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178950395-21d5f178-0a57-4c56-8960-1522a7db5923.png)

</details>

### Type Conversion

<details>
  <summary>:bulb:</summary>

#### <li>Converting Strings to Numbers</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>The JavaScript typeof Operator</h2>

<p>Strings to number conversion</p>

<p id="demo_1"></p>
<p id="demo_2"></p>
<p id="demo_3"></p>
<p id="demo_4"></p>

<script>
document.getElementById("demo_1").innerHTML = Number("3.14");
document.getElementById("demo_2").innerHTML = Number(" ");
document.getElementById("demo_3").innerHTML = Number("");
document.getElementById("demo_4").innerHTML = Number("99 88");
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178977740-728cfceb-3362-47c9-ac6c-e955e3a2ba2a.png)

#### <li>Converting Numbers to Strings</li>
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
![image](https://user-images.githubusercontent.com/75599178/178977970-d8c5ba11-34dd-47a9-8d50-cb63fc8b4c18.png)

#### <li>Converting Dates to Numbers</li>

``` JS
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Date to number</title>
</head>
<body>
    <p id="demo"></p>
    <script>
        d = new Date()
        document.getElementById("demo").innerHTML = d.getTime()
    </script>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/178978293-8738e6cd-723a-4da2-81cd-ca594ffb96f8.png)

#### <li>Converting Dates to Strings</li>

``` JS
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Date to number</title>
</head>
<body>
    <p id="demo"></p>
    <script>
        d = new Date()
        document.getElementById("demo").innerHTML = d.toString()
    </script>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/178978744-4684444a-1c39-4a2a-a163-bbac5a8d5851.png)
![image](https://user-images.githubusercontent.com/75599178/178978799-9c38e0ec-c172-4a83-a75a-fce7a35d53d5.png)

#### <li>Converting Booleans to Numbers and Booleans to strings</li>

``` JS
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bools to Number & Bools to strings</title>
</head>
<body>
    <p id="demo_1"></p>
    <p id="demo_2"></p>
    <script>
        
        document.getElementById("demo_1").innerHTML = Number(true)
        document.getElementById("demo_2").innerHTML = false.toString()
    </script>
</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/178979861-f652de15-f7d6-40c8-b6a1-6de9dc61f493.png)

</details>

### Scope

<details>
  <summary>:bulb:</summary>
JavaScript has 3 types of scope:
<li>Block scope</li>
<li>Function scope</li>
<li>Global scope</li>

#### <li>Block Scope</li>

> The block scope restricts a variable's access to the block in which it is declared.

![image](https://user-images.githubusercontent.com/75599178/179144507-7c387b3f-e67a-472c-a9c0-645b8591f863.png)

Variables declared with the var keyword can NOT have block scope.

Variables declared inside a { } block can be accessed from outside the block.

![image](https://user-images.githubusercontent.com/75599178/179144578-965e333d-a12e-4316-a977-162324c42e1a.png)

#### <li>local Scope</li>
> Variables declared within a JavaScript function, become LOCAL to the function.

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Scope</h2>

<p><b>carName</b> is undefined outside myFunction():</p>

<p id="demo1"></p>

<p id="demo2"></p>

<script>
myFunction();

function myFunction() {
  let carName = "Volvo";
  document.getElementById("demo1").innerHTML = typeof carName + " " + carName;
}

document.getElementById("demo2").innerHTML = typeof carName;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179147067-76d20a12-2729-4b18-aa7a-59322e20895f.png)

#### <li>Function Scope</li>

> Variables declared with var, let and const are quite similar when declared inside a function.They all have Function Scope.

![image](https://user-images.githubusercontent.com/75599178/179147340-a5249d6a-799a-45f1-81d6-13f5995d7c88.png)
![image](https://user-images.githubusercontent.com/75599178/179147371-a75c99cf-7552-42ce-b849-1855acfdf0c0.png)
![image](https://user-images.githubusercontent.com/75599178/179147423-df8c9a64-71c3-47b7-8350-6167db974dac.png)

#### <li>Global Scope</li>

Variables declared Globally (outside any function) have Global Scope.<br>
  
Global variables can be accessed from anywhere in a JavaScript program.<br>
  
Variables declared with var, let and const are quite similar when declared outside a block.<br>
  
They all have Global Scope
> var x = 2;       // Global scope <br> <br> let x = 2;       // Global scope <br> <br> const x = 2;       // Global scope
</details>

### Errors

<details>
  <summary>:bulb:</summary>

#### Throw, and Try...Catch...Finally

> The try statement defines a code block to run (to try).<br>
The catch statement defines a code block to handle any error.<br>
The finally statement defines a code block to run regardless of the result.<br>
The throw statement defines a custom error.

> Errors can be coding errors made by the programmer, errors due to wrong input, and other unforeseeable things.

#### JavaScript try and catch

``` JS
try {
  Block of code to try
}
catch(err) {
  Block of code to handle errors
}
```
#### Example 

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Error Handling</h2>

<p>How to use <b>catch</b> to display an error.</p>

<p id="demo"></p>

<script>
try {
  adddlert("Welcome guest!");
}
catch(err) {
  document.getElementById("demo").innerHTML = err.message;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179418139-03d99032-7c1d-4333-97e3-ab2dd569a4ad.png)

#### The finally Statement

> The finally statement lets you execute code, after try and catch, regardless of the result.

``` JS
try {
  Block of code to try
}
catch(err) {
  Block of code to handle errors
}
finally {
  Block of code to be executed regardless of the try / catch result
}
```
#### Example

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript try catch, finally</h2>

<script>
function get() {
  try {
    console.log("Inside try");
    throw new Error("Return error");
    return 10;
  } catch(e){
    console.log("Inside catch");
    return 20
  } finally{
    console.log("Inside finally");
    return 30;
  }
  
  console.log("Outside try...catch...finally");
  return 40;
}

console.log("The value is ", get());
</script>

</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/179418451-2bae59de-28e4-4336-9d7f-3e90f90f2dfb.png)

#### Error Name Values
![image](https://user-images.githubusercontent.com/75599178/179418506-f7e2e90d-fb7a-4cf1-bfc8-7432ace8326d.png)

#### Error Name Values
#### <li> Range Error</li>

> A RangeError is thrown if you use a number that is outside the range of legal values.

**Example**

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Errors</h2>

<p>You cannot set the number of significant digits of a number to 500:</p>

<p id="demo">

<script>
let num = 1;
try {
  num.toPrecision(500);
}
catch(err) {
  document.getElementById("demo").innerHTML = err.name;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179418660-188cb5f4-14b1-45d8-8bea-d97502edfa49.png)

#### <li>Reference Error</li>

> A ReferenceError is thrown if you use (reference) a variable that has not been declared.

**Example**

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Errors</h2>

<p>You cannot use the value of a non-existing variable:</p>

<p id="demo"></p>

<script>
let x = 5;
try {
  x = y + 1;
}
catch(err) {
  document.getElementById("demo").innerHTML = err.name;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179418748-dc51e416-9b07-4f01-9e4f-4427f9635dae.png)

#### <li>Syntax Error</li>

> A SyntaxError is thrown if you try to evaluate code with a syntax error..

**Example**

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Errors</h2>

<p>You cannot evaluate code that contains a syntax error:</p>

<p id="demo"></p>

<script>
try {
  eval("alert('Hello)");
}
catch(err) {
  document.getElementById("demo").innerHTML = err.name;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179419051-e4df82b1-bb26-454a-b307-66eba6f01f76.png)

#### <li>Type Error</li>

> A TypeError is thrown if you use a value that is outside the range of expected types.

**Example**

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Errors</h2>

<p>You cannot convert a number to upper case:</p>

<p id="demo"></p>

<script>
let num = 1;
try {
  num.toUpperCase();
}
catch(err) {
  document.getElementById("demo").innerHTML = err.name;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179419155-b36b5527-ebd2-4638-9976-347693e4ce41.png)

#### <li>URI (Uniform Resource Identifier) Error</li>

> A URIError is thrown if you use illegal characters in a URI function.

**Example**

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Errors</h2>

<p>Some characters cannot be decoded with decodeURI():</p>

<p id="demo"></p>

<script>
try {
  decodeURI("%%%");
}
catch(err) {
  document.getElementById("demo").innerHTML = err.name;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179419212-5778fe2f-e791-49b1-913e-35644ec0b171.png)

</details>

### Hoisting

<details>
  <summary>:bulb:</summary>

> Hoisting is the default behaviour of moving all the declarations at the top of the code before the code execution. <br> Declaration -> Initialisation/Agreement -> Usage

**Example**

``` JS
<!DOCTYPE html>
<html>
<body>

<p id="demo"></p>

<script>
var x; // Declare x
x = 5; // Assign 5 to x

elem = document.getElementById("demo"); // Find an element 
elem.innerHTML = x;           // Display x in the element
</script>

</body>
</html> 

``` 
![image](https://user-images.githubusercontent.com/75599178/179448533-a85307c1-196f-4e59-8bf4-03d5f9f45b4e.png)
  
**The let and const Keywords**

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Hoisting</h2>
<p>With <b>let</b>, you cannot use a variable before it is declared.</p>
<p id="demo"></p>

<script>
try {
  carName = "Saab";
  let carName = "Volvo";
}
catch(err) {
  document.getElementById("demo").innerHTML = err;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179449353-1095b809-7361-4467-8915-4857344a2d96.png)

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Hoisting</h2>

<p>With <b>const</b>, you cannot use a variable before it is declared.</p>
<p>Try to remove the //.</p>

<p id="demo"></p>

<script>
carName = "Volvo";
//const carName;
document.getElementById("demo").innerHTML = carName;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179449390-e9ed5092-49e5-4960-a956-ab41b2ad655d.png)
![image](https://user-images.githubusercontent.com/75599178/179449428-feb20081-016c-4626-8f38-a66be6c667ca.png)

</details>  
 

### this Keyword

<details>
  <summary>:bulb:</summary>  

#### What is **this**?  
<li>In JavaScript, the this keyword refers to an object.</li>
<li>Which object depends on how this is being invoked (used or called).</li>

![image](https://user-images.githubusercontent.com/75599178/179461499-22a16619-c940-478a-8d75-087eb8ccef26.png)

#### <li>this in a Method</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h1>The JavaScript <i>this</i> Keyword</h1>
<p>In this example, <b>this</b> refers to the <b>person</b> object.</p>
<p>Because <b>fullName</b> is a method of the person object.</p>

<p id="demo"></p>

<script>
// Create an object:
const person = {
  firstName: "John",
  lastName: "Doe",
  id: 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};

// Display data from the object:
document.getElementById("demo").innerHTML = person.fullName();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179463005-9ad85d5c-9df0-4c79-b1c3-fa824bea277f.png)

#### <li>this Alone</li>

``` JS
<!DOCTYPE html>
<html>
<body>

<h1>The JavaScript <i>this</i> Keyword</h1>

<p>In this example, <b>this</b> refers to the window object:</p>

<p id="demo"></p>

<script>
let x = this;
document.getElementById("demo").innerHTML = x;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179463201-250b86d7-27d6-4991-a6fe-9678b32c363e.png)

#### <li>this in a Function (Default)</li>

> In a function, the global object is the default binding for this. <br> In a browser window the global object is [object Window]

``` JS
<!DOCTYPE html>
<html>
<body>

<h1>The JavaScript <i>this</i> Keyword</h1>

<p>In a function, by default, <b>this</b> refers to the global object.</p>

<p>Strict mode does not allow default binding, so <b>this</b> is:</p>
<p id="demo"></p>

<script>
"use strict";
document.getElementById("demo").innerHTML = myFunction();

function myFunction() {
  return this;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179483130-193cfeb3-ffd9-4a05-a210-2b78a99a1928.png)

#### <li>this in a Function (Strict)</li>

> JavaScript strict mode does not allow default binding. <br> So, when used in a function, in strict mode, this is undefined.

``` JS
<!DOCTYPE html>
<html>
<body>

<h1>The JavaScript <i>this</i> Keyword</h1>

<p>In a function, by default, <b>this</b> refers to the global object.</p>

<p>Strict mode does not allow default binding, so <b>this</b> is:</p>
<p id="demo"></p>

<script>
"use strict";
document.getElementById("demo").innerHTML = myFunction();

function myFunction() {
  return this;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179483524-ec4334ff-5635-42cb-bc06-6d4540bac42f.png)


#### <li>this in Event Handlers</li>

> In HTML event handlers, this refers to the HTML element that received the event.

``` JS
<!DOCTYPE html>
<html>
<body>

<h1>The JavaScript <i>this</i> Keyword</h1>

<button onclick="this.style.display='none'">Click to Remove Me!</button>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179483831-47a7e869-d582-4050-b9df-b3693d1102ed.png)

#### <li>Function Borrowing</li>

> With the bind() method, an object can borrow a method from another object.

``` JS
<!DOCTYPE html>
<html>
<body>

<h1>JavaScript Function bind()</h1>

<p>This example creates 2 objects (person and member).</p>
<p>The member object borrows the fullname method from person:</p> 

<p id="demo"></p>

<script>
const person = {
  firstName:"John",
  lastName: "Doe",
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
}

const member = {
  firstName:"Hege",
  lastName: "Nilsen",
}

let fullName = person.fullName.bind(member);

document.getElementById("demo").innerHTML = fullName();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179484295-8572d5da-d774-4b86-9d77-9cfb56b110d1.png)

</details>  
  
 ### Function

<details>
  <summary>:bulb:</summary>

> JavaScript functions are defined with the function keyword. <br> You can use a function declaration or a function expression.

#### <li>Function Declarations</li>

**syntax**

``` JS
function functionName(parameters) {
  // code to be executed
}
```
**Example**
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>

<p>This example calls a function which performs a calculation and returns the result:</p>

<p id="demo"></p>

<script>
var x = myFunction(4, 3);
document.getElementById("demo").innerHTML = x;

function myFunction(a, b) {
  return a * b;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179511570-ff54cde6-a489-4054-9c38-12df708f0c19.png)

#### <li>Function() Constructor</li>

> Functions can also be defined with a built-in JavaScript function constructor called Function().

**Example**
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>
<p>JavaScript has an built-in function constructor.</p>
<p id="demo"></p>

<script>
const myFunction = new Function("a", "b", "return a * b");
document.getElementById("demo").innerHTML = myFunction(4, 3);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179512540-30ac49b2-eb42-43ab-ac6a-cfb4f4174a13.png)

#### <li>Function Hoisting</li>  
> JavaScript functions can be called before they are declared .
**Example**
``` JS
myFunction(5);

function myFunction(y) {
  return y * y;
}
``` 
#### <li>Arguments length</li>  

``` JS
<!DOCTYPE html>
<html>
<body>

<p>The arguments.length property returns the number of arguments received by the function:</p>

<p id="demo"></p>

<script>
function myFunction(a, b) {
  return arguments.length;
}
document.getElementById("demo").innerHTML = myFunction(4, 3);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179513546-c7343bfb-491b-4140-af84-123ae19b7d26.png)

#### <li>Arrow Functions</li>  

> Arrow functions allows a short syntax for writing function expressions. <br> You don't need the function keyword, the return keyword, and the curly brackets.

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Arrow Functions</h2>

<p>With arrow functions, you don't have to type the function keyword, the return keyword, and the curly brackets.</p>

<p>Arrow functions are not supported in IE11 or earlier.</p>

<p id="demo"></p>

<script>
const x = (x, y) => x * y;
document.getElementById("demo").innerHTML = x(5, 5);
</script>

</body>
</html>

```  
![image](https://user-images.githubusercontent.com/75599178/179515341-1caed37f-f2ef-4dcc-a5fd-94ff7abd04b1.png)
  
#### <li>Function Parameters</li>  

> Function parameters are the names listed in the function definition.<br> Function arguments are the real values passed to (and received by) the function.

``` JS
<!DOCTYPE html>
<html>
<body>

<p>Setting a default value to a function parameter (y=2).</p>
<p id="demo"></p>

<script>
function myFunction(x, y = 2) {
  return x * y;
}
document.getElementById("demo").innerHTML = myFunction(4);
</script>

</body>
</html>

```    
![image](https://user-images.githubusercontent.com/75599178/179516103-da616bc8-64df-4f2d-bb28-d79fb5a2636d.png)
  
#### <li>Function vs Method</li>  

Method : Method is a function when object is associated with it.
``` JS
var obj = {
name : "John snow",
work : function someFun(paramA, paramB) {
    // some code..
}
```
Function : When no object is associated with it , it comes to function.
``` JS
function fun(param1, param2){
// some code...
}
```  
#### <li>Method Reuse</li>    
With the call() method, you can write a method that can be used on different objects.

#### <li>The JavaScript call() Method</li>      
> The call() method is a predefined JavaScript method. <br> It can be used to invoke (call) a method with an owner object as an argument (parameter).  

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>
<p>This example calls the fullName method of person, using it on person1:
</p>

<p id="demo"></p>

<script>
const person = {
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
}
const person1 = {
  firstName:"John",
  lastName: "Doe"
}
const person2 = {
  firstName:"Mary",
  lastName: "Doe"
}
document.getElementById("demo").innerHTML = person.fullName.call(person1); 
</script>

</body>
</html>

```  
![image](https://user-images.githubusercontent.com/75599178/179524283-8bf717f0-e072-45fd-9f33-623c2a028609.png)

#### <li>The call() Method with Arguments</li>      
> The call() method is a predefined JavaScript method. <br> It can be used to invoke (call) a method with an owner object as an argument (parameter).  

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>
<p>This example calls the fullName method of person, using it on person1:
</p>

<p id="demo"></p>

<script>
const person = {
  fullName: function(city, country) {
    return this.firstName + " " + this.lastName + "," + city + "," + country;
  }
}

const person1 = {
  firstName:"John",
  lastName: "Doe"
}

const person2 = {
  firstName:"Mary",
  lastName: "Doe"
}

document.getElementById("demo").innerHTML = person.fullName.call(person1, "Oslo", "Norway"); 
</script>

</body>
</html>

```   
![image](https://user-images.githubusercontent.com/75599178/179525746-3d0c6fa5-37af-45b6-9e28-41dd18e15e59.png)
  
#### <li>JavaScript apply() Method</li>   
> The apply() method is similar to the call().

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>
<p>In this example the fulllName method of person is <b>applied</b> on person1:</p>

<p id="demo"></p>

<script>
const person = {
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
}

const person1 = {
  firstName:"John",
  lastName: "Doe"
}

document.getElementById("demo").innerHTML = person.fullName.apply(person1); 
</script>

</body>
</html>

```  
![image](https://user-images.githubusercontent.com/75599178/179528867-a61209ea-0ae7-4e97-b32b-f37154b20063.png)

#### <li>The Difference Between call() and apply()</li>   
> The call() method takes arguments separately.<br> The apply() method takes arguments as an array.

#### <li>The apply() Method with Arguments</li>   

**apply()**  

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>
<p>In this example the fulllName method of person is <b>applied</b> on person1:</p>

<p id="demo"></p>

<script>
const person = {
  fullName: function(city, country) {
    return this.firstName + " " + this.lastName + "," + city + "," + country;
  }
}

const person1 = {
  firstName:"John",
  lastName: "Doe"
}

document.getElementById("demo").innerHTML = person.fullName.apply(person1, ["Oslo", "Norway"]); 
</script>

</body>
</html>

```  
**call()**  
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>
<p>This example calls the fullName method of person, using it on person1:
</p>

<p id="demo"></p>

<script>
const person = {
  fullName: function(city, country) {
    return this.firstName + " " + this.lastName + "," + city + "," + country;
  }
}

const person1 = {
  firstName:"John",
  lastName: "Doe"
}

const person2 = {
  firstName:"Mary",
  lastName: "Doe"
}

document.getElementById("demo").innerHTML = person.fullName.call(person1, "Oslo", "Norway"); 
</script>

</body>
</html>

```  
![image](https://user-images.githubusercontent.com/75599178/179529878-83aab008-a9bc-4c76-a3a4-27cb66c8be92.png)


#### <li>Function bind()</li>

> With the bind() method, an object can borrow a method from another object.

``` JS
<!DOCTYPE html>
<html>
<body>

<h1>JavaScript Function bind()</h1>

<p>This example creates 2 objects (person and member).</p>
<p>The member object borrows the fullname method from person:</p> 

<p id="demo"></p>

<script>
const person = {
  firstName:"John",
  lastName: "Doe",
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
}

const member = {
  firstName:"Hege",
  lastName: "Nilsen",
}

let fullName = person.fullName.bind(member);

document.getElementById("demo").innerHTML = fullName();
</script>

</body>
</html>

```  
![image](https://user-images.githubusercontent.com/75599178/179568649-e7c964aa-28ba-4823-a1d4-76744b6a3091.png)

#### <li>JavaScript Closures</li>

> A closure is a function having access to the parent scope, even after the parent function has closed.

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Closures</h2>

<p>Counting with a local variable.</p>

<button type="button" onclick="myFunction()">Count!</button>

<p id="demo">0</p>

<script>
const add = (function () {
  let counter = 0;
  return function () {counter += 1; return counter;}
})();

function myFunction(){
  document.getElementById("demo").innerHTML = add();
}
</script>

</body>
</html>

``` 
![image](https://user-images.githubusercontent.com/75599178/179570301-458ba0b6-4824-4c0a-9dff-85b6a11ec623.png)

**Explanation for closure example**

> The variable add is assigned to the return value of a self-invoking function. <br> The self-invoking function only runs once. It sets the counter to zero (0), and returns a function expression. <br> This way add becomes a function. The "wonderful" part is that it can access the counter in the parent scope. <br> This is called a JavaScript closure. It makes it possible for a function to have "private" variables. <br> The counter is protected by the scope of the anonymous function, and can only be changed using the add function.
</details>
 
### Classes

<details>
  <summary>:bulb:</summary>
ECMAScript 2015, also known as ES6, introduced JavaScript Classes. <br> JavaScript Classes are templates for JavaScript Objects.

#### <li>Syntax</li>
``` JS
class ClassName {
  constructor() { ... }
}
```
#### <li>Example</li>
``` JS
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
}
```
#### <li>Example</li>
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Class</h2>

<p>How to use a JavaScript Class.</p>

<p id="demo"></p>

<script>
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
}

const myCar = new Car("Ford", 2014);
document.getElementById("demo").innerHTML =
myCar.name + " " + myCar.year;
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179571619-b1b6ba58-e5fb-492c-a0b9-73988e2d378d.png)

#### <li>Example</li>
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Class</h2>

<p>How to use a JavaScript Class.</p>

<p id="demo"></p>

<script>
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
}

const myCar = new Car("Ford", 2014);
document.getElementById("demo").innerHTML =
myCar.name + " " + myCar.year;
</script>

</body>
</html>

```
#### <li>The Constructor Method</li>
The constructor method is a special method:
    <li>It has to have the exact name "constructor"</li>
    <li>It is executed automatically when a new object is created</li>
    <li>It is used to initialize object properties</li>
If you do not define a constructor method, JavaScript will add an empty constructor method.

**Example**
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Class Method</h2>

<p>Pass a parameter into the "age()" method.</p>

<p id="demo"></p>

<script>
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
  age(x) {
    return x - this.year;
  }
}

let date = new Date();
let year = date.getFullYear();

let myCar = new Car("Ford", 2014);
document.getElementById("demo").innerHTML=
"My car is " + myCar.age(year) + " years old.";
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179572684-6c3a11c4-5643-47b8-bb6e-cd419ae681a2.png)

**Inheritance**
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Class Inheritance</h2>

<p>Use the "extends" keyword to inherit all methods from another class.</p>
<p>Use the "super" method to call the parent's constructor function.</p>

<p id="demo"></p>

<script>
class Car {
  constructor(brand) {
    this.carname = brand;
  }
  present() {
    return 'I have a ' + this.carname;
  }
}

class Model extends Car {
  constructor(brand, mod) {
    super(brand);
    this.model = mod;
  }
  show() {
    return this.present() + ', it is a ' + this.model;
  }
}

let myCar = new Model("Ford", "Mustang");
document.getElementById("demo").innerHTML = myCar.show();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179576241-08d52cd7-4ca9-4c8b-ad66-a882448d3d55.png)

</details > 

### Javascript Async

<details>
  <summary>:bulb:</summary>

### JS Callback
> A callback is a function passed as an argument to another function <br> This technique allows a function to call another function <br> A callback function can run after another function has finished

**Example**
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Function Sequence</h2>

<p>JavaScript functions are executed in the sequence they are called.</p>

<p id="demo"></p>

<script>
function myDisplayer(some) {
  document.getElementById("demo").innerHTML = some;
}

function myFirst() {
  myDisplayer("Hello");
}

function mySecond() {
  myDisplayer("Goodbye");
}

myFirst();
mySecond();
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179669951-697d0ca0-b5c1-48e9-8694-908f968b5e06.png)

**JavaScript Callbacks**

> A callback is a function passed as an argument to another function.

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Callbacks</h2>

<p>Do a calculation and then display the result.</p>

<p id="demo"></p>

<script>
function myDisplayer(something) {
  document.getElementById("demo").innerHTML = something;
}

function myCalculator(num1, num2, myCallback) {
  let sum = num1 + num2;
  myCallback(sum);
}

myCalculator(5, 5, myDisplayer);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179670745-a0e1d24c-6b46-4884-9305-abdfeb23a1a9.png) <br>
In the example above, myDisplayer is the name of a function. <br> It is passed to myCalculator() as an argument.

**When to Use a Callback?** <br>
*Where callbacks really shine are in asynchronous functions, where one function has to wait for another function (like waiting for a file to load).*

###JavaScript Promise 
>"Producing code" is code that can take some time <br> "Consuming code" is code that must wait for the result <br> A Promise is a JavaScript object that links producing code and consuming code.

**Syntax**

``` JS
let myPromise = new Promise(function(myResolve, myReject) {
// "Producing Code" (May take some time)

  myResolve(); // when successful
  myReject();  // when error
});

// "Consuming Code" (Must wait for a fulfilled Promise)
myPromise.then(
  function(value) { /* code if successful */ },
  function(error) { /* code if some error */ }
);
```

#### <li>Promise Object Properties</li>
A JavaScript Promise object can be:
   <li> Pending
   <li> Fulfilled
   <li> Rejected
<li> The Promise object supports two properties: state and result.
<li>While a Promise object is "pending" (working), the result is undefined.
<li>When a Promise object is "fulfilled", the result is a value.
<li>When a Promise object is "rejected", the result is an error object. 
    
#### <li>how to use a Promise</li>
``` JS
myPromise.then(
  function(value) { /* code if successful */ },
  function(error) { /* code if some error */ }
);
```
> Promise.then() takes two arguments, a callback for success and another for failure. <br> Both are optional, so you can add a callback for success or failure only.

**Example**
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Promise</h2>

<p id="demo"></p>

<script>
function myDisplayer(some) {
  document.getElementById("demo").innerHTML = some;
}

let myPromise = new Promise(function(myResolve, myReject) {
  let x = 0;

// some code (try to change x to 5)

  if (x == 0) {
    myResolve("OK");
  } else {
    myReject("Error");
  }
});

myPromise.then(
  function(value) {myDisplayer(value);},
  function(error) {myDisplayer(error);}
);
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179720882-d715c1d0-5741-4259-9ed4-00b28da250be.png)

#### <li>how to use a Promise</li>
<li>Waiting for a Timeout</li>
<li>Waiting for a File</li>
  
#### <li>Waiting for a Timeout</li>  

**Example Using Callback**

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript SetTimeout()</h2>

<p>Wait 3 seconds (3000 milliseconds) for this page to change.</p>

<h1 id="demo"></h1>

<script>
setTimeout(function() { myFunction("I love You !!!"); }, 3000);

function myFunction(value) {
  document.getElementById("demo").innerHTML = value;
}
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/179733552-366ad1b8-1922-430c-b95d-8bfed8920ed3.png)
  
**Example Using Promise**  
  
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Promise</h2>

<p>Wait 3 seconds (3000 milliseconds) for this page to change.</p>

<h1 id="demo"></h1>

<script>
const myPromise = new Promise(function(myResolve, myReject) {
  setTimeout(function(){ myResolve("I love You !!"); }, 3000);
});

myPromise.then(function(value) {
  document.getElementById("demo").innerHTML = value;
});
</script>

</body>
</html>


```  
![image](https://user-images.githubusercontent.com/75599178/179733724-3f535c3b-f19c-4f20-95bc-bc0326ea7705.png)
  
###Async/Await
> "async and await make promises easier to write" <br> async makes a function return a Promise <br> await makes a function wait for a Promise

**Async Syntax** 
``` JS
async function myFunction() {
  return "Hello";
}
```

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript async / await</h2>

<p id="demo"></p>

<script>
function myDisplayer(some) {
  document.getElementById("demo").innerHTML = some;
}

async function myFunction() {return "Hello";}

myFunction().then(
  function(value) {myDisplayer(value);},
  function(error) {myDisplayer(error);}
);</script>

</body>
</html>

```  
![image](https://user-images.githubusercontent.com/75599178/179738129-c011377d-75f1-4c69-a65c-333331d81133.png)
  
**Await Syntax** 
``` JS
let value = await promise;
``` 
 
``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript async / await</h2>

<h1 id="demo"></h1>

<script>
async function myDisplay() {
  let myPromise = new Promise(function(resolve, reject) {
    resolve("I love You !!");
  });
  document.getElementById("demo").innerHTML = await myPromise;
}

myDisplay();
</script>

</body>
</html>

```   
![image](https://user-images.githubusercontent.com/75599178/179738403-4de1eced-8336-4c78-9282-d3c1daba6691.png)

**Example**  

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript async / await</h2>

<p id="demo"></p>

<script>
async function getFile() {
  let myPromise = new Promise(function(resolve) {
    let req = new XMLHttpRequest();
    req.open('GET', "mycar.html");
    req.onload = function() {
      if (req.status == 200) {
        resolve(req.response);
      } else {
        resolve("File not Found");
      }
    };
    req.send();
  });
  document.getElementById("demo").innerHTML = await myPromise;
}

getFile();
</script>

</body>
</html>

```  
 ![image](https://user-images.githubusercontent.com/75599178/179738825-c2592de6-d1c9-4230-97eb-301cead3e1f2.png)
   
</details>  

# Interview Questions

### 1. What is javascript?
<details>
  <summary>:bulb:</summary>
   Javascript is the scripting challenge, It is light weight, object-oriented language. It is widely used in client-side validdation. 
</details>  
  
### 2. List some features of JavaScript.
<details>
  <summary>:bulb:</summary>
1. Light weight<br>
2. Opensource, cross-platform<br>
3. Interpreted programming challenge<br>
</details>  
  
### 3. Advantages and disadvantages.
<details>
  <summary>:bulb:</summary>

Advantages | Disadvantages
---------- | -------------
Server interaction less | No support for multi threading
Feedback to the visitors immediate | No support for multi processing
Interactive is high , Interfaces are rich | No dupport for networking applications.

</details>   

### 4. What are the different data types present in javascript?
<details>
  <summary>:bulb:</summary>  

There are two data types: <br>
  <li>Primitive type</li>
  <li>Non-Primitive type</li><br>

> Primitive data types can store only a single value. To store multiple and complex values, non-primitive data types are used.

**1.Primitive type** <br>

**String** => It represents a series of characters and is written with quotes. <br>
**Number** =>  It represents a number and can be written with or without decimals. <br>
**BigInt** => BigInt is a numeric data type that can represent integers in the arbitrary precision format.  <br>
**Boolean** =>  It represents a logical entity and can have only two values : true or false. <br>
**Undefined** => When a variable is declared but not assigned, it has the value of undefined <br>
**Null** => It represents a non-existent or a invalid value.<br>
**Symbol** => It is used to store an anonymous and unique value.<br>
![image](https://user-images.githubusercontent.com/75599178/179768514-d183dad1-7a43-4c48-8077-cb9b4d9038da.png)

**2. Non-primitive types** <br>

**Objects and Arrays**
![image](https://user-images.githubusercontent.com/75599178/179811971-9b39f364-72ed-443b-a2ab-82cbfa80d95a.png)

</details>  
  
### 5. Explain Hoisting in javascript.
<details>
  <summary>:bulb:</summary>    
  
Hoisting is the default behaviour of javascript where all the variable and function declarations are moved on top.

**Examples:**<br>

![image](https://user-images.githubusercontent.com/75599178/179813267-a4df0302-1300-4447-9a5d-f654a8e182c8.png)
![image](https://user-images.githubusercontent.com/75599178/179813337-9b2d60d6-e523-4e56-932c-09fb9e1992cf.png)

</details>  
 
### 6. Define named function in javascript.
<details>
  <summary>:bulb:</summary>    
  
The function which has named at the time of definition is called a named function.

``` JS
function msg()  
{  
  document.writeln("Named Function");  
}  
msg();  
```

</details>  
 
### 7. Define named anonymous function in javascript.
<details>
  <summary>:bulb:</summary>    
  
The function which has no name. These functions are declared dynamically at runtime using the function operator instead of the function declaration.

``` JS
var display=function()  
{  
  document.writeln("Anonymous Function");  
}  
display();  
```

</details>  

### 8. Define closure.
<details>
  <summary>:bulb:</summary>    
  
In JavaScript, we need closures when a variable which is defined outside the scope in reference is accessed from some inner scope. <br>

JavaScript variables can belong to the local or global scope.<br>

Global variables can be made local (private) with closures.

``` JS
A function can access all variables defined inside the function(a is a local variable.), like this:<br>

function myFunction() {
  let a = 4;
  return a * a;
}

But a function can also access variables defined outside the functiona is a global variable., like this:<br>
let a = 4;
function myFunction() {
  return a * a;
}
```

</details>  

### 9. Difference between “ == “ and “ === “ operators.
<details>
  <summary>:bulb:</summary>    
 
*The difference between both the operators is that “==” is used to compare values whereas, “ === “ is used to compare both values and types.*  
![image](https://user-images.githubusercontent.com/75599178/179813989-5d2686a6-045a-4d06-bde4-d80acce593e7.png)
  
</details>    
  
### 10. Difference between var and let keyword in javascript.
<details>
  <summary>:bulb:</summary>      
  
![image](https://user-images.githubusercontent.com/75599178/179814535-8229418e-0492-4ed5-bd3e-17b2a486c7df.png)
  
</details>     
  
### 11. Is javascript a statically typed or a dynamically typed language?  
<details>
  <summary>:bulb:</summary>    

JavaScript is a dynamically typed language.  
Variables in JS are not associated with any type.<br> A variable can hold the value of any data type. 
</details>     
  
###  12. What is NaN property in JavaScript?  
<details>
  <summary>:bulb:</summary>    

*NaN property represents the “Not-a-Number” value. It indicates a value that is not a legal number.*
![image](https://user-images.githubusercontent.com/75599178/179816562-24639335-edf5-4364-b474-35a06e0f1966.png)
  
</details>   

###  12. How to use external Javascript file? 
<details>
  <summary>:bulb:</summary>    
  I'm assuming that js file name is message.js, place the following script tag inside the head tag.

``` JS
<script type="text/javascript" src="message.js"></script>  
```
</details>   

###  13. Is JavaScript case sensitive language? 
<details>
  <summary>:bulb:</summary>    
  Yes, JavaScript is a case sensitive language. For example:

``` JS
Var msg = "JavaScript is a case-sensitive language"; //Here, var should be used to declare a variable  
function display()   
{  
document.writeln(msg); // It will not display the result.  
}   
display();  

Above code is executed as error. But if we modify "Var" to "var" it gives result.
```
</details>   	
	
###  14. What is BOM? 
<details>
  <summary>:bulb:</summary>    
  The Browser Object Model in js includes the properties and methods for js to interact with the web browser.<br>
BOM provides you a window objecs, for example to show the width and height of the window.It also includes the window.screen object to show the width and height of the scrreen.

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Window</h2>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML =
"Browser inner window width: " + window.innerWidth + "px<br>" +
"Browser inner window height: " + window.innerHeight + "px";
</script>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/186610812-2e5a1c82-19af-4f9e-a7ea-cc3d55df2979.png)

</details>  	
	
###  15. Is JavaScript case sensitive language? 
<details>
  <summary>:bulb:</summary>    
  Yes, JavaScript is a case sensitive language. For example:

``` JS
Var msg = "JavaScript is a case-sensitive language"; //Here, var should be used to declare a variable  
function display()   
{  
document.writeln(msg); // It will not display the result.  
}   
display();  

Above code is executed as error. But if we modify "Var" to "var" it gives result.
```
![image](https://user-images.githubusercontent.com/75599178/186611066-b5022092-7fb3-4e03-86c6-20f8361689d0.png)

</details>	
	
	
###  16. How to write a comment in JavaScript?
<details>
  <summary>:bulb:</summary>    
1. Single Line Comment: It is represented by // (double forward slash)<br>
2. Multi-Line Comment: Slash represents it with asterisk symbol as /* write comment here */

</details>	
		
###  17. How to create a function in JavaScript?
<details>
  <summary>:bulb:</summary>    
To create a function in JavaScript, follow the following syntax.

``` JS
function function_name(){  
//function body  
}  
```
</details>	
	
	
### 18. Explain passed by value and passed by reference.  
<details>
  <summary>:bulb:</summary>  
    
*In JavaScript, primitive data types are passed by value and non-primitive data types are passed by reference.*  <br>

![image](https://user-images.githubusercontent.com/75599178/179817006-4c72569b-b919-46f7-8b58-6fa7038885e4.png)

 In above example, variable y is directly assigned, but z is not like that. It returns only by memory. 
</details>  
  
### 19. What do you mean by strict mode in javascript and characteristics of javascript strict-mode?
<details>
  <summary>:bulb:</summary> 

*Strict Mode is a feature in JavaScript that was introduced in ECMAScript 5. It eliminates some JavaScript silent errors by changing them to throw errors.*  
 
Characteristics of strict mode in javascript:
<li>The 'use strict' keyword is used to define strict mode at the start of the script. Strict mode is supported by all browsers.</li>
<li>Duplicate arguments are not allowed by developers.</li> 
</details>   
  
### 20. Explain First class function & Higher Order Functions in javascript.
<details>
  <summary>:bulb:</summary> 

#### <li>First class function</li>
*A programming language said to have if first class function can be treated like other variable, and also  can be passed as an argument or returned by another functions.*

``` JS
<!DOCTYPE html>
<html>
<body>

<script>
const Arithmetics = {
	add:(a, b) => {
		return `${a} + ${b} = ${a+b}`;
	},
	subtract:(a, b) => {
		return `${a} - ${b} = ${a-b}`
	},
	multiply:(a, b) => {
		return `${a} * ${b} = ${a*b}`
	},
	division:(a, b) => {
		if(b!=0) return `${a} / ${b} = ${a/b}`;
		return `Cannot Divide by Zero!!!`;
	}

}

console.log(Arithmetics.add(100, 100));
console.log(Arithmetics.subtract(100, 7));
console.log(Arithmetics.multiply(5, 5));
console.log(Arithmetics.division(100, 5));

</script>

</body>
</html> 

```
![image](https://user-images.githubusercontent.com/75599178/179897996-41aa52f2-fdee-4f5a-841c-6409eaab0860.png)

  #### <li>Higher Order Functions</li>
*Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.*

``` JS
<!DOCTYPE html>
<html>
<body>

<h2>My First Web Page</h2>
<p>My First Paragraph.</p>

<p id="demo"></p>

<script>
function greet(name){
	return `Hi!! ${name} `;
}

function greet_name(greeting,message,name){
	console.log(`${greeting(name)} ${message}`);
}

greet_name(greet,'Welcome To GeeksForGeeks','JavaScript');

</script>

</body>
</html> 

```  
![image](https://user-images.githubusercontent.com/75599178/179898208-465fcc9e-42c2-4efd-9986-636b738fb9f9.png)

**<li>Key Differences between First-Order Function and Higher-Order Function:-</li>**

First-Order Function | Higher-Order Function
-------------------- | ---------------------
Function are treated as a variable that can be assigned to any other variable or passed as an argument. | Function receives another function as an argument or returns First-order a new function or both.
The “first-class” concept only has to do with functions in programming languages. | The “higher-order” concept can be applied to functions in general, like functions in the mathematical sense.
The presence of the First-class function implies the presence of a higher-order function. | The presence of a Higher-order function does not imply the presence of a First-order function.
</details>  

### 21. What does isNaN() function?
<details>
  <summary>:bulb:</summary> 
The isNaN() returns true if the variable value is not anumber.

``` JS
function number(num) {  
  if (isNaN(num)) {  
    return "Not a Number";  
  }  
  return "Number";  
}  
console.log(number('1000F'));  
// expected output: "Not a Number"  
  
console.log(number('1000'));  
// expected output: "Number"  
```
![image](https://user-images.githubusercontent.com/75599178/186629057-ba008784-41ff-4d0b-aa03-07b91deca91b.png)

</details>  
  
### 22. Difference between Client side JavaScript and Server side JavaScript?
<details>
  <summary>:bulb:</summary> 

**Client-side Javascript** an extended version of JS that enables the enhancement and manipulation of client browsers and web ages.
**Server-side Javascript** an extended version of JS that enables the backend access to databases , file systems and servers..
</details>    
  
  
### 23. Difference between event.preventDefault() and event.stopPropagation() methods in JavaScript?
<details>
  <summary>:bulb:</summary> 

**preventDefault** Prevents the default browser behaviour for a given element.<br>
**stopPropagation** stops an event from bubbling or propagating up the dom tree.<br>
**For example:** If you use it in a form element, it prevents it from submitting. If used in an anchor element, it prevents it from navigating. If used in a contextmenu, it prevents it from showing or displaying.

On the other hand, the event.stopPropagation() method is used to stop the propagation of an event or stop the event from occurring in the bubbling or capturing phase.
</details>     
  
### 24. Difference  between undefined value and null value?
<details>
  <summary>:bulb:</summary> 

**Undefined value** A value that is not defined and has no keyword is known as undefined value.<br>
**Null value** A value that explicitly specified by the keyword "null" is known as null value.<br>

</details>     
  
### 25.  How to set the cursor to wait in JavaScript?
<details>
  <summary>:bulb:</summary> 

``` JS
<script>
window,document.body.style.cursor = "wait"
</script>
```
</details>  
  
### 26.  What is negative infinity?
<details>
  <summary>:bulb:</summary> 
Negative infinity is anumber in JS which is derived by dividing the negative number by the zero.

``` JS
<script>
var num=-5;  
function display()  
{  
  document.writeln(num/0);  
}  
display();  
//expected output: -Infinity  
</script>
```
</details>  
    
### 27.  What are the pop-up boxes available in javascript?
<details>
  <summary>:bulb:</summary> 

1. Alert box <br>
2. Prompt box <br>
3. Confirm box

``` JS
/*alert => shows a message. */
<script type="text/javascript">  
function msg(){  
 alert("Hello Alert Box");  
}  
</script>  
<input type="button" value="click" onclick="msg()"/>  

```
![image](https://user-images.githubusercontent.com/75599178/186677982-bd22fb57-9954-4cb7-ae9e-2bea481cd5f5.png)


``` JS
/* prompt => shows a message asking the user to input text. */
<script type="text/javascript">  
function msg(){  
var v= prompt("Who are you?");  
alert("I am "+v);  
  
}  
</script>  
  
<input type="button" value="click" onclick="msg()"/>  

```
![image](https://user-images.githubusercontent.com/75599178/186677500-55e5c107-6a1f-4bb8-9f8f-409522eee238.png)

![image](https://user-images.githubusercontent.com/75599178/186677590-761a9a9f-3fd7-46a6-82d8-f02ce0cf4bbc.png)

``` JS
/* prompt => shows a message asking the user to input text. */
<script type="text/javascript">  
function msg(){  
var v= confirm("Are u sure?");  
if(v==true){  
alert("ok");  
}  
else{  
alert("cancel");  
}  
  
}  
</script>  
  
<input type="button" value="delete record" onclick="msg()"/>

```
![image](https://user-images.githubusercontent.com/75599178/186677761-4f16e37e-d877-4e9d-bade-e48964b86852.png)

![image](https://user-images.githubusercontent.com/75599178/186677827-7fd0a182-fc28-49d9-9cba-a6e9dae9441a.png)

</details>  
      
### 28.  How to submit a form using JavaScript by clicking a link?
<details>
  <summary>:bulb:</summary> 

``` JS
<!DOCTYPE html>
<html>

<body>
	<h2 style="color:green">GeeksforGeeks</h2>
	<b>Submit form details</b>

	<form id="form__submit" action="form.php" method="post">
		<label>NAME: </label><br />
		<input type="text" name="name" /><br />
		<label>AGE: </label><br />
		<input type="number" name="age" /><br />
		<label>CITY: </label><br />
		<input type="text" name="city" /><br /><br />
		<a href="#" onclick="submitForm()">Submit Here</a>
	</form>

	<script>
		function submitForm() {
			let form = document.getElementById("form__submit");
			form.submit();
		}
	</script>
</body>

</html>

```
</details>    
	
### 29.  How to validate a form in JavaScript?
<details>
  <summary>:bulb:</summary> 

``` JS
<script>
<html>
<body>
<script>  
function validateform(){  
var name=document.myform.name.value;  
var password=document.myform.password.value;  
  
if (name==null || name==""){  
  alert("Name can't be blank");  
  return false;  
}else if(password.length<6){  
  alert("Password must be at least 6 characters long.");  
  return false;  
  }  
}  
</script>  
<body>  
<form name="myform" method="post" action="http://www.javatpoint.com/javascriptpages/valid.jsp" onsubmit="return validateform()" >  
Name: <input type="text" name="name"><br/>  
Password: <input type="password" name="password"><br/>  
<input type="submit" value="register">  
</form>  
</body>
</html>

 

</script>
```
</details> 	
	
### 30.  How to submit a form using JavaScript by clicking a link?
<details>
  <summary>:bulb:</summary> 

``` JS
<!DOCTYPE html>
<html>

<body>
	<h2 style="color:green">GeeksforGeeks</h2>
	<b>Submit form details</b>

	<form id="form__submit" action="form.php" method="post">
		<label>NAME: </label><br />
		<input type="text" name="name" /><br />
		<label>AGE: </label><br />
		<input type="number" name="age" /><br />
		<label>CITY: </label><br />
		<input type="text" name="city" /><br /><br />
		<a href="#" onclick="submitForm()">Submit Here</a>
	</form>

	<script>
		function submitForm() {
			let form = document.getElementById("form__submit");
			form.submit();
		}
	</script>
</body>

</html>

```
</details>    
	
### 31.  What is this keyword in JavaScript?
<details>
  <summary>:bulb:</summary> 
The this keyword is a reference variable that refers to the current object.

``` JS
<script>
<html>
<body>
<script>  
var address=    
{    
company:"Javatpoint",    
city:"Noida",    
state:"UP",    
fullAddress:function()    
{    
return this.company+" "+this.city+" "+this.state;    
}    
};    
var fetch=address.fullAddress();    
document.writeln(fetch);   

</script>
```
</details> 
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
  
  
  
