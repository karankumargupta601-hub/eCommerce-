
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>ÉLÉGANCE | Timeless Fashion</title>

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    background: #f8f5ef;
    color: #29251f;
    font-family: 'Montserrat', sans-serif;
}

header {
    padding: 25px 8%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #f8f5ef;
}

.logo {
    font-family: 'Cormorant Garamond', serif;
    font-size: 36px;
    letter-spacing: 5px;
    font-weight: 600;
}

nav a {
    text-decoration: none;
    color: #29251f;
    margin: 0 15px;
    font-size: 11px;
    letter-spacing: 2px;
    transition: .3s;
}

nav a:hover {
    color: #a17d50;
}

.cart {
    border: 1px solid #29251f;
    padding: 10px 18px;
    font-size: 11px;
    letter-spacing: 1px;
}

.hero {
    height: 620px;
    background:
    linear-gradient(90deg, rgba(0,0,0,.48), transparent),
    url('https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&w=1800&q=85');
    background-size: cover;
    background-position: center 35%;
    display: flex;
    align-items: center;
    padding: 8%;
    color: white;
}

.hero-content {
    max-width: 520px;
}

.hero small {
    letter-spacing: 5px;
    font-size: 11px;
}

.hero h1 {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(55px, 8vw, 90px);
    line-height: .95;
    font-weight: 400;
    margin: 25px 0;
}

.hero p {
    font-size: 13px;
    line-height: 2;
    letter-spacing: 1px;
    margin-bottom: 30px;
}

.btn {
    display: inline-block;
    background: #f8f5ef;
    color: #29251f;
    padding: 16px 32px;
    text-decoration: none;
    font-size: 11px;
    letter-spacing: 2px;
    transition: .3s;
    border: none;
    cursor: pointer;
}

.btn:hover {
    background: #b99a70;
    color: white;
}

.section {
    padding: 85px 8%;
}

.section-heading {
    text-align: center;
    margin-bottom: 50px;
}

.section-heading small {
    letter-spacing: 4px;
    color: #a17d50;
    font-size: 10px;
}

.section-heading h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 48px;
    font-weight: 500;
    margin-top: 12px;
}

.products {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 25px;
}

.product img {
    width: 100%;
    height: 350px;
    object-fit: cover;
    transition: .5s;
}

.product {
    overflow: hidden;
}

.product:hover img {
    transform: scale(1.04);
}

.product h3 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 23px;
    font-weight: 500;
    margin-top: 15px;
}

.product p {
    font-size: 12px;
    margin-top: 8px;
    color: #917b62;
}

.product button {
    background: transparent;
    border: 1px solid #29251f;
    padding: 10px 15px;
    margin-top: 13px;
    font-size: 10px;
    letter-spacing: 1px;
    cursor: pointer;
    transition: .3s;
}

.product button:hover {
    background: #29251f;
    color: white;
}

.banner {
    min-height: 430px;
    background:
    linear-gradient(rgba(0,0,0,.25),rgba(0,0,0,.25)),
    url('https://images.unsplash.com/photo-1483985988355-763728e1935b?auto=format&fit=crop&w=1600&q=85');
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: white;
    padding: 40px;
}

.banner h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 65px;
    font-weight: 400;
}

.banner p {
    letter-spacing: 3px;
    font-size: 11px;
    margin: 20px 0;
}

.about {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    gap: 65px;
}

.about img {
    width: 100%;
    height: 480px;
    object-fit: cover;
}

.about h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 52px;
    font-weight: 400;
    margin: 20px 0;
}

.about p {
    font-size: 13px;
    line-height: 2.2;
    color: #70695f;
}

.newsletter {
    background: #eae2d6;
    text-align: center;
    padding: 75px 20px;
}

.newsletter h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 45px;
    font-weight: 500;
}

.newsletter p {
    font-size: 12px;
    margin: 15px 0 25px;
}

.newsletter input {
    padding: 16px;
    width: 280px;
    border: none;
    outline: none;
    background: white;
}

.newsletter button {
    padding: 16px 25px;
    border: none;
    background: #29251f;
    color: white;
    cursor: pointer;
}

footer {
    background: #29251f;
    color: #f8f5ef;
    text-align: center;
    padding: 45px 20px;
}

footer h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 35px;
    letter-spacing: 4px;
}

footer p {
    font-size: 10px;
    letter-spacing: 2px;
    margin-top: 15px;
    color: #c6b8a4;
}

@media(max-width: 850px) {
    header {
        flex-wrap: wrap;
        gap: 20px;
    }

    nav {
        order: 3;
        width: 100%;
        text-align: center;
    }

    nav a {
        margin: 0 7px;
        font-size: 9px;
    }

    .products {
        grid-template-columns: repeat(2, 1fr);
    }

    .about {
        grid-template-columns: 1fr;
    }
}

@media(max-width: 480px) {
    .products {
        grid-template-columns: 1fr;
    }

    .product img {
        height: 400px;
    }

    .hero {
        height: 520px;
    }

    .section-heading h2 {
        font-size: 38px;
    }

    .banner h2 {
        font-size: 45px;
    }

    .newsletter input {
        width: 100%;
        margin-bottom: 10px;
    }
}
</style>
</head>

<body>

<header>
    <div class="logo">ÉLÉGANCE.</div>

    <nav>
        <a href="#home">HOME</a>
        <a href="#collection">COLLECTION</a>
        <a href="#about">OUR STORY</a>
        <a href="#contact">CONTACT</a>
    </nav>

    <div class="cart">BAG (<span id="cart-count">0</span>)</div>
</header>

<!-- HERO SECTION -->
<section class="hero" id="home">
    <div class="hero-content">
        <small>THE ART OF DRESSING BEAUTIFULLY</small>

        <h1>Elegance is<br>Timeless.</h1>

        <p>
            Discover a world where sophistication meets
            simplicity. Designed for those who love
            effortless luxury.
        </p>

        <a href="#collection" class="btn">EXPLORE COLLECTION</a>
    </div>
</section>

<!-- COLLECTION -->
<section class="section" id="collection">

    <div class="section-heading">
        <small>CURATED FOR YOU</small>
        

<br>
  </div>
  <p id="store-message"></p>
  <button id="checkout-button" hidden>
    Proceed to Checkout
  </button>
</section>

<script src="shopify.js"></script>

    <div class="products">

        <div class="product">
            <img src="https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&w=700&q=80">
            <h3>The Classic Dress</h3>
            <p>₹2,499</p>
            <button onclick="addToCart()">ADD TO BAG</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1548036328-c9fa89d128fa?auto=format&fit=crop&w=700&q=80">
            <h3>Signature Handbag</h3>
            <p>₹3,299</p>
            <button onclick="addToCart()">ADD TO BAG</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1599643478518-a784e5dc4c8f?auto=format&fit=crop&w=700&q=80">
            <h3>Golden Elegance</h3>
            <p>₹999</p>
            <button onclick="addToCart()">ADD TO BAG</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1543163521-1bf539c55dd2?auto=format&fit=crop&w=700&q=80">
            <h3>Classic Heels</h3>
            <p>₹2,199</p>
            <button onclick="addToCart()">ADD TO BAG</button>
        </div>

    </div>
</section>

<!-- LUXURY BANNER -->
<section class="banner">
    <div>
        <h2>Less, But Luxurious.</h2>
        <p>BEAUTY IN EVERY LITTLE DETAIL</p>
        <a href="#collection" class="btn">SHOP NOW</a>
    </div>
</section>

<!-- ABOUT -->
<section class="section about" id="about">

    <img src="https://images.unsplash.com/photo-1483985988355-763728e1935b?auto=format&fit=crop&w=900&q=80">

    <div>
        <small>OUR PHILOSOPHY</small>

        <h2>Style fades.<br>Elegance remains.</h2>

        <p>
            At ÉLÉGANCE, we believe fashion is more than
            clothing. It is a feeling, a statement and
            an expression of individuality.

            <br><br>

            Our collections celebrate timeless silhouettes,
            refined details and effortless sophistication.
            Every piece is designed to make you feel
            beautiful, confident and unforgettable.
        </p>
    </div>

</section>

<!-- NEWSLETTER -->
<section class="newsletter" id="contact">

    <h2>A Little Note From Us</h2>

    <p>
        Subscribe to discover new collections,
        exclusive offers and a little luxury.
    </p>

    <form onsubmit="subscribe(event)">
        <input type="email" placeholder="Enter your email" required>
        <button type="submit">SUBSCRIBE</button>
    </form>

</section>

<!-- FOOTER -->
<footer>
    <h2>ÉLÉGANCE.</h2>

    <p>TIMELESS STYLE. EFFORTLESS BEAUTY.</p>

    <p>© 2026 ÉLÉGANCE. ALL RIGHTS RESERVED.</p>
</footer>

<script>

let cartCount = 0;

function addToCart() {
    cartCount++;

    document.getElementById("cart-count")
    .innerText = cartCount;

    alert("Beautiful choice! Item added to your bag.");
}

function subscribe(event) {
    event.preventDefault();

    alert("Thank you for shopping from ÉLÉGANCE!come again");

    event.target.reset();
}

</script>

</body>-
</html>

