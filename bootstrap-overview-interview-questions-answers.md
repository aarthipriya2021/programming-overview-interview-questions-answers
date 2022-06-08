# Overview

### What is bootstrap?
<details>
  <summary>:bulb:</summary>
    <ul>
           <li> Bootstrap is a CSS framework directed at responsive, mobile-first front-end web development.</li>
           <li> Bootstrap 5 is the newest version of Bootstrap. </li>
    </ul>
</details>

### Bootstrap 5 vs. Bootstrap 3 & 4:
<details>
  <summary>:bulb:</summary>
    <ul>
           <li> Bootstrap 5 is the newest version of Bootstrap; with new components, faster stylesheet and more responsiveness. </li>
           <li> Bootstrap 5 supports the latest, stable releases of all major browsers and platforms. However, Internet Explorer 11 and down is not supported. </li>
           <li> The main differences between Bootstrap 5 and Bootstrap 3 & 4, is that Bootstrap 5 has switched to JavaScript instead of jQuery. </li>
    </ul>
</details>

### How to use bootstrap 5?
<details>
  <summary>:bulb:</summary>
  Using CDN Link (Content Delivery Network)
 
![image](https://user-images.githubusercontent.com/75599178/172359891-4a41a562-68d3-4e6b-b6e5-b2bac99b191d.png)
  
</details>

### Advantages of Bootstrap:
<details>
  <summary>:bulb:</summary>
    <ul>
           <li> Easy to use: Anybody with just basic knowledge of HTML and CSS can start using Bootstrap.</li>
           <li> Responsive features: Bootstrap's responsive CSS adjusts to phones, tablets, and desktops.</li>
           <li> Mobile-first approach: In Bootstrap, mobile-first styles are part of the core framework</li>
           <li>Browser compatibility: Bootstrap 5 is compatible with all modern browsers (Chrome, Firefox, Edge, Safari, and Opera). 
             Note that if you need support for IE11 and down, you must use either BS4 or BS3.</li>
    </ul>
</details>

# Topics

### Containers
<details>
  <summary>:bulb:</summary>
  Containers are used to pad the content inside of them, and there are two container classes available:
		<ul>
			<li> The <b>.container</b> class provides a responsive fixed width container.</li>
			<li> The <b>.container-fluid</b> class provides a full width container, spanning the entire width of the viewport.</li>
   	</ul>
	
![image](https://user-images.githubusercontent.com/75599178/172364974-a2412833-f77a-49c5-8f2b-6c183a215e88.png)

</details>

### Responsive container
<details>
  <summary>:bulb:</summary>
		The max-width of the container will change on different screen sizes/viewports:
	
![image](https://user-images.githubusercontent.com/75599178/172365383-62c4f9b3-708f-4bcb-9540-e0e561792105.png)
	
</details>

### Table
<details>
  <summary>:bulb:</summary>
	A basic Bootstrap 5 table has a light padding and horizontal dividers.

``` html
	<!-- table -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Tables</title>
	</head>
	<body>
	    <div class="container text-center">
	    <table class="table">
		<thead>
		    <tr>
			<th>Firstname</th>
			<th>Lastname</th>
			<th>Email</th>
		    </tr>
		</thead>
		</tbody>
		    <tr>
			<td>Mary</td>
			<td>Moe</td>
			<td>mary@example.com</td>
		    </tr>
		    <tr>
			<td>July</td>
			<td>Dooley</td>
			<td>july@example.com</td>
		    </tr>
		    <tr></tr>
		</tbody>
	    </div>
	    </table>
	</body>
	</html> 
	
```
![image](https://user-images.githubusercontent.com/75599178/172455324-1c87ebd0-286f-437d-b0b7-d8bab47df1ae.png)

``` html
	<!-- table-striped-->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Tables</title>
	</head>
	<body>
	    <div class="container text-center">
	    <table class="table table-striped">
		<thead>
		    <tr>
			<th>Firstname</th>
			<th>Lastname</th>
			<th>Email</th>
		    </tr>
		</thead>
		</tbody>
		    <tr>
			<td>Mary</td>
			<td>Moe</td>
			<td>mary@example.com</td>
		    </tr>
		    <tr>
			<td>July</td>
			<td>Dooley</td>
			<td>july@example.com</td>
		    </tr>
		    <tr></tr>
		</tbody>
	    </div>
	    </table>
	</body>
	</html>
	
```
![image](https://user-images.githubusercontent.com/75599178/172455635-e54be125-c97b-4d03-9069-61b21ff20000.png)

``` html
	<!-- bordered table-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Tables</title>
	</head>
	<body>
	    <div class="container text-center">
	    <table class="table table-bordered">
		<thead>
		    <tr>
			<th>Firstname</th>
			<th>Lastname</th>
			<th>Email</th>
		    </tr>
		</thead>
		</tbody>
		    <tr>
			<td>Mary</td>
			<td>Moe</td>
			<td>mary@example.com</td>
		    </tr>
		    <tr>
			<td>July</td>
			<td>Dooley</td>
			<td>july@example.com</td>
		    </tr>
		    <tr></tr>
		</tbody>
	    </div>
	    </table>
	</body>
	</html>
	
```
![image](https://user-images.githubusercontent.com/75599178/172455829-621f56dd-0056-416f-a945-11f8629baec2.png)

``` html
	<!-- hover rows-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Tables</title>
	</head>
	<body>
	    <div class="container text-center">
	    <table class="table table-hover">
		<thead>
		    <tr>
			<th>Firstname</th>
			<th>Lastname</th>
			<th>Email</th>
		    </tr>
		</thead>
		</tbody>
		    <tr>
			<td>Mary</td>
			<td>Moe</td>
			<td>mary@example.com</td>
		    </tr>
		    <tr>
			<td>July</td>
			<td>Dooley</td>
			<td>july@example.com</td>
		    </tr>
		    <tr></tr>
		</tbody>
	    </div>
	    </table>
	</body>
	</html>
	
```
![image](https://user-images.githubusercontent.com/75599178/172456377-1c9e8753-ffe8-49c0-9125-3b15933b4fd2.png)

``` html
	
	<!-- borderless table-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Tables</title>
	</head>
	<body>
	    <div class="container text-center">
	    <table class="table table-borderless">
		<thead>
		    <tr>
			<th>Firstname</th>
			<th>Lastname</th>
			<th>Email</th>
		    </tr>
		</thead>
		</tbody>
		    <tr>
			<td>Mary</td>
			<td>Moe</td>
			<td>mary@example.com</td>
		    </tr>
		    <tr>
			<td>July</td>
			<td>Dooley</td>
			<td>july@example.com</td>
		    </tr>
		    <tr></tr>
		</tbody>
	    </div>
	    </table>
	</body>
	</html>
	
```
![image](https://user-images.githubusercontent.com/75599178/172456883-58f29aaf-7532-44be-94ff-e718912e9a6f.png)

</details>

### Images
<details>
  <summary>:bulb:</summary>

``` html
	<!-- Rounded corner-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Images</title>
	</head>
	<body>
	    <div class="container">
		<h2>Rounded Corners</h2>
		<p>The .rounded class adds rounded corners to an image:</p>            
		<img src="./Images/cat.jpg" class="rounded" alt="cat" width="304" height="236"> 
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172526287-f191c348-54cc-4f06-b792-c3b34137de37.png)

```html
	<!-- Circle -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Images</title>
	</head>
	<body>
	    <div class="container">
		<h2>Circle</h2>
		<p>The .rounded-circle class adds rounded corners to an image:</p>            
		<img src="./Images/cat.jpg" class="rounded-circle" alt="cat" width="304" height="236"> 
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172526393-83e22406-eef6-4f1a-befd-f1841f1b52ec.png)

``` html 
	<!-- Thumbnail -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Images</title>
	</head>
	<body>
	    <div class="container">
		<h2>Thumbnail</h2>
		<p>The .img-thumbnail class adds rounded corners to an image:</p>            
		<img src="./Images/cat.jpg" class="img-thumbnail" alt="cat" width="304" height="236"> 
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172526505-b0e5775d-9184-4ae2-ab55-d17920dc6e99.png)

``` html
	<!-- Aligning Images -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Images</title>
	</head>
	<body>
	    <h2>Aligning images</h2>
	    <p>Use the float classes to float the image to the left or to the right:</p> 
	    <img src="./Images/cat.jpg" class="float-start" alt="Paris" width="304" height="236"> 
	    <img src="./Images/cat.jpg" class="float-end" alt="Paris" width="304" height="236"> 
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172526715-8c5bb424-40e2-4287-85dd-7483f0513828.png)

``` html
	<!-- Centered Image -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Images</title>
	</head>
	<body>
	    <div>
		<h2>Centered Image</h2>
		<p>Center an image by adding the utility classes .mx-auto (margin:auto) and .d-block (display:block) to the image:</p> 
		<img src="./Images/cat.jpg" class="mx-auto d-block" style="width:20%"> 
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172526884-6a44fe2b-6610-44b9-8c6b-d54769a4fb38.png)
	
``` html 
	<!-- Responsive Images -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Images</title>
	</head>
	<body>
	    <div>
		<h2>Responsive Images</h2>
		<p>The .img-fluid class makes the image scale nicely to the parent element (resize the browser window to see the effect):</p>
		<img class="img-fluid" src="./Images/cat.jpg" alt="cat" width="1100" height="500"> 
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172527137-de53b9e7-f6fd-4287-94b0-c53c51da6700.png)

</details>

### 
<details>
	<summary>:bulb:</summary>
</details>
