# Overview

### What is Sass?

<details>
  <summary>:bulb:</summary>
 <li>Sass stands for Syntactically Awesome Stylesheet</li>
 <li>Sass is an extension to CSS</li>
 <li>Sass is a CSS pre-processor</li>
 <li>Sass stands for Syntactically Awesome Stylesheet</li>
 <li>Sass is completely compatible with all versions of CSS</li>
 <li>Sass reduces repetition of CSS and therefore saves time</li>
 <li>Sass is free to download and use</li>
</details>

### Why Use Sass?
<details>
  <summary>:bulb:</summary>
  
<li>It is easy, short and clean in a programming construct.</li>
<li>It contains all the features of CSS along with some advance features.</li>
<li>don't need to repeat similar CSS again and again in your project.</li>
</details>

### Sass vs scss
<details>
  <summary>:bulb:</summary>
  
![image](https://user-images.githubusercontent.com/75599178/174654405-8209e133-4386-4baa-8e73-bea84ad55c69.png)
</details>

### Sass install
<details>
  <summary>:bulb:</summary>
  * Sass for html page we have to add vscode extension which is sass live compiler.

  * To start, create a folder with two folders inside, CSS and images. Then inside the CSS folder create a file with the Sass extension (style.scss)in my case it's style.scss.

  * Then open it and the file will be detected right away. Below the editor a button will appear named Watch Sass. Just click on it to tell Sass to watch this file and start generating (compiling) code in the CSS file.

  * Once SASS finishes compiling it will create three files in the project's CSS folder: style.css, style.scss, and style.css.map. It tracks all the changes and it is ready to generate CSS code.

  * Then , we will link our CSS file in the index.html file.
  
For reference, visit https://www.youtube.com/watch?v=Zz6eOVaaelI.
``` css
<link rel="stylesheet" href="css/style.css">
 ```
</details>

### Example

<details>
  <summary>:bulb:</summary>
  
![image](https://user-images.githubusercontent.com/75599178/174790669-6cbb8473-dd03-4040-852b-823bedd762ad.png)

``` html
<!-- index.html -->  
  
  
<!DOCTYPE html>
<html lang="en">
<head>
      <meta charset="UTF-8">
      <meta http-equiv="X-UA-Compatible" content="IE=edge">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <link rel="stylesheet" href="css/style.css">
      <title>SASS Tutorial</title>
</head>
<body>
      <header>
            <h1>WELCOME</h1>
            <button>Add Details</button>
      </header>
      <div class="contact">
            
            <div class="info">
                  <h1>Contact Info</h1>
                  <p>This is the page to show the contacts.</p>
                  <button>Details</button>
            </div>
      </div>
</body>
</html>

```
``` css 
/* style.css */
  
  
header {
  margin: 2rem 2rem 2rem 50rem;
  display: flex;
  justify-content: center;
  color: rgb(58, 42, 42);
}
header button {
  background: rgb(56, 146, 142);
}
header button:hover {
  background: red;
}

body {
  background-color: #ab99ca;
  padding: 2rem;
  min-height: 100vh;
  align-items: center;
}
body .contact button {
  background: rgb(58, 148, 90);
}
/*# sourceMappingURL=style.css.map */
  
```
  
 ```css 
  
/* style.css.map */
  
{"version":3,"sources":["style.scss","style.css"],"names":[],"mappings":"AAMA;EACI,4BAAA;EACA,aAAA;EACA,uBAAA;EACA,sBANU;ACCd;ADMI;EACI,6BATM;ACKd;ADKQ;EACI,eAAA;ACHZ;;ADOA;EACI,yBAAA;EACA,aAAA;EACA,iBAAA;EACA,mBAAA;ACJJ;ADKI;EACI,4BAAA;ACHR","file":"style.css"}
  
```
```css 
 /* style.scss */


$primaryBtn : rgb(56, 146, 142);
$textColor  : rgb(58, 42, 42);

header{
    margin: 2rem 2rem 2rem 50rem;
    display: flex;
    justify-content: center;
    color: $textColor;
    button {
        background: $primaryBtn;
        &:hover {
            background: red;
        }
    }
}
body {
    background-color: #ab99ca;
    padding: 2rem;
    min-height: 100vh;
    align-items: center;
    .contact button {
        background: rgb(58, 148, 90);
    }
}
```
Interface will be :

![image](https://user-images.githubusercontent.com/75599178/174791880-5ded9321-c8a2-43b3-882f-9c10bf956fe7.png)
</details>

# Topics

### Variables

<details>
  <summary>:bulb:</summary>
  
> Sass variables are used to store information that can be reused throughout the stylesheet when you need. You can store things like colors, font stacks, or any CSS value according to your future reusability.  ** The $ symbol is used to make something a variable. **
``` css
$pageColor: rgb(178, 224, 197);
$fontFamily: Helvetica, sans-serif;
$fontColor:rgb(12, 62, 136);

body{
    background: 100% $pageColor;
    font-family: $fontFamily;
    color: $fontColor;
}
```
</details>

### Opertors
<details>
  <summary>:bulb:</summary>  

### 1) Assignment Operator

In Sass, the colon ( : ) operator is used to define a variable.

``` css
$main-color: lightpink;   
```
### 2) Arithmetic Operators
![image](https://user-images.githubusercontent.com/75599178/175319917-76eff30a-41ff-4453-ac39-074a3a87b9c1.png)
``` css

h2 {  
    font-size: 15px + 2em; // Show error due to incompatible units  
    font-size: 15px + 2; // 17px  
} 
2)Multiplication of two numbers of the same unit is not valid CSS:

h2 {  
    font-size: 5px * 2px; // invalid CSS  
}  
3)The division operator is an integral part of the CSS shorthand properties.

font: 16px / 24px Arial sans-serif;  
background: url("http://example.com") no-repeat fixed center / cover;   

h2 {  
    font-size: 16px / 24px // Outputs as CSS  
    font-size: (16px / 24px) // Uses parentheses, does division  
    font-size: #{$base-size} / #{$line-height}; // Uses interpolation, outputs as CSS  
    font-size: $base-size / $line-height // Uses variables, does division  
    opacity: random(4) / 5; // Uses a function, does division  
    padding-right: 2px / 4px + 3px // Uses an arithmetic expression, does division  
}  

```
</details>

### @-Rules and Directives

<details>
  <summary>:bulb:</summary>
A list of all the rules and directives used in Sass are given 

![image](https://user-images.githubusercontent.com/75599178/175326333-78f1998f-b850-4003-8fbf-2c90e08a913b.png)

![image](https://user-images.githubusercontent.com/75599178/175326411-335ee2ea-16df-4586-8093-316f5439556d.png)

### @import 

> CSS provides @import option that makes you able to split your CSS into smaller, more maintainable portions. 

> for Example we dont need to change anything related scss for after watching scss ... 
``` scss
// _component.scss

html,  
body,  
ul,  
ol {  
   margin: 0;  
  padding: 0;  
} 
// --------------------------------------------------------------------------------------

// style.scss (main sass file)

@import "./component";

body {  
    font: 100% Helvetica, sans-serif;  
    background-color: #419453;  
}  
```

### @media
> Sass @media directive is used to set style rules to different media types. 

> The Sass @media directive can be nested inside the selector SASS but the main impact is displayed to the top level of the stylesheet.
``` scss
// style.scss
h1,h3{  
    color: rgb(182, 68, 182);  
}  
.style{  
    width: 500px;  

    @media screen and (orientation: portrait){  
        width:200px;  
        margin-left: 80px;  
    }  
}  
```
### @extend
> Sass, @extend is used to share a set of CSS properties from one selector to another. It is a very important and useful feature of Sass.

``` scss
// style.scss
.message {  
    border: 1px solid #ccc;  
    padding: 10px;  
    color: #333;  
  }  
  .success {  
    @extend .message;  
    border-color: green;  
  }  
  .error {  
    @extend .message;  
    border-color: red;  
  }  
  .warning {  
    @extend .message;  
    border-color: yellow;  
  } 
```

### @at-root
> Sass @at-root directive is a collection of nested rules that are used to style block at the root of the document.

> syntax
``` scss
  @at-root (without: ...) and @at-root (with: ...)   
```

``` scss

// style.scss
h1, h3{  
    color: blue;  
    background-color: pink;  

    @at-root {  
        .style{  
        font-size: 20px;  
        font-style: bold;  
        color: violet;  
        }  
     }  
}
```

### @debug 

> Sass @debug directive is used to detect the errors and display the SassScript expressions values to the standard error output stream.

``` scss

// style.scss

$font-sizes: 10px + 20px;  
$style: (  
  color: #bdc3c7  
);  
.container{  
  @debug $style;  
  @debug $font-sizes;  
}  
```
### @warn 

> Sass @warn directive is used when you get a problem and want to give a cautionary advice to the users. It displays the value of a SassScript expression to the standard error output stream.

> There are two specific differences between @warn and @debug:
<li>Warning can be turned off with the --quiet command-line option or the: quiet Sass option.</li>
<li>Sass @warn directive provides a printed output along with the message so that the user being warned where the warning is occurred.</li>

``` scss

// style.scss
$main-color:  #bdc3c7;  
@warn "Darker: " darken($main-color, 30%);  
```

### @error 

> Sass @error directive is used when you want to display errors. It displays the SassScript expression values as fatal error including a nice stack trace.

``` scss

// style.scss
$colors: (  
  blue: #c0392b,  
  black: #2980b9,  
);  
@function style-variation($style) {  
  @if map-has-key($colors, $style) {  
    @return map-get($colors, $style);  
  }  
  @error "Invalid color: '#{$style}'.";  
}  
.container {  
  style: style-variation(white);  
}  
```
</details>


### Mixins

<details>
  <summary>:bulb:</summary>

> Mixins allow you to define styles that can be re-used throughout your stylesheet. Sass Mixins facilitates you to make groups of CSS declarations that you want to reuse repeatedly on your site.

> The mixin can store multiple values or parameters and call function to avoid writing repetitive codes. Mixin names can use underscores and hyphens interchangeably.

``` scss
// Example
@mixin border-radius($radius) {  
  -webkit-border-radius: $radius;  
     -moz-border-radius: $radius;  
      -ms-border-radius: $radius;  
          border-radius: $radius;  
}  
.box { @include border-radius(10px); }   
```
![image](https://user-images.githubusercontent.com/75599178/175813948-82eca641-59ef-472c-8767-47db1d74045e.png)

### Defining a Mixin

> The @mixin directive defines the mixins. It is used to include optionally the variables and arguments after the name of the mixin.
``` scss
@mixin style {  
  h1{  
   color: #FF0000 ;  
      }  
  }  
@include style;  
```

### Including a mixin

> The @include directive is used to include the style defined by the mixin into the document. The name of the mixin is taken and optional arguments are passed into it.
``` scss
@mixin style {  
  @mixin style {  
.container{  
 background-color: #77C1EF;  
 color: #ffffff;  
    }  
h3 {  
 color: #ffffff;  
 }  
}  
@include style;  
```

### Mixin arguments

> The mixin arguments are SassScript values that are passed when mixin is included and are available as variable.The argument is a name of a variable separated by a comma while defining a mixin. There are two types of mixin arguments in Sass.
<li>Keyword Arguments</li>
<li>Variable Arguments</li>

#### Keyword Arguments

> The keyword arguments are used to include in mixins. It specifies that the named arguments can be passed in any order and the default value of arguments can be omitted.|

``` scss
@mixin bordered($color, $width: 2px) {  
  color: #77C1EF;  
  border: $width solid black;  
  width: 500px;  
}  
.style  {  
  @include bordered($color:#77C1EF, $width: 5px);  
}   
```
<li>

#### Variable Argument
</li>

> The keyword arguments are used to include in mixins. It specifies that the named arguments can be passed in any order and the default value of arguments can be omitted.

``` scss
@mixin linear-gradient($direction, $gradients...) {  
  background-color: nth($gradients, 1);  
  background-image: linear-gradient($direction, $gradients...);  
}  
.style {  
  @include linear-gradient(to right, magenta, red, orange, yellow, green, blue, purple);  
}  
```
#### Passing content block to a mixin

> The content blocks are passed to the mixin for the placement inside the styles. This functionality is added in Sass version 3.2. Styles are included into the mixin in the @content directive location.

> The block of content is specified in the scope and the scope is passed in the mixin where block is defined.

``` scss
@mixin element{  
   @content;  
}  
@include element{  
  .block{  
    color: blue;  
  }  
 }   
```
</details>






















# Practice

<details>
  <summary>:bulb:</summary>
  
> Initial stage  
> Switch the watch sass in task bar of vscode.  

``` html
  <!DOCTYPE html>
<html lang="en">
<head>
      <meta charset="UTF-8">
      <meta http-equiv="X-UA-Compatible" content="IE=edge">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <link rel="stylesheet" href="css/style.css">
      <title>SASS Tutorial</title>
</head>
<body>
      <header>
            <h1>WELCOME</h1>
            <button>Add Details</button>
      </header>
      <div class="contact">
            
            <div class="info">
                  <h1>Contact Info</h1>
                  <p>This is the page to show the contacts.</p>
                  <button>Details</button>
            </div>
      </div>
</body>
</html>

```
  
``` scss
  /* style.scss */
   header{
    background: rgb(88, 192, 114);
    display: flex;
    justify-content: center;
    align-items: center;
}
```
![image](https://user-images.githubusercontent.com/75599178/174877844-9a35200a-5ec3-4206-a466-a73080f7da04.png)

</details>

<details>
  <summary>:bulb:</summary>
  
> Variables adding  
  
``` scss
  /* style.scss */
   $primaryBtn : rgb(180, 153, 223); // variable

header{
    background: rgb(88, 192, 114);
    display: flex;
    justify-content: center;
    align-items: center;
}

header button{
    background: $primaryBtn;
}

.contact button{
    background: $primaryBtn;
}
```
</details>
<details>
  <summary>:bulb:</summary>
  
 > Complex nesting 
  
``` scss
  /* style.scss */

$primaryBtn : rgb(180, 153, 223); // variable
$textColor: rgb(20, 20, 59);

header{
    background: rgb(88, 192, 114);
    display: flex;
    justify-content: center;
    align-items: center;
    color: $textColor;

    button{
        background: $primaryBtn;

        &:hover{
            background: rgb(226, 226, 144);
        }
    }

    &:hover{
        background-color: coral;
    }
}


.contact button{
    background: $primaryBtn;
}
``` 
![image](https://user-images.githubusercontent.com/75599178/174883631-e8607af3-b240-425e-b1f8-d01c9a45453f.png)

</details>

<details>
  <summary>:bulb:</summary>
  
> Separating code into multiple files
``` scss
  /* style.scss */

$primaryBtn : rgb(180, 153, 223); // variable
$textColor: rgb(20, 20, 59);

@import "./header";


.contact button{
    background: $primaryBtn;
}
``` 
> Add _header.scss in css folder to organize the codes as project flow.
> Then add header section styles to _header.scss file and import it in style.scss.  
``` scss
  /* _header.scss */

header{
    background: rgb(88, 192, 114);
    display: flex;
    justify-content: center;
    align-items: center;
    color: $textColor;

    button{
        background: $primaryBtn;

        &:hover{
            background: rgb(226, 226, 144);
        }
    }

    &:hover{
        background-color: coral;
    }
}
``` 
</details>
<details>
  <summary>:bulb:</summary>

> ### Variables, Mixins & custom mixins
<br>
  
> Create _variables.scss in css folder.
  
``` scss
 /* _variables.scss */

$primaryBtn : rgb(56, 146, 142);
$textColor  : rgb(58, 42, 42);
```

``` scss
 /* style.scss */

@import "./variables";
@import "./header";


.contact button{
    background: $primaryBtn;
}

```
> ### Mixins
<br>
  
> Create _mixins.scss file  in css folder.
``` scss
 /* style.scss */

@import "./variables";
@import "./header";
@import "./mixins";


.contact button{
    background: $primaryBtn;
}

```
``` scss
 /* _mixins.scss */

@mixin flexProp {
    display: flex;
    justify-content: center;
    align-items: center;
}

```
``` scss
 /* _header.scss */

header{
    background: rgb(88, 192, 114);
    height: 100vh;
    color: $textColor;

    @include flexProp();

    button{
        background: $primaryBtn;

        &:hover{
            background: rgb(226, 226, 144);
        }
    }

    &:hover{
        background-color: coral;
    }
}

```
![image](https://user-images.githubusercontent.com/75599178/174889770-b71e6fcb-ee93-46a8-bdec-4a7fdbd2a28f.png)

</details>
<details>
  <summary>:bulb:</summary>
  
``` scss
 /* _mixins.scss */


@mixin flexProp ($direction, $background) {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: $direction;
    background: $background
}

```
``` scss
 /* _header.scss */


header{
    @include flexProp(column, rgb(104, 129, 104));

    height: 100vh;
    // background: #ab99ca;;
    color: $textColor;
    button {
        background: $primaryBtn;
        height: fit-content;
        align-items: center;
        &:hover {
            background: red;
        }
    }
}

```
``` scss
 /* style.scss */
header{
  //  branch sassy files import
  @import "./variables";
  @import "./header";
  @import "./mixins";
  
.contact {
    @extend header;
    background: rgb(190, 190, 86);
    width: 100% - 30%;
    // padding: 2rem;
    // min-height: 100vh;
    // // align-items: center;
    // .contact button {
    //     background: rgb(58, 148, 90);
    // }
}

```
![screencapture-file-D-Sass-Exercise-1-html-2022-06-22-02_17_15](https://user-images.githubusercontent.com/75599178/174895098-f7d516cc-a3d5-4f09-9ebb-d0516d0e9fc6.png)
</details>

# Interview Questions

### 1) What is Sass?
<details>
  <summary>:bulb:</summary>

##### *SASS stands for Syntactically Awesome Style Sheets. SASS is the extension of the CSS which describes the document in a structured format. SASS provides more powerful syntax than CSS.*
</details>

### 2) What is the difference between Sass and CSS?
<details>
  <summary>:bulb:</summary>

![image](https://user-images.githubusercontent.com/75599178/175852463-10b3bc9a-81f0-40ea-a86e-cd072ba661b7.png)
</details>

### 3) How many ways can we use SASS?
<details>
  <summary>:bulb:</summary>

##### <li>SASS can be used as a Command Line Tool</li>
##### <li>SASS can be used as a Ruby Module</li>
##### <li>SASS can be used as a plugin for the Rack Enable Network</li>
</details>

### 4) Explain the features of SASS?
<details>
  <summary>:bulb:</summary>

##### <li>SASS is more stable, compatible and powerful with versions of CSS.</li>
##### <li>Nesting is one of the most important features of SASS. As a result of Nesting, the repetitions of the code is almost negligible and it is easier to maintain a document.SASS uses its own syntax and then it gets compiles to readable CSS.</li>
##### <li>Nesting is one of the most important features of SASS. As a result of Nesting, the repetitions of the code is almost negligible and it is easier to maintain a document.</li>
</details>

### 5) What is the difference between SCSS and Sass?
<details>
  <summary>:bulb:</summary>

![image](https://user-images.githubusercontent.com/75599178/175854973-43ac4be3-377c-464c-8fae-5c7a71486ebf.png)
</details>

### 6) What is the use of Sass @import function?
<details>
  <summary>:bulb:</summary>

##### SASS @import directive is used to include one stylesheet inside another stylesheet and in other words, we can say that it imports the .SASS and .scss files.
##### <li>@import "test.css";</li>
##### <li>@import "css/test.css";</li>
##### <li>@import url("http://check.com/css/test.css");</li>
</details>

### 7) Which is better, Sass or Less?
<details>
  <summary>:bulb:</summary>

**1) Cross Browser Support:-**  <h6> In SAAS, CSS transitions can be implemented by writing just one CSS rule and it adds up all the browsing rules for the coder.</h6>
**2) Mathematical Operations:-** <h6> SASS performs more accurate mathematical operations than LESS</h6>
**3) Compilation Time:-** <h6>Compilation time of SASS is less than LESS</h6>
**4) Documentation:-** <h6>SASS documentation is easier to read and understand as compared to LESS</h6>
***Above points clearly prove that the SASS is better CSS pre-processor than the LESS.***
</details>

### 8) Explain the Data Types of Sass supports?
<details>
  <summary>:bulb:</summary>

<li> Number</li>
<li>String</li>
<li>Colour</li>
<li>Map</li>
<li>Booleans and Null</li>
</details>

### 9) What is the use of @extend function in Sass?
<details>
  <summary>:bulb:</summary>

<h5> By using @extend function same style can be copied to the other classes also and there is no need to rewrite the code again.</h5>
</details>

### 10) Explain @include directive?
<details>
  <summary>:bulb:</summary>

<h5> The @include derivative is related to mixins that means it includes @mixin code. It allows the coder to create reusable code.</h5>
</details>

### 11) What is the use of @at-root directive in SASS? 
<details>
  <summary>:bulb:</summary>

<h5> Sass @at-root directive is a collection of nested rules that are used to style block at the root of the document.</h5>
</details>

### 12) What is Mixin function in SASS?
<details>
  <summary>:bulb:</summary>

<h5> Mixin function helps in making the group of the CSS declarations that need to be used throughout the coding and as result the length of the code reduces.</h5>
</details>

### 13) What is SASS output style?
<details>
  <summary>:bulb:</summary>

<h5> The CSS file that the SASS generates consists of default CSS style which reflects the structure of document. The default CSS styling is good but might not be suitable for all situations.</h5>
</details>









