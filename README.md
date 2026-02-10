# Ex08 Pharmacy Website using Bootstrap
## Date:

## AIM:
To design a responsive and visually appealing Pharmacy web page using Bootstrap, featuring a navigation bar, categorized product panels with images and descriptions, and a footer, ensuring easy navigation, user accessibility, and professional layout suitable for an online medical or wellness platform.

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Link Bootstrap CSS and JavaScript along with jQuery.

### Step 5:
Create a navigation bar at the top of the page.

### Step 6:
Add the brand name “PharmEasy” in the navigation bar.

### Step 7:
Insert menu options for Home, Services (with dropdown), and Contact Us.

### Step 8:
Add options for Sign Up and Login on the right side of the navigation bar.

### Step 9:
Include a search box with a submit button inside the navigation bar.

### Step 10:
Create the main content area centered on the page.

### Step 11:
Divide the page content into two rows.

### Step 12:
In the first row, place three panels for Pain Relief, Vitamins & Supplements, and Baby Care.

### Step 13:
In the second row, place three panels for Skin Care, Fitness Essentials, and Home Health Care.

### Step 14:
Add images inside each panel representing the respective category.

### Step 15:
Provide short descriptions under each image as panel footers.

### Step 16:
Add a footer at the bottom displaying copyright information.

### Step 17:
Publish the website in the LocalHost.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TrueMeds – Medicine Price Comparison</title>

<!-- Bootstrap 3 -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">

<style>
body {
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
    background-color: #ffffff;
}

/* Navbar */
.navbar {
    margin-bottom: 0;
    border-radius: 0;
}
.navbar-brand {
    font-weight: bold;
    color: #1a73e8 !important;
}

/* Hero Section */
.hero {
    background: #f1f7ff;
    padding: 60px 0;
    position: relative;
}
.hero h1 {
    font-size: 36px;
    font-weight: 600;
}
.hero p {
    font-size: 16px;
    color: #555;
    margin-bottom: 25px;
}

/* Search Bar */
.search-bar {
    max-width: 650px;
    margin: auto;
}
.search-bar input {
    height: 46px;
    font-size: 16px;
}
.search-bar button {
    height: 46px;
}

/* Order Section */
.order-section {
    padding: 40px 0;
}
.order-box {
    background: #f4f8ff;
    border-radius: 10px;
    padding: 25px;
    text-align: center;
    font-size: 16px;
}

/* Savings Section */
.savings-section {
    padding: 40px 0;
}
.save-box {
    background: #f6edff;
    padding: 30px;
    border-radius: 12px;
    text-align: center;
}
.save-box h1 {
    color: #7b3fe4;
    font-size: 48px;
    font-weight: bold;
}
.features li {
    margin-bottom: 10px;
    font-size: 15px;
}

/* Footer */
footer {
    background: #f5f5f5;
    padding: 20px;
    text-align: center;
    margin-top: 40px;
}
</style>
</head>

<body>

<!-- NAVBAR -->
<nav class="navbar navbar-default">
<div class="container-fluid">
<div class="navbar-header">
<button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#nav">
<span class="icon-bar"></span>
<span class="icon-bar"></span>
<span class="icon-bar"></span>
</button>
<a class="navbar-brand" href="#">truemeds</a>
</div>

<div class="collapse navbar-collapse" id="nav">
<ul class="nav navbar-nav">
<li><a href="#">Medicines</a></li>
<li><a href="#">Personal Care</a></li>
<li><a href="#">Health Conditions</a></li>
<li><a href="#">Vitamins & Supplements</a></li>
<li><a href="#">Diabetes Care</a></li>
<li><a href="#">Healthcare Devices</a></li>
<li><a href="#">Homeopathic</a></li>
<li><a href="#">Health Guide</a></li>
</ul>

<ul class="nav navbar-nav navbar-right">
<li><a href="#">Download App</a></li>
<li><a href="#">Login / Signup</a></li>
<li><a href="#">🛒</a></li>
</ul>
</div>
</div>
</nav>

<!-- HERO -->
<section class="hero text-center">
<div class="container">
<h1>Say GoodBye to high medicine prices</h1>
<p>Compare prices and save up to 51%</p>

<div class="search-bar">
<form class="form-inline">
<div class="form-group" style="width:75%">
<input type="text" class="form-control" style="width:100%" placeholder="Search for GLYCOMET">
</div>
<button type="submit" class="btn btn-primary">
<span class="glyphicon glyphicon-search"></span>
</button>
</form>
</div>
</div>
</section>

<!-- ORDER SECTION -->
<section class="order-section">
<div class="container text-center">
<h4>PLACE YOUR ORDER VIA</h4>
<br>
<div class="row">
<div class="col-sm-6">
<div class="order-box">
📞 Call <strong>09240250346</strong> to place order
</div>
</div>
<div class="col-sm-6">
<div class="order-box">
📄 Upload a <strong>prescription</strong>
</div>
</div>
</div>
</div>
</section>

<!-- SAVINGS -->
<section class="savings-section">
<div class="container">
<div class="row">
<div class="col-md-4">
<div class="save-box">
<h1>Save 51%</h1>
<p>With substitute medicines</p>
</div>
</div>

<div class="col-md-8">
<h3>Substitutes are the smarter choice</h3>
<ul class="features">
<li>✔ FDA and GMP certified medicines</li>
<li>✔ Exact same salt composition</li>
<li>✔ Up to 51% cheaper</li>
</ul>
</div>
</div>
</div>
</section>

<!-- FOOTER -->
<footer>
<p>© 2026 TrueMeds UI Clone | Educational Use Only</p>
</footer>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>

</body>
</html>
```

## OUTPUT:
<img width="700" height="700" alt="Screenshot 2026-02-10 092217" src="https://github.com/user-attachments/assets/02b30218-a063-4f15-b1ef-823f74b6a299" />

## RESULT:
A responsive and visually appealing Pharmacy web page using Bootstrap is designed successfully.
