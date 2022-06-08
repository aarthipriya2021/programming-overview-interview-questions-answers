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

### Jumbotron
<details>
	<summary>:bulb:</summary>
	<ul>
		<li>Big padded box for calling extra attention to some special content or information is called Jumbotron</li>
		<li>Jumbotron was no longer supported for bootstrap 5. It only supports bootstrap 3.</li>
	</ul>
	
``` html
	<!-- Jumbotron -->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Jumbotron</title>
	</head>
	<body>
	    <div class="container mt-3">
		<p>Big padded box for calling extra attention to some special content or information is called Jumbotron</p>
		<div class="mt-4 p-5 bg-primary text-white rounded">
		    <h1>Jumbotron Example</h1> 
		    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat..</p> 
		</div>
	    <p class="mt-3"><mark>p-5</mark> only displays the space around content. </p>
	    <p class="mt-3">Jumbotron was no longer supported for bootstrap 5. It only supports bootstrap 3.</p>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172573810-fee53a09-2ce3-469c-a7bb-5bcb7961057e.png)
	
</details>

### Spinners
<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- Spinner -->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Jumbotron</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Spinners</h2>
		<p>To create a spinner/loader, use the <code>.spinner-border</code> class:</p>

		<div class="spinner-border"></div>
	    </div>
	</body>
	</html>

```
![image](https://user-images.githubusercontent.com/75599178/172574092-90926982-e414-402c-a292-72001a111e04.png)

``` html
	<!-- Colored Spinners -->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Jumbotron</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Colored Spinners</h2>
		<p>Use any <strong>text color utilites</strong> to add a color to the spinner:</p>

		<div class="spinner-border text-muted"></div>
		<div class="spinner-border text-primary"></div>
		<div class="spinner-border text-success"></div>
		<div class="spinner-border text-info"></div>
		<div class="spinner-border text-warning"></div>
		<div class="spinner-border text-danger"></div>
		<div class="spinner-border text-secondary"></div>
		<div class="spinner-border text-dark"></div>
		<div class="spinner-border text-light"></div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172574858-ad84239c-2b6c-4238-95c9-6bbe7303ff45.png)

	
``` html
	<!-- Growing Spinners -->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Jumbotron</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Growing Spinners</h2>
		<p>Use the <code>.spinner-grow</code> class if you want the spinner/loader to grow instead of "spin":</p>

		<div class="spinner-grow text-muted"></div>
		<div class="spinner-grow text-primary"></div>
		<div class="spinner-grow text-success"></div>
		<div class="spinner-grow text-info"></div>
		<div class="spinner-grow text-warning"></div>
		<div class="spinner-grow text-danger"></div>
		<div class="spinner-grow text-secondary"></div>
		<div class="spinner-grow text-dark"></div>
		<div class="spinner-grow text-light"></div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172574930-cc618bf3-1c2c-471c-8a19-4ef3dd3ba572.png)

``` html
	<!-- Spinner Size -->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Jumbotron</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Spinner Size</h2>
		<p>Use <code>.spinner-border-sm</code> or <code>.spinner-grow-sm</code> to create a smaller spinner:</p>

		<div class="spinner-border spinner-border-sm"></div>
		<div class="spinner-grow spinner-grow-sm"></div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172575146-4e5329fe-7da9-4b55-b697-b45bc880af71.png)

	
</details>

### Alerts

<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- Alerts -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Alerts</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Alerts</h2>
		<p>Alerts are created with the .alert class, followed by a contextual color classes:</p>
		<div class="alert alert-success">
		  <strong>Success!</strong> This alert box could indicate a successful or positive action.
		</div>
		<div class="alert alert-info">
		  <strong>Info!</strong> This alert box could indicate a neutral informative change or action.
		</div>
		<div class="alert alert-warning">
		  <strong>Warning!</strong> This alert box could indicate a warning that might need attention.
		</div>
		<div class="alert alert-danger">
		  <strong>Danger!</strong> This alert box could indicate a dangerous or potentially negative action.
		</div>
		<div class="alert alert-primary">
		  <strong>Primary!</strong> Indicates an important action.
		</div>
		<div class="alert alert-secondary">
		  <strong>Secondary!</strong> Indicates a slightly less important action.
		</div>
		<div class="alert alert-dark">
		  <strong>Dark!</strong> Dark grey alert.
		</div>
		<div class="alert alert-light">
		  <strong>Light!</strong> Light grey alert.
		</div>
	      </div>
	</body>
	</html>
```
	
![image](https://user-images.githubusercontent.com/75599178/172579105-3c994ec2-d197-4a30-98db-8e5be9a10ba3.png)
	
``` html
	<!-- Alert Links -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Alerts</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Alert Links</h2>
		<p>Add the alert-link class to any links inside the alert box to create "matching colored links".</p>
		<div class="alert alert-success">
		    <strong>Success!</strong> You should <a href="#" class="alert-link">read this message</a>.
		</div>
		<div class="alert alert-info">
		    <strong>Info!</strong> You should <a href="#" class="alert-link">read this message</a>.
		</div>
		<div class="alert alert-warning">
		    <strong>Warning!</strong> You should <a href="#" class="alert-link">read this message</a>.
		</div>
		<div class="alert alert-danger">
		    <strong>Danger!</strong> You should <a href="#" class="alert-link">read this message</a>.
		</div>
		<div class="alert alert-primary">
		    <strong>Primary!</strong> You should <a href="#" class="alert-link">read this message</a>.
		</div>
		<div class="alert alert-secondary">
		    <strong>Secondary!</strong> You should <a href="#" class="alert-link">read this message</a>.
		</div>
		<div class="alert alert-dark">
		    <strong>Dark!</strong> You should <a href="#" class="alert-link">read this message</a>.
		</div>
		<div class="alert alert-light">
		    <strong>Light!</strong> You should <a href="#" class="alert-link">read this message</a>.
		</div>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172579262-0540dd55-2baf-4f54-ba7f-9eee5b6bcaef.png)
	
``` html
	<!-- Closing Alerts -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Alerts</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Closing Alerts</h2>
		<p>The button with class="btn-close" and data-bs-dismiss="alert" is used to close the alert box.</p>
		<p>The alert-dismissible class aligns the button to the right.</p>
		<div class="alert alert-success alert-dismissible">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Success!</strong> This alert box could indicate a successful or positive action.
		</div>
		<div class="alert alert-info alert-dismissible">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Info!</strong> This alert box could indicate a neutral informative change or action.
		</div>
		<div class="alert alert-warning alert-dismissible">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Warning!</strong> This alert box could indicate a warning that might need attention.
		</div>
		<div class="alert alert-danger alert-dismissible">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Danger!</strong> This alert box could indicate a dangerous or potentially negative action.
		</div>
		<div class="alert alert-primary alert-dismissible">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Primary!</strong> Indicates an important action.
		</div>
		<div class="alert alert-secondary alert-dismissible">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Secondary!</strong> Indicates a slightly less important action.
		</div>
		<div class="alert alert-dark alert-dismissible">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Dark!</strong> Dark grey alert.
		</div>
		<div class="alert alert-light alert-dismissible">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Light!</strong> Light grey alert.
		</div>
		</div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172580062-abb399d8-6d17-490f-b7a2-dc313aaff20d.png)
	
``` html 
	<!-- Animated Alerts -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Alerts</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Animated Alerts</h2>
		<p>The .fade and .show classes adds a fading effect when closing the alert message.</p>
		<div class="alert alert-success alert-dismissible fade show">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Success!</strong> This alert box could indicate a successful or positive action.
		</div>
		<div class="alert alert-info alert-dismissible fade show">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Info!</strong> This alert box could indicate a neutral informative change or action.
		</div>
		<div class="alert alert-warning alert-dismissible fade show">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Warning!</strong> This alert box could indicate a warning that might need attention.
		</div>
		<div class="alert alert-danger alert-dismissible fade show">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Danger!</strong> This alert box could indicate a dangerous or potentially negative action.
		</div>
		<div class="alert alert-primary alert-dismissible fade show">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Primary!</strong> Indicates an important action.
		</div>
		<div class="alert alert-secondary alert-dismissible fade show">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Secondary!</strong> Indicates a slightly less important action.
		</div>
		<div class="alert alert-dark alert-dismissible fade show">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Dark!</strong> Dark grey alert.
		</div>
		<div class="alert alert-light alert-dismissible fade show">
		    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
		    <strong>Light!</strong> Light grey alert.
		</div>
		</div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172579914-892be9a0-4e2a-4419-92af-700d0c22df78.png)
	
</details>












