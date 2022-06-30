# Overview

### What is tailwind css?
<details>
  <summary>:bulb:</summary>

  *Tailwind CSS is basically a Utility first CSS framework for building rapid custom UI. It is a highly customizable, low-level CSS framework that gives you all of the building blocks that you need. Also, it is a cool way to write inline styling and achieve an awesome interface without writing a single line of your own CSS.*
</details>

### Why Tailwind CSS?
<details>
  <summary>:bulb:</summary>

  <li>Faster UI building process</li>
  <li>It is a utility-first CSS framework which means we can use utility classes to build custom designs without writing CSS as in traditional approach. </li>
</details>

### Advantages of Tailwind CSS:
<details>
  <summary>:bulb:</summary>

  <li>No more silly names for CSS classes and Id’s.</li>
  <li>Minimum lines of Code in CSS file.</li>
  <li>We can customize the designs to make the components.</li>
  <li>Makes the website responsive.</li>
</details>

### Tailwind css install
<details>
  <summary>:bulb:</summary>

  <li>In terminal, "npm install -D tailwindcss"</li>
  <li>Then, "npx tailwindcss init"</li>
  <li>Create src folder , and into this create input.css file and index.html file also. And paste below code in input.css file.</li>

  ``` css

  /* src/input.css */
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
  ```
  <li>Create dist foler in project . and add output.css file in it.</li>
  <li>paste below code in index.html file.</li>

  ``` html

  <!doctype html>
  <html>
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="/dist/output.css" rel="stylesheet">
  </head>
  <body>
    <h1 class="text-3xl font-bold underline font-red-100">
      Hello world!
    </h1>
  </body>
  </html>
  ```
  <li>In terminal, "npm init -y"</li>
  <li>Then, in package.json add " "build": "tailwindcss -i ./src/input.css -o ./dist/output.css --watch" "for "test:.." query. </li>
  <li>Then in config .js file add content as "./src/index.html".</li>
  <li>After this in terminal "npm run build"</li>
  <li>Then proceed with Go Live.</li>
</details>

### Tailwind CSS Example
<details>
  <summary>:bulb:</summary>

Code | Output
------------ | -------------
![image](https://user-images.githubusercontent.com/75599178/176752988-401bec47-b19e-4bd3-841e-6399eb13cffe.png) | ![image](https://user-images.githubusercontent.com/75599178/176752909-a3ad2615-1088-4123-b3b9-f4b13aab9273.png)


</details>

#Topics

### Background
<details>
  <summary>:bulb:</summary>

</details>
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
