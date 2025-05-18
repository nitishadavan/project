# Project Responsive Web Design using Bootstrap
# Date:18-05-2025
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble Clone Landing Page</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .hero-section {
            background: #f8f9fa;
            padding: 60px 0;
            text-align: center;
        }
        .shots-section img {
            border-radius: 1rem;
        }
        .shots-section .card {
            border: none;
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-white shadow-sm">
        <div class="container">
            <a class="navbar-brand fw-bold text-pink" href="#" style="color:#ea4c89;">dribbble</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#">Inspiration</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Find Work</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Learn Design</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Go Pro</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Sign Up</a></li>
                    <li class="nav-item"><a class="btn btn-pink ms-2" style="background:#ea4c89;color:white;" href="#">Sign In</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-section">
        <div class="container">
            <h1 class="display-4 fw-bold" style="color:#ea4c89;">Discover the world’s top designers & creatives</h1>
            <p class="lead mt-3 mb-4">Dribbble is the leading destination to find & showcase creative work and home to the world's best design professionals.</p>
            <a href="#" class="btn btn-lg" style="background:#ea4c89;color:white;">Get Started</a>
        </div>
    </section>

    <!-- Shots Section with Tabs -->
    <section class="shots-section py-5">
        <div class="container">
            <h2 class="mb-4 text-center">Popular Shots</h2>
            <ul class="nav nav-pills justify-content-center mb-4" id="shotsTab" role="tablist">
                <li class="nav-item" role="presentation">
                    <button class="nav-link active" id="product-tab" data-bs-toggle="pill" data-bs-target="#product" type="button" role="tab" aria-controls="product" aria-selected="true">Product</button>
                </li>
                <li class="nav-item" role="presentation">
                    <button class="nav-link" id="webdesign-tab" data-bs-toggle="pill" data-bs-target="#webdesign" type="button" role="tab" aria-controls="webdesign" aria-selected="false">Web Design</button>
                </li>
                <li class="nav-item" role="presentation">
                    <button class="nav-link" id="branding-tab" data-bs-toggle="pill" data-bs-target="#branding" type="button" role="tab" aria-controls="branding" aria-selected="false">Branding</button>
                </li>
            </ul>
            <div class="tab-content" id="shotsTabContent">
                <!-- Product Tab -->
                <div class="tab-pane fade show active" id="product" role="tabpanel" aria-labelledby="product-tab">
                    <div class="row g-4">
                        <div class="col-12 col-md-4">
                            <div class="card">
                                <img src="pro1.webp" class="card-img-top" alt="Shot 1">
                                <div class="card-body">
                                    <h5 class="card-title">Creative App UI</h5>
                                    <p class="card-text">by Designer A</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-12 col-md-4">
                            <div class="card">
                                <img src="pro2.webp" class="card-img-top" alt="Shot 2">
                                <div class="card-body">
                                    <h5 class="card-title">Modern Dashboard</h5>
                                    <p class="card-text">by Designer B</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-12 col-md-4">
                            <div class="card">
                                <img src="pro3.webp" class="card-img-top" alt="Shot 3">
                                <div class="card-body">
                                    <h5 class="card-title">Landing Page Design</h5>
                                    <p class="card-text">by Designer C</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Web Design Tab -->
                <div class="tab-pane fade" id="webdesign" role="tabpanel" aria-labelledby="webdesign-tab">
                    <div class="row g-4">
                        <div class="col-12 col-md-4">
                            <div class="card">
                                <img src="web1.webp" class="card-img-top" alt="Web Design 1">
                                <div class="card-body">
                                    <h5 class="card-title">Portfolio Website</h5>
                                    <p class="card-text">by Designer D</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-12 col-md-4">
                            <div class="card">
                                <img src="web2.webp" class="card-img-top" alt="Web Design 2">
                                <div class="card-body">
                                    <h5 class="card-title">E-commerce UI</h5>
                                    <p class="card-text">by Designer E</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-12 col-md-4">
                            <div class="card">
                                <img src="web3.webp" class="card-img-top" alt="Web Design 3">
                                <div class="card-body">
                                    <h5 class="card-title">Blog Layout</h5>
                                    <p class="card-text">by Designer F</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Branding Tab -->
                <div class="tab-pane fade" id="branding" role="tabpanel" aria-labelledby="branding-tab">
                    <div class="row g-4">
                        <div class="col-12 col-md-4">
                            <div class="card">
                                <img src="brand1.webp" class="card-img-top" alt="Branding 1">
                                <div class="card-body">
                                    <h5 class="card-title">Logo Design</h5>
                                    <p class="card-text">by Designer G</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-12 col-md-4">
                            <div class="card">
                                <img src="brand2.webp" class="card-img-top" alt="Branding 2">
                                <div class="card-body">
                                    <h5 class="card-title">Brand Identity</h5>
                                    <p class="card-text">by Designer H</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-12 col-md-4">
                            <div class="card">
                                <img src="brand3.webp" class="card-img-top" alt="Branding 3">
                                <div class="card-body">
                                    <h5 class="card-title">Packaging Design</h5>
                                    <p class="card-text">by Designer I</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Call to Action Section -->
    <section class="py-5 bg-light text-center">
        <div class="container">
            <h2 class="mb-3">Ready to showcase your work?</h2>
            <a href="#" class="btn btn-lg" style="background:#ea4c89;color:white;">Join Dribbble</a>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-white text-center py-3 border-top">
        <div class="container">
            &copy; 2025 Designed by <strong>D.Nitish Adavan</strong>
        </div>
    </footer>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
~~~
# OUTPUT:
![Screenshot 2025-05-18 212228](https://github.com/user-attachments/assets/00b33300-3a46-4ca5-a150-9275172d2694)

![Screenshot 2025-05-18 212244](https://github.com/user-attachments/assets/76caeba7-288d-4cda-8892-dcbbee786907)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
