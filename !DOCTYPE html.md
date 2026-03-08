<!DOCTYPE html>  
<html>  
<head>  
<meta charset="UTF-8">  
<title>Secret Message</title>  
  
<style>  
body{  
font-family: Arial;  
background:#ffe6f0;  
text-align:center;  
padding-top:80px;  
}  
  
.box{  
background:white;  
padding:30px;  
border-radius:15px;  
width:350px;  
margin:auto;  
box-shadow:0 0 15px rgba(0,0,0,0.2);  
}  
  
button{  
padding:10px 20px;  
border:none;  
border-radius:10px;  
background:#ff4d88;  
color:white;  
font-size:16px;  
cursor:pointer;  
}  
  
input{  
padding:10px;  
border-radius:10px;  
border:1px solid #ccc;  
}  
  
.hidden{  
display:none;  
}  
  
.envelope{  
font-size:80px;  
cursor:pointer;  
}  
</style>  
  
</head>  
<body>  
  
<div class="box">  
  
<div id="step1">  
<div class="envelope">✉️</div>  
<h3>Click the envelope</h3>  
<button onclick="next(2)">Open</button>  
</div>  
  
<div id="step2" class="hidden">  
<h2>Surprise 👀</h2>  
<p>Someone has a secret message for you...</p>  
<button onclick="next(3)">Next</button>  
</div>  
  
<div id="step3" class="hidden">  
<h2>Another surprise 💌</h2>  
<p>The real message is protected...</p>  
<button onclick="next(4)">Unlock</button>  
</div>  
  
<div id="step4" class="hidden">  
<h3>Enter Password</h3>  
<input type="password" id="pass">  
<br><br>  
<button onclick="check()">Open Message</button>  
</div>  
  
<div id="final" class="hidden">  
<h3>💖</h3>  
  
<p>  
Mere ladlyyyyy future begummmm<br><br>  
  
Ma jane se pehle ye kahna chahta k    
I promise that k nikah k bad tm ne jasa Socha hua hm wase h life guzre g    
Blkay us se b kahin gunah zayda axhe    
Ma gurente deta k hmre life same wase h ho g jasa tm chahti jasa hm dono ne mil kr socha hua ❤️    
  
<br><br>  
  
Jasa tm ne muje call pr bataya thaaaaaaa bilkul wasaaa hiiiii    
Jasa tm chahti ek ghr ho us ma srf ma or tm    
  
<br><br>  
  
Hm mil kr cooking krein    
Ma talwat kru or mere shoulder pr tmra sr    
Bilkul asa he ho ga begum    
I promise 🤍    
  
<br><br>  
  
Ma talwat pr ke sunao ga tm mere shoulder pr sr rkna 🤍    
Dherrr sare batein krein ge hr topic k relatedd    
  
<br><br>  
  
Kabheeee ma bolo gaaa tm sunaaa    
Kabhe tm bolna ma suno gaaaa    
  
<br><br>  
  
Sameeeee dressing krein g jaha b jain ge    
Tme khd apne hatho se kana kilaua kro ga    
Tme khd apne hato se mehndi lagaya kro gaa    
  
<br><br>  
  
Apne hatho se tmre hatho ma churian pehnaya kru ga ❤️    
Khd tme rings pehnaya kro ga apne se 🤍    
  
<br><br>  
  
Tmre balo pr brush b ma h kia kru ga 🫠❤️    
  
<br><br>  
  
Hr chzzz hm mil kr krein h    
Bs ma itna kahna chahta jasa tm chahti hm waseeee h life gusre g mere ladlyyyy begummmmm 🤍    
  
<br><br>  
  
Tmra hathh kabhii ni chorne wala    
Ekele ma bi nahi or na h sb k smne 🤍    
  
<br><br>  
  
Begummmm ma tm se behadd pyar krta    
Khd se b zaydaaaaaaaaaaaaaaa    
  
<br><br>  
  
Maaaa srfff tmraaaaa huuuuuuu    
SRF TMAAAHARAAAA    
  
<br><br>  
  
I will really missss uhh alotttt Begummmmmm 🫠❤️    
  
<br><br>  
  
And I will alwaysssss love uhhhh the way uh want 🫠🤍    
Loveeeee uh alottt begummm 🤍  
</p>  
  
</div>  
  
</div>  
  
<script>  
  
function next(step){  
document.querySelectorAll(".box > div").forEach(d=>d.classList.add("hidden"))  
document.getElementById("step"+step).classList.remove("hidden")  
}  
  
function check(){  
let p=document.getElementById("pass").value  
if(p==="zanoor"){  
document.querySelectorAll(".box > div").forEach(d=>d.classList.add("hidden"))  
document.getElementById("final").classList.remove("hidden")  
}  
else{  
alert("Wrong password")  
}  
}  
  
</script>  
  
</body>  
</html>  
