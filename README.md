<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>🎂 عيد ميلاد رودي ❤️</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{

background:linear-gradient(135deg,#ff5fa2,#6a11cb);
height:100vh;
overflow:hidden;
font-family:Cairo,sans-serif;
display:flex;
justify-content:center;
align-items:center;
color:#fff;

}

.scene{

display:none;
text-align:center;
animation:fade .8s;

}

.scene.active{

display:block;

}

@keyframes fade{

from{
opacity:0;
transform:scale(.8);
}

to{
opacity:1;
transform:scale(1);
}

}

button{

padding:15px 35px;
font-size:22px;
border:none;
border-radius:50px;
cursor:pointer;
background:#fff;
color:#ff1493;
font-weight:bold;
margin-top:25px;
transition:.3s;

}

button:hover{

transform:scale(1.1);

}

img{

width:250px;
height:250px;
object-fit:cover;
border-radius:20px;
box-shadow:0 0 30px white;

}

h1{

margin-bottom:20px;

}

p{

font-size:22px;
margin-top:20px;

}

.heart{

position:fixed;
color:#ff4d6d;
font-size:25px;
animation:up 5s linear infinite;

}

@keyframes up{

0%{
transform:translateY(100vh);
opacity:1;
}

100%{
transform:translateY(-100px);
opacity:0;
}

}

</style>
</head>

<body><div id="scene1" class="scene active">

<h1>🎉 عيد ميلاد سعيد يا رودي ❤️</h1>

<p>عندي ليكي مفاجأة صغيرة 🎁</p>

<button onclick="goToScene(2)">
ابدئي الرحلة ❤️
</button>

</div>


<div id="scene2" class="scene">

<h1>أجمل صورة ❤️</h1>

<img src="rody.jpg" alt="رودي">

<br><br>

<button onclick="playMusic();goToScene(3)">
التالي ➜
</button>

</div>


<div id="scene3" class="scene">

<h1>🎂 Happy Birthday 🎂</h1>

<p>

كل سنة وانتي بخير ❤️<br><br>

يارب تكون سنة كلها فرحة وضحك وتحقيق لكل أحلامك 🌹

</p>

<br>

<button onclick="goToScene(4)">
افتحي الهدية 🎁
</button>

</div>


<div id="scene4" class="scene">

<h1>💖</h1>

<p>

وجودك في حياتي أحلى هدية ❤️

</p>

</div><script>

let audio = new Audio("birthday.mp3");

function playMusic(){

audio.play().catch(()=>{});

}

function goToScene(scene){

document.querySelectorAll(".scene").forEach(function(item){

item.classList.remove("active");

});

document.getElementById("scene"+scene).classList.add("active");

}

setInterval(function(){

let heart=document.createElement("div");

heart.className="heart";

heart.innerHTML="❤️";

heart.style.left=Math.random()*100+"vw";

heart.style.fontSize=(20+Math.random()*30)+"px";

document.body.appendChild(heart);

setTimeout(function(){

heart.remove();

},5000);

},300);

</script><img src="b5970d39fea4c14c0280f0dae3fd8f33.jpg" alt="رودي"> 

</body> 
</html>
