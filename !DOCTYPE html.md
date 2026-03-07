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
Begummmm ma tmra wait kru ga tme jtna jtna bolo g utna wait kru gaaaaa  
Ku k ma ne nikah srf tm se h krna ha srf tm se hi  
Or nikah k bad tm jase life chahte hm dono wase h guzre ge   
Blkay us se b acheee  
Tm ne jasa socha hua wase h hm kre g  
I promise k tm ne jasa socha hua jo kch tm ne mjje bataya hua hm wase life guzre g  
Ma tmraaaa khyal rku gaaa tme khushh rku ga tme dheeer sara pyarrr kruu gaaaa izzat du gaaaaaaaa   
Tm jasa kaho g ma wasa zain banu ga  
Or  
Ma srf tmra hu🫠❤️  
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
