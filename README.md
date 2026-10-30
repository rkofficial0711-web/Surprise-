# Surprise-
HTML
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Sri Venkatesh ❤️</title>
<style>
*{box-sizing:border-box}
body{
 margin:0;
 min-height:100vh;
 display:flex;
 justify-content:center;
 align-items:center;
 background:linear-gradient(135deg,#111827,#581c87,#be185d);
 color:white;
 font-family:Arial,sans-serif;
 text-align:center;
 padding:20px;
}
.card{
 width:100%;
 max-width:420px;
 background:#ffffff18;
 border:1px solid #ffffff40;
 border-radius:25px;
 padding:30px 22px;
 box-shadow:0 10px 40px #0005;
}
h1{color:#ffb6d5}
button,input{
 padding:13px;
 border:0;
 border-radius:12px;
 margin:8px;
 font-size:16px;
}
button{
 background:#ff4f91;
 color:white;
 cursor:pointer;
}
input{width:85%;text-align:center}
.hidden{display:none}
.message{line-height:1.7}
.heart{font-size:55px}
</style>
</head>
<body>
<div class="card">
 <div class="heart">❤️</div>
 <h1>Hey Sri Venkatesh!</h1>
 <p>A secret surprise is waiting for you...</p>

 <div id="login">
  <p>Enter the secret password 🔐</p>
  <input id="password" type="password" placeholder="Enter password">
  <br>
  <button onclick="unlock()">Unlock Surprise ❤️</button>
  <p id="error"></p>
 </div>

 <div id="surprise" class="hidden">
  <h2>MISSION UNLOCKED! 🎉</h2>
  <p class="message">
   Welcome to the most important website of your life 😂
   <br><br>
   <b>Friendship Quiz 🤔</b><br>
   Who is the biggest troublemaker?
  </p>
  <button onclick="quiz('You obviously! 😂')">You</button>
  <button onclick="quiz('Definitely Rathna! 😂')">Rathna</button>
  <p id="answer"></p>

  <hr>
  <h2>😂 Special Roast</h2>
  <p>You are not a normal human...
  You are a limited edition headache! 🤣</p>

  <h2>🤝 Secret Mission</h2>
  <p>Your mission: Never forget this friendship.
  Complete it for a lifetime!</p>

  <button onclick="finalMessage()">Open Final Surprise 🎁</button>
  <div id="final" class="hidden">
   <h1>❤️ Forever Friends ❤️</h1>
   <p class="message">
    Dear Sri Venkatesh,<br><br>
    Life becomes more memorable with friends like you.
    There may be fights, silly jokes and unlimited teasing,
    but true friendship always stays special.<br><br>
    Thanks for being part of my journey.<br><br>
    <b>From Rathna Kumar ❤️</b>
   </p>
   <h2>END OF SURPRISE! 🎉</h2>
  </div>
 </div>
</div>

<script>
function unlock(){
 if(document.getElementById("password").value==="311012"){
  document.getElementById("login").classList.add("hidden");
  document.getElementById("surprise").classList.remove("hidden");
 }else{
  document.getElementById("error").innerText="Wrong password! Try again 😂";
 }
}
function quiz(answer){
 document.getElementById("answer").innerText=answer;
}
function finalMessage(){
 document.getElementById("final").classList.remove("hidden");
}
</script>
</body>
</html>
