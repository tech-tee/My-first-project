<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Speedlink Clone</title>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            line-height: 1.6;
            color: #333;
        }

        header {
            background: #004aad;
            padding: 20px;
            color: #fff;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 20px;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 15px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: 600;
        }

        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                gap: 10px;
            }
        }
    </style>
</head>
<body>

<header>
    <div class="container">
        <nav>
            <div class="logo">
                <h1>Speedlink</h1>
            </div>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </div>
</header>

</body>
</html>


General Header Styles
.promo-header {
    background-color: #f1f1f1;
    padding: 10px 20px;
}

.promo-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap; /* Ensures content wraps on smaller screens */
}

.contact-info {
    font-size: 14px;
    color: #333;
    margin-right: 20px;
}

.social-media a {
    color: #333;
    padding: 5px;
    text-decoration: none;
    margin: 0 5px;
}

/* Existing Promotional Header Styles (if you have any) */

/* Add the new promotional header styles below or integrate it with your existing styles */
.promo-header {
    background: linear-gradient(to right, white 0%, #f0f0f0 25%, black 75%, #101010 100%);
    color: black; /* Text color on black background will be black by default */
    padding: 10px 0;
    position: fixed;  /* Fixes the header to the top */
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1000;  /* Ensures it's above other content */
    text-align: center;
    font-size: 14px;
    transition: background 1s ease; /* Add a transition effect */
}

.promo-header .promo-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

.promo-header .promo-content .social-media {
    display: flex;
    gap: 15px;
}

.promo-header .promo-content .social-icon {
    color: white;
    font-size: 20px;
    text-decoration: none;
}

.promo-header .promo-content .social-icon:hover {
    color: #007bff;
}

/* Add space below the fixed header */
body {
    margin-top: 50px; /* Adjust this value based on your header's height */
}

/* Main Header Styling */
.main-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    color: white;
  
}

/* Logo Styling */
.logo-img {
    width: 100px;
    height: auto;
    display: block;
    padding-left: 20px;
}

/* Navbar Section */
.navbar {
    list-style: none;
    display: flex;
    justify-content: center;
    padding: 0;
    background: linear-gradient(to right, white 0%, #f0f0f0 25%, black 75%, #101010 100%);
    margin: 0;
    position: relative; /* Fixes the navbar to the top */
    
    
    
}

/* Navbar styles */
.navbar {
    background-color: #333;
    padding: 10px;
}

.navbar ul {
    list-style-type: none;
    display: flex;
    justify-content: space-around;
    gap: 20px;
    margin: 0;
    padding: 0;
}

/* Optional hover effect */
.navbar a:hover {
    text-decoration: underline;
}

.navbar li {
    padding: 15px;
}

.navbar a {
    text-decoration: none;
    
}

/* Hero Section Styling with Video */
.hero {
    position: relative;
    height: 400px;  /* Adjust height based on design */
    overflow: hidden; /* Hide any overflowed content */
    background-size: cover; /* Ensure the background image covers the section */
    background-position: center center; /* Center the background image */
    display: flex;
    justify-content: center;
    align-items: center;
    color: white; /* White text on dark background */
    text-align: center;
}

#hero-video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;  /* Ensures the video covers the section without distorting */
    z-index: -1;  /* Keeps the video in the background */
}

.hero-content {
    position: relative;
    z-index: 1;  /* Keeps the text content above the video */
    color: black; /* Text color */
    text-align: center; /* Centers the content */
    padding: 20px;  /* Adds some padding */
}

.hero h1 {
    font-size: 36px;
    margin-bottom: 10px;
}

.hero p {
    font-size: 18px;
    margin-bottom: 20px;
}

.cta-button {
    background-color: #007bff;
    color: white;
    text-decoration: none;
    padding: 15px 30px;
    font-size: 16px;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

.cta-button:hover {
    background-color: #0056b3;
}

@media (max-width: 768px) {
    #hero-video {
        display: none; /* Hide video on mobile */
    }
    .hero {
        background: url('images/8597294-hd_1920_1080_30fps.mp4') no-repeat center center/cover;
    }
}

/* Main Section */
.main-section {
    padding: 40px;
    background: url('images/pexels-gdtography-277628-911738.jpg'); /* Same background for both the text and image */
    height:400px;
    background-position: center center;
    background-size: cover;
}

/* Content: Flexbox for side-by-side layout */
.content {
    display: flex;
    align-items: center; /* Vertically align the text and image */
    justify-content: space-between; /* Space between the text and the image */
    padding: 20px;
    border-radius: 10px; /* Optional rounded corners */
} 

/* Text Section */
.text {
    flex: 1; /* Takes up available space */
    padding-right: 20px; /* Space between text and image */
}

.text h2 {
    font-size: 2em;
    color: #333;
}

.text p {
    font-size: 1.2em;
    color: #666;
}

/* Image Section */
.image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    object-fit: cover; /* Ensures the image covers the space properly */
    max-width: 500px; /* Optional: Limit image size */
}

/* Responsive Design for Smaller Screens */
@media (max-width: 768px) {
    .content {
        flex-direction: column; /* Stack the text and image vertically on small screens */
        text-align: center; /* Center the text on smaller screens */
    }

    .image img {
        max-width: 100%; /* Make the image responsive */
    }
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Website</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
    <link rel="stylesheet" href="assets/styles.css">  <!-- Link to external CSS file -->
</head>
<body>
    <!-- Top Promotional Header Section -->
    <header class="promo-header">
        <div class="promo-content">
            <span class="contact-info">Call us at: 1-800-123-4567</span>
            <div class="social-media">
            <a href="https://facebook.com" target="_blank" class="social-icon"><i class="fab fa-facebook-f"></i></a>
            <a href="https://twitter.com" target="_blank" class="social-icon"><i class="fab fa-twitter"></i></a>
            <a href="https://instagram.com" target="_blank" class="social-icon"><i class="fab fa-instagram"></i></a>
            </div>
        </div>    
    </header>

    <!-- Main Header Section -->
    <header class="main-header">
        <!-- Logo Section -->
        <div class="logo">
            <a href="#"><img src="assets/images/big-wing-butterfly.png" alt="Your Brand Name" class="logo-img" /></a>
        </div>

        <!-- Navbar Section -->
        <nav>
            <ul class="navbar">
                <nav class="navbar">
                    <ul >
                        <li><a href="#home" style="color: #101010;">Home</a></li>
                        <li><a href="#services" style="color: black;">Services</a></li>
                        <li><a href="#about" style="color:  #f0f0f0;">About</a></li>
                        <li><a href="#contact" style="color: white;">Contact</a></li>
                    </ul>
                </nav>
                
            </ul>
        </nav>
    </header>
    <!-- Hero Section Below Navbar -->
     <!-- Video Background -->
    <video autoplay muted loop id="hero-video">
        <source src="assets/images/8597294-hd_1920_1080_30fps.mp4" type="video/mp4">
    </video>
<section class="hero">
    <div class="hero-content">
        <h1>Welcome to Our Website</h1>
        <p>We provide high-quality services for your needs.</p>
        <br>
        <a href="#services" class="cta-button">Explore Our Services</a>
    </div>
</section>

<!-- Main Section -->
<section class="main-section">
    <div class="content">
        <div class="text">
            <h2>Our Amazing Services</h2>
            <p>We provide top-notch solutions to help you achieve your goals. Get started today!</p>
        </div>
        <div class="image">
            <img src="assets/images/pexels-martabranco-30147363.jpg" alt="Amazing Services" />
        </div>
    </div>
</section>

</body>
<footer>
    <p>Icons made by <a href="https://www.flaticon.com/free-icons/insect" title="Insect icons">Freepik</a> from <a href="https://www.flaticon.com" title="Flaticon">www.flaticon.com</a></p>
</footer>

</html>
