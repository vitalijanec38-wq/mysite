<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Anasta Production</title>

<style>

body{
margin:0;
font-family:Arial, sans-serif;
background:#111;
color:white;
overflow-x:hidden;
text-align:center;
}

/* HERO */

.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
cursor:pointer;
}

.hero h1{
font-size:48px;
letter-spacing:3px;
margin:0;
}

.hero p{
opacity:0.6;
margin-top:10px;
}

/* ANIMATION PHOTOS */

.animation{
position:relative;
height:100vh;
overflow:hidden;
display:none;
}

.slide{
position:absolute;
left:50%;
transform:translateX(-50%);
width:320px;
border-radius:14px;
box-shadow:0 30px 80px rgba(0,0,0,0.6);
transition:1.5s ease;
}

.top{
top:-400px;
}

.bottom{
bottom:-400px;
}

.animation.active .top{
top:50%;
transform:translate(-50%,-110%);
}

.animation.active .bottom{
bottom:50%;
transform:translate(-50%,110%);
}

/* PORTFOLIO */

.portfolio{
display:none;
padding:80px 20px;
max-width:700px;
margin:auto;
animation:fade 1.5s forwards;
}

@keyframes fade{
from{opacity:0;}
to{opacity:1;}
}

.portfolio img{
width:260px;
border-radius:14px;
margin:15px;
box-shadow:0 20px 60px rgba(0,0,0,0.7);
}

.insta a{
display:inline-block;
margin-top:25px;
padding:14px 30px;
background:linear-gradient(45deg,#fd1d1d,#e1306c,#f77737);
border-radius:30px;
color:white;
text-decoration:none;
font-weight:bold;
}

</style>
</head>

<body>

<!-- START SCREEN -->

<div class="hero" onclick="startShow()">
<h1>ANASTA PRODUCTION</h1>
<p>🌸 Нажми меня</p>
</div>

<!-- ANIMATION -->

<div class="animation" id="animation">
<img src="photo.jpg" class="slide top">
<img src="photo2.jpg" class="slide bottom">
</div>

<!-- PORTFOLIO -->

<div class="portfolio" id="portfolio">

<h2>Anasta — Model Portfolio</h2>

<p>
Professional model with experience in fashion, lifestyle and brand promotion.<br><br>

• Modeling experience — 3+ years<br>
• Brand collaborations<br>
• Photo & video production<br>
• Commercial and creative shoots<br>
• Social media promotion<br><br>

Open for collaborations worldwide.
</p>

<img src="photo.jpg">
<img src="photo2.jpg">
<img src="photo3.jpg">

<div class="insta">
<h3>@anasta.production</h3>

<a href="https://www.instagram.com/anasta.production/" target="_blank">
Open Instagram →
</a>
</div>

</div>

<script>

function startShow(){

document.querySelector(".hero").style.display="none";

let anim=document.getElementById("animation");
anim.style.display="block";

setTimeout(()=>{
anim.classList.add("active");
},100);

setTimeout(()=>{
anim.style.display="none";
document.getElementById("portfolio").style.display="block";
},2200);

}

</script>

</body>
</html>
