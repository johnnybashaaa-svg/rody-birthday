# rody-birthday 
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>عيد ميلاد رودي ❤️</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:linear-gradient(135deg,#0f172a,#1e293b,#312e81);
height:100vh;
display:flex;
justify-content:center;
align-items:center;
overflow:hidden;
color:white;
text-align:center;
}

.card{
width:90%;
max-width:420px;
background:rgba(255,255,255,.08);
backdrop-filter:blur(12px);
padding:30px;
border-radius:25px;
box-shadow:0 0 30px rgba(255,255,255,.15);
animation:fade 1.5s;
}

h1{
font-size:34px;
margin-bottom:20px;
}

p{
line-height:1.8;
font-size:18px;
margin-bottom:25px;
}

button{
padding:15px 35px;
border:none;
border-radius:50px;
background:#ff4d88;
color:white;
font-size:18px;
cursor:pointer;
transition:.3s;
}

button:hover{
transform:scale(1.1);
}

#msg{
display:none;
margin-top:25px;
font-size:20px;
line-height:2;
}

@keyframes fade{
from{opacity:0;transform:translateY(40px);}
to{opacity:1;transform:translateY(0);}
}

.confetti{
position:fixed;
width:10px;
height:10px;
background:red;
top:-10px;
animation:fall linear forwards;
}

@keyframes fall{
to{
transform:translateY(110vh) rotate(720deg);
}
}
</style>
</head>

<body>

<div class="card">

<h1>🎂 كل سنة وانتي بخير يا رودي ❤️</h1>

<p>
في ملايين الناس في الدنيا...
بس مفيش حد شبهك.
</p>

<button onclick="openGift()">
افتحي المفاجأة 🎁
</button>

<div id="msg">

كل سنة وانتي بخير يا بنوتي ❤️

يارب السنة دي تكون كلها ضحكة وفرحة وراحة لقلبك.

وأتمنى كل أمنية تتمنيها تتحقق.

شكرا إنك بقي
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>عيد ميلاد رودي ❤️</title>

<style>
body{
margin:0;
background:#0f172a;
display:flex;
justify-content:center;
align-items:center;
height:100vh;
font-family:Arial,sans-serif;
color:white;
overflow:hidden;
}

.box{
text-align:center;
padding:25px;
max-width:400px;
}

button{
padding:15px 30px;
border:none;
border-radius:40px;
background:#ff4d8d;
color:white;
font-size:18px;
cursor:pointer;
}

#msg{
display:none;
margin-top:20px;
line-height:2;
font-size:20px;
}

.heart{
position:fixed;
font-size:25px;
animation:fall 6s linear infinite;
}

@keyframes fall{
0%{transform:translateY(-100px);}
100%{transform:translateY(110vh);}
}
</style>

</head>

<body>

<div class="box">

<h1>🎂 كل سنة وانتي بخير يا رودي ❤️</h1>

<p>اضغطي على الزر وافتحي المفاجأة</p>

<button onclick="showMsg()">🎁 افتحي المفاجأة</button>

<div id="msg">
كل سنة وانتي بخير يا بنوتي ❤️<br><br>
يارب السنة دي تكون أحلى سنة في حياتك.<br>
وتحققي كل اللي نفسك فيه.<br>
وتفضلي دايما مبتسمة وسعيدة.<br><br>
شكرا إنك موجودة في حياتي.<br><br>
❤️🎉
</div>

</div>

<script>

function showMsg(){
document.getElementById("msg").style.display="block";
}

setInterval(()=>{
let h=document.createElement("div");
h.className="heart";
h.innerHTML="❤️";
h.style.left=Math.random()*100+"vw";
document.body.appendChild(h);
setTimeout(()=>h.remove(),6000);
},300);

</script>

</body>
</html>
<canvas id="fireworks"></canvas>

<style>
#fireworks{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
pointer-events:none;
z-index:999;
}
</style>

<script>
const canvas = document.getElementById("fireworks");
const ctx = canvas.getContext("2d");

canvas.width = innerWidth;
canvas.height = innerHeight;

let particles=[];

function firework(){
let x=Math.random()*canvas.width;
let y=Math.random()*canvas.height/2;

for(let i=0;i<80;i++){
particles.push({
x:x,
y:y,
speed:Math.random()*5+2,
angle:Math.random()*Math.PI*2,
life:100,
color:`hsl(${Math.random()*360},100%,60%)`
});
}
}

function animate(){
ctx.clearRect(0,0,canvas.width,canvas.height);

particles.forEach((p,index)=>{
p.x+=Math.cos(p.angle)*p.speed;
p.y+=Math.sin(p.angle)*p.speed;
p.life--;

ctx.beginPath();
ctx.arc(p.x,p.y,3,0,Math.PI*2);
ctx.fillStyle=p.color;
ctx.fill();

if(p.life<=0) particles.splice(index,1);
});

requestAnimationFrame(animate);
}

setInterval(firework,700);
animate();
</script>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>عيد ميلاد رودي ❤️</title>

<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Cairo',sans-serif;
}

body{
background:linear-gradient(135deg,#14002d,#2a0055,#4a0080);
overflow:hidden;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
position:relative;
color:white;
}

/* النجوم */

.star{
position:absolute;
width:2px;
height:2px;
background:white;
border-radius:50%;
animation:twinkle 2s infinite alternate;
}

@keyframes twinkle{
from{
opacity:.2;
transform:scale(.5);
}
to{
opacity:1;
transform:scale(1.8);
}
}

/* الكارت */

.card{

width:90%;
max-width:430px;

background:rgba(255,255,255,.1);

backdrop-filter:blur(18px);

border:1px solid rgba(255,255,255,.2);

border-radius:30px;

padding:30px;

text-align:center;

box-shadow:0 0 30px rgba(255,105,180,.4);

z-index:10;

}

/* الصورة */

.photo{

width:170px;

height:170px;

border-radius:50%;

object-fit:cover;

border:5px solid hotpink;

box-shadow:0 0 35px hotpink;

margin-bottom:20px;

animation:glow 2s infinite alternate;

}

@keyframes glow{

from{

box-shadow:0 0 20px hotpink;

}

to{

box-shadow:0 0 45px deeppink;

}

}

h1{

font-size:34px;

margin-bottom:15px;

}

p{

font-size:20px;

line-height:1.9;

}

button{

margin-top:25px;

padding:16px 35px;

font-size:22px;

background:#ff1493;

color:white;

border:none;

border-radius:40px;

cursor:pointer;

box-shadow:0 0 25px hotpink;

transition:.3s;

}

button:hover{

transform:scale(1.08);

}

#message{

margin-top:25px;

font-size:22px;

color:#fff;

min-height:150px;

}
<div class="card">

<img src="rody.jpg" class="photo">

<h1>كل سنة وانتي بخير يا رودي ❤️</h1>

<button id="openBtn">
💖 افتحي المفاجأة
</button>

<div id="message"></div>

<audio id="music" src="birthday.mp3"></audio>

</div>

<div id="hearts"></div>
<div id="flowers"></div>
<div id="fireworks"></div>
<script>

const text=`كل سنة وانتي بخير يا بنوتي ❤️
يارب تكون السنة دي كلها فرحة وضحكة ليكي
وتحققي كل اللي نفسك فيه
وربنا يخليكي دايما سعيدة

انتي تستحقي كل حاجة حلوة 🌹`;

const btn=document.getElementById("openBtn");
const msg=document.getElementById("message");
const music=document.getElementById("music");

btn.onclick=()=>{

music.play();

btn.style.display="none";

let i=0;

let timer=setInterval(()=>{

msg.innerHTML+=text.charAt(i);

i++;

if(i>=text.length){
clearInterval(timer);
}

},45);

}

</script>
<div id="stars"></div>
style #stars{
  position:fixed;
  top:0;
  left:0;
  width:100%;
  height:100%;
  overflow:hidden;
  z-index:-1;
}

.star{
  position:absolute;
  width:2px;
  height:2px;
  background:white;
  border-radius:50%;
  animation:twinkle linear infinite;
}

@keyframes twinkle{
  0%{
    opacity:.2;
    transform:scale(1);
  }
  50%{
    opacity:1;
    transform:scale(2);
  }
  100%{
    opacity:.2;
    transform:scale(1);
  }
} </script> const stars = document.getElementById("stars");

for(let i=0;i<200;i++){

  const star=document.createElement("div");

  star.className="star";

  star.style.left=Math.random()*100+"%";
  star.style.top=Math.random()*100+"%";

  star.style.animationDuration=(2+Math.random()*4)+"s";

  stars.appendChild(star);

} <body><div id="hearts"></div> 
#hearts{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
pointer-events:none;
overflow:hidden;
z-index:5;
}

.heart{
position:absolute;
color:#ff4fa3;
font-size:18px;
animation:fall linear forwards;
opacity:.9;
text-shadow:0 0 10px #ff4fa3;
}

@keyframes fall{
0%{
transform:translateY(-10vh) rotate(0deg);
opacity:0;
}
10%{
opacity:1;
}
100%{
transform:translateY(110vh) rotate(360deg);
opacity:0;
}
}const hearts=document.getElementById("hearts");

function createHeart(){

const heart=document.createElement("div");

heart.className="heart";

heart.innerHTML="💖";

heart.style.left=Math.random()*100+"vw";

heart.style.fontSize=(15+Math.random()*25)+"px";

heart.style.animationDuration=(4+Math.random()*4)+"s";

hearts.appendChild(heart);

setTimeout(()=>{
heart.remove();
},8000);

}

setInterval(createHeart,300);
<script>

</script> function goToScene(sceneNum) {
    // تشغيل الأغنية
    playAudio();

    // إخفاء كل المشاهد
    document.querySelectorAll('.scene').forEach(scene => {
        scene.classList.remove('active');
    });

    // إظهار المشهد المطلوب
    document.getElementById('scene' + sceneNum).classList.add('active');
}
