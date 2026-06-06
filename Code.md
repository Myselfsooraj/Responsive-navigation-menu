<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VELVORÉ | Men's Apparel</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
scroll-behavior:smooth;
font-family:'Poppins',sans-serif;
}

body{
background:#0f172a;
color:white;
overflow-x:hidden;
}

.progress-bar{
position:fixed;
top:0;
left:0;
height:4px;
width:0%;
background:linear-gradient(90deg,#c9a66b,#f5d28f);
z-index:9999;
}

/* NAVBAR */

.navbar{
position:fixed;
top:20px;
left:50%;
transform:translateX(-50%);
width:90%;
max-width:1200px;

padding:15px 40px;

display:flex;
justify-content:space-between;
align-items:center;

background:rgba(255,255,255,0.08);
backdrop-filter:blur(15px);

border:1px solid rgba(255,255,255,.1);
border-radius:20px;

z-index:1000;
transition:.4s;
}

.navbar.scrolled{
background:rgba(15,23,42,.95);
box-shadow:0 10px 30px rgba(0,0,0,.4);
}

.logo{
font-size:1.8rem;
font-weight:700;
letter-spacing:2px;
color:#f5d28f;
}

.nav-menu{
display:flex;
list-style:none;
gap:30px;
}

.nav-menu a{
color:white;
text-decoration:none;
font-weight:500;
position:relative;
}

.nav-menu a::after{
content:'';
position:absolute;
left:0;
bottom:-5px;
width:0;
height:2px;
background:#f5d28f;
transition:.3s;
}

.nav-menu a:hover::after{
width:100%;
}

/* HERO */

.hero{
height:100vh;

background:
linear-gradient(
rgba(0,0,0,.45),
rgba(0,0,0,.65)
),
url('https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?auto=format&fit=crop&w=1500&q=80');

background-size:cover;
background-position:center;

display:flex;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
}

.hero-content{
max-width:800px;
}

.hero h1{
font-size:5rem;
font-weight:700;
margin-bottom:20px;
}

.hero span{
color:#f5d28f;
}

.hero p{
font-size:1.2rem;
opacity:.9;
margin-bottom:30px;
}

.btn{
padding:15px 40px;
border:none;
border-radius:50px;

background:linear-gradient(135deg,#c9a66b,#f5d28f);

font-size:1rem;
font-weight:600;

cursor:pointer;
transition:.4s;
}

.btn:hover{
transform:translateY(-5px);
}

/* COLLECTION */

.collection{
padding:100px 10%;
background:#111827;
}

.section-title{
text-align:center;
font-size:3rem;
margin-bottom:50px;
color:#f5d28f;
}

.collection-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
gap:30px;
}

.card{
background:#1f2937;
border-radius:20px;
overflow:hidden;
transition:.4s;
}

.card:hover{
transform:translateY(-10px);
box-shadow:0 15px 30px rgba(0,0,0,.4);
}

.card img{
width:100%;
height:400px;
object-fit:cover;
}

.card-content{
padding:20px;
}

.card h3{
margin-bottom:10px;
}

.card p{
opacity:.7;
}

/* ABOUT */

.about{
padding:100px 10%;
text-align:center;
background:#0f172a;
}

.about p{
max-width:800px;
margin:auto;
line-height:1.8;
opacity:.8;
}

/* CONTACT */

.contact{
padding:100px 10%;
text-align:center;
background:#111827;
}

.contact h2{
margin-bottom:20px;
color:#f5d28f;
}

/* REVEAL */

.reveal{
opacity:0;
transform:translateY(60px);
transition:1s;
}

.reveal.active{
opacity:1;
transform:translateY(0);
}

/* MOBILE */

@media(max-width:768px){

.hero h1{
font-size:3rem;
}

.nav-menu{
gap:15px;
font-size:.9rem;
}

.section-title{
font-size:2rem;
}

}

</style>
</head>

<body>

<div class="progress-bar"></div>

<nav class="navbar">

<div class="logo">VELVORÉ</div>

<ul class="nav-menu">
<li><a href="#home">Home</a></li>
<li><a href="#collection">Collection</a></li>
<li><a href="#about">About</a></li>
<li><a href="#contact">Contact</a></li>
</ul>

</nav>

<section class="hero" id="home">

<div class="hero-content reveal">

<h1>Elevate Your <span>Style</span></h1>

<p>
Luxury menswear crafted for confidence, comfort, and timeless elegance.
</p>

<button class="btn">Shop Collection</button>

</div>

</section>

<section class="collection" id="collection">

<h2 class="section-title reveal">Featured Collection</h2>

<div class="collection-grid">

<div class="card reveal">
<img src="https://images.unsplash.com/photo-1514996937319-344454492b37?auto=format&fit=crop&w=800&q=80">
<div class="card-content">
<h3>Casual Essentials</h3>
<p>Premium everyday wear designed for comfort and style.</p>
</div>
</div>

<div class="card reveal">
<img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?auto=format&fit=crop&w=800&q=80">
<div class="card-content">
<h3>Street Collection</h3>
<p>Bold fashion inspired by modern urban culture.</p>
</div>
</div>

<div class="card reveal">
<img src="https://images.unsplash.com/photo-1521572267360-ee0c2909d518?auto=format&fit=crop&w=800&q=80">
<div class="card-content">
<h3>Luxury Line</h3>
<p>Refined pieces for those who appreciate timeless elegance.</p>
</div>
</div>

</div>

</section>

<section class="about reveal" id="about">

<h2 class="section-title">About Us</h2>

<p>
VELVORÉ is a premium men's apparel brand focused on combining luxury aesthetics with modern comfort. Every piece is crafted to help you express confidence and individuality.
</p>

</section>

<section class="contact reveal" id="contact">

<h2>Get In Touch</h2>

<p>Email: contact@velvore.com</p>
<p>Instagram: @velvoreofficial</p>

</section>

<script>

/* NAVBAR */

const navbar=document.querySelector('.navbar');

window.addEventListener('scroll',()=>{

if(window.scrollY>50){
navbar.classList.add('scrolled');
}else{
navbar.classList.remove('scrolled');
}

});

/* PROGRESS BAR */

window.addEventListener('scroll',()=>{

const winScroll=document.documentElement.scrollTop;

const height=document.documentElement.scrollHeight-document.documentElement.clientHeight;

const scrolled=(winScroll/height)*100;

document.querySelector('.progress-bar').style.width=scrolled+'%';

});

/* REVEAL ANIMATION */

function reveal(){

document.querySelectorAll('.reveal').forEach(el=>{

const windowHeight=window.innerHeight;

const revealTop=el.getBoundingClientRect().top;

if(revealTop<windowHeight-100){

el.classList.add('active');

}

});

}

window.addEventListener('scroll',reveal);

reveal();

</script>

</body>
</html>
