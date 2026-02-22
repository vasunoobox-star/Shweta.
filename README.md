<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Shweta 🎉</title>

<style>
body{
  margin:0;
  padding:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background: linear-gradient(45deg,#ff6ec4,#7873f5);
  font-family:sans-serif;
  overflow:hidden;
}

.card{
  background:white;
  padding:25px;
  border-radius:20px;
  text-align:center;
  width:90%;
  max-width:400px;
  box-shadow:0 10px 30px rgba(0,0,0,0.3);
  animation:pop 1.2s ease;
}

h1{
  color:#ff4081;
}

p{
  font-size:15px;
}

button{
  padding:10px 20px;
  border:none;
  border-radius:20px;
  background:#ff4081;
  color:white;
  font-size:15px;
  cursor:pointer;
  margin-top:15px;
}

button:hover{
  background:#e91e63;
}

@keyframes pop{
  from{transform:scale(0);}
  to{transform:scale(1);}
}

/* Cake */
.cake{
  position:relative;
  margin:20px auto;
  width:120px;
  height:80px;
  background:#ffb6c1;
  border-radius:10px;
}

.candle{
  position:absolute;
  width:10px;
  height:30px;
  background:white;
  top:-30px;
}

.candle:nth-child(1){ left:20px; }
.candle:nth-child(2){ left:55px; }
.candle:nth-child(3){ left:90px; }

.flame{
  width:10px;
  height:15px;
  background:orange;
  border-radius:50%;
  position:absolute;
  top:-15px;
  animation:flicker 0.3s infinite alternate;
}

@keyframes flicker{
  from{transform:scale(1);}
  to{transform:scale(1.2);}
}

.hidden-message{
  display:none;
  margin-top:15px;
  font-weight:bold;
  color:#e91e63;
  animation:fadeIn 2s ease forwards;
}

@keyframes fadeIn{
  from{opacity:0;}
  to{opacity:1;}
}
</style>
</head>

<body>

<div class="card">
  <h1>🎉 Happy Birthday Shweta 🎉</h1>

  <p>
  Happy Birthday dear 🌹 <br><br>
  i don't know link open hua ki nahi but ager ho gya hai to happy birthday mare tarf se ❤️ <br><br>
  Jo Dil mein aaye oh karo or khul ke jiyo apni life and love u 💕 <br><br>
  Good Night 👋
  </p>

  <!-- Cake -->
  <div class="cake">
    <div class="candle"><div class="flame"></div></div>
    <div class="candle"><div class="flame"></div></div>
    <div class="candle"><div class="flame"></div></div>
  </div>

  <button onclick="blowCandles()">Blow Candles 🎂</button>

  <div class="hidden-message" id="secret">
    💖 Wish Maang Lo... <br>
    Kyunki meri wish to tum ho Shweta 💕
  </div>

</div>

<script>
function blowCandles(){
  const flames = document.querySelectorAll(".flame");
  flames.forEach(f => f.style.display="none");
  document.getElementById("secret").style.display="block";
}
</script>

</body>
</html>
