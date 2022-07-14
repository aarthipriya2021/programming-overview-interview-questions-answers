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
![image](https://user-images.githubusercontent.com/75599178/178327727-b2b74e27-7fa9-4c58-a2de-ea9061e04631.png)

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



