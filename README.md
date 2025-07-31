<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Modern Mode</title>
  <link rel="stylesheet" href="styles.css"/>
</head>
<body>

  <!-- Navigation Bar -->
  <header class="navbar">
    <div class="nav-left">
      <a href="#">HOME</a>
      <a href="#">ABOUT</a>
      <a href="#">WEDDING</a>
    </div>
    <div class="nav-center">
      <div class="brand">
        <p class="established">ESTD 2018</p>
        <h1>MODERN MODE</h1>
        <p class="tagline">PREMIUM BRAND</p>
      </div>
    </div>
    <div class="nav-right">
      <a href="#">MENS</a>
      <a href="#">WOMENS</a>
      <a href="#">LOGIN</a>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <div class="hero-content">
      <h2>MODERN MODE</h2>
      <p class="quote">Style is a way to say who you are without having to speak.</p>
      <button onclick="shopNow()">SHOP NEW ARRIVALS</button>
    </div>
  </section>

  <script src="script.js"></script>
</body>
</html>


style css.
/* Reset & Base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body {
  background-color: #102224;
  color: white;
}

/* Navbar Styling */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #1f3a3d;
  padding: 20px 40px;
}

.navbar a {
  margin: 0 10px;
  color: white;
  text-decoration: none;
  font-weight: 500;
}

.navbar a:hover {
  color: gold;
}

.brand {
  text-align: center;
}

.brand h1 {
  font-size: 20px;
  font-weight: bold;
}

.established {
  font-size: 10px;
  color: #ccc;
}

.tagline {
  font-size: 12px;
  color: gold;
  font-weight: bold;
}

/* Hero Section */
.hero {
  background: url('clothes.jpg') center center/cover no-repeat;
  height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 30px;
  text-align: center;
  position: relative;
}

.hero::before {
  content: "";
  position: absolute;
  top: 0; left: 0;
  height: 100%; width: 100%;
  background-color: rgba(16, 34, 36, 0.8);
}

.hero-content {
  position: relative;
  z-index: 1;
}

.hero h2 {
  font-size: 36px;
  margin-bottom: 20px;
}

.quote {
  font-style: italic;
  font-size: 18px;
  margin-bottom: 30px;
  color: #ccc;
}

.hero button {
  padding: 12px 25px;
  background-color: #264746;
  color: white;
  border: none;
  border-radius: 25px;
  cursor: pointer;
  font-weight: 600;
}

.hero button:hover {
  background-color: #356a69;
}