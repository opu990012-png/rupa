<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday My Love ❤️</title>

<style>
body{
margin:0;
font-family:'Segoe UI',sans-serif;
background:#ffe6eb;
color:#ff4d6d;
overflow:hidden;
}

/* COMMON PAGE */
.page{
display:none;
height:100vh;
justify-content:center;
align-items:center;
flex-wrap:wrap;
position:relative;
}
.active{ display:flex; }

/* LEFT SIDE */
.left{
flex:1;
text-align:center;
padding:20px;
}
.left h1{
font-size:42px;
color:#ff4d6d;
text-shadow:2px 2px 10px white;
}
.subtitle{
font-size:18px;
color:#444;
margin-bottom:20px;
}

/* BUTTON */
button{
padding:10px 20px;
border:none;
border-radius:25px;
background:#ff4d6d;
color:white;
cursor:pointer;
box-shadow:0 4px 10px rgba(0,0,0,0.2);
margin:10px;
}

/* RIGHT SIDE IMAGE */
.right{
flex:1;
text-align:center;
position:relative;
}
.circle-img{
width:260px;
height:260px;
border-radius:50%;
object-fit:cover;
border:8px solid #ff4d6d;
box-shadow:0 0 25px #ff4d6d;
}

/* FLOAT ANIMATION */
.float{
position:absolute;
font-size:30px;
animation:float 3s infinite ease-in-out;
}
@keyframes float{
0%{transform:translateY(0);}
50%{transform:translateY(-20px);}
100%{transform:translateY(0);}
}

/* MODAL */
.modal{
position:fixed;
top:0;left:0;
width:100%;height:100%;
background:rgba(0,0,0,0.6);
display:none;
justify-content:center;
align-items:center;
}
.modal-content{
background:white;
padding:25px;
width:90%;
max-width:500px;
border-radius:15px;
max-height:80vh;
overflow:auto;
animation:fade 1s;
}
@keyframes fade{from{opacity:0;}to{opacity:1;}}

#wishText{
white-space:pre-line;
color:#333;
}

/* LOVE LETTER ANIMATION */
#loveLetters span{
font-size:38px;
font-weight:bold;
margin:4px;
opacity:0;
transition:1s;
}

/* Romantic Frame */
.frame{
border:8px solid #ff4d6d;
padding:10px;
border-radius:25px;
box-shadow:0 0 20px #ff4d6d;
}
.memory-img{
width:130px;
margin:5px;
border-radius:15px;
}

/* Final Gift */
#finalPhoto{
display:none;
width:220px;
border-radius:20px;
margin-top:20px;
}
</style>
</head>
<body>

<!-- PAGE 1 -->
<div class="page active" id="page1">

<div class="left">
<h1>🎉 Happy Birthday My Love</h1>
<div class="subtitle">You are the most special person in my life 💕</div>
<button onclick="openModal()">Click for Surprise 💌</button>
</div>

<div class="right">
<img src="gf.jpg" class="circle-img">
<div class="float" style="top:10%;left:10%;">🎈</div>
<div class="float" style="top:20%;right:10%;">❤️</div>
<div class="float" style="bottom:15%;left:20%;">🎈</div>
</div>

</div>

<!-- WISH MODAL -->
<div class="modal" id="modal">
<div class="modal-content">
<h3 style="color:#ff4d6d;text-shadow:1px 1px 5px #ddd;">To My Love ❤️</h3>
<div id="wishText"></div>
<br>
<button onclick="goPage2()">Next</button>
</div>
</div>

<!-- PAGE 2 -->
<div class="page" id="page2" style="flex-direction:column;">
<h2>DO YOU LOVE ME ❤️</h2>
<button onclick="goLovePage()">Yes</button>
<button id="noBtn" onmouseover="moveNo()">No</button>
</div>

<!-- PAGE 3 LOVE PAGE -->
<div class="page" id="pageLove" style="flex-direction:column;">
<div id="loveLetters"></div>

<div class="float" style="top:10%;left:10%;">🎈</div>
<div class="float" style="top:20%;right:10%;">❤️</div>
<div class="float" style="bottom:15%;left:25%;">😘</div>

<button onclick="goMystery()">Next</button>
</div>

<!-- PAGE 4 MYSTERY -->
<div class="page" id="pageMystery" style="flex-direction:column;">
<h2>Select Your Surprise 💖</h2>
<button onclick="goGallery()">Gift 🎁</button>
</div>

<!-- PAGE 5 GALLERY -->
<div class="page" id="pageGallery" style="flex-direction:column;">
<h2>Our Beautiful Memories ❤️</h2>

<div class="frame">
<img src="memory1.jpg" class="memory-img">
<img src="memory2.jpg" class="memory-img"><br>
<img src="memory3.jpg" class="memory-img">
<img src="memory4.jpg" class="memory-img">
</div>

<div class="float" style="top:15%;left:10%;">❤️</div>
<div class="float" style="bottom:15%;right:10%;">😘</div>

<button onclick="showFinalGift()">Open Gift 🎁</button>
<img src="photo.jpg" id="finalPhoto">
</div>![photo jpg](https://github.com/user-attachments/assets/54c92446-a20f-40fa-a34e-1309e818c614)
![memory4 jpg](https://github.com/user-attachments/assets/70eddb96-f3bb-4167-a725-989d45910520)
![myphoto jpg](https://github.com/user-attachments/assets/0fed91d2-45b1-4b5b-974a-1943a9dcd315)
![memory3 jpg](https://github.com/user-attachments/assets/7febc049-30e6-4d9f-904f-5591b16f06b2)
![memory2 jpg](https://github.com/user-attachments/assets/d422148e-072a-41f6-a121-001035495d8b)
![gf jpg](https://github.com/user-attachments/assets/e9dacc53-4eec-461a-9bd8-b19094809dd9)


<script>

/* PAGE SWITCH */
function switchPage(id){
document.querySelectorAll(".page").forEach(p=>p.classList.remove("active"));
document.getElementById(id).classList.add("active");
}

/* TYPEWRITER LETTER */
var text= `প্রিয় জান,

শুভ জন্মদিন আমার ভালোবাসা। 🎂💖
আজকের এই বিশেষ দিনে আমি শুধু একটা কথাই বলতে চাই — তুমি আমার জীবনের সবচেয়ে সুন্দর প্রাপ্তি। তিন বছরেরও বেশি সময় ধরে আমরা একসাথে আছি। এই সময়টায় রাগ ছিল, অভিমান ছিল, ভুল বোঝাবুঝি ছিল… কিন্তু সব কিছুর মাঝেও আমাদের ভালোবাসাটা কখনো কমে যায়নি। বরং আরও গভীর হয়েছে।

আমি জানি, এতদিনে তোমাকে ঠিকভাবে বড় কোনো গিফট দিতে পারিনি। তোমার প্রাপ্যটা সবসময় দিতে পারিনি। কিন্তু বিশ্বাস করো, আমার মন থেকে তোমার জন্য ভালোবাসা আর সম্মান কখনো কম ছিল না। আমার সামর্থ্য যতটুকু, তার চেয়েও বেশি ভালোবাসা আমি তোমাকে দিতে চাই।

আমাদের সম্পর্কটা শুধু আজকের না — এটা আমাদের ভবিষ্যতেরও। আমি চাই আমরা একসাথে পূর্ণতা পাই, একসাথে স্বপ্ন দেখি, একসাথে সব রাগ-অভিমান পেরিয়ে জীবনের প্রতিটা মুহূর্ত কাটাই।

তুমি আমার শান্তি, তুমি আমার হাসি, তুমি আমার ভরসা। তোমার হাতটা যেন কোনোদিন না ছুটে যায়।

আল্লাহর কাছে শুধু এই দোয়া করি — তোমার জীবন সুখে, স্বাস্থ্যে আর সফলতায় ভরে উঠুক। আর সেই সুখের প্রতিটা মুহূর্তে যেন আমি তোমার পাশে থাকতে পারি।

শুভ জন্মদিন আমার জান।
অনেক অনেক ভালোবাসা রইলো তোমার জন্য। ❤️

তোমার জামাই 💕`;

var i=0;

function openModal(){
document.getElementById("modal").style.display="flex";
typeWriter();
}
function typeWriter(){
if(i<text.length){
document.getElementById("wishText").innerHTML+=text.charAt(i);
i++;
setTimeout(typeWriter,20);
}
}

function goPage2(){
document.getElementById("modal").style.display="none";
switchPage("page2");
}

/* NO BUTTON MOVE */
function moveNo(){
let btn=document.getElementById("noBtn");
btn.style.position="absolute";
btn.style.top=Math.random()*80+"%";
btn.style.left=Math.random()*80+"%";
}

/* LOVE PAGE */
function goLovePage(){
switchPage("pageLove");
animateLoveText();
}

function animateLoveText(){
let text="I LOVE YOU MY JAN";
let container=document.getElementById("loveLetters");
container.innerHTML="";
for(let i=0;i<text.length;i++){
let span=document.createElement("span");
span.innerText=text[i];
container.appendChild(span);
setTimeout(()=>{span.style.opacity=1;},i*150);
}
}

function goMystery(){ switchPage("pageMystery"); }
function goGallery(){ switchPage("pageGallery"); }

function showFinalGift(){
document.getElementById("finalPhoto").style.display="block";
}

</script>

</body>
</html>
