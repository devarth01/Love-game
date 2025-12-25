<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Christmas Game for Neetu 🎄</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
  body {
    margin: 0;
    font-family: "Comic Sans MS", cursive;
    background: linear-gradient(135deg, #ffdde1, #ee9ca7);
    text-align: center;
    color: #880e4f;
  }

  .page {
    display: none;
    padding: 40px 20px;
    min-height: 100vh;
  }

  .page.active {
    display: block;
  }

  h1 {
    font-size: 2.5em;
    margin-bottom: 20px;
  }

  p {
    font-size: 1.3em;
    margin-bottom: 25px;
  }

  button {
    padding: 12px 30px;
    font-size: 1.1em;
    border: none;
    border-radius: 25px;
    background: #d81b60;
    color: white;
    cursor: pointer;
    box-shadow: 0 6px 12px rgba(0,0,0,0.25);
  }

  button:hover {
    background: #ad1457;
  }

  .heart {
    font-size: 2em;
    animation: pulse 1s infinite alternate;
  }

  @keyframes pulse {
    from { transform: scale(1); }
    to { transform: scale(1.2); }
  }
</style>
</head>

<body>

<!-- PAGE 1 -->
<div class="page active" id="page1">
  <h1>🎄 Merry Christmas 🎄</h1>
  <p>
    Hey Neetu 💕<br>
    I made a small game for you<br>
    because you are my baby girl 🧸
  </p>
  <button onclick="nextPage(2)">Start the Game 🎮</button>
</div>

<!-- PAGE 2 -->
<div class="page" id="page2">
  <h1>❤️ Level 1 ❤️</h1>
  <p>
    Question for you 😌<br><br>
    Who loves you the most in this world?
  </p>
  <button onclick="nextPage(3)">You 😄</button><br><br>
  <button onclick="nextPage(3)">Me 😎</button>
</div>

<!-- PAGE 3 -->
<div class="page" id="page3">
  <h1>💝 Correct Answer 💝</h1>
  <p>
    Of course… <b>ME + YOU</b> 😭❤️<br>
    Because love is always together.
  </p>
  <button onclick="nextPage(4)">Next Surprise 🎁</button>
</div>

<!-- PAGE 4 -->
<div class="page" id="page4">
  <h1>🎄 Indian Love Level 🇮🇳</h1>
  <p>
    Neetu,<br>
    Tum meri zindagi ki<br>
    sabse pyari kahani ho 💫
  </p>
  <button onclick="nextPage(5)">Final Gift 💖</button>
</div>

<!-- PAGE 5 -->
<div class="page" id="page5">
  <h1>💖 For My Baby Girl Neetu 💖</h1>
  <p>
    “Christmas ho ya normal din,<br>
    meri har khushi ka reason tum ho ❤️<br><br>
    Tumhari hasi meri taqat hai,<br>
    aur tumhara naam…<br>
    <b>Neetu</b> mera sukoon 💝”
  </p>
  <div class="heart">💗💗💗</div>
  <p>
    Forever yours,<br>
    ❤️ Your Baby ❤️
  </p>
</div>

<script>
  function nextPage(n) {
    document.querySelectorAll(".page").forEach(p => p.classList.remove("active"));
    document.getElementById("page" + n).classList.add("active");
  }
</script>

</body>
</html>
