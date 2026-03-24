<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Food Order Website</title>

  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f8f8f8;
    }

    header {
      background: #ff4d4d;
      color: white;
      padding: 15px;
      text-align: center;
      font-size: 22px;
      font-weight: bold;
    }

    .container {
      padding: 15px;
    }

    .food-card {
      background: white;
      border-radius: 10px;
      padding: 15px;
      margin-bottom: 15px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      transition: transform 0.2s;
    }

    .food-card:hover {
      transform: scale(1.03);
    }

    .food-card img {
      width: 100%;
      border-radius: 10px;
      height: 180px;
      object-fit: cover;
    }

    .food-card h3 {
      margin: 10px 0 5px;
    }

    .food-card p {
      color: gray;
      font-size: 14px;
    }

    .price {
      font-weight: bold;
      margin: 8px 0;
    }

    button {
      width: 100%;
      padding: 10px;
      background: #ff4d4d;
      color: white;
      border: none;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
    }

    button:hover {
      background: #e60000;
    }

    footer {
      text-align: center;
      padding: 10px;
      font-size: 13px;
      color: gray;
    }
  </style>
</head>

<body>

<header>
  🍽️ Food Order
</header>

<div class="container">

  <div class="food-card">
    <img src="https://images.unsplash.com/photo-1600891964599-f61ba0e24092">
    <h3>Pizza</h3>
    <p>Cheesy delicious pizza</p>
    <div class="price">₹199</div>
    <button onclick="order('Pizza')">Order Now</button>
  </div>

  <div class="food-card">
    <img src="https://images.unsplash.com/photo-1550547660-d9450f859349">
    <h3>Burger</h3>
    <p>Juicy burger with fries</p>
    <div class="price">₹149</div>
    <button onclick="order('Burger')">Order Now</button>
  </div>

  <div class="food-card">
    <img src="https://images.unsplash.com/photo-1628294895950-9805252327bc">
    <h3>Dosa</h3>
    <p>South Indian crispy dosa</p>
    <div class="price">₹99</div>
    <button onclick="order('Dosa')">Order Now</button>
  </div>

</div>

<footer>
  © 2025 Food Order Website
</footer>

<script>
  function order(item) {
    alert(item + " ordered successfully!");
  }
</script>

</body>
</html>
