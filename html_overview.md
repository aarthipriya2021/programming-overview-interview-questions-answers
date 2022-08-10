### HTML DOCUMENTATION

[HTML-DOCUMENTATION.pdf](https://github.com/aarthipriya2021/programming-overview-interview-questions-answers/files/8849662/HTML-DOCUMENTATION.pdf)


### INTERVIEW QUESTIONS

#### 1. What is HTML?

<details>
<summary>:bulb:</summary>
HTML is a markup language, which is used to structure the web page and and its content. 
</details>

#### 2. Are the HTML tags, elements, attributes the same thing?
<details>
<summary>:bulb:</summary>
<li>HTML tags are used to hold the HTML element.<br>

For Example :  ![image](https://user-images.githubusercontent.com/75599178/183475600-7abca317-f0f4-4abd-980c-f5f172b0eddd.png)
</li>
<li>HTML element holds the content.<br>
<li>HTML attributes are used to describe the characteristic of an HTML element in detail.</li>
 </li>

![image](https://user-images.githubusercontent.com/75599178/183480845-699de049-1e66-4b66-aa8f-79cb1a6c7729.png)

</details>

#### 3. What are void elements in HTML?
<details>
<summary>:bulb:</summary>
HTML elements which do not have closing tags or do not need to be closed are Void elements. For Example <br />, <img />, <hr />, etc.
</details>

#### 4. What is the advantage of collapsing white space?
<details>
<summary>:bulb:</summary>
<li>Collapsing white spaces decreases the transmission time between the server and the client because collapsing features remove unnecessary bytes that are occupied by the white spaces.</li>
<li>By mistake, if you leave extra white space, the browser will ignore it and display the UI perfectly.</li>

</details>

#### 5. What are HTML Entities?
<details>
<summary>:bulb:</summary>
In HTML some characters are reserved like ‘<’, ‘>’, ‘/’, etc. To use these characters in our webpage we need to use the character entities called HTML Entities. 

![image](https://user-images.githubusercontent.com/75599178/183559626-5c832ac7-f748-47a0-adad-6f3df3294555.png)

</details>

#### 6. What are different types of lists in HTML?
<details>
<summary>:bulb:</summary>

![image](https://user-images.githubusercontent.com/75599178/183560386-b0ada959-2534-444b-9cb3-0b625ed39005.png)

</details>

#### 6. What is the ‘class’ attribute in HTML?
<details>
<summary>:bulb:</summary>
<li>The class attribute is used to specify the class name for an html element.</li>
<li>Multiple elements can have same class value.</li>
<li>Also, it is mainly used to associate the styles written in the stylesheet with the HTML elements.</li>

</details>

#### 7. What is the difference between the ‘id’ attribute and the ‘class’ attribute of HTML elements?
<details>
<summary>:bulb:</summary>

**Class attribute** -  Multiple elements can associate. <br>
**Id attribute** - Only one element can have.

</details>

#### 8. Describe HTML layout structure.
<details>
<summary>:bulb:</summary>
Every webpage has different layout structure, But globally accepted way to structure the webpage  such as:

``` html
1. <header>: Stores the starting information about the web page.
2. <footer>: Represents the last section of the page.
3. <nav>: The navigation menu of the HTML page.
4. <article>: It is a set of information.
5. <section>: It is used inside the article block to define the basic structure of a page.
6. <aside>: Sidebar content of the page.
```

</details>

#### 9.How to optimize website assets loading?
<details>
<summary>:bulb:</summary>
<li>CDN hosting : A Content Delivery Network is geographically distributed servers to help the reduce latency.</li>
<li>File compression : This is a method that reduces the size of an asset to reduce the data transfer.</li>
<li>File Concatenation : This reduces the api calls.</li>
<li>Lazy loading : Instead of loading all th assets at once, the non-critical assets can be loaded on a need basis.</li>
</details>

#### 10. What are the various formatting tags in html?
<details>
<summary>:bulb:</summary>

``` html
1. <b> - makes text bold
2. <i> - makes text italic
3. <em> - makes text italic but with added semantics importance
4. <big> - increases the font size of the text by one unit
5. <small> - decreases the font size of the text by one unit
6. <sub> - makes the text a subscript
7. <sup> - makes the text a superscript
8. <del> - displays as strike out text
9. <strong> - marks the text as important
10. <mark> - highlights the text
11. <ins> - displays as added text
```
</details>

#### 11. What are the different kinds of Doctype available?
<details>
<summary>:bulb:</summary>
<li>Strict Doctype</li>
<li>Tansitional Doctype</li>
<li>Frameset Doctype</li>
</details>

#### 12. What are the different kinds of Doctype available?
<details>
<summary>:bulb:</summary>

``` html
<!DOCTYPE html>
<html>
 <head>
   <meta charset="UTF-8">
   ...
   ...
 </head>
 ...
</html>
```
</details>

#### 13. Difference between ![image](https://user-images.githubusercontent.com/75599178/183624976-50c05934-a408-49df-a2df-e6eaf7bb97c3.png)

<details>
<summary>:bulb:</summary>

<li>b tag , i tag are stands for bold and italic.Apart from this these tags dont say anything about the text. <br> </li>
<li>em tag , strong tag are stands semantic tags it represents that the span of text is strong and importance an emphatic stress respectively than the rest of the text.</li>
</details>

#### 14. What is the significance of <head> and <body> tag in HTML?

<details>
<summary>:bulb:</summary>
<head> tag provide the information about web page or document like meata data, characterset,..etc.Also it can be only one head tag in the entire html and it should be represents the before of the body tag also. <br>

<body> tag defines the body of the html documnt. All the contents needs to be displayed on web page like images, videos, links, texts are useing with respecct of their tags in body tag part. Also only one body tag is in html document , which is should be after the head tag.

</details>

#### 15. Can we display a web page inside a web page or Is nesting of webpages possible?

<details>
<summary>:bulb:</summary>
Yes, we can display a web page inside another web page. HTML provides a tag <iframe> using which we can achieve this functionality.

``` html
<iframe src=”https://youtube.com" />
```
</details>

#### 16.How is Cell Padding different from Cell Spacing?

<details>
<summary>:bulb:</summary>
Cell spacing: Cell spacing is space or gap  is space between two consecutive cells <br>
Cell padding: Cell padding is space inside the cell which  is space between content border/edge of the cell.
</details>

#### 17. How can we club two or more rows or columns into a single row or column in an HTML table?

<details>
<summary>:bulb:</summary>
HTML provides two table attributes “rowspan” and “colspan” to make a cell span to multiple rows and columns respectively.

```html
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Cell that spans two rows</h2>
<p>To make a cell span more than one row, use the rowspan attribute.</p>

<table style="width:100%">
  <tr>
    <th>Name</th>
    <td>Jill</td>
  </tr>
  <tr>
    <th rowspan="2">Phone</th>
    <td>555-1234</td>
  </tr>
  <tr>
    <td>555-8745</td>
  </tr>
</table>
</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/183661662-eb61a12d-277e-4789-ad77-7259eb9eaa4c.png)

```html
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Cell that spans two columns</h2>
<p>To make a cell span more than one column, use the colspan attribute.</p>

<table style="width:100%">
  <tr>
    <th colspan="2">Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>43</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>57</td>
  </tr>
</table>
</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/183662222-7a0eb506-e8d0-4279-a92f-c50d472ae259.png)

</details>
                                 
#### 18. Is it possible to change an inline element into a block level element?

<details>
<summary>:bulb:</summary>
Yes, it is possible using the “display” property with its value as “block”, to change the inline element into a block-level element                               
</details>                                 
               
#### 19. In how many ways can we position an HTML element? Or what are the permissible values of the position attribute?

<details>
<summary>:bulb:</summary>
1.Static :  This is not positioned in special way. It is positioned on flow of the document.<br>
2.Absolute : This is positioned relative to the nearest positioned ancestor.<br>
3.Fixed : This is positioned relative to the viewport, which means it always in the same place even if the page is scrolled.Position of the element might be top, bottom, right, left.<br>
4.Relative : This is positioned according to normal flow of the document and positioned relative to its original/normal position.<br>
5.Initial : This resets the property to its default value.<br>
6.Inherit : Here the element inherits or takes the property of its parent.                              
</details>                                    
                                 
#### 20. What is the difference between “display: none” and “visibility: hidden”, when used as attributes to the HTML element.

<details>
<summary>:bulb:</summary>
When we use the attribute “visibility: hidden” for an HTML element then that element will be hidden from the webpage but still takes up space. Whereas, if we use the “display: none” attribute for an HTML element then the element will be hidden, and also it won’t take up any space on the webpage.                              
</details>                                   
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 
                                 




