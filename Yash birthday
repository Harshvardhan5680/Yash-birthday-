<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy Birthday Mitra</title>

<style>
body{
margin:0;
height:100vh;
overflow:hidden;
display:flex;
justify-content:center;
align-items:center;
font-family:Arial, sans-serif;
background:linear-gradient(135deg,#ff9a9e,#fad0c4,#a1c4fd);
}

/* Gift Box */
#gift{
font-size:80px;
cursor:pointer;
display:none;
animation:bounce 1s infinite;
}

@keyframes bounce{
0%,100%{transform:translateY(0);}
50%{transform:translateY(-15px);}
}

/* Wish Card */
.card{
background:white;
padding:30px;
width:340px;
border-radius:20px;
text-align:center;
box-shadow:0 20px 40px rgba(0,0,0,0.3);
display:none;
animation:zoomIn 1s;
}

@keyframes zoomIn{
from{transform:scale(0);}
to{transform:scale(1);}
}

button{
padding:10px 20px;
font-size:16px;
background:#ff4b5c;
color:white;
border:none;
border-radius:12px;
cursor:pointer;
}

/* Firework */
.firework{
position:absolute;
font-size:26px;
animation:explode 1s ease-out forwards;
}

@keyframes explode{
from{transform:scale(0);opacity:1;}
to{transform:scale(2);opacity:0;}
}

/* Emoji Rain */
.emoji{
position:absolute;
animation:fall 5s linear forwards;
}

@keyframes fall{
from{transform:translateY(-10vh);}
to{transform:translateY(110vh);}
}

</style>
</head>

<body>

<div id="gift">🎁</div>

<div class="card" id="card">
<h2>🎂 Happy Birthday Mitra 🎉</h2>
<p id="message">Wishing you happiness 😊</p>
<button onclick="nextWish()">Next Wish</button>
</div>

<script>

const wishes=[
"May your day be full of joy 🎉",
"Stay happy and keep smiling 😊",
"You are special 🌟",
"May all dreams come true ✨",
"Enjoy every moment 🥳",
"Lots of happiness to you 💖",
"Keep shining always 🌈",
"You are amazing 🎂"
];

function nextWish(){
let msg=document.getElementById("message");
let randomWish=wishes[Math.floor(Math.random()*wishes.length)];
msg.innerText=randomWish;
}

/* Crackers animation */
function fireworks(){
let interval=setInterval(()=>{
let f=document.createElement("div");
f.className="firework";
f.innerHTML="🎆";
f.style.left=Math.random()*100+"vw";
f.style.top=Math.random()*100+"vh";
document.body.appendChild(f);
setTimeout(()=>f.remove(),1000);
},200);

setTimeout(()=>{
clearInterval(interval);
document.getElementById("gift").style.display="block";
},5000);
}

/* Gift click */
document.getElementById("gift").onclick=function(){
this.style.display="none";
document.getElementById("card").style.display="block";
}

/* Emoji rain non-stop */
const emojis=["🎈","🎉","💖","✨","🥳","🌟","🎊"];

setInterval(()=>{
let e=document.createElement("div");
e.className="emoji";
e.innerHTML=emojis[Math.floor(Math.random()*emojis.length)];
e.style.left=Math.random()*100+"vw";
e.style.fontSize=(Math.random()*20+20)+"px";
document.body.appendChild(e);
setTimeout(()=>e.remove(),5000);
},300);

window.onload=fireworks;

</script>

</body>
</html>
