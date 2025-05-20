# Project Responsive Web Design using Bootstrap
## Date:20.05.25

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```<html>
<head>
    <title>Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
     
    <nav class="navbar navbar-expand-lg navbar-light bg-white shadow-sm">
        <div class="container">
            <a class="navbar-brand" href="#"><img src="logo.png" alt="Logo" class="img-fluid" style="height: 40px;"></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                
                <ul class="navbar-nav me-auto">
                    <li class="nav-item"><a class="nav-link text-dark" href="#">Explore</a></li>
                    <li class="nav-item"><a class="nav-link text-dark" href="#">Hire a Designer</a></li>
                    <li class="nav-item"><a class="nav-link text-dark" href="#">Find Jobs</a></li>
                    <li class="nav-item"><a class="nav-link text-dark" href="#">Blog</a></li>
                </ul>

                <div class="d-flex">
                    <button class="btn btn-dark me-2" data-bs-toggle="modal" data-bs-target="#loginModal">Login</button>
                    <button class="btn btn-outline-dark" data-bs-toggle="modal" data-bs-target="#signupModal">Sign Up</button>
                </div>
            </div>
        </div>
    </nav>

    <div class="modal fade" id="loginModal" tabindex="-1" aria-labelledby="loginModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="loginModalLabel">Login</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <form>
                        <div class="mb-3">
                            <label for="loginEmail" class="form-label">Email address</label>
                            <input type="email" class="form-control" id="loginEmail" placeholder="Enter your email">
                        </div>
                        <div class="mb-3">
                            <label for="loginPassword" class="form-label">Password</label>
                            <input type="password" class="form-control" id="loginPassword" placeholder="Enter your password">
                        </div>
                        <button type="submit" class="btn btn-dark w-100">Login</button>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <div class="modal fade" id="signupModal" tabindex="-1" aria-labelledby="signupModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="signupModalLabel">Sign Up</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <form>
                        <div class="mb-3">
                            <label for="signupName" class="form-label">Full Name</label>
                            <input type="text" class="form-control" id="signupName" placeholder="Enter your full name">
                        </div>
                        <div class="mb-3">
                            <label for="signupEmail" class="form-label">Email address</label>
                            <input type="email" class="form-control" id="signupEmail" placeholder="Enter your email">
                        </div>
                        <div class="mb-3">
                            <label for="signupPassword" class="form-label">Password</label>
                            <input type="password" class="form-control" id="signupPassword" placeholder="Create a password">
                        </div>
                        <button type="submit" class="btn btn-dark w-100">Sign Up</button>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <div class="container text-center py-5">
        <h1 class="display-4 fw-bold">Discover the world's top designers</h1>
        <p class="lead text-muted">Explore work from the most talented and accomplished designers ready to take on your next project.</p>
        <div class="input-group my-4">
            <input type="text" class="form-control border-dark text-dark" placeholder="What are you looking for?" style="background-color: white;">
            <button class="btn btn-dark" type="button">Search</button>
        </div>
        <div class="d-flex justify-content-center">
            <span class="badge bg-light text-dark me-2">Trending searches:</span>
            <span class="badge bg-secondary me-2">Landing Page</span>
            <span class="badge bg-secondary me-2">Mobile App</span>
            <span class="badge bg-secondary me-2">Logo Design</span>
        </div>
    </div>

    <div class="container py-5">
        <h2 class="mb-4">Popular Projects</h2>
        <div class="row row-cols-1 row-cols-md-3 g-4">
            <div class="col">
                <div class="card border-dark">
                    <img src="image1.jpg" class="card-img-top" alt="Project 1">
                    <div class="card-body">
                        <h5 class="card-title">Geometrics</h5>
                        <p class="card-text">A project on geometric designs.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card border-dark">
                    <img src="image2.jpg" class="card-img-top" alt="Project 2">
                    <div class="card-body">
                        <h5 class="card-title">Low Poly Designs</h5>
                        <p class="card-text">A project on low poly designs.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card border-dark">
                    <img src="image3.jpg" class="card-img-top" alt="Project 3">
                    <div class="card-body">
                        <h5 class="card-title">Conspiracies</h5>
                        <p class="card-text">A project on Conspiracies.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <footer class="bg-dark text-white py-4">
        <div class="container text-center">
            <p>Designed by SANTHOSH KUMAR P</p>
        </div>
    </footer>
 
</body>
</html>
```

## OUTPUT:

![Screenshot (27)](https://github.com/user-attachments/assets/7a40c0a8-9f5b-47f5-875e-dedab42e1663)


![Screenshot (28)](https://github.com/user-attachments/assets/efb52613-9e12-4791-a076-e2c5a280870b)


![Screenshot (29)](https://github.com/user-attachments/assets/05b4c840-32eb-4a3c-9f19-5be0f0956e3f)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
