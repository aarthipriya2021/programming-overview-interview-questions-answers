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

<details>
  <summary>:bulb:</summary>
Switch the watch sass in task bar of vscode.  

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
  
``` css
  /* style.scss */
   header{
    background: rgb(88, 192, 114);
    display: flex;
    justify-content: center;
    align-items: center;
}
```

</details>


