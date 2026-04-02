# Anjali-s-BUTIQUE-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Anjali’s Butiq</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Poppins&display=swap" rel="stylesheet">

<style>
body {
  margin: 0;
  font-family: 'Poppins', sans-serif;
  scroll-behavior: smooth;
}

/* HERO */
.hero {
  height: 100vh;
  position: relative;
  overflow: hidden;
}

.hero img {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
  animation: fade 10s infinite;
}

.hero img:nth-child(2) {
  animation-delay: 5s;
}

@keyframes fade {
  0% {opacity: 0;}
  20% {opacity: 1;}
  45% {opacity: 1;}
  70% {opacity: 0;}
  100% {opacity: 0;}
}

.hero-content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: white;
}

.shop-name {
  font-family: 'Playfair Display', serif;
  font-size: 50px;
}

.tagline {
  font-size: 18px;
}

.btn {
  background: #ff4d6d;
  color: white;
  padding: 12px 25px;
  border: none;
  cursor: pointer;
  border-radius: 5px;
}

/* LOGO */
.logo {
  position: fixed;
  top: 20px;
  right: 20px;
  width: 70px;
  animation: spin 5s linear infinite;
}

@keyframes spin {
  from {transform: rotate(0deg);}
  to {transform: rotate(360deg);}
}

/* PRODUCTS */
.products {
  padding: 50px;
  text-align: center;
}

.carousel {
  display: flex;
  gap: 20px;
  overflow: hidden;
}

.track {
  display: flex;
  gap: 20px;
  animation: scroll 15s linear infinite;
}

@keyframes scroll {
  from {transform: translateX(0);}
  to {transform: translateX(-50%);}
}

.card {
  min-width: 250px;
  border: 1px solid #ddd;
  border-radius: 10px;
  overflow: hidden;
}

.card img {
  width: 100%;
  height: 250px;
  object-fit: cover;
}

.price {
  color: green;
  font-weight: bold;
}

.order-btn {
  display: inline-block;
  margin: 10px;
  padding: 10px 20px;
  background: green;
  color: white;
  text-decoration: none;
  border-radius: 5px;
}

footer {
  background: #111;
  color: white;
  text-align: center;
  padding: 20px;
}
</style>
</head>

<body>

<!-- LOGO -->
<img src="https://i.ibb.co/5g7XvmjH/IMG-3412.png" class="logo">

<!-- HERO -->
<div class="hero">
  <img src="https://i.ibb.co/xKSQXd2j/IMG-2704.jpg">
  <img src="https://i.ibb.co/fzmJtPKb/IMG-2710.jpg">

  <div class="hero-content">
    <div class="shop-name">Anjali’s Butiq</div>
    <div class="tagline">We offer all types of female wear stitch at very low price in market</div>
    <br>
    <button class="btn" onclick="scrollToProducts()">Shop Now</button>
  </div>
</div>

<!-- PRODUCTS -->
<div id="products" class="products">
  <h2>Our Services</h2>

  <div class="carousel">
    <div class="track">

      <!-- Suit -->
      <div class="card">
        <img src="https://i.ibb.co/cS6pcV4h/IMG-3413.jpg">
        <h3>Suit Salwar Stitch</h3>
        <p class="price">₹400</p>
        <a href="https://wa.me/9050953173" class="order-btn">Order Now</a>
      </div>

      <!-- Plazo -->
      <div class="card">
        <img src="https://i.ibb.co/KxM3ZRPq/IMG-3414.webp">
        <h3>Plazo Stitch</h3>
        <p class="price">₹299</p>
        <a href="https://wa.me/9050953173" class="order-btn">Order Now</a>
      </div>

      <!-- Kurti -->
      <div class="card">
        <img src="https://i.ibb.co/v6m3CMfh/IMG-3415.jpg">
        <h3>Kurti Stitch</h3>
        <p class="price">₹350</p>
        <a href="https://wa.me/9050953173" class="order-btn">Order Now</a>
      </div>

      <!-- duplicate for smooth loop -->
      <div class="card">
        <img src="https://i.ibb.co/cS6pcV4h/IMG-3413.jpg">
        <h3>Suit Salwar Stitch</h3>
        <p class="price">₹400</p>
      </div>

    </div>
  </div>
</div>

<!-- FOOTER -->
<footer>
  <p>Email: abhisheksharma73031@gmail.com</p>
  <p>THANKS FOR VISITING ❤️ LOVE FROM ANJALI’s BUTIQ</p>
</footer>

<script>
function scrollToProducts() {
  document.getElementById("products").scrollIntoView({ behavior: "smooth" });
}
</script>

</body>
</html>
