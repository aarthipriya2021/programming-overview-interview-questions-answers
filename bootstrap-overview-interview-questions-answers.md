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

