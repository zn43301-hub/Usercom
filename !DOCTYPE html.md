<!DOCTYPE html>  
<html>  
<head>  
<meta charset="UTF-8">  
<title>For My Begumm ❤️</title>  
  
<style>  
  
body{  
margin:0;  
font-family: 'Segoe UI', sans-serif;  
background:linear-gradient(135deg,#ff758c,#ff7eb3,#ffc3a0);  
height:100vh;  
display:flex;  
justify-content:center;  
align-items:center;  
overflow:hidden;  
}  
  
/* envelope */  
  
.envelope{  
width:220px;  
height:140px;  
background:#fff;  
position:relative;  
cursor:pointer;  
border-radius:8px;  
box-shadow:0 20px 40px rgba(0,0,0,.3);  
transition:.4s;  
}  
  
.envelope:hover{  
transform:scale(1.08);  
}  
  
.flap{  
position:absolute;  
top:-70px;  
border-left:110px solid transparent;  
border-right:110px solid transparent;  
border-bottom:70px solid #fff;  
}  
  
/* letter */  
  
#letter{  
display:none;  
position:absolute;  
background:white;  
width:85%;  
max-width:700px;  
height:70vh;  
overflow:auto;  
padding:35px;  
border-radius:20px;  
box-shadow:0 25px 60px rgba(0,0,0,.4);  
color:#333;  
}  
  
/* hearts */  
  
.heart{  
position:absolute;  
font-size:22px;  
animation:fall linear infinite;  
}  
  
@keyframes fall{  
  
0%{  
transform:translateY(-100px);  
opacity:1;  
}  
  
100%{  
transform:translateY(100vh);  
opacity:0;  
}  
  
}  
  
</style>  
</head>  
  
<body>  
  
<div class="envelope" onclick="openLetter()">  
<div class="flap"></div>  
</div>  
  
<div id="letter">  
<h2>For My Begumm ❤️</h2>  
<p id="text"></p>  
</div>  
  
<audio id="music" loop>  
<source src="https://cdn.pixabay.com/audio/2022/03/15/audio_c8c8a73467.mp3">  
</audio>  
  
<script>  
  
const message = `Mere ladlyyyyy future begummmm  
  
Ma jane se pehle ye kahna chahta k    
  
I promise that k nikah k bad tm ne jasa Socha hua hm wase h life guzre g    
Blkay us se b kahin gunah zayda axhe    
  
Ma gurente deta k hmre life same wase h ho g jasa tm chahti jasa hm dono ne mil kr socha hua ❤️    
  
Jasa tm ne muje call pr bataya thaaaaaaa bilkul wasaaa hiiiii    
  
Jasa tm chahti ek ghr ho us ma srf ma or tm    
Hm mil kr cooking krein    
  
Ma talwat kru or mere shoulder pr tmra sr    
  
Bilkul asa he ho ga begum    
I promise 🤍    
  
Ma talwat pr ke sunao ga tm mere shoulder pr sr rkna 🤍    
  
Dherrr sare batein krein ge hr topic k relatedd    
  
Kabheeee ma bolo gaaa tm sunaaa    
Kabhe tm bolna ma suno gaaaa    
  
Sameeeee dressing krein g jaha b jain ge    
  
Tme khd apne hatho se kana kilaua kro ga    
Tme khd apne hato se mehndi lagaya kro gaa    
  
Apne hatho se tmre hatho ma churian pehnaya kru ga ❤️    
  
Khd tme rings pehnaya kro ga apne se 🤍    
  
Tmre balo pr brush b ma h kia kru ga 🫠❤️    
  
Hr chzzz hm mil kr krein h    
  
Bs ma itna kahna chahta jasa tm chahti hm waseeee h life gusre g mere ladlyyyy begummmmm 🤍    
  
Tmra hathh kabhii ni chorne wala    
  
Begummmm ma tm se behadd pyar krta    
Khd se b zaydaaaaaaaaaaaaaaa    
  
Maaaa srfff tmraaaaa huuuuuuu    
  
SRF TMAAAHARAAAA    
  
I will really missss uhh alotttt Begummmmmm 🫠❤️    
  
And I will alwaysssss love uhhhh the way uh want 🫠🤍    
  
Loveeeee uh alottt begummm 🤍`;  
  
function openLetter(){  
  
let pass1 = prompt("Enter password");  
  
if(pass1 === "zanoor"){  
  
let pass2 = prompt("Enter second password");  
  
if(pass2 === "Mere ladlyyyyy future begummmm"){  
  
document.querySelector(".envelope").style.display="none";  
document.getElementById("letter").style.display="block";  
  
document.getElementById("music").play();  
  
typeText();  
hearts();  
  
}else{  
alert("Wrong second password");  
}  
  
}else{  
alert("Wrong password");  
}  
  
}  
  
function typeText(){  
  
let i=0;  
let speed=40;  
  
function typing(){  
  
if(i < message.length){  
document.getElementById("text").innerHTML += message.charAt(i);  
i++;  
setTimeout(typing,speed);  
}  
  
}  
  
typing();  
  
}  
  
function hearts(){  
  
setInterval(()=>{  
  
let heart=document.createElement("div");  
heart.classList.add("heart");  
heart.innerHTML="❤️";  
  
heart.style.left=Math.random()*100+"vw";  
heart.style.animationDuration=(3+Math.random()*5)+"s";  
  
document.body.appendChild(heart);  
  
setTimeout(()=>{  
heart.remove();  
},8000);  
  
},300);  
  
}  
  
</script>  
  
</body>  
</html>  
