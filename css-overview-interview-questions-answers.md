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
1. Bandwidth <br>
2. Site-wide consistency <br>
3. Page reformatting <br>
4. Accessibility <br>
5. Content separated from presentation <br>
</details>

#### 3. What are the limitations of CSS?

<details>
<summary>:bulb:</summary>
1. No expressions <br>
2. Limitations of vertical control <br>
3. No column declaration <br>
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
<style>    
#para1 {    
    text-align: center;    
    color: blue;    
}    
</style>    
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
3. Padding - It removes the area around the content. It i stransparent.<br>
4. Content - It represents like text, images.
</details>

#### 17. What is the float property of css ? 

<details>
<summary>:bulb:</summary>
The css float property is used to move the image to the right or left along with the texts to be wrapped around it.
![image](https://user-images.githubusercontent.com/75599178/184190114-853751d8-1fc9-4d8f-a721-679ea179185b.png)

</details>

#### 18. What is thye purpose of z-index?

<details>
<summary>:bulb:</summary>
The z-index helps to specify the stack order of elements in that may overlap one another. The z-index value is zero , it may  either positive or negative. 
</details>

