
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cappy's Cozy Corner 🦫</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

body {
  font-family: 'Trebuchet MS', sans-serif;
  background-color: #FFF8ED;
  color: #65452F;
}

header {
  background-color: #F6DCE1;
  padding: 22px;
  text-align: center;
}

header h1 {
  font-size: 32px;
  color: #8B5E3C;
}

nav {
  margin-top: 15px;
}

nav a {
  text-decoration: none;
  color: #65452F;
  margin: 12px;
  font-weight: bold;
}

nav a:hover {
  color: #C58B5B;
}

.hero {
  text-align: center;
  padding: 75px 20px;
  background: linear-gradient(135deg, #F6DCE1, #FFF8ED, #C9D8B8);
}

.hero h2 {
  font-size: 42px;
  margin-bottom: 15px;
}

.hero p {
  font-size: 18px;
  margin-bottom: 25px;
}

.button {
  display: inline-block;
  background-color: #C58B5B;
  color: white;
  padding: 13px 25px;
  border-radius: 25px;
  text-decoration: none;
  border: none;
  cursor: pointer;
  font-size: 16px;
}

.button:hover {
  background-color: #8B5E3C;
}

section {
  padding: 55px 20px;
  text-align: center;
}

section h2 {
  font-size: 30px;
  margin-bottom: 25px;
}

.about {
  background-color: #FFFFFF;
}

.plushies {
  background-color: #FFF8ED;
}

.products {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 25px;
}

.card {
  background-color: white;
  width: 260px;
  padding: 18px;
  border-radius: 18px;
  box-shadow: 0 4px 12px #65452F20;
  transition: transform 0.3s;
}

.card:hover {
  transform: translateY(-8px);
}

.card img {
  width: 100%;
  height: 190px;
  object-fit: cover;
  border-radius: 13px;
}

.card h3 {
  margin: 14px 0 8px;
}

.price {
  color: #B47748;
  font-weight: bold;
  margin: 10px;
}

.fun {
  background-color: #C9D8B8;
}

.fun p {
  margin: 12px;
}

footer {
  background-color: #65452F;
  color: white;
  padding: 25px;
  text-align: center;
}

#message {
  font-weight: bold;
  margin-top: 15px;
  min-height: 24px;
}

@media(max-width: 600px) {
  .hero h2 {
    font-size: 30px;
  }

  nav a {
    display: inline-block;
    margin: 7px;
  }
}
</style>
</head>

<body>

<header>
  <h1>🦫 Cappy's Cozy Corner</h1>
  <p>Your little world of capybara cuteness!</p>

  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#shop">Plushies</a>
    <a href="#fun">Fun Facts</a>
  </nav>
</header>

<div class="hero" id="home">
  <h2>Welcome to the Cozy Side! 🧸</h2>
  <p>Soft hugs, tiny noses, and the cutest capybara plushies ever!</p>
  <a href="#shop" class="button">Explore Plushies ♡</a>
</div>

<section class="about" id="about">
  <h2>♡ About Our Little Shop ♡</h2>
  <p>
    Welcome to Cappy's Cozy Corner, a happy place made for
    capybara lovers! We celebrate the world's most relaxed
    animal through adorable plushies, cozy vibes, and lots of love.
  </p>
  <p>Our motto: Stay calm, stay cozy, and be a capybara!</p>
</section>

<section class="plushies" id="shop">
  <h2>Meet Our Plushie Collection 🧸</h2>

  <div class="products">

    <div class="card">
      <img src="https://loremflickr.com/500/400/capybara,plush,toy" alt="Cute capybara plushie">
      <h3>Classic Cappy</h3>
      <p>Your new cuddly best friend!</p>
      <p class="price">$19.99</p>
      <button class="button" onclick="addToCart('Classic Cappy')">♡ Choose Me</button>
    </div>

    <div class="card">
      <img src="https://loremflickr.com/500/400/capybara,stuffed,animal" alt="Capybara stuffed animal">
      <h3>Sleepy Cappy</h3>
      <p>Perfect for cozy nap times.</p>
      <p class="price">$24.99</p>
      <button class="button" onclick="addToCart('Sleepy Cappy')">♡ Choose Me</button>
    </div>

    <div class="card">
      <img src="https://loremflickr.com/500/400/capybara,baby,animal" alt="Adorable baby capybara">
      <h3>Baby Cappy</h3>
      <p>Small, sweet, and extra adorable!</p>
      <p class="price">$16.99</p>
      <button class="button" onclick="addToCart('Baby Cappy')">♡ Choose Me</button>
    </div>

  </div>

  <p id="message"></p>
</section>

<section class="fun" id="fun">
  <h2>Did You Know? 🌿</h2>
  <p>🦫 Capybaras are the largest rodents in the world!</p>
  <p>🌊 They are excellent swimmers.</p>
  <p>💚 They are known for their calm and social personalities.</p>
  <p>🍊 They enjoy eating plants and fruits.</p>
</section>

<footer>
  <h3>🦫 Cappy's Cozy Corner</h3>
  <p>Made with ♡ and lots of capybara love!</p>
  <p>© 2026 Cappy's Cozy Corner</p>
</footer>

<script>
let cart = [];

function addToCart(name) {
  cart.push(name);

  document.getElementById("message").innerHTML =
    "♡ " + name + " has been added to your favorites! Total: " + cart.length;
}
</script>

</body>
</html>
