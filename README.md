<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>All Game Platform</title>
<style>
body{margin:0;background:#10152b;color:white;font-family:Arial}
header{text-align:center;padding:25px;background:#202c50}
h1,h2{color:#ffd34e}
.card{background:#202b49;padding:20px;margin:15px;border-radius:15px;text-align:center}
button{background:#ffca36;padding:12px;border:0;border-radius:8px;margin:5px}
input{padding:10px;width:100px}
.result{color:#64f5a2;margin:10px}
</style>
</head>
<body>
<header>
<h1>🎮 All Game Platform</h1>
<p>এক জায়গায় মজার সব ফ্রি গেম</p>
</header>
<main>
<div class="card">
<h2>🎯 Number Guess</h2>
<p>১ থেকে ১০০-এর মধ্যে সংখ্যা অনুমান করো</p>
<input id="guess" type="number">
<button onclick="checkGuess()">খেলুন</button>
<div id="guessResult" class="result"></div>
</div><div class="card">
<h2>✊ Rock Paper Scissors</h2>
<button onclick="rps('পাথর')">✊ পাথর</button>
<button onclick="rps('কাগজ')">✋ কাগজ</button>
<button onclick="rps('কাঁচি')">✌️ কাঁচি</button>
<div id="rpsResult" class="result"></div>
</div>

<div class="card">
<h2>🧠 Memory Game</h2>
<div id="memoryBoard"></div>
<div id="memoryResult" class="result"></div>
<button onclick="newMemory()">নতুন খেলা</button>
</div>

<div class="card">
<h2>🎲 Dice Game</h2>
<div id="dice" style="font-size:50px">🎲</div>
<button onclick="rollDice()">পাশা ফেলো</button>
<div id="diceResult" class="result"></div>
</div>

<div class="card">
<h2>✈️ Aviator</h2>
<div id="plane">✈️</div>
<div id="multiplier" style="font-size:40px">1.00x</div>
<p>পয়েন্ট: <b id="balance">1000</b></p>
<button id="startBtn" onclick="startAviator()">খেলা শুরু</button>
<button id="cashBtn" onclick="cashOut()" disabled>পয়েন্ট সংগ্রহ</button>
<div id="aviatorResult" class="result"></div>
</div>
</main>
<footer style="text-align:center;padding:20px">
All Game Platform © 2026
</footer>
