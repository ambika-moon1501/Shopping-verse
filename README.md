<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>ShopVerse</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#0f172a;
    color:white;
}

/* Navbar */

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 60px;
    background:#111827;
    position:sticky;
    top:0;
    z-index:1000;
}

.logo{
    font-size:32px;
    font-weight:bold;
    color:#ff4da6;
}

nav ul{
    display:flex;
    list-style:none;
    gap:25px;
}

nav ul li a{
    text-decoration:none;
    color:white;
    transition:0.3s;
}

nav ul li a:hover{
    color:#ff4da6;
}

/* Hero */

.hero{
    min-height:90vh;
    display:flex;
    align-items:center;
    justify-content:center;
    flex-direction:column;
    text-align:center;
    padding:20px;
    background:linear-gradient(to right,#4c1d95,#0f172a,#be185d);
}

.hero h1{
    font-size:65px;
    margin-bottom:20px;
}

.hero p{
    font-size:20px;
    max-width:700px;
    line-height:1.6;
    color:#d1d5db;
    margin-bottom:35px;
}

.hero button{
    padding:16px 40px;
    border:none;
    border-radius:40px;
    background:#ff4da6;
    color:white;
    font-size:18px;
    cursor:pointer;
    transition:0.3s;
}

.hero button:hover{
    background:#ff2d95;
    transform:scale(1.05);
}

/* Search Box */

.search-section{
    text-align:center;
    padding:40px 20px;
}

.search-section input{
    width:60%;
    max-width:500px;
    padding:15px;
    border:none;
    border-radius:30px;
    font-size:16px;
    outline:none;
}

/* Shopping Apps */

.shops{
    padding:60px 50px;
}

.shops h2{
    text-align:center;
    font-size:45px;
    margin-bottom:50px;
}

.card-container{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(230px,1fr));
    gap:30px;
}

.card{
    background:#1e293b;
    padding:30px;
    border-radius:25px;
    text-align:center;
    transition:0.3s;
    box-shadow:0 0 15px rgba(0,0,0,0.3);
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:120px;
    height:120px;
    object-fit:contain;
    margin-bottom:20px;
}

.card h3{
    margin-bottom:20px;
    font-size:25px;
}

.card button{
    padding:12px 25px;
    border:none;
    border-radius:30px;
    background:#ff4da6;
    color:white;
    cursor:pointer;
    transition:0.3s;
    font-size:16px;
}

.card button:hover{
    background:#ff2d95;
}

/* Features */

.features{
    padding:80px 30px;
    background:#111827;
}

.features h2{
    text-align:center;
    margin-bottom:50px;
    font-size:45px;
}

.feature-box{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.feature{
    background:#1e293b;
    padding:30px;
    border-radius:20px;
    text-align:center;
}

.feature h3{
    margin-bottom:15px;
    color:#ff4da6;
}

/* Footer */

footer{
    background:#020617;
    text-align:center;
    padding:25px;
    color:gray;
}

/* Mobile */

@media(max-width:768px){

    nav{
        flex-direction:column;
        gap:15px;
    }

    .hero h1{
        font-size:42px;
    }

    .hero p{
        font-size:16px;
    }

    .search-section input{
        width:90%;
    }
}

</style>
</head>

<body>

<!-- Navbar -->

<nav>

<div class="logo">ShopVerse</div>

<ul>
<li><a href="#">Home</a></li>
<li><a href="#shops">Shops</a></li>
<li><a href="#features">Features</a></li>
<li><a href="#">Contact</a></li>
</ul>

</nav>

<!-- Hero Section -->

<section class="hero">

<h1>One Place For <br> All Shopping Apps</h1>

<p>
Explore all popular shopping websites from one premium platform.
Click any shopping app below and start shopping instantly.
</p>

<button onclick="document.getElementById('shops').scrollIntoView()">
Start Shopping
</button>

</section>

<!-- Search -->

<section class="search-section">

<input type="text" id="searchInput" placeholder="Search Shopping App..." onkeyup="searchApps()">

</section>

<!-- Shopping Apps -->

<section class="shops" id="shops">

<h2>Popular Shopping Apps</h2>

<div class="card-container" id="shopContainer">

<!-- Flipkart -->

<div class="card">
<img src="https://cdn-icons-png.flaticon.com/512/5968/5968144.png">
<h3>Flipkart</h3>

<a href="https://www.flipkart.com" target="_blank">
<button>Open Store</button>
</a>
</div>

<!-- Amazon -->

<div class="card">
<img src="https://cdn-icons-png.flaticon.com/512/5968/5968500.png">
<h3>Amazon</h3>

<a href="https://www.amazon.in" target="_blank">
<button>Open Store</button>
</a>
</div>

<!-- Myntra -->

<div class="card">
<img src="https://images.seeklogo.com/logo-png/39/1/myntra-logo-png_seeklogo-397396.png">
<h3>Myntra</h3>

<a href="https://www.myntra.com" target="_blank">
<button>Open Store</button>
</a>
</div>

<!-- Ajio -->

<div class="card">
<img src="https://images.seeklogo.com/logo-png/44/1/ajio-logo-png_seeklogo-441995.png">
<h3>Ajio</h3>

<a href="https://www.ajio.com" target="_blank">
<button>Open Store</button>
</a>
</div>

<!-- Meesho -->

<div class="card">
<img src="https://images.seeklogo.com/logo-png/43/1/meesho-logo-png_seeklogo-439720.png">
<h3>Meesho</h3>

<a href="https://www.meesho.com" target="_blank">
<button>Open Store</button>
</a>
</div>

<!-- Nykaa -->

<div class="card">
<img src="https://upload.wikimedia.org/wikipedia/commons/0/00/Nykaa_New_Logo.svg">
<h3>Nykaa</h3>

<a href="https://www.nykaa.com" target="_blank">
<button>Open Store</button>
</a>
</div>

</div>

</section>

<!-- Features -->

<section class="features" id="features">

<h2>Why Use ShopVerse?</h2>

<div class="feature-box">

<div class="feature">
<h3>All Apps In One Place</h3>
<p>Access multiple shopping websites from one platform.</p>
</div>

<div class="feature">
<h3>Fast Access</h3>
<p>Open shopping apps instantly with one click.</p>
</div>

<div class="feature">
<h3>Premium Design</h3>
<p>Modern responsive UI with beautiful animations.</p>
</div>

<div class="feature">
<h3>Mobile Friendly</h3>
<p>Works perfectly on desktop and mobile devices.</p>
</div>

</div>

</section>

<!-- Footer -->

<footer>

© 2026 ShopVerse | All Rights Reserved

</footer>

<!-- JavaScript -->

<script>

function searchApps() {

let input = document.getElementById("searchInput").value.toLowerCase();

let cards = document.getElementsByClassName("card");

for(let i=0; i<cards.length; i++){

    let title = cards[i].getElementsByTagName("h3")[0];

    let textValue = title.textContent || title.innerText;

    if(textValue.toLowerCase().indexOf(input) > -1){

        cards[i].style.display = "";

    } else {

        cards[i].style.display = "none";
    }
}

}

</script>

</body>
</html>
