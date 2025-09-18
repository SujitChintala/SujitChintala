<div align="center">

<!-- Bomb Blast Animation Container -->
<div class="explosion-container">
  <div class="bomb">💣</div>
  <div class="blast-circle blast-1"></div>
  <div class="blast-circle blast-2"></div>
  <div class="blast-circle blast-3"></div>
  <div class="particles">
    <div class="particle p1">✨</div>
    <div class="particle p2">💥</div>
    <div class="particle p3">⭐</div>
    <div class="particle p4">✨</div>
    <div class="particle p5">💥</div>
    <div class="particle p6">⭐</div>
    <div class="particle p7">✨</div>
    <div class="particle p8">💥</div>
  </div>
</div>

<!-- Profile Information that emerges from blast -->
<div class="profile-info">
  <div class="info-card card-1">
    <h1>🚀 Sujit Chintala</h1>
    <p>💻 Full Stack Developer</p>
  </div>
  
  <div class="info-card card-2">
    <h3>🎯 What I Do</h3>
    <p>🔥 Building amazing web applications<br>
    ⚡ Creating scalable solutions<br>
    🌟 Turning ideas into reality</p>
  </div>
  
  <div class="info-card card-3">
    <h3>🛠️ Tech Stack</h3>
    <p>
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
      <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React"/>
      <img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js"/>
      <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
    </p>
  </div>
  
  <div class="info-card card-4">
    <h3>🌐 Connect With Me</h3>
    <p>
      <a href="https://github.com/SujitChintala">
        <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
      </a>
      <a href="https://linkedin.com/in/sujitchintala">
        <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
      </a>
    </p>
  </div>
  
  <div class="info-card card-5">
    <h3>📊 GitHub Stats</h3>
    <p>
      <img src="https://github-readme-stats.vercel.app/api?username=SujitChintala&show_icons=true&theme=radical&hide_border=true" alt="GitHub Stats"/>
    </p>
    <p>
      <img src="https://github-readme-streak-stats.herokuapp.com/?user=SujitChintala&theme=radical&hide_border=true" alt="GitHub Streak"/>
    </p>
  </div>
</div>

<!-- Final blast effect -->
<div class="final-blast">
  <div class="blast-text">🎉 Welcome to my GitHub! 🎉</div>
</div>

<!-- CSS Animations -->
<style>
  .explosion-container {
    position: relative;
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 50px 0;
    overflow: hidden;
  }
  
  .bomb {
    font-size: 3em;
    animation: bombCountdown 3s ease-in-out;
    z-index: 10;
  }
  
  .blast-circle {
    position: absolute;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(255,69,0,0.8) 0%, rgba(255,140,0,0.6) 30%, rgba(255,215,0,0.4) 60%, transparent 100%);
    opacity: 0;
  }
  
  .blast-1 {
    width: 100px;
    height: 100px;
    animation: explode 1.5s ease-out 2.5s;
  }
  
  .blast-2 {
    width: 200px;
    height: 200px;
    animation: explode 2s ease-out 2.7s;
  }
  
  .blast-3 {
    width: 300px;
    height: 300px;
    animation: explode 2.5s ease-out 2.9s;
  }
  
  .particles {
    position: absolute;
    width: 100%;
    height: 100%;
  }
  
  .particle {
    position: absolute;
    font-size: 1.5em;
    opacity: 0;
    animation: particleFly 3s ease-out 3s;
  }
  
  .p1 { 
    top: 20%; left: 10%; 
    animation: particleFly1 3s ease-out 3s forwards;
  }
  .p2 { 
    top: 10%; left: 80%; 
    animation: particleFly2 3s ease-out 3.2s forwards;
  }
  .p3 { 
    top: 60%; left: 90%; 
    animation: particleFly3 3s ease-out 3.1s forwards;
  }
  .p4 { 
    top: 80%; left: 20%; 
    animation: particleFly4 3s ease-out 3.3s forwards;
  }
  .p5 { 
    top: 30%; left: 70%; 
    animation: particleFly5 3s ease-out 3.4s forwards;
  }
  .p6 { 
    top: 70%; left: 60%; 
    animation: particleFly6 3s ease-out 3.2s forwards;
  }
  .p7 { 
    top: 15%; left: 40%; 
    animation: particleFly7 3s ease-out 3.5s forwards;
  }
  .p8 { 
    top: 85%; left: 45%; 
    animation: particleFly8 3s ease-out 3.1s forwards;
  }
  
  .profile-info {
    opacity: 0;
    animation: revealInfo 2s ease-out 4s forwards;
  }
  
  .info-card {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border: 2px solid #ff6b6b;
    border-radius: 15px;
    padding: 20px;
    margin: 20px;
    box-shadow: 0 8px 32px rgba(31, 38, 135, 0.37);
    backdrop-filter: blur(4px);
    transform: scale(0) rotate(180deg);
    opacity: 0;
    color: white;
  }
  
  .card-1 {
    animation: cardPop 1s ease-out 4.5s forwards;
  }
  
  .card-2 {
    animation: cardPop 1s ease-out 5s forwards;
  }
  
  .card-3 {
    animation: cardPop 1s ease-out 5.5s forwards;
  }
  
  .card-4 {
    animation: cardPop 1s ease-out 6s forwards;
  }
  
  .card-5 {
    animation: cardPop 1s ease-out 6.5s forwards;
  }
  
  .final-blast {
    opacity: 0;
    text-align: center;
    margin: 30px 0;
    animation: finalBlastAppear 2s ease-out 7.5s forwards;
  }
  
  .blast-text {
    font-size: 2em;
    font-weight: bold;
    background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #96ceb4, #feca57);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: textGlow 2s ease-in-out infinite alternate;
  }
  
  /* Keyframe Animations */
  @keyframes bombCountdown {
    0% { transform: scale(1); }
    20% { transform: scale(1.1); }
    40% { transform: scale(1); }
    60% { transform: scale(1.1); }
    80% { transform: scale(1); }
    95% { transform: scale(1.2); }
    100% { transform: scale(0); opacity: 0; }
  }
  
  @keyframes explode {
    0% {
      transform: scale(0);
      opacity: 1;
    }
    50% {
      opacity: 0.8;
    }
    100% {
      transform: scale(1);
      opacity: 0;
    }
  }
  
  @keyframes particleFly {
    0% {
      transform: translate(0, 0) scale(1);
      opacity: 1;
    }
    100% {
      transform: translate(var(--random-x, 200px), var(--random-y, -200px)) scale(0);
      opacity: 0;
    }
  }
  
  @keyframes particleFly1 {
    0% { transform: translate(0, 0) scale(1) rotate(0deg); opacity: 1; }
    100% { transform: translate(-150px, -200px) scale(0) rotate(360deg); opacity: 0; }
  }
  
  @keyframes particleFly2 {
    0% { transform: translate(0, 0) scale(1) rotate(0deg); opacity: 1; }
    100% { transform: translate(200px, -180px) scale(0) rotate(-360deg); opacity: 0; }
  }
  
  @keyframes particleFly3 {
    0% { transform: translate(0, 0) scale(1) rotate(0deg); opacity: 1; }
    100% { transform: translate(100px, 150px) scale(0) rotate(180deg); opacity: 0; }
  }
  
  @keyframes particleFly4 {
    0% { transform: translate(0, 0) scale(1) rotate(0deg); opacity: 1; }
    100% { transform: translate(-180px, 120px) scale(0) rotate(-180deg); opacity: 0; }
  }
  
  @keyframes particleFly5 {
    0% { transform: translate(0, 0) scale(1) rotate(0deg); opacity: 1; }
    100% { transform: translate(250px, -150px) scale(0) rotate(270deg); opacity: 0; }
  }
  
  @keyframes particleFly6 {
    0% { transform: translate(0, 0) scale(1) rotate(0deg); opacity: 1; }
    100% { transform: translate(-200px, 180px) scale(0) rotate(-270deg); opacity: 0; }
  }
  
  @keyframes particleFly7 {
    0% { transform: translate(0, 0) scale(1) rotate(0deg); opacity: 1; }
    100% { transform: translate(0px, -250px) scale(0) rotate(450deg); opacity: 0; }
  }
  
  @keyframes particleFly8 {
    0% { transform: translate(0, 0) scale(1) rotate(0deg); opacity: 1; }
    100% { transform: translate(180px, 200px) scale(0) rotate(-450deg); opacity: 0; }
  }
  
  @keyframes finalBlastAppear {
    0% {
      opacity: 0;
      transform: scale(0) rotate(180deg);
    }
    50% {
      opacity: 1;
      transform: scale(1.2) rotate(0deg);
    }
    100% {
      opacity: 1;
      transform: scale(1) rotate(0deg);
    }
  }
  
  @keyframes textGlow {
    0% {
      text-shadow: 0 0 10px rgba(255, 107, 107, 0.5);
    }
    100% {
      text-shadow: 0 0 20px rgba(255, 107, 107, 0.8), 0 0 30px rgba(78, 205, 196, 0.6);
    }
  }
  
  @keyframes revealInfo {
    0% {
      opacity: 0;
      transform: translateY(50px);
    }
    100% {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  @keyframes cardPop {
    0% {
      transform: scale(0) rotate(180deg);
      opacity: 0;
    }
    50% {
      transform: scale(1.1) rotate(10deg);
      opacity: 0.8;
    }
    100% {
      transform: scale(1) rotate(0deg);
      opacity: 1;
    }
  }
  
  /* Hover effects */
  .info-card:hover {
    transform: translateY(-10px) scale(1.05);
    box-shadow: 0 15px 40px rgba(31, 38, 135, 0.5);
    transition: all 0.3s ease;
  }
  
  /* Mobile responsiveness */
  @media (max-width: 768px) {
    .explosion-container {
      height: 150px;
      margin: 30px 0;
    }
    
    .bomb {
      font-size: 2em;
    }
    
    .info-card {
      margin: 10px;
      padding: 15px;
    }
    
    .blast-1, .blast-2, .blast-3 {
      width: 80px;
      height: 80px;
    }
    
    .blast-2 {
      width: 150px;
      height: 150px;
    }
    
    .blast-3 {
      width: 220px;
      height: 220px;
    }
  }
</style>

</div>👋 Hi, I’m @SujitChintala
- 👀 I’m interested in building things.