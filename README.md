<!DOCTYPE html> 
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<title>My Special One 🤍</title>  <style>  
body{  
  margin:0;  
  font-family:"Segoe UI",sans-serif;  
  text-align:center;  
  color:white;  
  background:linear-gradient(135deg,#ff5fa2,#ff8fba,#ffd1e3);  
  overflow-x:hidden;  
}  
  
.screen{display:none;}  
.show{display:block;}  
  
button{  
  padding:14px 30px;  
  border:none;  
  border-radius:30px;  
  background:white;  
  color:#ff2f7d;  
  font-size:17px;  
  cursor:pointer;  
  box-shadow:0 6px 15px rgba(0,0,0,0.2);  
}  
  
/* 💗 Big heart animation */  
.big-heart{  
  font-size:130px;  
  margin-top:80px;  
  animation:beat 1.5s infinite;  
}  
@keyframes beat{  
  0%{transform:scale(1);}  
  50%{transform:scale(1.15);}  
  100%{transform:scale(1);}  
}  
  
.envelope{  
  font-size:100px;  
  margin-top:120px;  
  cursor:pointer;  
}  
  
.feelings{  
  font-size:17px;  
  line-height:1.8;  
  padding:20px;  
  max-width:900px;  
  margin:auto;  
  animation:fade 2s ease;  
}  
@keyframes fade{  
  from{opacity:0;transform:translateY(20px);}  
  to{opacity:1;transform:translateY(0);}  
}  
  
/* Floating hearts background */  
.heart{  
  position:fixed;  
  bottom:-10px;  
  animation:float 6s linear infinite;  
  opacity:0.7;  
}  
@keyframes float{  
  from{transform:translateY(0);}  
  to{transform:translateY(-100vh);opacity:0;}  
}  
</style>  </head>  <body>  <!-- Screen 1 : Pink Heart -->  <div id="heart" class="screen show">  
  <div class="big-heart">💗</div>  
  <h3>For someone very special 🤍</h3>  
  <button onclick="openEnvelope()">Open Letter</button>  
</div>  <!-- Screen 2 : Envelope -->  <div id="envelope" class="screen">  
  <div class="envelope" onclick="openMessage()">💌</div>  
</div>  <!-- Screen 3 : Message -->  <div id="message" class="screen">  
  <!-- Photo removed as requested -->  
  <div class="feelings">  
    <p>  
      my special one..🤍<br>  
      Tumhi mazasathi khup jast special ahes, ani te words madhe sangayla thode kami padtat..<br>  
      Tumcha sobat bolayla, hasayla, ani fakt asa connect feel karayla khup changla watat..<br>  
      I just wish tumhi nehmi asa ch khush raha, calm raha, ani tumhi jase ahat tasach raha..💖  
    </p>  <p>  
  You are my favorite person 🤍 ज्यांच्या सोबत silence pan comfortable वाटते ..🌙..<br>  
  You are not just my man, tumhi माझं safe place आहात, माझं home feeling आहात..🏡..<br>  
  tumchya एका smile ने माझा whole day bright होतो..☀️..<br>  
  U make me feel calm, strong, and happy एकाच वेळी and ते खूप rare आहे...<br>  
  मी perfect नाही, situations pan perfect नसतात, but with u everything feels worth it..🤍<br>  
  U are my constant, जग बदललं तरी ज्यांच्यावर मी भरोसा ठेवते.<br>  
  Forever नाही म्हणत, but as long as life allows — I choose u, every single day..✨  
</p>

  </div>  
</div>  <script>  
function openEnvelope(){  
  heart.classList.remove("show");  
  envelope.classList.add("show");  
}  
function openMessage(){  
  envelope.classList.remove("show");  
  message.classList.add("show");  
}  
  
/* floating hearts */  
setInterval(()=>{  
  let h=document.createElement("div");  
  h.className="heart";  
  h.innerHTML="💗";  
  h.style.left=Math.random()*100+"vw";  
  h.style.fontSize=(14+Math.random()*22)+"px";  
  document.body.appendChild(h);  
  setTimeout(()=>h.remove(),6000);  
},450);  
</script>  
</body>  
</html>  
