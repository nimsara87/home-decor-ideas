<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Home Decor World</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #f4f4f4;
      overflow-x: hidden;
    }

    /* NAVIGATION BAR */
    .nav-bar {
      position: absolute;
      top: 20px;
      left: 30px;
      right: 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 10;
    }

    .nav-bar .logo {
      color: rgb(255, 255, 255);
      font-size: 22px;
      font-weight: bold;
    }

    .nav-bar ul {
      list-style: none;
      display: flex;
      gap: 20px;
    }

    .nav-bar ul li a {
      color: rgb(255, 255, 255);
      text-decoration: none;
      font-weight: bold;
      font-size: 16px;
      transition: color 0.3s;
    }

    .nav-bar ul li a:hover {
      color: #ffd700;
    }

    /* HERO SECTION */
    .hero {
      height: 100vh;
      background: url('https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&w=1500&q=80') no-repeat center center/cover;
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
    }

    .hero::after {
      content: "";
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background-color: rgba(0,0,0,0.6);
      z-index: 0;
    }

    .hero-content {
      position: relative;
      z-index: 1;
      animation: fadeInZoom 2s ease;
    }

    .hero h1 {
      font-size: 48px;
      font-weight: bold;
      margin-bottom: 15px;
      text-shadow: 0 2px 8px rgba(0,0,0,0.3);
    }

    .hero p {
      font-size: 20px;
      color: #eee;
      margin-bottom: 25px;
    }

    .hero a {
      background: #ffffff;
      color: #333;
      padding: 12px 24px;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
      transition: all 0.3s ease;
    }

    .hero a:hover {
      background: #007BFF;
      color: white;
    }

    @keyframes fadeInZoom {
      0% { opacity: 0; transform: scale(0.8); }
      100% { opacity: 1; transform: scale(1); }
    }

    /* ROOMS SECTION */
    #rooms {
      padding: 60px 20px;
      text-align: center;
    }

    #rooms h2 {
      font-size: 32px;
      margin-bottom: 30px;
      color: #333;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 25px;
      padding: 0 10px;
    }

    .card {
      background: #fff;
      border-radius: 5px;
      box-shadow: 0 6px 16px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 12px 20px rgba(0,0,0,0.15);
    }

    .card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }

    .card h3 {
      padding: 15px 10px 5px;
      font-size: 20px;
      color: #222;
    }

    .card p {
      padding: 0 10px 15px;
      color: #555;
      font-size: 14px;
    }

    .card a {
      display: inline-block;
      margin: 0 0 15px;
      background: #007BFF;
      color: white;
      padding: 10px 20px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s;
    }

    .card a:hover {
      background: #0056b3;
    }
  </style>
</head>
<body>

<!-- Navigation -->
<div class="nav-bar">
  <div class="logo">Home Decor World</div>
  <ul>
    <li><a href="about.html">Home</a></li>
    <li><a href="https://amzn.to/4nlDzUP">Shop</a></li>
    <li><a href="about-index.html">About</a></li>
  </ul>
</div>

<!-- Hero Section -->
<div class="hero">
  <div class="hero-content">
    <h1>Welcome</h1>
    <p>Find amazing inspiration for every room in your home</p>
    <a href="#rooms">Explore Rooms</a>
  </div>
</div>

<!-- Rooms Section -->
<div id="rooms">
  <h2>Our Room Inspirations</h2>

  <div class="grid">
    <div class="card">
      <img src="https://cdn.pixabay.com/photo/2014/11/27/20/14/waiting-room-548136_1280.jpg" alt="Living Room">
      <h3>Living Room</h3>
      <p>Creative and cozy space to welcome guests and relax.</p>
      <a href="living room-index.html">See more</a>
    </div>

    <div class="card">
      <img src="https://cdn.pixabay.com/photo/2015/04/18/13/23/kitchen-728727_1280.jpg" alt="Kitchen">
      <h3>Kitchen</h3>
      <p>Clean and functional design for joyful cooking.</p>
      <a href="kitchen-index.html">See more</a>
    </div>

    <div class="card">
      <img src="https://cdn.pixabay.com/photo/2021/02/01/09/55/bedroom-5969977_1280.jpg" alt="Bedroom">
      <h3>Bedroom</h3>
      <p>Comfortable and peaceful for a perfect night's sleep.</p>
      <a href="privet room-index.html">See more</a>
    </div>

   <div class="card">
  <img src="https://cdn.pixabay.com/photo/2024/04/10/14/03/bathroom-8688132_1280.jpg" alt="Modern Bathroom">
  <h3>Bathroom</h3>
  <p>Minimalist design with clean lines and smart fixtures ideas</p>
  <a href="Bathroom-index.html">See more</a>
</div>

    <div class="card">
      <img src="https://cdn.pixabay.com/photo/2021/02/11/23/21/house-6006723_1280.jpg" alt="Dining Room">
      <h3>Dining Room</h3>
      <p>Elegant dining area for meals and memories.</p>
      <a href="Dining Room-index.html">See more</a>
    </div>

    <div class="card">
      <img src="https://cdn.pixabay.com/photo/2016/07/10/15/58/house-1507920_1280.jpg" alt="Garden">
      <h3>Garden</h3>
      <p>Relaxing outdoor area with plants and fresh air.</p>
      <a href="Garden-index.html">See more</a>
    </div>
  </div>
</div>

</body>
</html>
