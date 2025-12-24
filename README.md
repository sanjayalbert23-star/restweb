# Ex.07 Restaurant Website
## Date:24/12/2025
## ref:25011969

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
~~~
home.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Restaurant Homepage</title>

  <style>
    body { 
      font-family: Arial, sans-serif; 
      margin: 0; 
      padding: 0; 
    }

    header { 
      background: #b22222; 
      color: white; 
      padding: 20px; 
      text-align: center; 
    }

    nav { 
      background: #333; 
      display: flex; 
      justify-content: center; 
    }

    nav a { 
      color: white; 
      padding: 14px 20px; 
      text-decoration: none;
      transition: background 0.3s; 
    }

    nav a:hover { 
      background: #ff6347; 
    }

    section {
      padding: 60px; 
      text-align: center; 
    }

    footer { 
      background: #333; 
      color: white; 
      text-align: center; 
      padding: 15px;
      font-size: 14px; 
    }
  </style>
</head>

<body>
  <header>
    <h1>🍴 CUTLERY KINGS 🍴</h1>
    <p>Welcome to our restaurant</p>
  </header>

  <nav>
    <a href="offers.html">Offers</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact</a>
  </nav>

  <section>
    <h2>Welcome!</h2>
    <p>This is the homepage. Use the navigation above to view menu, administration, and contact pages.</p>
  </section>

  <footer>
    <p>&copy; 2025 Cutlery Kings | All Rights Reserved</p>
  </footer>
</body>
</html>

offers.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Special Offers</title>

  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; }

    header { 
      background: #b22222; 
      color: white; 
      padding: 20px; 
      text-align: center; 
    }

    nav { 
      background: #333; 
      display: flex; 
      justify-content: center; 
    }

    nav a { 
      color: white; 
      padding: 14px 20px; 
      text-decoration: none;
      transition: background 0.3s;  
    }

    nav a:hover { 
      background: #ff6347; 
    }

    section { 
      padding: 40px; 
      text-align: center; 
    }

    .offers { 
      display: grid; 
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); 
      gap: 20px; 
      padding: 20px; 
    }

    .offers img { 
      width: 100%; 
      border-radius: 10px; 
      box-shadow: 0 3px 6px rgba(0,0,0,0.2);
      transition: transform 0.3s;   
    }

    .offers img:hover {
      transform: scale(1.03);      
    }

    .offer-card {
      background: #fff8f0;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 3px 6px rgba(0,0,0,0.1);
      transition: transform 0.3s;   
    }

    .offer-card:hover {
      transform: translateY(-5px); 
    }

    .offer-card h3 {
      color: #b22222;
    }
  </style>
</head>

<body>
  <header>
    <h1>🎉 Special Offers 🎉</h1>
    <p>Grab the best deals while they last!</p>
  </header>

  <nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact</a>
  </nav>

  <section>
    <div class="offers">
      <div class="offer-card">
        <img src="/static/pizza.jpg" alt="50% Off Pizza">
        <h3>50% Off on All Pizzas</h3>
        <p>Enjoy delicious pizzas at half the price every Monday.</p>
      </div>

      <div class="offer-card">
        <img src="/static/burger.jpg" alt="Buy 1 Get 1 Free Burger">
        <h3>Buy 1 Get 1 Free</h3>
        <p>Order a burger and get another one absolutely free every Friday.</p>
      </div>

      <div class="offer-card">
        <img src="/static/desert.jpg" alt="Free Dessert">
        <h3>Free Dessert</h3>
        <p>Get a free dessert with every meal above ₹500.</p>
      </div>
    </div>
  </section>
</body>
</html>

menu.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Menu</title>

  <style>
    body { 
      font-family: Arial, sans-serif; 
      margin: 0; 
      padding: 0; 
    }

    header { 
      background: #b22222; 
      color: white; 
      padding: 20px; 
      text-align: center; 
    }

    nav { 
      background: #333; 
      display: flex; 
      justify-content: center; 
    }

    nav a { 
      color: white; 
      padding: 14px 20px; 
      text-decoration: none; 
    }

    nav a:hover { 
      background: #ff6347; 
    }

    .gallery { 
      display: grid; 
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); 
      gap: 20px; 
      padding: 20px; 
      text-align: center;
    }

    .gallery img { 
      width: 100%; 
      border-radius: 10px; 
      box-shadow: 0 3px 6px rgba(0,0,0,0.2);
    }

    .gallery h2 {
      color: #ed3a3a;
    }
  </style>
</head>

<body>
  <header>
    <h1>Our Menu</h1>
  </header>

  <nav>
    <a href="home.html">Home</a>
    <a href="offers.html">Offers</a>
    <a href="admin.html">Administration</a>
    <a href="contact.html">Contact</a>
  </nav>

  <div class="gallery">
    <h2>Burger</h2>
    <img src="/static/burger.jpg" alt="Burger">

    <h2>Pizza</h2>
    <img src="/static/pizza.jpg" alt="Pizza">

    <h2>Pasta</h2>
    <img src="/static/pasta.jpg" alt="Pasta">

    <h2>Dessert</h2>
    <img src="/static/desert.jpg" alt="Dessert">

    <h2>Sandwich</h2>
    <img src="/static/sandwich.webp" alt="Sandwich">

    <h2>Noodles</h2>
    <img src="/static/noodles.webp" alt="Noodles">
  </div>
</body>
</html>

admin.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Administration</title>

  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; }

    header { 
      background: #b22222; 
      color: white; 
      padding: 20px; 
      text-align: center; 
    }

    nav { 
      background: #333; 
      display: flex; 
      justify-content: center; 
    }

    nav a { 
      color: white; 
      padding: 14px 20px; 
      text-decoration: none; 
    }

    nav a:hover { 
      background: #ff6347; 
    }

    .team { 
      display: flex; 
      justify-content: center; 
      flex-wrap: wrap; 
      gap: 20px; 
      padding: 20px; 
    }

    .member { 
      text-align: center; 
    }

    .member img { 
      width: 180px; 
      border-radius: 50%;
      transition: transform 0.3s;  
    }

    .member img:hover {
      transform: scale(1.05);       
    }
  </style>
</head>

<body>
  <header>
    <h1>Administration</h1>
  </header>

  <nav>
    <a href="home.html">Home</a>
    <a href="offers.html">Offers</a>
    <a href="menu.html">Menu</a>
    <a href="contact.html">Contact</a>
  </nav>

  <div class="team">
    <div class="member">
      <img src="/static/chef1.avif" alt="Chef">
      <p><b>Chef Frank</b></p>
    </div>

    <div class="member">
      <img src="/static/chef2.webp" alt="Chef">
      <p><b>Chef John</b></p>
    </div>

    <div class="member">
      <img src="/static/chef3.avif" alt="Chef">
      <p><b>Chef Mark</b></p>
    </div>

    <div class="member">
      <img src="/static/manager.jpg" alt="Manager">
      <p><b>Manager Johan</b></p>
    </div> <!-- fixed -->

    <div class="member">
      <img src="/static/assiatant.jpg" alt="Asst-Manager">
      <p><b>Manager Josan</b></p>
    </div>
  </div>
</body>
</html>

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact</title>

  <style>
    body { 
      font-family: Arial, sans-serif; 
      margin: 0; 
      padding: 0; 
    }

    header { 
      background: #b22222; 
      color: white; 
      padding: 20px; 
      text-align: center; 
    }

    nav { 
      background: #333; 
      display: flex; 
      justify-content: center; 
    }

    nav a { 
      color: white; 
      padding: 14px 20px; 
      text-decoration: none;
      transition: background 0.3s;   
    }

    nav a:hover { 
      background: #ff6347; 
    }

    section { 
      padding: 40px; 
      text-align: center;
      font-size: 16px;              
    }
  </style>
</head>

<body>
  <header>
    <h1>Contact Us</h1>
  </header>

  <nav>
    <a href="home.html">Home</a>
    <a href="offers.html">Offers</a>
    <a href="menu.html">Menu</a>
    <a href="admin.html">Administration</a>
  </nav>

  <section>
    <p>📍 Address: 123 Main Street, Your City</p>
    <p>📞 Phone: +91 98765 43210</p>
    <p>📧 Email: contact@restaurant.com</p>
  </section>
</body>
</html>
~~~

## OUTPUT:
![alt text](<first image.jpeg>)
![alt text](<second image.jpeg>)
![alt text](<third image.jpeg>)
![alt text](<fourth image.jpeg>)
![alt text](<fifth image.jpeg>)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
