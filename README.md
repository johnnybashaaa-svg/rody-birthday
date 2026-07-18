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
