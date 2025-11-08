<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>New Year Surprise 🎉</title>
<style>
  body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(135deg, #ffb6c1, #ffe4e1);
    overflow: hidden;
  }

  /* Screens as flex row */
  .screen {
    display: none;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: 20px;
    gap: 30px;
    opacity: 0;
    transform: scale(0.9);
    transition: all 0.6s ease;
    position: relative;
    z-index: 1;
  }
  .active { display: flex; opacity: 1; transform: scale(1); }

  /* Text container */
  .text-container {
    max-width: 600px;
  }
  h1 { font-size: 2rem; margin-bottom: 20px; }
  p { font-size: 1.2rem; margin-bottom: 15px; }

  button {
    padding: 12px 24px;
    margin: 5px;
    font-size: 1rem;
    border-radius: 12px;
    border: none;
    cursor: pointer;
    background: #ff69b4;
    color: white;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  button:hover {
    transform: scale(1.1);
    box-shadow: 0 0 15px rgba(255,105,180,0.6);
  }

  /* Shinchan image beside text */
  .shinchan {
    width: 180px;
    height: auto;
    animation: bounce 1.5s infinite alternate;
  }

  @keyframes bounce {
    0% { transform: translateY(0deg); }
    50% { transform: translateY(-15px); }
    100% { transform: translateY(0deg); }
  }

  /* Confetti */
  .confetti {
    position: absolute;
    width: 8px;
    height: 8px;
    top: -10px;
    background-color: red;
    animation: fall 3s linear infinite;
    z-index: 0;
  }
  @keyframes fall {
    0% { transform: translateY(0) rotate(0deg); opacity:1; }
    100% { transform: translateY(100vh) rotate(360deg); opacity:0; }
  }
</style>
</head>
<body>

<!-- Confetti container -->
<div id="confetti-container"></div>

<!-- Screens -->
<div id="screen1" class="screen active">
  <img src="shinchan.jpeg.jpeg" class="shinchan" alt="Shinchan">
  <div class="text-container">
    <h1>Do you like me? 💖</h1>
    <button onclick="showScreen(true)">Yes</button>
    <button onclick="showScreen(false)">No</button>
  </div>
</div>

<div id="screen2" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan" alt="Shinchan">
  <div class="text-container">
    <h1>Please, my cute bestie! 😘</h1>
    <p>Click Yes! I promise a special message is waiting for u💕! 🎉</p>
    <button onclick="showScreen(true)">Yes, I like you! 💖</button>
  </div>
</div>

<div id="screen3" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan" alt="Shinchan">
  <div class="text-container">
    <h1>❤️ Thank you for staying with me ❤️</h1>
    <p>You changed my life a lot,ur actually!! a god's gift for me💖💖. 💖</p>
    <button onclick="showScreen('bond')">Next</button>
  </div>
</div>

<div id="screen4" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan" alt="Shinchan">
  <div class="text-container">
    <h1>💞 Please don’t leave me 💞</h1>
    <p>I want this bond forever, you’re my world and my best friend always. 🥺💖</p>
    <button onclick="showScreen('sorry')">Next</button>
  </div>
</div>

<div id="screen5" class="screen">
  <img src="shinchan.jpeg.jpeg" class="shinchan" alt="Shinchan">
  <div class="text-container">
    <h1>🙏 Sorry madam 🙏</h1>
    <p>If I ever hurt you at any time, please forgive me. 💖</p>
    <button onclick="showScreen('heartfelt')">Next</button>
  </div>
</div>

<div id="screen6" class="screen">
  <img src="heart png.png" class="shinchan" alt="Shinchan">
  <div class="text-container">
    <h1>🌸 Madam 🌸</h1>
    <p>I don’t know if you like me or not… but I like you.  
    You’re always my first priority, madam.  
    Still now my day won’t get completed without speaking to you.  
    I feel so lucky to have a friend and someone like u , you in my life.  
    You mean so much to me mahh 💖</p>
    <button onclick="showScreen('newyear')">Next</button>
  </div>
</div>

<div id="screen7" class="screen">
  <img src="png-transparent-shin-chan-crayon-shin-chan-cartoon-humour-television-animation-crayon-television-child-food-thumbnail.png" class="shinchan" alt="Shinchan">
  <div class="text-container">
    <h1>🎆 Happy New Year, paithiyam🥰🥰! 🥳</h1>
    <p>Wishing you a year full of happiness, success, love, and unforgettable moments!  
    May this new year bring you closer to your dreams and fill your life with joy 💖</p>
  </div>
</div>

<script>
function showScreen(choice) {
  document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
  switch(choice) {
    case true: document.getElementById('screen3').classList.add('active'); break;
    case false: document.getElementById('screen2').classList.add('active'); break;
    case 'bond': document.getElementById('screen4').classList.add('active'); break;
    case 'sorry': document.getElementById('screen5').classList.add('active'); break;
    case 'heartfelt': document.getElementById('screen6').classList.add('active'); break;
    case 'newyear': document.getElementById('screen7').classList.add('active'); break;
  }
}

// Confetti effect on all screens
function startConfetti() {
  const container = document.getElementById('confetti-container');
  for(let i=0;i<150;i++){
    const confetti = document.createElement('div');
    confetti.classList.add('confetti');
    confetti.style.left = Math.random() * window.innerWidth + 'px';
    confetti.style.backgroundColor = `hsl(${Math.random()*360},100%,50%)`;
    confetti.style.width = confetti.style.height = (5 + Math.random()*10) + 'px';
    confetti.style.animationDuration = (2 + Math.random()*3) + 's';
    container.appendChild(confetti);
  }
}

// Start confetti immediately
startConfetti();
</script>

</body>
</html>

