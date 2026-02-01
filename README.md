<h1 align="center">
  <a href="https://git.io/typing-svg" target="_blank">
    <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=600&size=70&pause=1000&color=35eddc&background=FFFFFF00&center=true&vCenter=true&width=900&height=80&lines=NANZ+HENRIX" alt="Typing SVG" />
  </a>
</h1>
<h2 align="center">
  <b>&lt;(^_^)&gt; END OF BEGINNING &lt;(^_^)&gt;</b>
</h2>
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=js,html,css,python,ae,windows,github,vscode,git,figma,au,react" />
  </a>
</p>
<h2  align="center">✧Activity Graph Based On Commits✧</h2>

[![Ashutosh's github activity graph](https://github-readme-activity-graph.vercel.app/graph?username=NanzHenrix&theme=react&bg_color=122533)](https://github.com/NanzHenrix/github-readme-activity-graph)

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Real-Time Clock</title>
<style>
  body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background: #1e1e1e;
    color: white;
    font-family: sans-serif;
  }

  .clock {
    width: 250px;
    height: 250px;
    border: 8px solid #fff;
    border-radius: 50%;
    position: relative;
    background: radial-gradient(#2c2c2c 95%, transparent 100%);
    box-shadow: 0 0 20px rgba(255,255,255,0.2);
  }

  .hand {
    position: absolute;
    width: 50%;
    height: 4px;
    background: #fff;
    top: 50%;
    transform-origin: 100%;
    transform: rotate(90deg);
    transition: all 0.05s cubic-bezier(0.4, 2.3, 0.3, 1);
  }

  .hour {
    height: 6px;
    background: #fff;
  }

  .minute {
    height: 4px;
    background: #0f0;
  }

  .second {
    height: 2px;
    background: #f00;
  }

  .center {
    position: absolute;
    width: 12px;
    height: 12px;
    background: #fff;
    border-radius: 50%;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
</style>
</head>
<body>
  <div class="clock">
    <div class="hand hour" id="hour"></div>
    <div class="hand minute" id="minute"></div>
    <div class="hand second" id="second"></div>
    <div class="center"></div>
  </div>

<script>
function updateClock() {
  const now = new Date();
  const hours = now.getHours() % 12;
  const minutes = now.getMinutes();
  const seconds = now.getSeconds();

  const hourDeg = (hours + minutes / 60) * 30; // 360/12 = 30
  const minuteDeg = (minutes + seconds / 60) * 6; // 360/60 = 6
  const secondDeg = seconds * 6;

  document.getElementById('hour').style.transform = `rotate(${hourDeg}deg)`;
  document.getElementById('minute').style.transform = `rotate(${minuteDeg}deg)`;
  document.getElementById('second').style.transform = `rotate(${secondDeg}deg)`;
}

// Update every 100ms for smooth movement
setInterval(updateClock, 100);
updateClock();
</script>
</body>
</html>
