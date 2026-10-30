# Care-
Dua

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>A Little Love for Dua 💗</title>

<style>
*{box-sizing:border-box;margin:0;padding:0}

body{
 font-family:Georgia,serif;
 background:linear-gradient(145deg,#ffe3ed,#fff5f8,#fbd9e7);
 color:#854b63;
 text-align:center;
 overflow-x:hidden;
}

.container{
 max-width:480px;
 margin:auto;
 padding:25px 17px 45px;
}

.hero{padding:45px 10px 25px}

.heart{
 font-size:65px;
 animation:beat 1.5s infinite;
}

@keyframes beat{
 50%{transform:scale(1.18)}
}

h1{
 color:#ce628b;
 font-size:34px;
 margin:15px 0;
}

h2{
 color:#cc6289;
 margin-bottom:14px;
 font-size:23px;
}

p{
 font-size:15px;
 line-height:1.8;
}

.small{
 font-size:13px;
 color:#ae7890;
 margin-top:10px;
}

.card{
 background:#ffffffc9;
 border:1px solid #ffffff;
 border-radius:25px;
 padding:25px 20px;
 margin:20px 0;
 box-shadow:0 8px 30px #c86d9020;
}

button{
 background:linear-gradient(135deg,#ec8eaf,#d96793);
 color:white;
 border:none;
 border-radius:30px;
 padding:14px 23px;
 font-size:14px;
 margin:9px 5px;
 cursor:pointer;
 box-shadow:0 5px 15px #d9679330;
}

button:active{transform:scale(.96)}

.message{
 display:none;
 background:#fff0f5;
 padding:18px;
 border-radius:18px;
 margin-top:17px;
 line-height:1.8;
 animation:fade .5s;
}

@keyframes fade{
 from{opacity:0;transform:translateY(10px)}
 to{opacity:1;transform:translateY(0)}
}

.item{
 background:#fff4f8;
 border-radius:15px;
 padding:13px;
 margin:10px 0;
 text-align:left;
 font-size:14px;
}

footer{
 padding:30px 10px;
 color:#b27b91;
 font-size:13px;
}

.float{
 position:fixed;
 bottom:-40px;
 pointer-events:none;
 animation:rise 7s linear forwards;
 z-index:-1;
}

@keyframes rise{
 to{transform:translateY(-110vh) rotate(35deg);opacity:0}
}
</style>
</head>

<body>

<div class="container">

<section class="hero">
<div class="heart">💗</div>
<p class="small">A LITTLE CORNER MADE WITH LOVE</p>
<h1>For My Dua 🌷</h1>
<p>
Hey beautiful Dua! This little website is
just for you. A reminder to take care of
yourself and give yourself some extra love.
</p>
<p class="small">You deserve all the happiness in the world ✨</p>
</section>

<div class="card">
<h2>💌 A Sweet Message</h2>
<p>
Dear Dua,<br><br>
I know some days can feel a little difficult.
You don't always have to be happy,
and you don't have to pretend that
everything is okay.<br><br>

Take your time, relax and be kind to yourself.
Your feelings matter, your comfort matters
and YOU matter. ❤️<br><br>

Sending you lots of love and warm wishes.
</p>
</div>

<div class="card">
<h2>🌸 How's Your Mood?</h2>
<p>Tell me how you're feeling today.</p>

<button onclick="mood('happy')">😊 Happy</button>
<button onclick="mood('sad')">🥺 Sad</button>
<button onclick="mood('angry')">😤 Angry</button>
<button onclick="mood('tired')">😴 Tired</button>

<div class="message" id="moodBox"></div>
</div>

<div class="card">
<h2>☕ Your Comfort Corner</h2>
<p>Little things that might make today better.</p>

<div class="item">🧸 Get cozy and take some rest.</div>
<div class="item">☕ Enjoy a warm drink if you like.</div>
<div class="item">🍫 Have your favourite little snack.</div>
<div class="item">🎧 Listen to your favourite music.</div>
<div class="item">🌷 Take a break and relax.</div>
<div class="item">💗 Remember, you don't have to rush.</div>
</div>

<div class="card">
<h2>🫶 A Little Reminder</h2>
<p>
You are allowed to rest.<br>
You are allowed to feel everything.<br>
You are allowed to have a slow day.<br><br>
Be gentle with yourself, Dua.
</p>
</div>

<div class="card">
<h2>🎁 Your Special Surprise</h2>
<p>There's a little message waiting for you...</p>

<button onclick="surprise()">
Open Your Special Gift 💝
</button>

<div class="message" id="gift">
<h2>For You, Dua! 💗</h2>
<p>
If today feels difficult, remember
that you deserve patience, kindness
and comfort.<br><br>

May your worries feel lighter,
your heart feel happier,
and your days be filled with beautiful moments.<br><br>

Take care of yourself, beautiful! 🌸<br><br>
<strong>Sending you endless virtual hugs! 🫂</strong>
</p>
</div>
</div>

<div class="card">
<h2>💗 One Last Thing</h2>
<p>
Drink some water, get comfortable,
take a deep breath and give yourself
the kindness you deserve.
</p>
<button onclick="finalMessage()">
Click For A Smile 🌷
</button>
<div class="message" id="last">
Dua, don't forget how special you are.
A little difficult day doesn't take away
your beautiful tomorrow. 💕
</div>
</div>

<footer>
Made with lots of care for Dua 💗<br>
Stay happy, stay cozy, stay beautiful 🌸
</footer>

</div>

<script>
function mood(type){
 const messages={
 happy:"Keep that beautiful smile, Dua! You deserve every bit of happiness. 🌸",
 sad:"It's okay to have a slow day. Be gentle with yourself. Sending warm wishes. 💗",
 angry:"Take a little break, breathe and give yourself some space. You deserve peace. 🫶",
 tired:"Time to get cozy! Rest a little and don't rush yourself. 🧸"
 };
 let box=document.getElementById("moodBox");
 box.style.display="block";
 box.innerHTML=messages[type];
}

function surprise(){
 document.getElementById("gift").style.display="block";
}

function finalMessage(){
 document.getElementById("last").style.display="block";
}

function hearts(){
 const el=document.createElement("div");
 el.className="float";
 el.innerHTML=["💗","💕","🌸","✨","🦋"][Math.floor(Math.random()*5)];
 el.style.left=Math.random()*100+"vw";
 el.style.fontSize=(18+Math.random()*18)+"px";
 document.body.appendChild(el);
 setTimeout(()=>el.remove(),7000);
}
setInterval(hearts,850);
</script>

</body>
</html>
