<div align="center">
  <img src="https://github.com/khawajaharoon/khawajaharoon/blob/main/assets/banner.gif?raw=true" alt="Cyber Banner" width="100%"/>
  
  <h1>
    <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28">
    Hey! I'm Khawaja Muhammad Haroon
    <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28">
  </h1>

  <p>
    <code>AI Engineer • Full-Stack Wizard • Linux Ninja • Public Dealing Expert</code>
  </p>

  <!-- Typing Effect -->
  <p><span id="typewriter"></span><span class="cursor">|</span></p>

  <!-- Live Visitor Count + Stats -->
  <div style="margin:30px 0;">
    <img src="https://komarev.com/ghpvc/?username=khawajaharoon&label=Profile%20Views&color=ff0048&style=for-the-badge" />
    <img src="https://img.shields.io/github/followers/khawajaharoon?label=Followers&style=for-the-badge&color=7209b7" />
  </div>
</div>

<!-- Animated Terminal -->
<div align="center">
  <div class="terminal" id="terminal">
    <div class="terminal-header">
      <span class="dot red"></span><span class="dot yellow"></span><span class="dot green"></span>
      <span style="margin-left:10px;color:#fff;">root@haroon:~#</span>
    </div>
    <div class="terminal-body" id="terminal-output"></div>
  </div>
</div>

<br>

<!-- Skills with Progress Bars -->
<h2 align="center">⚡ Tech Arsenal</h2>
<div align="center" class="skills-container">
  <div class="skill">Python <div class="bar"><div style="width:98%"></div></div> 98%</div>
  <div class="skill">React / Next.js <div class="bar"><div style="width:95%"></div></div> 95%</div>
  <div class="skill">AI/ML (PyTorch/TF) <div class="bar"><div style="width:93%"></div></div> 93%</div>
  <div class="skill">FastAPI / Django <div class="bar"><div style="width:96%"></div></div> 96%</div>
  <div class="skill">Linux & DevOps <div class="bar"><div style="width:97%"></div></div> 97%</div>
  <div class="skill">Cloud (AWS/GCP) <div class="bar"><div style="width:90%"></div></div> 90%</div>
</div>

<br>

<!-- Connect Buttons -->
<div align="center">
  <a href="https://linkedin.com/in/khawajaharoon"><img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin" /></a>
  <a href="mailto:haroonaziz2030@gmail.com"><img src="https://img.shields.io/badge/Email-Me-red?style=for-the-badge&logo=gmail" /></a>
  <a href="https://github.com/khawajaharoon"><img src="https://img.shields.io/badge/GitHub-Follow-000?style=for-the-badge&logo=github" /></a>
</div>

<!-- Particle Background + All Styling + JS -->
<style>
  @import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@300;400;600&family=Orbitron:wght@700&display=swap');

  body {
    background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
    color: #fff;
    font-family: 'Fira Code', monospace;
    overflow-x: hidden;
  }

  .terminal {
    width: 90%;
    max-width: 800px;
    background: rgba(0,0,0,0.8);
    border-radius: 10px;
    margin: 30px auto;
    box-shadow: 0 0 30px #ff00ff, 0 0 60px #00ffff;
    border: 1px solid #00ffff;
  }

  .terminal-header {
    background: #1e1e1e;
    padding: 10px;
    border-radius: 10px 10px 0 0;
    text-align: left;
  }

  .dot { height: 12px; width: 12px; border-radius: 50%; display: inline-block; margin: 0 5px; }
  .red { background: #ff5f56; }
  .yellow { background: #ffbd2e; }
  .green { background: #27c93f; }

  .terminal-body {
    padding: 20px;
    color: #00ff00;
    min-height: 150px;
    text-align: left;
    font-size: 14px;
  }

  .cursor {
    animation: blink 1s infinite;
    color: #00ffff;
  }

  @keyframes blink {
    0%,50% { opacity: 1; }
    51%,100% { opacity: 0; }
  }

  .skills-container {
    width: 80%;
    margin: 40px auto;
    display: grid;
    gap: 15px;
  }

  .skill {
    background: rgba(255,255,255,0.1);
    padding: 12px 20px;
    border-radius: 10px;
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255,255,255,0.2);
    color: #00ffff;
    font-weight: bold;
  }

  .bar {
    height: 10px;
    background: #333;
    border-radius: 5px;
    margin-top: 8px;
    overflow: hidden;
  }

  .bar > div {
    height: 100%;
    background: linear-gradient(90deg, #ff00ff, #00ffff);
    border-radius: 5px;
    animation: fill 2s ease-out forwards;
  }

  @keyframes fill {
    from { width: 0; }
  }
</style>

<script>
// Typing Effect
const texts = [
  "Building AI that thinks like humans...",
  "Turning coffee into production code...",
  "Deploying dreams on Kubernetes...",
  "Making terminals look sexy since 2023...",
  "Currently training models & breaking systems..."
];
let i = 0;
let j = 0;
let current = "";
const typewriter = document.getElementById("typewriter");

function type() {
  if (i < texts.length) {
    if (j < texts[i].length) {
      current += texts[i].charAt(j);
      typewriter.innerHTML = current;
      j++;
      setTimeout(type, 80);
    } else {
      setTimeout(deleteText, 2000);
    }
  }
}

function deleteText() {
  if (j > 0) {
    current = current.slice(0, -1);
    typewriter.innerHTML = current;
    j--;
    setTimeout(deleteText, 50);
  } else {
    i = (i + 1) % texts.length;
    setTimeout(type, 500);
  }
}
type();

// Terminal Live Text
const terminalLines = [
  "> Initializing neural network... [OK]",
  "> Loading sarcasm module... [OK]",
  "> Compiling badass projects... [OK]",
  "> Connecting to the Matrix... [CONNECTED]",
  "> Scanning for bugs... 0 found (lies)",
  "> Deploying chaos to production... [DONE]",
  "<span style='color:#ff00ff'>root@haroon:~# whoami</span>",
  "<span style='color:#00ffff'>Legend in making...</span>",
  "",
  "<span style='color:#00ff00'>✨ System ready. Let's break something beautiful today.</span>"
];

let lineIndex = 0;
const output = document.getElementById("terminal-output");

function printLine() {
  if (lineIndex < terminalLines.length) {
    const line = document.createElement("div");
    line.innerHTML = terminalLines[lineIndex];
    output.appendChild(line);
    output.scrollTop = output.scrollHeight;
    lineIndex++;
    setTimeout(printLine, 800 + Math.random() * 600);
  }
}

setTimeout(printLine, 1500);

// Particle Background (lightweight)
const canvas = document.createElement("canvas");
canvas.style.position = "fixed";
canvas.style.top = "0";
canvas.style.left = "0";
canvas.style.width = "100%";
canvas.style.height = "100%";
canvas.style.zIndex = "-1";
canvas.style.pointerEvents = "none";
document.body.appendChild(canvas);

const ctx = canvas.getContext("2d");
canvas.width = window.innerWidth;
canvas.height = window.innerHeight;

const particles = [];
for(let i=0; i<80; i++) {
  particles.push({
    x: Math.random() * canvas.width,
    y: Math.random() * canvas.height,
    size: Math.random() * 3,
    speedX: Math.random() * 1 - 0.5,
    speedY: Math.random() * 1 - 0.5,
    color: Math.random() > 0.5 ? "#00ffff" : "#ff00ff"
  });
}

function animate() {
  ctx.clearRect(0,0,canvas.width,canvas.height);
  particles.forEach(p => {
    ctx.fillStyle = p.color;
    ctx.beginPath();
    ctx.arc(p.x, p.y, p.size, 0, Math.PI * 2);
    ctx.fill();

    p.x += p.speedX;
    p.y += p.speedY;

    if(p.x < 0 || p.x > canvas.width) p.speedX *= -1;
    if(p.y < 0 || p.y > canvas.height) p.speedY *= -1;
  });
  requestAnimationFrame(animate);
}
animate();

window.addEventListener("resize", () => {
  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;
});
</script>

<!-- Final Quote -->
<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=22&pause=1000&color=00FFFF&center=true&vCenter=true&width=600&lines=Bridging+Humans+%26+Machines+Since+2023;Building+the+Future%2C+One+Bug+at+a+Time;Deploying+with+Confidence%2C+Breaking+with+Style" alt="Typing SVG" />
</p>
