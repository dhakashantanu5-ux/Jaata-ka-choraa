# Jaata-ka-choraa
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Nainuu ❤️</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
background:linear-gradient(135deg,#ff5f9e,#ff8b5c);
overflow:hidden;
color:white;
}

.container{
text-align:center;
width:90%;
max-width:700px;
}

h1{
font-size:60px;
font-family:Georgia,serif;
}

h2{
font-size:45px;
margin-top:10px;
}

p{
margin:20px;
font-size:22px;
}

.buttons{
margin-top:30px;
position:relative;
height:100px;
}

button{
padding:18px 40px;
font-size:22px;
border:none;
border-radius:40px;
cursor:pointer;
transition:.3s;
}

#yes{
background:white;
color:#ff3f6c;
font-weight:bold;
}

#no{
background:#ffffff55;
color:white;
position:absolute;
left:60%;
}

#page2{
display:none;
animation:fade 1s;
}

img{
width:260px;
border-radius:20px;
margin-top:20px;
box-shadow:0 0 20px white;
}

@keyframes fade{
from{opacity:0;}
to{opacity:1;}
}

.heart{
position:absolute;
color:white;
font-size:22px;
animation:float 6s linear infinite;
}

@keyframes float{
0%{
transform:translateY(100vh);
opacity:1;
}
100%{
transform:translateY(-120vh);
opacity:0;
}
}
</style>

</head>
<body>

<div class="container" id="page1">

<h3>From: Shntnu ❤️</h3>

<h1>Will you forever be mine?</h1>

<h2>Nainuu 🫶💝</h2>

<p>Babyyyyy, loveeee youuuu coohhh ❤️</p>

<div class="buttons">

<button id="yes">Yes ❤️</button>

<button id="no">No 😈</button>

</div>

</div>

<div class="container" id="page2">

<h1>Yay! I knew you'd say YES! ❤️</h1>

<p>
You're the most amazing person I know.<br>
I love you endlessly.
</p>

<h3>— Shntnu ❤️</h3>

<img src="https://media.tenor.com/mCiM7CmGGI4AAAAC/cute-cat.gif">

<h2 style="margin-top:20px;">🤍 You just made me the happiest!</h2>

</div>

<script>

const no=document.getElementById("no");

no.addEventListener("mouseover",()=>{

let x=Math.random()*(window.innerWidth-120);

let y=Math.random()*(window.innerHeight-60);

no.style.left=x+"px";
no.style.top=y+"px";

});

document.getElementById("yes").onclick=function(){

document.getElementById("page1").style.display="none";

document.getElementById("page2").style.display="block";

}

setInterval(()=>{

let heart=document.createElement("div");

heart.className="heart";

heart.innerHTML="❤️";

heart.style.left=Math.random()*100+"vw";

heart.style.fontSize=(20+Math.random()*30)+"px";

document.body.appendChild(heart);

setTimeout(()=>heart.remove(),6000);

},300);

</script>

</body>
</html>
