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

### Buttons
<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- Buttons -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Buttons</title>
	</head>
	<body>
	    <div class="container">
		<h2>Button Styles</h2>
		<button type="button" class="btn">Basic</button>
		<button type="button" class="btn btn-primary">Primary</button>
		<button type="button" class="btn btn-secondary">Secondary</button>
		<button type="button" class="btn btn-success">Success</button>
		<button type="button" class="btn btn-info">Info</button>
		<button type="button" class="btn btn-warning">Warning</button>
		<button type="button" class="btn btn-danger">Danger</button>
		<button type="button" class="btn btn-dark">Dark</button>
		<button type="button" class="btn btn-light">Light</button>
		<button type="button" class="btn btn-link">Link</button>      
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172627223-db628315-06a9-41d1-8b52-ad942c782680.png)
	
``` html
	<!-- Buttons Elements-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Buttons</title>
	</head>
	<body>
	    <div class="container">
		<h2>Button Elements</h2>
		<a href="#" class="btn btn-success">Link Button</a>
		<button type="button" class="btn btn-success">Button</button>
		<input type="button" class="btn btn-success" value="Input Button">
		<input type="submit" class="btn btn-success" value="Submit Button">
		<input type="reset" class="btn btn-success" value="Reset Button" disabled>    
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172628293-c8fe321f-3597-4901-804c-4530c797c0ed.png)
	
``` html
	<!-- Buttons Outline -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Buttons</title>
	</head>
	<body>
	    <div class="container">
		<h2>Button Outline</h2>
		<button type="button" class="btn btn-outline-primary">Primary</button>
		<button type="button" class="btn btn-outline-secondary">Secondary</button>
		<button type="button" class="btn btn-outline-success">Success</button>
		<button type="button" class="btn btn-outline-info">Info</button>
		<button type="button" class="btn btn-outline-warning">Warning</button>
		<button type="button" class="btn btn-outline-danger">Danger</button>
		<button type="button" class="btn btn-outline-dark">Dark</button>
		<button type="button" class="btn btn-outline-light text-dark">Light</button>   
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172628371-ccec0c0f-90d6-46ae-8ef4-6d05bec827d9.png)
	
``` html
	<!-- Button Sizes -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Buttons</title>
	</head>
	<body>
	    <div class="container">
		<h2>Button Sizes</h2>
		<button type="button" class="btn btn-primary btn-lg">Large</button>
		<button type="button" class="btn btn-primary btn-md">Default</button>    
		<button type="button" class="btn btn-primary btn-sm">Small</button>  
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172628445-2099cc5b-03ef-4298-badb-6638f03544d5.png)
	
``` html
	<!-- Block Level Buttons -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Buttons</title>
	</head>
	<body>
	    <div class="container">
		<div class="d-grid">
		    <h2>Button Sizes</h2>
		    <button type="button" class="btn btn-primary btn-block">Full-Width Button</button>
		</div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172628547-c0f6d054-2f1d-4ffc-909e-8c0f49acde5d.png)
	
``` html
	<!-- space between buttons vertically-->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Buttons</title>
	</head>
	<body>
	    <div class="container">
		<div class="d-grid gap-3">
		    <h2>Button Sizes</h2>
		    <button type="button" class="btn btn-primary btn-block">Full-Width Button</button>
		    <button type="button" class="btn btn-primary btn-block">Full-Width Button</button>
		    <button type="button" class="btn btn-primary btn-block">Full-Width Button</button>
		</div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172628685-2a989978-a471-4025-a830-9c2cdf53ac9b.png)

``` html
	<!-- Active/Disabled Buttons -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Buttons</title>
	</head>
	<body>
	    <div class="container">
		<h2>Button States</h2>
		<button type="button" class="btn btn-primary">Primary Button</button>
		<button type="button" class="btn btn-primary active">Active Primary</button>
		<button type="button" class="btn btn-primary" disabled>Disabled Primary</button>
		<a href="#" class="btn btn-primary disabled">Disabled Link</a>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172628855-335e9a3b-244e-4b51-be81-d75db0dbfd98.png)

``` html
	  <!-- button group / dropdown-item-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Buttons</title>
	</head>
	<body>
	    <div class="container">
		    <h2>Nesting Button Groups</h2>
		    <p>Nest button groups to create dropdown menus:</p>
		    <div class="btn-group">
		      <button type="button" class="btn btn-primary">Apple</button>
		      <button type="button" class="btn btn-primary">Samsung</button>
		      <div class="btn-group">
			<button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">Sony</button>
			<ul class="dropdown-menu">
			  <li><a class="dropdown-item" href="#">Tablet</a></li>
			  <li><a class="dropdown-item" href="#">Smartphone</a></li>
			</ul>
		      </div>
		    </div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172628941-b61430f6-3ccb-482c-acfc-83fbcd08c4d4.png)
	
</details>

### Badges
<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- Badges -->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Badges | Progress Bars</title>
	</head>
	<body>
	    <div class="container mt-3 d-grid"></div>
		<h2 class="text-center">Badges</h2>
		<p class="text-center">Use the .badge class together with a contextual class (like .bg-secondary) within <span> elements to create rectangular badges. </p>
		<h1 class="text-center">Example heading <span class="badge bg-secondary">New</span></h1>
		<h2 class="text-center">Example heading <span class="badge bg-secondary">New</span></h2>
		<h3 class="text-center">Example heading <span class="badge bg-secondary">New</span></h3>
		<h4 class="text-center">Example heading <span class="badge bg-secondary">New</span></h4>
		<h5 class="text-center">Example heading <span class="badge bg-secondary">New</span></h5>
		<h6 class="text-center">Example heading <span class="badge bg-secondary">New</span></h6>    

	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172632666-579347bd-7c68-46d2-a6a3-8b3c6978d3b3.png)

``` html

	<!-- Contextual Badges -->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Badges | Progress Bars</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Contextual Badges</h2>
		<span class="badge bg-primary">Primary</span>
		<span class="badge bg-secondary">Secondary</span>
		<span class="badge bg-success">Success</span>
		<span class="badge bg-danger">Danger</span>
		<span class="badge bg-warning">Warning</span>
		<span class="badge bg-info">Info</span>
		<span class="badge bg-light">Light</span>
		<span class="badge bg-dark">Dark</span>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172632734-f1d6d333-616c-460f-ba13-d82798446cfa.png)

``` html
	<!-- Pill Badges -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Badges | Progress Bars</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Pill Badges</h2>
		<span class="badge rounded-pill bg-primary">Primary</span>
		<span class="badge rounded-pill bg-secondary">Secondary</span>
		<span class="badge rounded-pill bg-success">Success</span>
		<span class="badge rounded-pill bg-danger">Danger</span>
		<span class="badge rounded-pill bg-warning">Warning</span>
		<span class="badge rounded-pill bg-info">Info</span>
		<span class="badge rounded-pill bg-light">Light</span>
		<span class="badge rounded-pill bg-dark">Dark</span>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172632798-f10e2a78-8b88-4ab2-9bed-df43100a7ab4.png)

``` html
	<!-- Badge inside a Button -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Badges | Progress Bars</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Badge inside a Button</h2>
		<button type="button" class="btn btn-primary">
		  Messages <span class="badge bg-danger">4</span>
		</button>
		<button type="button" class="btn btn-danger">
		  Notifications <span class="badge bg-dark">7</span>
		</button>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172632863-b2ee6297-0297-449d-9efe-551282aab0d4.png)

</details>

### Progress Bar 
<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- Progress bars -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Badges | Progress Bars</title>
	</head>
	<body>
	    <div class="container mt-3">
		<p>A progress bar can be used to show how far a user is in a process.</p>
		<h2>Basic Progress Bar</h2>
		<p>To create a default progress bar, add a .progress class to a container element and add the progress-bar class to its child element. Use the CSS width property to set the width of the progress bar:</p>
		<div class="progress">
		    <div class="progress-bar" style="width:70%"></div>
		</div>
		<p>width indicates progresses.</p>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172638653-59d656ab-b9ad-4606-8455-a5d17300d869.png)	
	
``` html
	<!-- Progress Bar Height -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Badges | Progress Bars</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Progress Bar Height</h2>
		<p>The height of the progress bar is 1rem (16px) by default. Use the CSS height property to change the height:</p> 
		<div class="progress" style="height:10px">
		    <div class="progress-bar" style="width:40%;height:10px">40%</div>
		</div>
		<br>
		<div class="progress" style="height:20px">
		    <div class="progress-bar" style="width:50%;height:20px">50%</div>
		</div>
		<br>
		<div class="progress" style="height:30px">
		    <div class="progress-bar" style="width:60%;height:30px">60%</div>
		</div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172638741-2cc75fa4-7e3d-482c-8753-c7f8fa0a3a57.png)
	
``` html
	<!-- Colored Progress Bars -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Badges | Progress Bars</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Colored Progress Bars</h2>
		<p>Use any of the contextual color classes to change the color of the progress bar:</p> 
		<!-- Blue -->
		<div class="progress">
		    <div class="progress-bar" style="width:10%"></div>
		</div><br>

		<!-- Green -->
		<div class="progress">
		    <div class="progress-bar bg-success" style="width:20%"></div>
		</div><br>

		<!-- Turquoise -->
		<div class="progress">
		    <div class="progress-bar bg-info" style="width:30%"></div>
		</div><br>

		<!-- Orange -->
		<div class="progress">
		    <div class="progress-bar bg-warning" style="width:40%"></div>
		</div><br>

		<!-- Red -->
		<div class="progress">
		    <div class="progress-bar bg-danger" style="width:50%"></div>
		</div><br>

		<!-- White -->
		<div class="progress border">
		    <div class="progress-bar bg-white" style="width:60%"></div>
		</div><br>

		<!-- Grey -->
		<div class="progress">
		    <div class="progress-bar bg-secondary" style="width:70%"></div>
		</div><br>

		<!-- Light Grey -->
		<div class="progress border">
		    <div class="progress-bar bg-light" style="width:80%"></div>
		</div><br>

		<!-- Dark Grey -->
		<div class="progress">
		    <div class="progress-bar bg-dark" style="width:90%"></div>
		</div>
	    </div>
	</body>
	</html>
	
```	
![image](https://user-images.githubusercontent.com/75599178/172638836-54df12ea-7caa-448c-9101-002e741aa776.png)
	
``` html
	<!-- Striped Progress Bars -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Badges | Progress Bars</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Striped Progress Bars</h2>
		<p>The .progress-bar-striped class adds stripes to the progress bars:</p> 
		<div class="progress">
		    <div class="progress-bar progress-bar-striped" style="width:30%"></div>
		</div>
		<br>
		<div class="progress">
		    <div class="progress-bar bg-success progress-bar-striped" style="width:40%"></div>
		</div>
		<br>
		<div class="progress">
		    <div class="progress-bar bg-info progress-bar-striped" style="width:50%"></div>
		</div>
		<br>
		<div class="progress">
		    <div class="progress-bar bg-warning progress-bar-striped" style="width:60%"></div>
		</div>
		<br>
		<div class="progress">
		    <div class="progress-bar bg-danger progress-bar-striped" style="width:70%"></div>
		</div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172639001-c3030749-05c1-4209-a676-bd0502c7f9fd.png)

	
``` html
	<!-- Animated Progress Bar -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Badges | Progress Bars</title>
	</head>
	<body>
	    <div class="container mt-3 mb-4">
		<h2>Animated Progress Bar</h2>
		<p>Add the .progress-bar-animated class to animate the progress bar:</p> 
		<div class="progress">
		    <div class="progress-bar progress-bar-striped progress-bar-animated" style="width:40%"></div>
		</div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172639105-efa8ffd3-8bab-44c0-b25e-86f4432f3770.png)
	

</details>

### Pagination

<details>
	<summary>:bulb:</summary>

``` html
	<!-- Pagination -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Pagination</h2>
		<p>To create a basic pagination, add the .pagination class to an ul element. Then add the .page-item to each li element and a .page-link class to each link inside li:</p>                  
		<ul class="pagination">
		  <li class="page-item"><a class="page-link" href="#">Previous</a></li>
		  <li class="page-item"><a class="page-link" href="#">1</a></li>
		  <li class="page-item"><a class="page-link" href="#">2</a></li>
		  <li class="page-item"><a class="page-link" href="#">3</a></li>
		  <li class="page-item"><a class="page-link" href="#">Next</a></li>
		</ul>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172673217-b67893a8-8455-4f2c-ba3d-dd63af2c5958.png)
	
``` html
	<!-- Active State -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Active State Pagination</h2>
		<p>Add class .active to let the user know which page he/she is on:</p>
		<ul class="pagination">
		    <li class="page-item"><a class="page-link" href="#">Previous</a></li>
		    <li class="page-item"><a class="page-link" href="#">1</a></li>
		    <li class="page-item active"><a class="page-link" href="#">2</a></li>
		    <li class="page-item"><a class="page-link" href="#">3</a></li>
		    <li class="page-item"><a class="page-link" href="#">Next</a></li>
		</ul>
	      </div>
	</body>
	</html>
	
```
![image](https://user-images.githubusercontent.com/75599178/172673404-5dbfe32b-26bd-4ac8-a832-e598ef0b55c9.png)
	
``` html
	<!-- Disabled State -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Disabled State Pagination</h2>
		<p>Add class .disabled if a page for some reason is disabled:</p>
		<ul class="pagination">
		    <li class="page-item disabled"><a class="page-link" href="#">Previous</a></li>
		    <li class="page-item"><a class="page-link" href="#">1</a></li>
		    <li class="page-item"><a class="page-link" href="#">2</a></li>
		    <li class="page-item"><a class="page-link" href="#">3</a></li>
		    <li class="page-item"><a class="page-link" href="#">Next</a></li>
		</ul>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172673451-4d9974f3-3013-4f38-8118-e31588a1cf9f.png)
	
``` html
	<!-- Pagination Sizing -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Pagination Sizing</h2>
		<p>Add class .pagination-lg for larger blocks or .pagination-sm for smaller blocks.</p>
		<p>Large:</p>
		<ul class="pagination pagination-lg">
		    <li class="page-item"><a class="page-link" href="#">Previous</a></li>
		    <li class="page-item"><a class="page-link" href="#">1</a></li>
		    <li class="page-item"><a class="page-link" href="#">2</a></li>
		    <li class="page-item"><a class="page-link" href="#">3</a></li>
		    <li class="page-item"><a class="page-link" href="#">Next</a></li>
		</ul>

		<p>Default:</p>
		<ul class="pagination">
		    <li class="page-item"><a class="page-link" href="#">Previous</a></li>
		    <li class="page-item"><a class="page-link" href="#">1</a></li>
		    <li class="page-item"><a class="page-link" href="#">2</a></li>
		    <li class="page-item"><a class="page-link" href="#">3</a></li>
		    <li class="page-item"><a class="page-link" href="#">Next</a></li>
		</ul>

		<p>Small:</p>
		<ul class="pagination pagination-sm">
		    <li class="page-item"><a class="page-link" href="#">Previous</a></li>
		    <li class="page-item"><a class="page-link" href="#">1</a></li>
		    <li class="page-item"><a class="page-link" href="#">2</a></li>
		    <li class="page-item"><a class="page-link" href="#">3</a></li>
		    <li class="page-item"><a class="page-link" href="#">Next</a></li>
		</ul>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172673502-7b41c847-0186-4616-8a58-a25bcfbc83cd.png)
	
``` html
	<!-- Pagination Alignment -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Pagination Alignment</h2>
		<p>Use utilitiy classes to change the alignment of the pagination:</p>                  
		<ul class="pagination">
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">Previous</a></li>
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">1</a></li>
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">2</a></li>
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">Next</a></li>
		</ul>
		<ul class="pagination justify-content-center">
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">Previous</a></li>
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">1</a></li>
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">2</a></li>
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">Next</a></li>
		</ul>
		<ul class="pagination justify-content-end">
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">Previous</a></li>
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">1</a></li>
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">2</a></li>
		    <li class="page-item"><a class="page-link" href="javascript:void(0);">Next</a></li>
		</ul>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172673560-e606e9e8-eb97-4f4b-b2d2-de25f7d9fbb2.png)
	
``` html
	<!-- Breadcrumbs -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3">
		<h2>Breadcrumbs</h2>
		<p>The .breadcrumb class indicates the current page's location within a navigational hierarchy:</p>                  
		<ul class="breadcrumb">
		    <li class="breadcrumb-item"><a href="#">Photos</a></li>
		    <li class="breadcrumb-item"><a href="#">Summer 2017</a></li>
		    <li class="breadcrumb-item"><a href="#">Italy</a></li>
		    <li class="breadcrumb-item active">Rome</li>
		</ul>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172673633-ce02b33e-db4d-4a4a-8631-b980f7736bf5.png)
	
</details>

### List Groups

<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- List Group -->>
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3 mb-3">
		<h2>Basic List Group</h2>
		<ul class="list-group">
		  <li class="list-group-item">First item</li>
		  <li class="list-group-item">Second item</li>
		  <li class="list-group-item">Third item</li>
		</ul>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172750040-8c9d29d6-4a29-4e85-b344-5acd3b8f0004.png)
	
``` html
	<!-- List Group Active State-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3 mb-3">
		<h2>Active Item in a List Group</h2>
		<ul class="list-group">
		    <li class="list-group-item active">Active item</li>
		    <li class="list-group-item">Second item</li>
		    <li class="list-group-item">Third item</li>
		</ul>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172750075-1377c8ba-6d3d-4824-8b1b-50c7d23b60d1.png)
	
``` html
	<!-- List Group With Linked Items-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3 mb-3">
		<h2>List Group With Linked Items</h2>
		<div class="list-group">
		    <a href="#" class="list-group-item list-group-item-action">First item</a>
		    <a href="#" class="list-group-item list-group-item-action">Second item</a>
		    <a href="#" class="list-group-item list-group-item-action">Third item</a>
		</div>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172750117-a00cd2d9-dc98-46a4-b84e-5cd4d1c1d286.png)

``` html
	<!-- List Group With a Disabled Item-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3 mb-3">
		<h2>List Group With a Disabled Item</h2>
		<p>The disabled class adds a lighter text color to the disabled item. And if used on links, it will remove the default hover effect.</p>
		<div class="list-group">
		    <a href="#" class="list-group-item disabled">Disabled item</a>
		    <a href="#" class="list-group-item disabled">Disabled item</a>
		    <a href="#" class="list-group-item">Third item</a>
		</div>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172750163-07086951-8961-4981-929f-d27c0d466dab.png)
	
``` html
	<!-- Flush / Remove Borders-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3 mb-3">
		<h2>Flush / Remove Borders</h2>
		<p>Use the .list-group-flush class to remove some borders and rounded corners:</p>
	    </div>

	    <div class="container mt-3 mb-3">
		<ul class="list-group list-group-flush">
		    <li class="list-group-item">First item</li>
		    <li class="list-group-item">Second item</li>
		    <li class="list-group-item">Third item</li>
		    <li class="list-group-item">Fourth item</li>
		  </ul>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172750213-7a6895ff-1811-4777-9761-6288ab54286a.png)

``` html
	<!-- Numbered List Groups -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3 mb-3">
		<h2>Numbered List Group</h2>
		<p>Use the .list-group-numbered class to create list items with numbers in front of them:</p>
	    </div>

	    <div class="container mt-3 mb-3">
		<ol class="list-group list-group-numbered">
		    <li class="list-group-item">First item</li>
		    <li class="list-group-item">Second item</li>
		    <li class="list-group-item">Third item</li>
		</ol>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172750244-21069770-587c-42b0-9a0e-e22984672eda.png)
	
``` html
	<!-- Horizontal List Groups -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3 mb-3">
		<h2>Horizontal List Groups</h2>
		<p>The .list-group-horizontal class displays the list items horizontally instead of vertically:</p>
	    </div>

	    <div class="container mt-3 mb-3">
		<ul class="list-group list-group-horizontal">
		    <li class="list-group-item">First item</li>
		    <li class="list-group-item">Second item</li>
		    <li class="list-group-item">Third item</li>
		    <li class="list-group-item">Fourth item</li>
		</ul>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172750272-c9dc78be-7b07-480f-9a8d-69efe399a42d.png)
	
``` html
	<!-- List Group With Badges -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Pagination | Lists</title>
	</head>
	<body>
	    <div class="container mt-3 mb-3">
		<h2>List Group With Badges</h2>
		<p>Combine .badge classes with utility/helper classes to add badges inside the list group:</p>
	    </div>

	    <div class="container mt-3 mb-3">
		<ul class="list-group">
		    <li class="list-group-item d-flex justify-content-between align-items-center">
		      Inbox
		      <span class="badge bg-primary rounded-pill">12</span>
		    </li>
		    <li class="list-group-item d-flex justify-content-between align-items-center">
		      Ads
		      <span class="badge bg-primary rounded-pill">50</span>
		    </li>
		    <li class="list-group-item d-flex justify-content-between align-items-center">
		      Junk
		      <span class="badge bg-primary rounded-pill">99</span>
		    </li>
		</ul>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172750322-50c1cc6d-4495-48ab-ae7c-31bffc38e8af.png)	

</details>

### Cards

<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- Basic Card-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Basic Card</h2>
	      <div class="card">
		<div class="card-body">Basic card</div>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172761210-e1d306ab-3453-45af-b148-7696be37815f.png)
		
``` html
	<!-- Header and Footer-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Card Header and Footer</h2>
	      <div class="card">
		<div class="card-header">Header</div>
		<div class="card-body">Content</div> 
		<div class="card-footer">Footer</div>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172761254-283760d3-bfe4-4e62-b310-ef1c7b038473.png)

``` html
	<!-- Cards with Contextual Classes-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Cards with Contextual Classes</h2>
	      <div class="card">
		<div class="card-body">Basic card</div>
	      </div>
	      <br>
	      <div class="card bg-primary text-white">
		<div class="card-body">Primary card</div>
	      </div>
	      <br>
	      <div class="card bg-success text-white">
		<div class="card-body">Success card</div>
	      </div>
	      <br>
	      <div class="card bg-info text-white">
		<div class="card-body">Info card</div>
	      </div>
	      <br>
	      <div class="card bg-warning text-white">
		<div class="card-body">Warning card</div>
	      </div>
	      <br>
	      <div class="card bg-danger text-white">
		<div class="card-body">Danger card</div>
	      </div>
	      <br>
	      <div class="card bg-secondary text-white">
		<div class="card-body">Secondary card</div>
	      </div>
	      <br>
	      <div class="card bg-dark text-white">
		<div class="card-body">Dark card</div>
	      </div>
	      <br>
	      <div class="card bg-light text-dark">
		<div class="card-body">Light card</div>
	      </div>
	    </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172761297-e35ce124-ad07-4365-95e1-26b79ba0b0f3.png)
		
``` html
	<!-- Card titles, text, and links-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Card titles, text, and links</h2>
	      <p>Use .card-title to add card titles to any heading element. The .card-text class is used to remove bottom margins for a p element if it is the last child (or the only one) in card-body. The .card-link class adds a blue color to any link, and a hover effect.</p>
	      <div class="card">
		<div class="card-body">
		  <h4 class="card-title">Card title</h4>
		  <p class="card-text">Some example text. Some example text.</p>
		  <a href="#" class="card-link">Card link</a>
		  <a href="#" class="card-link">Another link</a>
		</div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172761346-9fc04958-489a-4e47-a7d4-0792381b2618.png)
		
``` html
	<!-- Card Image-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Card Image</h2>
	      <p>Image at the top (card-img-top):</p>
	      <div class="card" style="width:400px">
		<img class="card-img-top" src="./Images/man.png" alt="Card image" style="width:100%">
		<div class="card-body">
		  <h4 class="card-title">John Doe</h4>
		  <p class="card-text">Some example text some example text. John Doe is an architect and engineer</p>
		  <a href="#" class="btn btn-primary">See Profile</a>
		</div>
	      </div>
	      <br>

	      <p>Image at the bottom (card-img-bottom):</p>
	      <div class="card" style="width:400px">
		<div class="card-body">
		  <h4 class="card-title">Jane Doe</h4>
		  <p class="card-text">Some example text some example text. Jane Doe is an architect and engineer</p>
		  <a href="#" class="btn btn-primary">See Profile</a>
		</div>
		<img class="card-img-bottom" src="./Images/man.png" alt="Card image" style="width:100%">
	      </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172761420-5389677c-1cde-4ba8-a85d-ae3266674ef3.png)

![image](https://user-images.githubusercontent.com/75599178/172761445-c3f06179-466a-4730-b985-dc718e0723a3.png)

``` html
	<!-- Card Image Overlay-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Card Image Overlay</h2>
	      <p>Turn an image into a card background and use .card-img-overlay to overlay the card's text:</p>
	      <div class="card img-fluid" style="width:500px">
		<img class="card-img-top" src="./Images/man.png" alt="Card image" style="width:100%">
		<div class="card-img-overlay">
		  <h4 class="card-title">John Doe</h4>
		  <p class="card-text">Some example text some example text. Some example text some example text. Some example text some example text. Some example text some example text.</p>
		  <a href="#" class="btn btn-primary">See Profile</a>
		</div>
	      </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172761487-082b2ad4-3378-497a-a23e-2ec48572e016.png)
	
</details>
		
### Dropdown
		
<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- Dropdowns-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	  <div class="container mt-3 mb-5">
	    <h2>Dropdowns</h2>
	    <p>The .dropdown class is used to indicate a dropdown menu.</p>
	    <p>Use the .dropdown-menu class to actually build the dropdown menu.</p>
	    <p>To open the dropdown menu, use a button or a link with a class of .dropdown-toggle and data-toggle="dropdown".</p>                                          
	    <div class="dropdown">
	      <button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
		Dropdown button
	      </button>
	      <ul class="dropdown-menu">
		<li><a class="dropdown-item" href="#">Link 1</a></li>
		<li><a class="dropdown-item" href="#">Link 2</a></li>
		<li><a class="dropdown-item" href="#">Link 3</a></li>
	      </ul>
	    </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172788277-1bbb2036-4fbf-4408-ace0-01316156e754.png)
	
``` html
	<!-- Dropdown divider-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3 mb-5">
	      <h2>Dropdowns</h2>
	      <p>The .dropdown-divider class is used to separate links inside the dropdown menu with a thin horizontal line:</p>

	      <div class="dropdown">
		<button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
		  Dropdown button
		</button>
		<ul class="dropdown-menu">
		  <li><a class="dropdown-item" href="#">Link 1</a></li>
		  <li><a class="dropdown-item" href="#">Link 2</a></li>
		  <li><a class="dropdown-item" href="#">Link 3</a></li>
		  <li><hr class="dropdown-divider"></li>
		  <li><a class="dropdown-item" href="#">Another link</a></li>
		</ul>
	      </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172788604-f71e324b-27d7-41e7-acaf-5bf6095b1a8d.png)

``` html
	<!-- Dropdown header-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Dropdown header</h2>
	      <p>The .dropdown-header class is used to add headers inside the dropdown menu:</p>

	      <div class="dropdown">
		<button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
		  Dropdown button
		</button>
		<ul class="dropdown-menu">
		  <li><h5 class="dropdown-header">Dropdown header 1</h5></li>
		  <li><a class="dropdown-item" href="#">Link 1</a></li>
		  <li><a class="dropdown-item" href="#">Link 2</a></li>
		  <li><a class="dropdown-item" href="#">Link 3</a></li>
		  <li><h5 class="dropdown-header">Dropdown header 2</h5></li>
		  <li><a class="dropdown-item" href="#">Another link</a></li>
		</ul>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172789061-4c351c2f-06f7-4654-8902-00198cba930b.png)

``` html
	<!-- Dropdown Active state-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Dropdowns</h2>
	      <p>The .active class adds a blue background color to the active link.</p>
	      <p>The .disabled class disables a dropdown item (grey text color and a no-parking-sign on hover).</p>

	      <div class="dropdown">
		<button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
		  Dropdown button
		</button>
		<ul class="dropdown-menu">
		  <li><a class="dropdown-item" href="#">Normal</a></li>
		  <li><a class="dropdown-item active" href="#">Active</a></li>
		  <li><a class="dropdown-item disabled" href="#">Disabled</a></li>
		</ul>
	      </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172789595-fd118e8a-0b8d-4bd7-9028-f719e0dc75aa.png)

``` html
	<!-- Dropend - Dropstart-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Dropend - Dropstart</h2>
	      <p>Add the .dropend class next to the dropdown menu to right-align the dropdown. Note that the caret/arrows is added automatically:</p>
	      <p>Add the .dropstart class next to the dropdown menu to left-align the dropdown. Note that the caret/arrow is added automatically. Also note that we float the dropdown to the right:</p>

	      <div class="dropdown dropend">
		<button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
		  Dropend
		</button>
		<ul class="dropdown-menu">
		  <li><a class="dropdown-item" href="#">Normal</a></li>
		  <li><a class="dropdown-item active" href="#">Active</a></li>
		  <li><a class="dropdown-item disabled" href="#">Disabled</a></li>
		</ul>
	      </div>

	      <div class="dropdown dropstart text-end">
		<button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
		  Dropstart
		</button>
		<ul class="dropdown-menu">
		  <li><a class="dropdown-item" href="#">Normal</a></li>
		  <li><a class="dropdown-item active" href="#">Active</a></li>
		  <li><a class="dropdown-item disabled" href="#">Disabled</a></li>
		</ul>
	      </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172789939-0d298d77-dd0c-4ada-a1b2-884eae9b9520.png)
![image](https://user-images.githubusercontent.com/75599178/172789998-1245d103-7197-45ec-b6c2-754a26e58896.png)

``` html
	<!-- Dropdown Menu Right-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3 mb-3">
	      <h2>Dropdown Menu Right</h2>
	      <p>Add the .dropdown-menu-end class to .dropdown-menu to right-align the dropdown menu.</p>

	      <div class="dropdown dropdown-menu-end">
		<button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
		  Wide dropdown button to demonstrate this example
		</button>
		<ul class="dropdown-menu">
		  <li><a class="dropdown-item" href="#">Link 1</a></li>
		  <li><a class="dropdown-item" href="#">Link 2</a></li>
		  <li><a class="dropdown-item" href="#">Link 3</a></li>
		</ul>
	      </div>
	  </div>
	</body>
	</html>
```		
![image](https://user-images.githubusercontent.com/75599178/172790350-d1e26129-e7de-4e2e-9212-b8aa295b54d4.png)

``` html
	<!-- Dropup-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Dropup</h2>
	      <p>The .dropup class makes the dropdown menu expand upwards instead of downwards:</p>
	      <p>It must be room for the dropup menu to grow. That is why we add some extra lorem ipsum text.</p>
	      <p>Lorem ipsum one more time!</p>

	      <div class="dropup">
		<button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
		  Dropup button
		</button>
		<ul class="dropdown-menu">
		  <li><a class="dropdown-item" href="#">Link 1</a></li>
		  <li><a class="dropdown-item" href="#">Link 2</a></li>
		  <li><a class="dropdown-item" href="#">Link 3</a></li>
		</ul>
	      </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172790685-04dbb40e-4a72-48dc-bc0d-f740a88471bd.png)

``` html
	<!-- Dropdown Text-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Cards | Dropdowns</title>
	</head>
	<body>
	    <div class="container mt-3">
	      <h2>Dropdown Text</h2>
	      <button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
		Dropdown button
	      </button>
	      <ul class="dropdown-menu">
		<li><a class="dropdown-item" href="#">Link 1</a></li>
		<li><a class="dropdown-item" href="#">Link 2</a></li>
		<li><a class="dropdown-item" href="#">Link 3</a></li>
		<li><a class="dropdown-item-text" href="#">Text Link</a></li>
		<li><span class="dropdown-item-text">Just Text</span></li>
	      </ul>
	    </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/172790944-982e3810-621e-4e81-a0c6-6a5d905be0f8.png)
		
</details>

### Accordion

<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- Simple collapse-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Bootstrap Example</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body>

	<div class="container mt-3">
	  <h2>Simple Collapsible</h2>
	  <p>Click on the button to toggle between showing and hiding content.</p>
	  <button type="button" class="btn btn-primary" data-bs-toggle="collapse" data-bs-target="#demo">Simple collapsible</button>
	  <div id="demo" class="collapse">
	    Lorem ipsum dolor sit amet, consectetur adipisicing elit,
	    sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
	    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
	  </div>
	</div>

	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173309601-1f45926f-e48d-4980-bd81-7ea48434218c.png)

``` html	
	<!-- Accordion-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Accordion</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body>

	<div class="container mt-3">
	  <h2>Accordion Example</h2>
	  <p><strong>Note:</strong> The <strong>data-bs-parent</strong> attribute makes sure that all collapsible elements under the specified parent will be closed when one of the collapsible item is shown.</p>
	  <div id="accordion">
	    <div class="card">
	      <div class="card-header">
		<a class="btn" data-bs-toggle="collapse" href="#collapseOne">
		  Collapsible Group Item #1
		</a>
	      </div>
	      <div id="collapseOne" class="collapse show" data-bs-parent="#accordion">
		<div class="card-body">
		  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
		</div>
	      </div>
	    </div>
	    <div class="card">
	      <div class="card-header">
		<a class="collapsed btn" data-bs-toggle="collapse" href="#collapseTwo">
		Collapsible Group Item #2
	      </a>
	      </div>
	      <div id="collapseTwo" class="collapse" data-bs-parent="#accordion">
		<div class="card-body">
		  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
		</div>
	      </div>
	    </div>
	    <div class="card">
	      <div class="card-header">
		<a class="collapsed btn" data-bs-toggle="collapse" href="#collapseThree">
		  Collapsible Group Item #3
		</a>
	      </div>
	      <div id="collapseThree" class="collapse" data-bs-parent="#accordion">
		<div class="card-body">
		  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
		</div>
	      </div>
	    </div>
	  </div>
	</div>

	</body>
	</html>
```	
![image](https://user-images.githubusercontent.com/75599178/173309772-56440cfd-8d26-465d-9010-78e5db0217ce.png)

</details>

### Carousel

<details>
	<summary>:bulb:</summary>

``` html
	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Bootstrap Example</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body>

	<!-- Carousel -->
	<div id="demo" class="carousel slide" data-bs-ride="carousel">

	  <!-- Indicators/dots -->
	  <div class="carousel-indicators">
	    <button type="button" data-bs-target="#demo" data-bs-slide-to="0" class="active"></button>
	    <button type="button" data-bs-target="#demo" data-bs-slide-to="1"></button>
	    <button type="button" data-bs-target="#demo" data-bs-slide-to="2"></button>
	  </div>

	  <!-- The slideshow/carousel -->
	  <div class="carousel-inner">
	    <div class="carousel-item active">
	      <img src="./Images/1.jpg" alt="Los Angeles" class="d-block" style="width:100%">
	    </div>
	    <div class="carousel-item">
	      <img src="./Images/2.jpg" alt="Chicago" class="d-block" style="width:100%">
	    </div>
	    <div class="carousel-item">
	      <img src="./Images/3.jpg" alt="New York" class="d-block" style="width:100%">
	    </div>
	  </div>

	  <!-- Left and right controls/icons -->
	  <button class="carousel-control-prev" type="button" data-bs-target="#demo" data-bs-slide="prev">
	    <span class="carousel-control-prev-icon"></span>
	  </button>
	  <button class="carousel-control-next" type="button" data-bs-target="#demo" data-bs-slide="next">
	    <span class="carousel-control-next-icon"></span>
	  </button>
	</div>

	<div class="container-fluid mt-3">
	  <h3>Carousel Example</h3>
	  <p>The following example shows how to create a basic carousel with indicators and controls.</p>
	</div>

	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173334128-f4991e09-e432-4d12-910a-684a694fd96c.png)

![image](https://user-images.githubusercontent.com/75599178/173334046-cec2ada8-c017-415b-b23c-e09fb7781634.png)

</details>

### Navigation Tab

<details>
	<summary>:bulb:</summary>
	
``` html
	<!-- Toggable Tab -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Navigation Bar</title>
	</head>
	<body>
	    <h2>Toggleable Tabs</h2>
	  <br>
	  <!-- Nav tabs -->
	  <ul class="nav nav-tabs" role="tablist">
	    <li class="nav-item">
	      <a class="nav-link active" data-bs-toggle="tab" href="#home">Home</a>
	    </li>
	    <li class="nav-item">
	      <a class="nav-link" data-bs-toggle="tab" href="#menu1">Menu 1</a>
	    </li>
	    <li class="nav-item">
	      <a class="nav-link" data-bs-toggle="tab" href="#menu2">Menu 2</a>
	    </li>
	  </ul>

	  <!-- Tab panes -->
	  <div class="tab-content">
	    <div id="home" class="container tab-pane active"><br>
	      <h3>HOME</h3>
	      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
	    </div>
	    <div id="menu1" class="container tab-pane fade"><br>
	      <h3>Menu 1</h3>
	      <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
	    </div>
	    <div id="menu2" class="container tab-pane fade"><br>
	      <h3>Menu 2</h3>
	      <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam.</p>
	    </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173335115-654e2380-9c19-4860-a9f7-ec86c8ca3b75.png)

``` html
	<!-- Toggleable Pills -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Navigation Bar</title>
	</head>
	<body>
	    <h2>Toggleable Pills</h2>
	  <br>
	    <!-- Nav pills -->
	    <ul class="nav nav-pills" role="tablist">
		<li class="nav-item">
		<a class="nav-link active" data-bs-toggle="pill" href="#home">Home</a>
		</li>
		<li class="nav-item">
		<a class="nav-link" data-bs-toggle="pill" href="#menu1">Menu 1</a>
		</li>
		<li class="nav-item">
		<a class="nav-link" data-bs-toggle="pill" href="#menu2">Menu 2</a>
		</li>
	    </ul>

	    <!-- Tab panes -->
	    <div class="tab-content">
		<div id="home" class="container tab-pane active"><br>
		    <h3>HOME</h3>
		    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
		</div>
		<div id="menu1" class="container tab-pane fade"><br>
		    <h3>Menu 1</h3>
		    <p>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
		</div>
		<div id="menu2" class="container tab-pane fade"><br>
		    <h3>Menu 2</h3>
		    <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam.</p>
		</div>
	    </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173335971-3e203cfd-220d-49f2-81fd-2b94b5f29158.png)

``` html
	<!---- vertical nav bar -->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	    <title>Navigation Bar</title>
	</head>
	<body>
	  <br>
	    <!-- vertical nav bar -->
	    <nav class="navbar bg-light">
		<div class="container-fluid">
		  <ul class="navbar-nav">
		    <li class="nav-item">
		      <a class="nav-link" href="#">Link 1</a>
		    </li>
		    <li class="nav-item">
		      <a class="nav-link" href="#">Link 2</a>
		    </li>
		    <li class="nav-item">
		      <a class="nav-link" href="#">Link 3</a>
		    </li>
		  </ul>
		</div>
	      </nav>

	      <div class="container-fluid mt-3">
		<h3>Vertical Navbar Example</h3>
		<p>A navigation bar is a navigation header that is placed at the top of the page.</p>
	      </div>
	  </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173336252-1e46386d-0bda-4092-b11a-11398eecade5.png)

``` html
	<!-- Fixed top nav bar -->

	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Navigation Bar</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body style="height:1500px">

	<nav class="navbar navbar-expand-sm bg-dark navbar-dark fixed-top">
	  <div class="container-fluid">
	    <a class="navbar-brand" href="#">Fixed top</a>
	  </div>
	</nav>

	<div class="container-fluid" style="margin-top:80px">
	  <h3>Top Fixed Navbar</h3>
	  <p>A fixed navigation bar stays visible in a fixed position (top or bottom) independent of the page scroll.</p>
	  <h1>Scroll this page to see the effect</h1>
	</div>

	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173344446-77c14684-a834-4198-beb4-aaa96538c22e.png)

``` html
	<!-- Fixed bottom nav bar-->

	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Navigation Bar</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body style="height:1500px">

	<nav class="navbar navbar-expand-sm bg-dark navbar-dark fixed-bottom">
	  <div class="container-fluid">
	    <a class="navbar-brand" href="#">Fixed bottom</a>
	  </div>
	</nav>

	<div class="container-fluid" style="margin-top:80px">
	  <h3>Top Fixed Navbar</h3>
	  <p>A fixed navigation bar stays visible in a fixed position (top or bottom) independent of the page scroll.</p>
	  <h1>Scroll this page to see the effect</h1>
	</div>

	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173344623-5dff61c4-b183-49eb-974a-2778cab4fd1f.png)

``` html
	<!-- sticky top nav bar-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Navigation Bar</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body style="height:1500px">

	<br>
	  <h3>Sticky Navbar</h3>
	  <p>A sticky navigation bar stays fixed at the top of the page when you scroll past it.</p>
	  <p>Scroll this page to see the effect. <strong>Note:</strong> sticky-top does not work in IE11 and earlier.</p>
	</div>

	<nav class="navbar navbar-expand-sm bg-dark navbar-dark sticky-top">
	  <div class="container-fluid">
	    <a class="navbar-brand" href="#">Sticky top</a>
	  </div>
	</nav>

	<div class="container-fluid"><br>
	  <p>Some example text. Some example text. Some example text. Some example text. Some example text.</p>
	  <p>Some example text. Some example text. Some example text. Some example text. Some example text.</p>
	  <p>Some example text. Some example text. Some example text. Some example text. Some example text.</p>
	  <p>Some example text. Some example text. Some example text. Some example text. Some example text.</p>
	</div>

	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173345272-73aefbd2-542d-448e-89c1-32450defabda.png)

</details>

### Scrollspy

<details>
	<summary>:bulb:</summary>

``` html
	<!-- scrollspy-->

	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Navigation Bar</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>

	  <style>
	    body {
		position: relative; 
	    }
	    </style>

	</head>
	<body data-bs-spy="scroll" data-bs-target=".navbar" data-bs-offset="50">

	<nav class="navbar navbar-expand-sm bg-dark navbar-dark fixed-top">
	  <div class="container-fluid">
	    <ul class="navbar-nav">
	      <li class="nav-item">
		<a class="nav-link" href="#section1">Section 1</a>
	      </li>
	      <li class="nav-item">
		<a class="nav-link" href="#section2">Section 2</a>
	      </li>
	      <li class="nav-item">
		<a class="nav-link" href="#section3">Section 3</a>
	      </li>
	    </ul>
	  </div>
	</nav>

	<div id="section1" class="container-fluid bg-success text-white" style="padding:600px 20px;">
	  <h1>Section 1</h1>
	  <p>Try to scroll this section and look at the navigation bar while scrolling! Try to scroll this section and look at the navigation bar while scrolling!</p>
	  <p>Try to scroll this section and look at the navigation bar while scrolling! Try to scroll this section and look at the navigation bar while scrolling!</p>
	</div>

	<div id="section2" class="container-fluid bg-warning" style="padding:600px 20px;">
	  <h1>Section 2</h1>
	  <p>Try to scroll this section and look at the navigation bar while scrolling! Try to scroll this section and look at the navigation bar while scrolling!</p>
	  <p>Try to scroll this section and look at the navigation bar while scrolling! Try to scroll this section and look at the navigation bar while scrolling!</p>
	</div>

	<div id="section3" class="container-fluid bg-secondary text-white" style="padding:600px 20px;">
	  <h1>Section 3</h1>
	  <p>Try to scroll this section and look at the navigation bar while scrolling! Try to scroll this section and look at the navigation bar while scrolling!</p>
	  <p>Try to scroll this section and look at the navigation bar while scrolling! Try to scroll this section and look at the navigation bar while scrolling!</p>
	</div>

	</body>
	</html>

	<pre>
	    Example Explained :

	    Add data-bs-spy="scroll" to the element that should be used as the scrollable area (often this is the <body> element).

	    Then add the data-bs-target attribute with a value of the id or the class name of the navigation bar (.navbar). This is to make sure that the navbar is connected with the scrollable area.

	    Note : that scrollable elements must match the ID of the links inside the navbar's list items.

	    The optional data-bs-offset attribute specifies the number of pixels to offset from top when calculating the position of scroll. This is useful when you feel that the links inside the navbar changes the active state too soon or too early when jumping to the scrollable elements. Default is 10 pixels.

	    Requires relative positioning: The element with data-bs-spy="scroll" requires the CSS position property, with a value of "relative" to work properly.


	</pre>
```
![image](https://user-images.githubusercontent.com/75599178/173503513-e4cd35b6-9b79-425b-bbc3-a8f7465e523c.png)
![image](https://user-images.githubusercontent.com/75599178/173503650-8d0be7b4-91ec-448e-92bc-8453a0c1b22f.png)
![image](https://user-images.githubusercontent.com/75599178/173503715-73baf945-318e-413c-ac47-3392413f14dc.png)

</details>

### Modal

<details>
	<summary>:bulb:</summary>
	
``` html
	<!--Modal-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <title>Modal</title>
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body>
	    <div class="container mt-3">
		<h3>Modal Example</h3>
		<p>Click on the button to open the modal.</p>

		<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#myModal">
		  Open modal
		</button>
	      </div>

	      <!-- The Modal -->
	      <div class="modal" id="myModal">
		<div class="modal-dialog">
		  <div class="modal-content">

		    <!-- Modal Header -->
		    <div class="modal-header">
		      <h4 class="modal-title">Modal Heading</h4>
		      <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
		    </div>

		    <!-- Modal body -->
		    <div class="modal-body">
		      Modal body..
		    </div>

		    <!-- Modal footer -->
		    <div class="modal-footer">
		      <button type="button" class="btn btn-danger" data-bs-dismiss="modal">Close</button>
		    </div>

		  </div>
		</div>
	      </div>
	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173524164-ae12b0c4-9955-4add-b98f-3195a340eed7.png)
	
``` html
	<!--Modal-animation-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <title>Modal animation</title>
	    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body>
	    <div class="container mt-3">
		<h3>Modal Example</h3>
		<p>Click on the button to open the modal.</p>

		<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#myModal">
		  Open modal
		</button>
	      </div>

	      <!-- The Modal -->
	      <div class="modal fade" id="myModal">
		<div class="modal-dialog">
		  <div class="modal-content">

		    <!-- Modal Header -->
		    <div class="modal-header">
		      <h4 class="modal-title">Modal Heading</h4>
		      <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
		    </div>

		    <!-- Modal body -->
		    <div class="modal-body">
		      Modal body..
		    </div>

		    <!-- Modal footer -->
		    <div class="modal-footer">
		      <button type="button" class="btn btn-danger" data-bs-dismiss="modal">Close</button>
		    </div>

		  </div>
		</div>
	      </div>
	</body>
	</html>
```
	
``` html
	<!--modal size-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Modal size</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body>

	<div class="container mt-3">
	  <h3>Small Modal Example</h3>
	  <p>Click on the button to open the modal.</p>

	  <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#myModal">
	    Open modal
	  </button>
	</div>

	<!-- The Modal -->
	<div class="modal" id="myModal">
	  <div class="modal-dialog modal-sm"> <!--modal-lg  / modal-xl -->
	    <div class="modal-content">

	      <!-- Modal Header -->
	      <div class="modal-header">
		<h4 class="modal-title">Modal Heading</h4>
		<button type="button" class="btn-close" data-bs-dismiss="modal"></button>
	      </div>

	      <!-- Modal body -->
	      <div class="modal-body">
		Modal body..
	      </div>

	      <!-- Modal footer -->
	      <div class="modal-footer">
		<button type="button" class="btn btn-danger" data-bs-dismiss="modal">Close</button>
	      </div>

	    </div>
	  </div>
	</div>


	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173524358-cd329709-037c-46ef-9585-bbc4894d5b19.png)

``` html
	<!--modal scroll-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Modal scroll</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body>

	    <div class="container mt-3">
		<h2>Modal Scroll Example</h2>
		<p>Click on the button to open the modal.</p>

		<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#myModal">
		  Open modal
		</button>
	      </div>

	      <!-- The Modal -->
	      <div class="modal" id="myModal">
		<div class="modal-dialog">
		  <div class="modal-content">

		    <!-- Modal Header -->
		    <div class="modal-header">
		      <h4 class="modal-title">Modal Heading</h4>
		      <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
		    </div>

		    <!-- Modal body -->
		    <div class="modal-body">
		      <h3>Some text to enable scrolling..</h3>
		      <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
		      <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>

		      <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p> 
		    </div>

		    <!-- Modal footer -->
		    <div class="modal-footer">
		      <button type="button" class="btn btn-danger" data-bs-dismiss="modal">Close</button>
		    </div>

		  </div>
		</div>
	      </div>


	</body>
	</html>

```
![image](https://user-images.githubusercontent.com/75599178/173524660-676037c2-953c-4587-a20c-2f4f1d7a9c2b.png)

``` html
	<!--modal dialog scroll-->
	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <title>Modal scroll</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
	  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
	  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
	</head>
	<body>

	    <div class="container mt-3">
		<h2>Modal Scroll Example</h2>
		<p>Click on the button to open the modal.</p>

		<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#myModal">
		  Open modal
		</button>
	      </div>

	      <!-- The Modal -->
	      <div class="modal" id="myModal">
		<div class="modal-dialog modal-dialog-scrollable">
		  <div class="modal-content">

		    <!-- Modal Header -->
		    <div class="modal-header">
		      <h4 class="modal-title">Modal Heading</h4>
		      <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
		    </div>

		    <!-- Modal body -->
		    <div class="modal-body">
		      <h3>Some text to enable scrolling..</h3>
		      <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
		      <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>

		      <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p> 
		    </div>

		    <!-- Modal footer -->
		    <div class="modal-footer">
		      <button type="button" class="btn btn-danger" data-bs-dismiss="modal">Close</button>
		    </div>

		  </div>
		</div>
	      </div>


	</body>
	</html>
```
![image](https://user-images.githubusercontent.com/75599178/173524813-45ba1ec5-7ff2-4b16-b8be-30da80e1ac98.png)

</details>
		
### Flex
	
<details>
	<summary>:bulb:</summary>
	
``` html

<!--Flex-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Flex</h2>
        <p>To create a flexbox container and transform direct children into flex items, use the d-flex class:</p>
        <div class="d-flex p-3 bg-secondary text-white">
            <div class="p-2 bg-info">Button_1</div>
            <div class="p-2 bg-success">Button_2</div>
            <div class="p-2 bg-warning">Button_3</div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173612795-85e66c0e-dcae-46c5-b9a6-c329d8da752a.png)
	
``` html
<!--Flex-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Inline Flex</h2>
        <p>To create an inline flexbox container, use the d-inline-flex class:</p>
        <div class="d-inline-flex p-3 bg-secondary text-white">
            <div class="p-2 bg-info">Button_1</div>
            <div class="p-2 bg-success">Button_2</div>
            <div class="p-2 bg-warning">Button_3</div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173612853-18c014ea-e772-452d-ab45-434f92cd51b0.png)

``` html

<!--Horizontal direction-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Horizontal direction</h2>
        <p>Use .flex-row to make the flex items appear side by side (default).Use .flex-row-reverse to right-align the horizontal direction.</p>
        <div class="d-flex flex-row bg-secondary">
            <div class="p-2 bg-info">Button_1</div>
            <div class="p-2 bg-success">Button_2</div>
            <div class="p-2 bg-warning">Button_3</div>
        </div>
    </div>
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Horizontal direction</h2>
        <p>Use .flex-row to make the flex items appear side by side (default).Use .flex-row-reverse to right-align the horizontal direction.</p>
        <div class="d-flex flex-row-reverse bg-secondary">
            <div class="p-2 bg-info">Button_1</div>
            <div class="p-2 bg-success">Button_2</div>
            <div class="p-2 bg-warning">Button_3</div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173612998-781881e5-45c2-4044-8533-60238e213407.png)
	
``` html
<!--Vertical direction-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Vertical direction</h2>
        <p>Use .flex-column to make the flex items appear side by side (default).Use .flex-column-reverse to right-align the horizontal direction.</p>
        <div class="d-flex flex-column bg-secondary">
            <div class="p-2 bg-info">Button_1</div>
            <div class="p-2 bg-success">Button_2</div>
            <div class="p-2 bg-warning">Button_3</div>
        </div>
    </div>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Vertical direction</h2>
        <p>Use .flex-column to make the flex items appear side by side (default).Use .flex-column-reverse to right-align the horizontal direction.</p>
        <div class="d-flex flex-column-reverse bg-secondary">
            <div class="p-2 bg-info">Button_1</div>
            <div class="p-2 bg-success">Button_2</div>
            <div class="p-2 bg-warning">Button_3</div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173613080-d6e7bc6d-17f6-4627-8515-8dd5d8d970b0.png)
	
``` html
<!--Justify content-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3 mb-3">
        <h2>Justify content</h2>
        <p>Use the .justify-content-* classes to change the alignment of flex items. Choose from start (default), end, center, between or around:</p>
        <div class="d-flex justify-content-start bg-secondary mb-3">
            <div class="p-2 bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 bg-primary">Flex item 3</div>
          </div>
          <div class="d-flex justify-content-end bg-secondary mb-3">
            <div class="p-2 bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 bg-primary">Flex item 3</div>
          </div>
          <div class="d-flex justify-content-center bg-secondary mb-3">
            <div class="p-2 bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 bg-primary">Flex item 3</div>
          </div>
          <div class="d-flex justify-content-between bg-secondary mb-3">
            <div class="p-2 bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 bg-primary">Flex item 3</div>
          </div>
          <div class="d-flex justify-content-around bg-secondary mb-3">
            <div class="p-2 bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 bg-primary">Flex item 3</div>
          </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173613241-354c42df-4844-464c-9129-4171b71bf024.png)

``` html
<!--Fill / Equal Widths-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Fill / Equal Widths</h2>
        <p>Use .flex-fill on flex items to force them into equal widths:</p>
        <div class="d-flex mb-3">
            <div class="p-2 flex-fill bg-info">Flex item 1</div>
            <div class="p-2 flex-fill bg-warning">Flex item 2</div>
            <div class="p-2 flex-fill bg-primary">Flex item 3</div>
        </div>
        <p>Example without .flex-fill:</p>
        <div class="d-flex mb-3 bg-secondary">
            <div class="p-2 bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 bg-primary">Flex item 3</div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173613328-1844843e-66db-40b1-8fc9-6266f78412a7.png)
	
``` html
<!--Grow-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Grow</h2>
        <p>Use .flex-grow-1 on a flex item to take up the rest of the space:</p>
        <div class="d-flex mb-3">
            <div class="p-2 bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 flex-grow-1 bg-primary">Flex item 3</div>
        </div>
        <p>Example without .flex-grow-1:</p>
        <div class="d-flex mb-3 bg-secondary">
            <div class="p-2 bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 bg-primary">Flex item 3</div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173613626-422f3c9e-84e1-496a-bbaf-b50830b5ac60.png)
	
``` html
<!--Order-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Order</h2>
        <p>Change the visual order of a specific flex item(s) with the .order classes. Valid classes are from 0 to 5:</p>
        <div class="d-flex mb-3">
            <div class="p-2 order-3 bg-info">Flex item 1</div>
            <div class="p-2 order-2 bg-warning">Flex item 2</div>
            <div class="p-2 order-1 bg-primary">Flex item 3</div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173613688-1a745119-950c-442c-ade9-6dc096355134.png)
	
``` html
<!--Auto Margins-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Auto Margins</h2>
        <p>Easily add auto margins to flex items with .mr-auto (push items to the right), or by using .ml-auto (push items to the left):</p>
        <div class="d-flex mb-3 bg-secondary">
            <div class="p-2 ms-auto bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 bg-primary">Flex item 3</div>
        </div>
        <div class="d-flex mb-3 bg-secondary">
            <div class="p-2  bg-info">Flex item 1</div>
            <div class="p-2 bg-warning">Flex item 2</div>
            <div class="p-2 me-auto bg-primary">Flex item 3</div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173613771-e73d2f43-86fa-4cd2-a6b9-61071887a625.png)
	
``` html
<!--Wrap-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Wrap</h2>
        <p>Control how flex items wrap in a flex container with .flex-nowrap (default), .flex-wrap or .flex-wrap-reverse.</p>
        <p><code>.flex-wrap:</code></p>
        <div class="d-flex flex-wrap bg-light">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
            <div class="p-2 border">Flex item 4</div>
            <div class="p-2 border">Flex item 5</div>
            <div class="p-2 border">Flex item 6</div>
            <div class="p-2 border">Flex item 7</div>
            <div class="p-2 border">Flex item 8</div>
            <div class="p-2 border">Flex item 9</div>
            <div class="p-2 border">Flex item 10</div>
            <div class="p-2 border">Flex item 11</div>
            <div class="p-2 border">Flex item 12</div>
            <div class="p-2 border">Flex item 13 </div>
            <div class="p-2 border">Flex item 14</div>
            <div class="p-2 border">Flex item 15</div>
            <div class="p-2 border">Flex item 16</div>
            <div class="p-2 border">Flex item 17</div>
            <div class="p-2 border">Flex item 18</div>
            <div class="p-2 border">Flex item 19</div>
            <div class="p-2 border">Flex item 20</div>
            <div class="p-2 border">Flex item 21</div>
            <div class="p-2 border">Flex item 22</div>
            <div class="p-2 border">Flex item 23</div>
            <div class="p-2 border">Flex item 24</div>
            <div class="p-2 border">Flex item 25</div>
        </div>
        <br>
        <p><code>.flex-wrap-reverse:</code></p>
        <div class="d-flex flex-wrap-reverse bg-light">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
            <div class="p-2 border">Flex item 4</div>
            <div class="p-2 border">Flex item 5</div>
            <div class="p-2 border">Flex item 6</div>
            <div class="p-2 border">Flex item 7</div>
            <div class="p-2 border">Flex item 8</div>
            <div class="p-2 border">Flex item 9</div>
            <div class="p-2 border">Flex item 10</div>
            <div class="p-2 border">Flex item 11</div>
            <div class="p-2 border">Flex item 12</div>
            <div class="p-2 border">Flex item 13 </div>
            <div class="p-2 border">Flex item 14</div>
            <div class="p-2 border">Flex item 15</div>
            <div class="p-2 border">Flex item 16</div>
            <div class="p-2 border">Flex item 17</div>
            <div class="p-2 border">Flex item 18</div>
            <div class="p-2 border">Flex item 19</div>
            <div class="p-2 border">Flex item 20</div>
            <div class="p-2 border">Flex item 21</div>
            <div class="p-2 border">Flex item 22</div>
            <div class="p-2 border">Flex item 23</div>
            <div class="p-2 border">Flex item 24</div>
            <div class="p-2 border">Flex item 25</div>
        </div>
        <br>
        <p><code>.flex-nowrap:</code></p>
        <div class="d-flex flex-nowrap bg-light">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
            <div class="p-2 border">Flex item 4</div>
            <div class="p-2 border">Flex item 5</div>
            <div class="p-2 border">Flex item 6</div>
            <div class="p-2 border">Flex item 7</div>
            <div class="p-2 border">Flex item 8</div>
            <div class="p-2 border">Flex item 9</div>
            <div class="p-2 border">Flex item 10</div>
            <div class="p-2 border">Flex item 11</div>
            <div class="p-2 border">Flex item 12</div>
            <div class="p-2 border">Flex item 13 </div>
            <div class="p-2 border">Flex item 14</div>
            <div class="p-2 border">Flex item 15</div>
            <div class="p-2 border">Flex item 16</div>
            <div class="p-2 border">Flex item 17</div>
            <div class="p-2 border">Flex item 18</div>
            <div class="p-2 border">Flex item 19</div>
            <div class="p-2 border">Flex item 20</div>
            <div class="p-2 border">Flex item 21</div>
            <div class="p-2 border">Flex item 22</div>
            <div class="p-2 border">Flex item 23</div>
            <div class="p-2 border">Flex item 24</div>
            <div class="p-2 border">Flex item 25</div>
            <div class="p-2 border">Flex item 26</div>
            <div class="p-2 border">Flex item 27</div>
            <div class="p-2 border">Flex item 28</div>
            <div class="p-2 border">Flex item 29</div>
            <div class="p-2 border">Flex item 30</div>
            <div class="p-2 border">Flex item 31</div>
            <div class="p-2 border">Flex item 32</div>
            <div class="p-2 border">Flex item 33</div>
            <div class="p-2 border">Flex item 34</div>
            <div class="p-2 border">Flex item 35</div>
        </div>
        <br>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173613973-35aa453d-f89d-400a-8fa5-7063b8ff9f9c.png)
	
``` html
<!--Align content-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Align Content</h2>
        <p>Control the vertical alignment of gathered flex items with the .align-content-* classes.</p>
        <p><strong>Note:</strong> This example does not look good on a small devices. Also note that these classes have no effect on single rows of flex items.</p>
        <p>.align-content-start (default):</p>
        <div class="d-flex flex-wrap align-content-start bg-light" style="height:300px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
            <div class="p-2 border">Flex item 4</div>
            <div class="p-2 border">Flex item 5</div>
            <div class="p-2 border">Flex item 6</div>
            <div class="p-2 border">Flex item 7</div>
            <div class="p-2 border">Flex item 8</div>
            <div class="p-2 border">Flex item 9</div>
            <div class="p-2 border">Flex item 10</div>
            <div class="p-2 border">Flex item 11</div>
            <div class="p-2 border">Flex item 12</div>
            <div class="p-2 border">Flex item 13 </div>
            <div class="p-2 border">Flex item 14</div>
            <div class="p-2 border">Flex item 15</div>
            <div class="p-2 border">Flex item 16</div>
            <div class="p-2 border">Flex item 17</div>
            <div class="p-2 border">Flex item 18</div>
            <div class="p-2 border">Flex item 19</div>
            <div class="p-2 border">Flex item 20</div>
            <div class="p-2 border">Flex item 21</div>
            <div class="p-2 border">Flex item 22</div>
            <div class="p-2 border">Flex item 23</div>
            <div class="p-2 border">Flex item 24</div>
            <div class="p-2 border">Flex item 25</div>
        </div>
        <br>
        <p>.align-content-end:</p>
        <div class="d-flex flex-wrap align-content-end bg-light" style="height:300px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
            <div class="p-2 border">Flex item 4</div>
            <div class="p-2 border">Flex item 5</div>
            <div class="p-2 border">Flex item 6</div>
            <div class="p-2 border">Flex item 7</div>
            <div class="p-2 border">Flex item 8</div>
            <div class="p-2 border">Flex item 9</div>
            <div class="p-2 border">Flex item 10</div>
            <div class="p-2 border">Flex item 11</div>
            <div class="p-2 border">Flex item 12</div>
            <div class="p-2 border">Flex item 13 </div>
            <div class="p-2 border">Flex item 14</div>
            <div class="p-2 border">Flex item 15</div>
            <div class="p-2 border">Flex item 16</div>
            <div class="p-2 border">Flex item 17</div>
            <div class="p-2 border">Flex item 18</div>
            <div class="p-2 border">Flex item 19</div>
            <div class="p-2 border">Flex item 20</div>
            <div class="p-2 border">Flex item 21</div>
            <div class="p-2 border">Flex item 22</div>
            <div class="p-2 border">Flex item 23</div>
            <div class="p-2 border">Flex item 24</div>
            <div class="p-2 border">Flex item 25</div>
        </div>
        <br>
        <p>.align-content-center:</p>
        <div class="d-flex flex-wrap align-content-center bg-light" style="height:300px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
            <div class="p-2 border">Flex item 4</div>
            <div class="p-2 border">Flex item 5</div>
            <div class="p-2 border">Flex item 6</div>
            <div class="p-2 border">Flex item 7</div>
            <div class="p-2 border">Flex item 8</div>
            <div class="p-2 border">Flex item 9</div>
            <div class="p-2 border">Flex item 10</div>
            <div class="p-2 border">Flex item 11</div>
            <div class="p-2 border">Flex item 12</div>
            <div class="p-2 border">Flex item 13 </div>
            <div class="p-2 border">Flex item 14</div>
            <div class="p-2 border">Flex item 15</div>
            <div class="p-2 border">Flex item 16</div>
            <div class="p-2 border">Flex item 17</div>
            <div class="p-2 border">Flex item 18</div>
            <div class="p-2 border">Flex item 19</div>
            <div class="p-2 border">Flex item 20</div>
            <div class="p-2 border">Flex item 21</div>
            <div class="p-2 border">Flex item 22</div>
            <div class="p-2 border">Flex item 23</div>
            <div class="p-2 border">Flex item 24</div>
            <div class="p-2 border">Flex item 25</div>
        </div>
        <br>
        <p>.align-content-around:</p>
        <div class="d-flex flex-wrap align-content-around bg-light" style="height:300px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
            <div class="p-2 border">Flex item 4</div>
            <div class="p-2 border">Flex item 5</div>
            <div class="p-2 border">Flex item 6</div>
            <div class="p-2 border">Flex item 7</div>
            <div class="p-2 border">Flex item 8</div>
            <div class="p-2 border">Flex item 9</div>
            <div class="p-2 border">Flex item 10</div>
            <div class="p-2 border">Flex item 11</div>
            <div class="p-2 border">Flex item 12</div>
            <div class="p-2 border">Flex item 13 </div>
            <div class="p-2 border">Flex item 14</div>
            <div class="p-2 border">Flex item 15</div>
            <div class="p-2 border">Flex item 16</div>
            <div class="p-2 border">Flex item 17</div>
            <div class="p-2 border">Flex item 18</div>
            <div class="p-2 border">Flex item 19</div>
            <div class="p-2 border">Flex item 20</div>
            <div class="p-2 border">Flex item 21</div>
            <div class="p-2 border">Flex item 22</div>
            <div class="p-2 border">Flex item 23</div>
            <div class="p-2 border">Flex item 24</div>
            <div class="p-2 border">Flex item 25</div>
        </div>
        <br>
        <p>.align-content-stretch:</p>
        <div class="d-flex flex-wrap align-content-stretch bg-light" style="height:300px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
            <div class="p-2 border">Flex item 4</div>
            <div class="p-2 border">Flex item 5</div>
            <div class="p-2 border">Flex item 6</div>
            <div class="p-2 border">Flex item 7</div>
            <div class="p-2 border">Flex item 8</div>
            <div class="p-2 border">Flex item 9</div>
            <div class="p-2 border">Flex item 10</div>
            <div class="p-2 border">Flex item 11</div>
            <div class="p-2 border">Flex item 12</div>
            <div class="p-2 border">Flex item 13 </div>
            <div class="p-2 border">Flex item 14</div>
            <div class="p-2 border">Flex item 15</div>
            <div class="p-2 border">Flex item 16</div>
            <div class="p-2 border">Flex item 17</div>
            <div class="p-2 border">Flex item 18</div>
            <div class="p-2 border">Flex item 19</div>
            <div class="p-2 border">Flex item 20</div>
            <div class="p-2 border">Flex item 21</div>
            <div class="p-2 border">Flex item 22</div>
            <div class="p-2 border">Flex item 23</div>
            <div class="p-2 border">Flex item 24</div>
            <div class="p-2 border">Flex item 25</div>
        </div>
        <br>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173614154-12c6ed5e-22e8-440c-afe0-16c8907d0966.png)
![image](https://user-images.githubusercontent.com/75599178/173614212-fb9e9249-f53d-498e-8e1a-578edb53a877.png)
![image](https://user-images.githubusercontent.com/75599178/173614295-5c520c29-095d-4569-aff6-10deaf7840c0.png)
	
``` html
<!--Align Items-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Align Items</h2>
        <p>Control the vertical alignment of single rows of flex items with the .align-content-* classes.</p>
        <p>.align-items-start:</p>
        <div class="d-flex align-items-start bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
        <p>.align-items-end:</p>
        <div class="d-flex align-items-end bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
        <p>.align-items-center:</p>
        <div class="d-flex align-items-center bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
        <p>.align-items-baseline:</p>
        <div class="d-flex align-items-baseline bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
        <p>.align-items-stretch (default):</p>
        <div class="d-flex align-items-stretch bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173614496-0d12424f-c8b2-4cea-9762-595be95ab9de.png)
![image](https://user-images.githubusercontent.com/75599178/173614647-f361e8a2-25f0-4b4d-958c-4ac40702642e.png)

``` html
<!--Align Self-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container mt-3">
        <h2>Align Self</h2>
        <p>Control the vertical alignment of a specific flex item with the .align-self-* classes.</p>
        <p>.align-self-start:</p>
        <div class="d-flex bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border align-self-start">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
        <p>.align-self-end:</p>
        <div class="d-flex bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border align-self-end">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
        <p>.align-self-center:</p>
        <div class="d-flex bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border align-self-center">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
        <p>.align-self-baseline:</p>
        <div class="d-flex bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border align-self-baseline">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
        <p>.align-self-stretch (default):</p>
        <div class="d-flex bg-light" style="height:150px">
            <div class="p-2 border">Flex item 1</div>
            <div class="p-2 border align-self-stretch">Flex item 2</div>
            <div class="p-2 border">Flex item 3</div>
        </div>
        <br>
    </div>
</body>
</html>

```

![image](https://user-images.githubusercontent.com/75599178/173614735-8471de21-fc30-4112-876a-accb2051e9da.png)
![image](https://user-images.githubusercontent.com/75599178/173614816-e0d762cc-28ea-4cf2-9f60-a33b0018d1ae.png)
	
</details>	
	
### Grid 
	
<details>
	<summary>:bulb:</summary>

The Grid System

Bootstrap's grid system is built with flexbox and allows up to 12 columns across the page.

If you do not want to use all 12 columns individually, you can group the columns together to create wider columns.

``` html
<!--Basic grid-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>Basic Grid Structure</h1>
        <p>Resize the browser window to see the effect.</p>
        <p>The first, second and third row will automatically stack on top of each other when the screen is less than 576px wide.</p>
        
        <!-- Control the column width, and how they should appear on different devices -->
        <div class="row">
          <div class="col-sm-6 bg-primary text-white">50%</div>
          <div class="col-sm-6 bg-dark text-white">50%</div>
        </div>
        <br>
          
        <div class="row">
          <div class="col-sm-4 bg-primary text-white">33.33%</div>
          <div class="col-sm-4 bg-dark text-white">33.33%</div>
          <div class="col-sm-4 bg-primary text-white">33.33%</div>
        </div>
        <br>
      
        <!-- Or let Bootstrap automatically handle the layout -->
        <div class="row">
          <div class="col-sm bg-primary text-white">25%</div>
          <div class="col-sm bg-dark text-white">25%</div>
          <div class="col-sm bg-primary text-white">25%</div>
          <div class="col-sm bg-dark text-white">25%</div>
        </div>
        <br>
          
        <div class="row">
          <div class="col bg-primary text-white">25%</div>
          <div class="col bg-dark text-white">25%</div>
          <div class="col bg-primary text-white">25%</div>
          <div class="col bg-dark text-white">25%</div>
        </div>
      </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173734387-4b1d9723-d500-41dd-affa-ba756df2399e.png)
	
``` html
<!--Grid Xsmall-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>Extra Small Grid</h1>
        <p>The following example will result in a 33.3%/66.6% split on all devices.</p>
        <p>Resize the browser window to see the effect.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-1 bg-primary text-white p-3">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-11 bg-dark text-white p-3">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
        <br>
        
        <p>This example will result in a 50%/50% split on all devices.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-6 bg-primary text-white p-3">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-6 bg-dark text-white p-3">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
      </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173734458-0218c482-4393-4615-8dce-5f587a1e4e55.png)
	
``` html
<!-- Grid small-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>Small Grid</h1>
        <p>The following example will result in a 33.3%/66.6% split on small, medium, large and xlarge devices (<strong>576px and above</strong>). On extra small devices, it will stack (100% width).</p>
        <p>Resize the browser window to see the effect.</p>
        <p>Small devices are defined as having a screen width from 576 pixels to 767 pixels.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-sm-4 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-sm-8 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
        <br>
        
        <p>This example will result in a 50%/50% split on small, medium, large and xlarge devices (<strong>576px and above</strong>). On extra small devices, it will stack (100% width).</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-sm-6 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-sm-6 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173734542-d4867911-7729-4ea6-9c3f-5cfb2397d1c1.png)
	
``` html
<!-- Grid smal + medium-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>Medium Grid</h1>
        <p>The following example will result in a 25%/75% split on small devices and a 50%/50% split on medium (and large, xlarge, xxlarge) devices. On extra small devices, it will automatically stack (100%).</p>
        <p>Resize the browser window to see the effect.</p>
        <p>Medium devices are defined as having a screen width from 768 pixels to 991 pixels.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-sm-3 col-md-6 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-sm-9 col-md-6 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
      </div>
</body>
</html>
```
	
``` html
<!-- Grid medium-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>Medium Grid</h1>
        <p>The following example will result in a 50%/50% split on medium, large, xlarge and xxlarge devices (<strong>768px and above</strong>). On small (and extra small) devices, it will automatically stack (100%).</p>
        <p>Resize the browser window to see the effect.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-md-6 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-md-6 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173734590-c6235e58-a561-45b6-959b-3e17d9424486.png)
	
``` html
<!-- Grid smal + medium +  large-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>Large Grid</h1>
        <p>The following example will result in a 25%/75% split on small devices, a 50%/50% split on medium devices, and a 33%/66% split on large, xlarge and xxlarge devices. On extra small devices, it will automatically stack (100%).</p>
        <p>Resize the browser window to see the effect.</p>
        <p>Large devices are defined as having a screen width from 992 pixels to 1199 pixels.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-sm-3 col-md-6 col-lg-4 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-sm-9 col-md-6 col-lg-8 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
      </div>
</body>
</html>
```
	
``` html
<!-- Grid large-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>Medium Grid</h1>
        <p>The following example will result in a 50%/50% split on medium, large, xlarge and xxlarge devices (<strong>768px and above</strong>). On small (and extra small) devices, it will automatically stack (100%).</p>
        <p>Resize the browser window to see the effect.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-lg-6 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-lg-6 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173734640-e054c965-42da-47d6-a634-4b86191c7dbc.png)
	
``` html
<!-- Grid smal + medium +  large + Xlarge-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>XLarge Grid</h1>
        <p>The following example will result in a 25%/75% split on small devices, a 50%/50% split on medium devices, a 33%/66% split on large devices and a 20%/80% on xlarge and xxlarge devices. On extra small devices, it will automatically stack (100%).</p>
        <p>Resize the browser window to see the effect.</p>
        <p>Extra large devices are defined as having a screen width from 1200 pixels and above.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-sm-3 col-md-6 col-lg-4 col-xl-2 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-sm-9 col-md-6 col-lg-8 col-xl-10 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
    </div>
</body>
</html>
```
	
``` html

<!-- Grid Xlarge-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>XLarge Grid</h1>
        <p>The following example will result in a 25%/75% split on small devices, a 50%/50% split on medium devices, a 33%/66% split on large devices and a 20%/80% on xlarge and xxlarge devices. On extra small devices, it will automatically stack (100%).</p>
        <p>Resize the browser window to see the effect.</p>
        <p>Extra large devices are defined as having a screen width from 1200 pixels and above.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-xl-6 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-xl-6 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173734694-1a816a3e-bdd9-432a-a702-0444367c8b9f.png)
	
``` html

<!-- Grid medium + XXlarge-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>XXL Grid</h1>
        <p>The following example will result in a 50%/50% split on medium, large and extra large devices, and a 25%/75% split on XXL devices. On 
        small and extra small devices, it will automatically stack (100%):</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-md-6 col-xxl-3 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-md-6 col-xxl-9 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
      </div>
</body>
</html>
```
	
``` html
<!-- Grid XXlarge-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-fluid mt-3">
        <h1>XXL Grid</h1>
        <p>The following example will result in a 50%/50% split on XXL devices (<strong>1400px and above</strong>). On extra large, large, medium, small and extra small devices, it will automatically stack (100%).</p>
        <p>Resize the browser window to see the effect.</p>
        <p>XXL devices are defined as having a screen width from 1400 pixels and above.</p>
        <div class="container-fluid">
          <div class="row">
            <div class="col-xxl-6 bg-primary text-white">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br>
              Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </div>
            <div class="col-xxl-6 bg-dark text-white">
              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
            </div>
          </div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/173734735-292f80ae-997b-48fa-8553-150b1229b671.png)

</details>

### Forms
<details>
	<summary>:bulb:</summary>
	
``` html
<!-- Forms-->

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Stacked form</h2>
  <form action="/action_page.php">
    <div class="mb-3 mt-3">
      <label for="email">Email:</label>
      <input type="email" class="form-control" id="email" placeholder="Enter email" name="email">
    </div>
    <div class="mb-3">
      <label for="pwd">Password:</label>
      <input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pswd">
    </div>
    <div class="form-check mb-3">
      <label class="form-check-label">
        <input class="form-check-input" type="checkbox" name="remember"> Remember me
      </label>
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</div>

</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/174486973-8679ad85-3f65-4325-b0ac-b8e6878032ab.png)

	
Also note that we add a .form-label class to each label element to ensure correct padding.

Checkboxes have different markup. They are wrapped around a container element with .form-check, and labels have a class of .form-check-label, while checkboxes and radio buttons use .form-check-input.
``` html
<!-- Select menu-->>

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Select Menu</h2>
  <p>To style a select menu in Bootstrap 5, add the .form-select class to the select element:</p>
  <form action="/action_page.php">
    <label for="sel1" class="form-label">Select list (select one):</label>
    <select class="form-select" id="sel1" name="sellist1">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
    </select>
    <br>
    
    <label for="sel2" class="form-label">Mutiple select list (hold shift to select more than one):</label>
    <select multiple class="form-select" id="sel2" name="sellist2">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
    
    <label for="browser" class="form-label">Choose your browser from the list:</label>
    <input class="form-control" list="browsers" name="browser" id="browser">
    <datalist id="browsers">
    <option value="Edge">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
    </datalist>
    <button type="submit" class="btn btn-primary mt-3">Submit</button>
  </form>
</div>

</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/174488066-c4c018dc-600e-47c9-a544-ff7eccc2581b.png)
``` html

<!--Checkbox -->

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Checkboxes</h2>
  <p>To style a checkbox, use a container element with a .form-check class, and add .form-check-label to labels, and .form-check-input to the input with type="checkbox".</p>
  <p>The form below contains three checkboxes. The first option is checked by default, and the last option is disabled:</p>
  <form action="/action_page.php">
    <div class="form-check">
      <input type="checkbox" class="form-check-input" id="check1" name="option1" value="something" checked>
      <label class="form-check-label" for="check1">Option 1</label>
    </div>
    <div class="form-check">
      <input type="checkbox" class="form-check-input" id="check2" name="option2" value="something">
      <label class="form-check-label" for="check2">Option 2</label>
    </div>
    <div class="form-check">
      <input type="checkbox" class="form-check-input" disabled>
      <label class="form-check-label">Option 3</label>
    </div>
    <button type="submit" class="btn btn-primary mt-3">Submit</button>
  </form>
</div>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/174488085-3e8cf79d-4347-4f8e-bbf4-2a4ef4d91010.png)

``` html

<!-- Radio-->
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Radio buttons</h2>
  <p>The form below contains three radio buttons. The first option is checked by default, and the last option is disabled:</p>
  <form action="/action_page.php">
    <div class="form-check">
      <input type="radio" class="form-check-input" id="radio1" name="optradio" value="option1" checked>
      <label class="form-check-label" for="radio1">Option 1</label>
    </div>
    <div class="form-check">
      <input type="radio" class="form-check-input" id="radio2" name="optradio" value="option2">
      <label class="form-check-label" for="radio2">Option 2</label>
    </div>
    <div class="form-check">
      <input type="radio" class="form-check-input" disabled>
      <label class="form-check-label">Option 3</label>
    </div>
    <button type="submit" class="btn btn-primary mt-3">Submit</button>
  </form>
</div>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/174488104-4908e7c6-af53-4e8b-91e2-b253a8b35509.png)

``` html

<!--- Toggle switches-->

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Toggle Switch</h2>
  <p>Try to submit the form with and without toggling the switch.</p>
  <form action="/action_page.php">
    <div class="form-check form-switch">
      <input class="form-check-input" type="checkbox" id="mySwitch" name="darkmode" value="yes" checked>
      <label class="form-check-label" for="mySwitch">Dark Mode</label>
    </div>
    <button type="submit" class="btn btn-primary mt-3">Submit</button>
  </form>
</div>

</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/174488125-0a224e08-bd4e-4985-abaf-4c99dbc19148.png)

``` html

<!-- Range-->

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Custom Range</h2>
  <p>To create a custom range menu, add the .form-range class to the input element with type="range":</p>
  <form action="/action_page.php">
    <label for="customRange" class="form-label">Custom range</label>
    <input type="range" class="form-range" id="customRange" name="points">
    
    <button type="submit" class="btn btn-primary mt-3">Submit</button>
  </form>
</div>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/174488145-c84c24e9-5a43-47a2-8dbf-833320b81d16.png)

``` html
<!-- Steps -->


<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Steps in a Range</h2>
  <p>By default, the interval between the range numbers is 1. You can change it by using the step attribute:</p>
  <form action="/action_page.php">
    <label for="customRange" class="form-label">Custom range</label>
    <input type="range" class="form-range" id="customRange" step="10" name="points">
    
    <button type="submit" class="btn btn-primary mt-3">Submit</button>
  </form>
</div>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/174488172-ef5beae9-eb1c-4ced-a0bd-d3d052a689e3.png)

``` html

<!-- Min. Max.-->

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Min and Max Range</h2>
  <p>Use the min and/or max attribute to specify the minimum/maximum value of a range:</p>
  <form action="/action_page.php">
    <label for="customRange" class="form-label">Custom range</label>
    <input type="range" class="form-range" id="customRange" name="points" min="0" max="4">
    
    <button type="submit" class="btn btn-primary mt-3">Submit</button>
  </form>
</div>

</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/174488197-4f236063-dd42-4bcb-851f-342bbef7b26b.png)

``` html

<!-- Input-->

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h2>Input Group Size</h2>
  <p>Use the .input-group-sm class for small input groups and .input-group-lg for large inputs groups:</p>
  
  <div class="input-group input-group-sm mb-3">
    <span class="input-group-text">Small</span>
    <input type="text" class="form-control">
  </div>
  <div class="input-group mb-3">
    <span class="input-group-text">Default</span>
    <input type="text" class="form-control">
  </div>
  <div class="input-group input-group-lg mb-3">
    <span class="input-group-text">Large</span>
    <input type="text" class="form-control">
  </div>
</div>

</body>
</html>
```
![image](https://user-images.githubusercontent.com/75599178/174488214-b628d855-a75a-4dfd-9259-50b2a8930ede.png)

``` html

<!-- Form validation-->

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>

<div class="container mt-3">
  <h3>Form Validation</h3>
  <p>Try to submit the form.</p>
    
  <form action="/action_page.php" class="was-validated">
    <div class="mb-3 mt-3">
      <label for="uname" class="form-label">Username:</label>
      <input type="text" class="form-control" id="uname" placeholder="Enter username" name="uname" required>
      <div class="valid-feedback">Valid.</div>
      <div class="invalid-feedback">Please fill out this field.</div>
    </div>
    <div class="mb-3">
      <label for="pwd" class="form-label">Password:</label>
      <input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pswd" required>
      <div class="valid-feedback">Valid.</div>
      <div class="invalid-feedback">Please fill out this field.</div>
    </div>
    <div class="form-check mb-3">
      <input class="form-check-input" type="checkbox" id="myCheck"  name="remember" required>
      <label class="form-check-label" for="myCheck">I agree on blabla.</label>
      <div class="valid-feedback">Valid.</div>
      <div class="invalid-feedback">Check this checkbox to continue.</div>
    </div>
  <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</div>

</body>
</html>

```
![image](https://user-images.githubusercontent.com/75599178/174488233-ab127682-3056-421c-8510-293608146b6e.png)

</details>		
		
# Interview questions

### What is bootstrap?
<details>
  <summary>:bulb:</summary>
    <ul>
           <li> Bootstrap is a CSS framework directed at responsive, mobile-first front-end web development.</li>
           <li> Bootstrap 5 is the newest version of Bootstrap. </li>
    </ul>
</details>		
		
		
		
		
		
		
		
		
		
