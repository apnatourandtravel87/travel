<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apna Tour & Travel - Car Rental</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
    <style>
        .success-popup {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: white;
            border: 1px solid #4CAF50;
            padding: 20px;
            z-index: 1000;
        }
        .carousel-inner img {
            max-height: 400px;
            object-fit: cover;
        }
    </style>
</head>
<body>

    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="index.html">Apna Tour & Travel</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
                <li class="nav-item"><a class="nav-link" href="services.html">Services</a></li>
                <li class="nav-item"><a class="nav-link" href="contact.html">Contact Us</a></li>
                <li class="nav-item"><a class="nav-link" href="about.html">About Us</a></li>
            </ul>
        </div>
    </nav>

    <!-- Header -->
    <header class="header text-center">
        <div class="container">
            <h1 class="display-4">WELCOME TO APNA TOUR & TRAVEL</h1>
            <p class="lead">BOOK YOUR DESTINATION TODAY CALL:- 8709917730</p>
        </div>
    </header>

    <!-- Car Gallery Carousel -->
    <div class="container text-center">
        <h2 class="mt-5 font-weight-bold">Available Cars</h2>
        <p>Explore our diverse fleet, featuring top brands like Tata, Suzuki, and Hyundai, available at unbeatable rates.</p>
        <div id="carGalleryCarousel" class="carousel slide" data-ride="carousel">
            <div class="carousel-inner" id="carGallery">
                <!-- First car (Active) - Suzuki Ertiga -->
                <div class="carousel-item active">
                    <img src="https://www.dropbox.com/scl/fi/wsj8f972ccewv9gruxdzn/2018-Suzuki-Ertiga-2018-Maruti-Ertiga-Metallic-Magma-Gray.jpg?rlkey=ivhcd0l6zxn8qgm6qp7x84xbz&st=u3plvzvg&dl=0" class="d-block w-100" alt="Suzuki Ertiga 2018">
                </div>
                <!-- Second car -->
                <div class="carousel-item">
                    <img src="images/car2.jpg" class="d-block w-100" alt="Car Model 2">
                </div>
                <!-- Third car -->
                <div class="carousel-item">
                    <img src="images/car3.jpg" class="d-block w-100" alt="Car Model 3">
                </div>
            </div>
            <a class="carousel-control-prev" href="#carGalleryCarousel" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carGalleryCarousel" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
    </div>

    <!-- Booking Section -->
    <div class="container text-center my-5">
        <h2 class="font-weight-bold">Book Your Car Now!</h2>
        <p>If you're interested in booking a car, click the button below to contact us directly via WhatsApp.</p>
        <a href="https://wa.me/+918434512031?text=I%20want%20to%20book%20a%20car" class="btn btn-success btn-lg" target="_blank">Book Now</a>
        <p class="mt-3">Our car rental services are available 24/7, ensuring you always have a vehicle when you need it.</p>
    </div>

    <!-- Callback Request Form -->
    <div class="container my-5">
        <h2 class="font-weight-bold text-center">Request a Callback</h2>
        <form id="callbackForm" action="https://docs.google.com/forms/d/e/1FAIpQLSdveHs8SyPT_iYo7yOmpfLEFdOc_Ro9kk7uf2DzO3LACfc4aw/formResponse" method="POST" target="hidden_iframe">
            <input type="hidden" name="entry.2051638085" id="nameEntry" required>
            <input type="hidden" name="entry.646178205" id="mobileEntry" required>
            <div class="form-group">
                <label for="name">Name:</label>
                <input type="text" class="form-control" id="name" required>
            </div>
            <div class="form-group">
                <label for="mobile">Mobile Number:</label>
                <input type="tel" class="form-control" id="mobile" required>
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
        </form>
    </div>

    <!-- Success Popup -->
    <div class="success-popup" id="successPopup">
        <h4>Success!</h4>
        <p>You will receive a call back within minutes.</p>
        <button class="btn btn-success" onclick="closePopup()">Close</button>
    </div>

    <!-- Hidden Iframe for Google Forms submission -->
    <iframe name="hidden_iframe" style="display:none;"></iframe>

    <!-- Contact Info -->
    <div class="container contact-info text-center">
        <h2 class="font-weight-bold">Contact Us</h2>
        <p><a href="mailto:apnatourandtravel87@gmail.com"><i class="fas fa-envelope"></i> apnatourandtravel87@gmail.com</a></p>
        <p><a href="tel:+918709917730"><i class="fas fa-phone-alt"></i> +91 8709917730</a></p>
        <p><a href="https://maps.app.goo.gl/8eivgp8uJgXrBYzi7" target="_blank"><i class="fas fa-map-marker-alt"></i> Roshpa Tower, Kanka, Ranchi, Jharkhand 834001</a></p>
        <p>Follow us on social media!</p>
        <a href="https://facebook.com/iamsayanmandal" target="_blank" class="social-icon"><i class="fab fa-facebook-f"></i> Facebook</a> |
        <a href="https://www.instagram.com/nnehal_singh_rajput/" target="_blank" class="social-icon"><i class="fab fa-instagram"></i> Instagram</a>
    </div>

    <!-- Footer -->
    <footer class="text-center mt-5">
        <p>© 2024 Apna Tour & Travel. All rights reserved.</p>
        <p>Enjoy our affordable and transparent pricing for all your travel needs.</p>
    </footer>

    <!-- jQuery -->
    <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
    <!-- Bootstrap JS -->
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.bundle.min.js"></script>
    
    <script>
        // Handle form submission
        $(document).ready(function() {
            $('#callbackForm').on('submit', function(event) {
                event.preventDefault(); // Prevent default form submission
                
                // Get input values
                const name = $('#name').val();
                const mobile = $('#mobile').val();

                // Assign values to hidden fields
                $('#nameEntry').val(name);
                $('#mobileEntry').val(mobile);

                // Submit the form
                this.submit();

                // Show success popup
                $('#successPopup').fadeIn();
            });
        });

        // Close the success popup
        function closePopup() {
            $('#successPopup').fadeOut();
        }
    </script>
</body>
</html>
