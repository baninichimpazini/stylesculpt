index.html:

<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>StyleSculpt</title>

<link rel="stylesheet" href="style.css">

</head>

<body>

<header>

<nav>

<ul>

<li><a href="#home">Home</a></li>

<li><a href="#about">About</a></li>

<li><a href="#products">Products</a></li>

<li><a href="#contact">Contact</a></li>

</ul>

</nav>

</header>

<section id="home" class="hero">

<div class="hero-content">

<h1>StyleSculpt</h1>

<p>Fashion That Shapes You</p>

</div>

</section>

<section id="about" class="about">

<h2>About Us</h2>

<p>StyleSculpt is a fashion brand dedicated to helping you express your individuality through carefully curated collections. We believe in sustainable fashion that doesn't compromise on style.</p>

</section>

<section id="products" class="products">

<h2>Our Products</h2>

<div class="product-list">

<div class="product-item">

<img src="https://via.placeholder.com/300x400?text=Product+1" alt="Product 1">

<h3>Elegant Blouse</h3>

<p>$49.99</p>

</div>

<div class="product-item">

<img src="https://via.placeholder.com/300x400?text=Product+2" alt="Product 2">

<h3>Classic Trousers</h3>

<p>$59.99</p>

</div>

<div class="product-item">

<img src="https://via.placeholder.com/300x400?text=Product+3" alt="Product 3">

<h3>Statement Jacket</h3>

<p>$89.99</p>

</div>

</div>

</section>

<section id="contact" class="contact">

<h2>Contact Us</h2>

<form>

<label for="name">Name:</label>

<input type="text" id="name" name="name">

<label for="email">Email:</label>

<input type="email" id="email" name="email">

<label for="message">Message:</label>

<textarea id="message" name="message"></textarea>

<button type="submit">Send</button>

</form>

</section>

<footer>

<p>&copy; 2025 StyleSculpt. All rights reserved.</p>

</footer>

<script src="script.js"></script>

</body>

</html>

style.css:

body, html {

margin: 0;

padding: 0;

font-family: Arial, sans-serif;

}

header {

background-color: #fff;

box-shadow: 0 2px 4px rgba(0,0,0,0.1);

position: fixed;

width: 100%;

top: 0;

z-index: 1000;

}

nav ul {

list-style: none;

display: flex;

justify-content: center;

padding: 20px;

}

nav ul li a {

text-decoration: none;

color: #333;

padding: 10px 20px;

font-weight: bold;

}

.hero {

height: 100vh;

background-image: url('https://via.placeholder.com/1920x1080?text=StyleSculpt+Hero');

background-size: cover;

background-position: center;

display: flex;

align-items: center;

justify-content: center;

text-align: center;

color: white;

margin-top: 60px;

}

.hero-content h1 {

font-size: 4rem;

margin-bottom: 20px;

}

.hero-content p {

font-size: 1.5rem;

}

.about, .products, .contact {

padding: 80px 20px;

text-align: center;

}

.about {

background-color: #f9f9f9;

}

.products {

background-color: #fff;

}

.product-list {

display: flex;

justify-content: center;

flex-wrap: wrap;

gap: 20px;

margin-top: 40px;

}

.product-item {

border: 1px solid #ddd;

padding: 20px;

border-radius: 5px;

width: 300px;

}

.product-item img {

max-width: 100%;

height: auto;

}

.contact form {

max-width: 500px;

margin: 0 auto;

display: flex;

flex-direction: column;

gap: 10px;

}

.contact form input, .contact form textarea {

padding: 10px;

border: 1px solid #ddd;

border-radius: 5px;

}

.contact form button {

padding: 10px;

background-color: #333;

color: white;

border: none;

cursor: pointer;

border-radius: 5px;

}

footer {

background-color: #333;

color: white;

text-align: center;

padding: 20px;

}

script.js: (optional, for form submission handling - we'll just prevent default for now)

document.querySelector('form').addEventListener('submit', function(e) {

e.preventDefault();

alert('Thank you for your message! We will get back to you soon.');

this.reset();

});
