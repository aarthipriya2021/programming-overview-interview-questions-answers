## CSS Overview

https://docs.google.com/document/d/1xY7HwCGxHgBOIVT1CVx-CH_K6N5RhXCpXpSJySApUeY/edit

### INTERVIEW QUESTIONS

#### 1. What is CSS ?

<details>
<summary>:bulb:</summary>
CSS stands for Cascading Style Sheet. It determines the how the website or content shown/looked.
</details>

#### 2. What are advantages ?

<details>
<summary>:bulb:</summary>
1. Separation of content from presentation - CSS provides a way to present the same content in multiple presentation formats in mobile or desktop or laptop.<br>
2. Easy to maintain - CSS, built effectively can be used to change the look and feel complete by making small changes. To make a global change, simply change the style, and all elements in all the web pages will be updated automatically. <br>
3. Bandwidth - Used effectively, the style sheets will be stored in the browser cache and they can be used on multiple pages, without having to download again. <br>
4. Accessibility <br>
</details>

#### 3. What are the limitations of CSS?

<details>
<summary>:bulb:</summary>
1. Browser compatibility <br>
2. Cross browser issue <br>
3. There is no parent selector <br>
</details>

#### 4. What is Embedded Style Sheet?

<details>
<summary>:bulb:</summary>
We can embed the whole style elements in html document using <style>  tag.

```CSS
<style>    
body {    
    background-color: linen;    
}    
h1 {    
    color: red;    
    margin-left: 80px;    
}     
</style>    
       
```
</details>

#### 5. What are the advantages of Embedded Style Sheets?

<details>
<summary>:bulb:</summary>
1. It is posible to create classes for use on multiple tag types in the document. <br>
2. Under complex situations, selector and grouping methods can be used to apply styles.<br>
3. No extra downloads are required to import the information. <br>
</details>

#### 6. What is a CSS selector?

<details>
<summary>:bulb:</summary>
CSS selectors are used to select the content you want to style. 
1. CSS Element Selector <br>
2. CSS Id Selector <br>
3. CSS Class Selector <br>
4. CSS Universal Selector <br>
5. CSS Group Selector <br>
</details>

#### 7. Name some CSS style components.

<details>
<summary>:bulb:</summary>
1. Selector <br>
2. Property <br>
3. value <br>
</details>

#### 8. What is the use of CSS Opacity?

<details>
<summary>:bulb:</summary>
The css properity is used to specify the transparency of an element . (Opacity is defined as the degree to which light is allowed to travel through an object.)

``` css
<style>    
img.trans {    
    opacity: 0.4;    
    filter: alpha(opacity=40); /* For IE8 and earlier */    
}    
</style>   
```
</details>

#### 9. Explain universal selector.

<details>
<summary>:bulb:</summary>
It matches elements of any type. An asterish("*") is ususally denoted as universal selector.

``` css
<style>    
* {    
   color: green;    
   font-size: 20px;    
}     
</style>  
```
</details>

#### 10. Name the property for controlling the image repetition of the background.

<details>
<summary>:bulb:</summary>
The background-repeat property controlls the repetition of image.
</details>

#### 11. Name the property for controlling the image position in the background.

<details>
<summary>:bulb:</summary>
The background-position property controlls the position of image.

``` css
background: white url('good-morning.jpg');  
background-repeat: no-repeat;  
background-attachment: fixed;  
background-position: center;  
/*center/top/bottom/left/right*/ 
```
</details>

#### 12. Name the property for controlling the image scroll in the background.

<details>
<summary>:bulb:</summary>
The background-attachment property controlls the image scroll in the background.
</details>

#### 13. What is the difference between class selectors and id selectors?

<details>
<summary>:bulb:</summary>
An overall block is given to class selector while id selectors take only a single element differing from other elements.
**CSS Class Selector**

``` css
<style>    
.center {    
    text-align: center;    
    color: blue;    
}    
</style>  
```

**CSS id selector**

``` css
<style>    
#para1 {    
    text-align: center;    
    color: blue;    
}    
</style> 
```   
</details>

#### 14. What are the advantages of External Style Sheets?

<details>
<summary>:bulb:</summary>
1. You can create classes for reusing it in many documents. <br>
2. By using it, you can control the styles of multiple documents from one file. <br>
3. In complex situations, you can use selectors and grouping methods to apply styles. <br>
</details>

#### 15. What RWD?

<details>
<summary>:bulb:</summary>
Responsive Web Design. This technique is used to display the website on different devices like, mobiles, tablets, laptops, desktop.
</details>

#### 16. What is css box model and its elements.

<details>
<summary>:bulb:</summary>
CSS box model is used to define the design and layout of elements of css. <br>

![image](https://user-images.githubusercontent.com/75599178/184180252-64816840-f292-4582-ad53-154781e5df70.png)

1. Margin - It removes the area around border. It is transparent.<br>
2. Border - It represents area around padding .<br>
3. Padding - It removes the area around the content. It is transparent.<br>
4. Content - It represents like text, images.
</details>

#### 17. What is the float property of css ? 

<details>
<summary>:bulb:</summary>
The css float property is used to move the image to the right or left along with the texts to be wrapped around it.

![image](https://user-images.githubusercontent.com/75599178/184190114-853751d8-1fc9-4d8f-a721-679ea179185b.png)

</details>

#### 18. What is the purpose of z-index?

<details>
<summary>:bulb:</summary>
The z-index helps to specify the stack order of elements in that may overlap one another. The z-index value is zero , it may  either positive or negative. 
</details>

#### 19. What is CSS Preprocesor ? What are Sass, Less ?

<details>
<summary>:bulb:</summary>
Css preprocessor is a tool used to extend the basic functionality of default vanilla css through its own scripting language. It helps to use complex logical syntax like variables, functions,mixins.<br><br>

##### SASS :
SASS is the acronym for "Syntactically Awesome Style Sheets". 

###### SASS vs SCSS
1. SASS is based on indentation and SCSS(Sassy CSS) is not.<br>
2. SASS uses .sass extension while SCSS uses .scss extension. <br>
3. SASS doesnt use curly brackets or semicolons. SCSS just like the CSS.
   
SASS SYNTAX | SCSS SYNTAX
------------ | -------------    
![image](https://user-images.githubusercontent.com/75599178/184363604-190c71d8-0693-441b-b80d-bc1e6611df9f.png) | ![image](https://user-images.githubusercontent.com/75599178/184363682-6abdc43d-33e8-445b-a7dd-8d6776fb5388.png)

##### LESS :
LESS is the acronym for "Leaner Style Sheets".  LESS is easy to add to any javascript projects by using .less.<br>
LESS syntax is the same as the SCSS with some exceptions. LESS uses @to define the variable. 
</details>     
    
#### 20. What are Pseudo elements and Pseudo classes ?

<details>
<summary>:bulb:</summary>

**PSEUDO ELEMENTS :** It is keyword added selector, that lets you style a specific part of the selected element(s) .

**Example:**
1. ::before <br>
2. ::after <br>
3. ::first-line <br>
4. ::first-letter 

**PSEUDO ELEMENTS :** It is keyword added selector, that specifies the state of selected elements.
    
**Example:**
1. :link<br>
2. :active <br>
3. :hover <br>
4. :focus 
</details>    
    
#### 21. What is flexbox?

<details>
<summary>:bulb:</summary>
Flexbox is flexible box.  It allows elements to align the distribute space within a container.

![screencapture-flexboxsheet-2022-08-12-22_51_53](https://user-images.githubusercontent.com/75599178/184412716-300159bd-c869-46d5-a893-5e0b683e7442.png)

</details>    
    
    
    
    
    
    
    
    
    
    
