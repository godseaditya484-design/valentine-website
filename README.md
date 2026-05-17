<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>For Sakshi ❤️</title>
<style>
body{
margin:0;
font-family:Arial;
background:#ffd6e7;
display:flex;
justify-content:center;
align-items:center;
height:100vh;
overflow:hidden;
text-align:center;
}
.box{
background:white;
padding:30px;
border-radius:25px;
width:320px;
box-shadow:0 0 20px rgba(0,0,0,.2);
}
button{
padding:12px 25px;
border:none;
border-radius:20px;
background:pink;
font-size:18px;
}
#page2,#page3{display:none}
.flower{
position:absolute;
font-size:30px;
animation:fall 5s linear infinite;
}
@keyframes fall{
from{transform:translateY(-100px)}
to{transform:translateY(100vh)}
}
img{
width:250px;
border-radius:25px;
}
</style>
</head>

<body>

<div id="page1" class="box">
<h1>💌 A Letter For Sakshi</h1>
<button onclick="openLetter()">Open ❤️</button>
</div>

<div id="page2" class="box">
<h2>Hey Sakshi ❤️</h2>
<p>
Before you press next, I just want you to know
you're my favorite person and favorite feeling.
</p>
<button onclick="nextPage()">Next ❤️</button>
</div>

<div id="page3">
<img src="photo.jpg">
<h2>You deserve flowers everyday 🌸</h2>
</div>

<script>
function openLetter(){
page1.style.display="none"
page2.style.display="block"
}
function nextPage(){
page2.style.display="none"
page3.style.display="block"

for(let i=0;i<25;i++){
let f=document.createElement("div")
f.innerHTML="🌸"
f.className="flower"
f.style.left=Math.random()*100+"%"
document.body.appendChild(f)
}
}
</script>

</body>
</html>
