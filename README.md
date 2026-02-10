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
    <title>MedStore Pharmacy</title>
    <!-- Link Bootstrap CSS from CDN -->
    <link href="https://cdn.jsdelivr.net" rel="stylesheet">
    <style>
        /* Custom styles to ensure uniform image size and center the content */
        .product-img {
            height: 180px; /* Uniform height */
            width: 100%; /* Responsive width */
            object-fit: cover; /* Ensures images cover the area without distortion */
            padding: 10px;
        }
        .panel-body {
            text-align: center;
        }
        .main-content {
            padding-top: 20px;
            padding-bottom: 20px;
        }
        footer {
            margin-top: 40px;
            padding: 20px 0;
            background-color: #f5f5f5;
            text-align: center;
        }
    </style>
</head>
<body>

    <!-- Navigation Bar -->
    <nav class="navbar navbar-default">
        <div class="container-fluid">
            <div class="navbar-header">
                <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar-collapse" aria-expanded="false">
                    <span class="sr-only">Toggle navigation</span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
                <a class="navbar-brand" href="#">MedStore Pharmacy</a>
            </div>

            <div class="collapse navbar-collapse" id="navbar-collapse">
                <ul class="nav navbar-nav">
                    <li class="active"><a href="#">Home <span class="sr-only">(current)</span></a></li>
                    <li><a href="#">Shop</a></li>
                    <li class="dropdown">
                        <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Categories <span class="caret"></span></a>
                        <ul class="dropdown-menu">
                            <li><a href="#">Vitamins & Supplements</a></li>
                            <li><a href="#">Personal Care</a></li>
                            <li><a href="#">Prescriptions</a></li>
                            <li role="separator" class="divider"></li>
                            <li><a href="#">Wellness Products</a></li>
                        </ul>
                    </li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
                
                <form class="navbar-form navbar-left" role="search">
                    <div class="form-group">
                        <input type="text" class="form-control" placeholder="Search products...">
                    </div>
                    <button type="submit" class="btn btn-default">Search</button>
                </form>

                <ul class="nav navbar-nav navbar-right">
                    <li><a href="#">Sign Up</a></li>
                    <li><a href="#">Login</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Main Content Section (Centered using container) -->
    <div class="container main-content">
        <h1 class="text-center">Featured Products</h1>
        <p class="text-center">Browse our top wellness and medical products.</p>

        <!-- First Row of Product Categories -->
        <div class="row">
            <!-- Product 1 -->
            <div class="col-sm-6 col-md-4">
                <div class="panel panel-default">
                    <div class="panel-heading">Vitamins</div>
                    <div class="panel-body">
                        <img src="https://via.placeholder.com" alt="Vitamin C Bottle" class="img-responsive product-img">
                        <h4>Vitamin C Supplements</h4>
                        <p>Boost your immune system with our high-quality Vitamin C tablets.</p>
                        <a href="#" class="btn btn-primary">View Details</a>
                    </div>
                </div>
            </div>
            <!-- Product 2 -->
            <div class="col-sm-6 col-md-4">
                <div class="panel panel-default">
                    <div class="panel-heading">Pain Relief</div>
                    <div class="panel-body">
                        <img src="https://via.placeholder.com" alt="Pain Relief Medication" class="img-responsive product-img">
                        <h4>Advanced Pain Medication</h4>
                        <p>Fast-acting relief for headaches and muscle aches.</p>
                        <a href="#" class="btn btn-primary">View Details</a>
                    </div>
                </div>
            </div>
            <!-- Product 3 -->
            <div class="col-sm-6 col-md-4">
                <div class="panel panel-default">
                    <div class="panel-heading">Skin Care</div>
                    <div class="panel-body">
                        <img src="https://via.placeholder.com" alt="Moisturizer Bottle" class="img-responsive product-img">
                        <h4>Hydrating Moisturizer</h4>
                        <p>Keep your skin soft and hydrated all day long.</p>
                        <a href="#" class="btn btn-primary">View Details</a>
                    </div>
                </div>
            </div>
        </div>

        <!-- Second Row of Product Categories -->
        <div class="row">
            <!-- Product 4 -->
            <div class="col-sm-6 col-md-4">
                <div class="panel panel-default">
                    <div class="panel-heading">First Aid</div>
                    <div class="panel-body">
                        <img src="https://via.placeholder.com" alt="First Aid Kit" class="img-responsive product-img">
                        <h4>Comprehensive First Aid Kit</h4>
                        <p>Essential supplies for minor injuries and emergencies.</p>
                        <a href="#" class="btn btn-primary">View Details</a>
                    </div>
                </div>
            </div>
            <!-- Product 5 -->
            <div class="col-sm-6 col-md-4">
                <div class="panel panel-default">
                    <div class="panel-heading">Sleep Aids</div>
                    <div class="panel-body">
                        <img src="https://via.placeholder.com" alt="Sleep Aid Pills" class="img-responsive product-img">
                        <h4>Natural Sleep Aid</h4>
                        <p>Drift off easily and wake up refreshed with our natural formula.</p>
                        <a href="#" class="btn btn-primary">View Details</a>
                    </div>
                </div>
            </div>
            <!-- Product 6 -->
            <div class="col-sm-6 col-md-4">
                <div class="panel panel-default">
                    <div class="panel-heading">Dental Care</div>
                    <div class="panel-body">
                        <img src="https://via.placeholder.com" alt="Toothpaste Box" class="img-responsive product-img">
                        <h4>Whitening Toothpaste</h4>
                        <p>Achieve a brighter smile with our advanced whitening formula.</p>
                        <a href="#" class="btn btn-primary">View Details</a>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2026 MedStore Pharmacy | Designed by [Your Name]</p>
        </div>
    </footer>

    <!-- Link jQuery and Bootstrap JS from CDNs (required for dropdowns and navigation toggle) -->
    <script src="https://code.jquery.com"></script>
    <script src="https://cdn.jsdelivr.net"></script>
</body>
</html>
```

## OUTPUT:
<img width="1898" height="1025" alt="image" src="https://github.com/user-attachments/assets/f19de291-953b-457a-a8a3-a1668cadcb88" />


## RESULT:
A responsive and visually appealing Pharmacy web page using Bootstrap is designed successfully.
