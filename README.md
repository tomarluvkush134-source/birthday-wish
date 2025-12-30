# birthday-wish
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy Birthday Priyanshi 🎉</title>
<style>
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(120deg,#ff758c,#ff7eb3);
  color: white;
  text-align: center;
  overflow-x: hidden;
}

h1 {
  font-size: 3em;
  margin-top: 40px;
}

.countdown {
  font-size: 2em;
  margin: 20px 0;
  background: rgba(255,255,255,0.2);
  display: inline-block;
  padding: 15px 30px;
  border-radius: 15px;
}

.gallery {
  display: flex;
  justify-content: center;
  gap: 15px;
  flex-wrap: wrap;
  margin: 40px 20px;
}

.gallery img {
  width: 200px;
  height: 200px;
  object-fit: cover;
  border-radius: 20px;
  box-shadow: 0 10px 20px rgba(0,0,0,0.3);
  transition: transform 0.3s;
}

.gallery img:hover {
  transform: scale(1.1);
}

.message {
  font-size: 1.4em;
  margin: 30px;
}

.footer {
  margin-bottom: 40px;
  font-size: 1.2em;
}

/* Confetti */
.confetti {
  position: fixed;
  width: 10px;
  height: 10px;
  background: yellow;
  top: -10px;
  animation: fall 5s linear infinite;
}

@keyframes fall {
  to {
    transform: translateY(110vh) rotate(360deg);
  }
}
</style>
</head>

<body>

<h1>🎉 Happy Birthday Priyanshi 🎂</h1>

<div class="countdown" id="countdown"></div>

<div class="message">
✨ Wishing you endless smiles, love, and happiness on your special day ✨
</div>

<h2>📸 Beautiful Memories</h2>
<div class="gallery">
  <img 
  <img src="images/photo1.jpg">
<img src="images/photo![Snapchat-1554694633](https://github.com/user-attachments/assets/2e1d2862-0394-4f90-b63f-d44088ef04d3)
2.jpg">
<img src="images/photo3.jpg">![Snapchat-523982384](https://github.com/user-attachments/assets/2b6c9b6f-e8aa-4c16-bd29-6fee5f9ed688)


<div class="footer">
💖 Made with love by <b>Luvkush</b> 💖  
<br>🎈 1 January 2026 🎈
</div>

<script>
// Countdown
const birthday = new Date("January 1, 2026 00:00:00").getTime();
setInterval(() => {
  const now = new Date().getTime();
  const diff = birthday - now;

  const d = Math.floor(diff / (1000*60*60*24));
  const h = Math.floor((diff%(1000*60*60*24))/(1000*60*60));
  const m = Math.floor((diff%(1000*60*60))/(1000*60));
  const s = Math.floor((diff%(1000*60))/1000);

  document.getElementById("countdown").innerHTML =
    `⏳ ${d} Days ${h} Hours ${m} Minutes ${s} Seconds`;
},1000);

// Confetti
for(let i=0;i<80;i++){
  let confetti = document.createElement("div");
  confetti.className = "confetti";
  confetti.style.left = Math.random()*100 + "vw";
  confetti.style.background = `hsl(${Math.random()*360},100%,50%)`;
  confetti.style.animationDuration = (Math.random()*3+2)+"s";
  document.body.appendChild(confetti);
}
</script>

</body>
</html>
