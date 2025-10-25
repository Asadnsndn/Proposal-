<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>I Proposed You 💍</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500;700&display=swap');

  body {
    margin: 0;
    padding: 0;
    height: 100vh;
    background: radial-gradient(circle at bottom, #0b0c10, #1f2833);
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    perspective: 1000px;
    font-family: 'Poppins', sans-serif;
  }

  .creator {
    position: absolute;
    top: 40px;
    font-size: 1.2em;
    color: #00ffff;
    text-shadow: 0 0 15px #00ffff, 0 0 25px #33ffff;
    animation: fadeIn 3s ease-in-out infinite alternate;
  }

  @keyframes fadeIn {
    from { opacity: 0.3; transform: translateY(-10px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .ring {
    width: 220px;
    height: 220px;
    border: 6px solid #ff6699;
    border-radius: 50%;
    position: absolute;
    animation: spin 5s linear infinite;
    box-shadow: 0 0 40px #ff6699, inset 0 0 20px #ff3366;
  }

  @keyframes spin {
    from { transform: rotateX(0deg) rotateY(0deg); }
    to { transform: rotateX(360deg) rotateY(360deg); }
  }

  .heart {
    position: relative;
    width: 130px;
    height: 130px;
    background: #ff3366;
    transform: rotate(-45deg);
    box-shadow: 0 0 40px #ff3366;
    animation: float 3s ease-in-out infinite;
  }

  .heart::before,
  .heart::after {
    content: "";
    position: absolute;
    width: 130px;
    height: 130px;
    background: #ff3366;
    border-radius: 50%;
  }

  .heart::before {
    top: -65px;
    left: 0;
  }

  .heart::after {
    left: 65px;
    top: 0;
  }

  @keyframes float {
    0%, 100% { transform: translateY(0) rotate(-45deg); }
    50% { transform: translateY(-20px) rotate(-45deg); }
  }

  h1 {
    position: absolute;
    bottom: 100px;
    font-size: 2.8em;
    color: #ff3366;
    text-shadow: 0 0 25px #ff3366, 0 0 45px #ff6699;
    animation: glow 2s infinite alternate;
  }

  @keyframes glow {
    from { text-shadow: 0 0 10px #ff6699; }
    to { text-shadow: 0 0 30px #ff3366, 0 0 60px #ff6699; }
  }

  .light {
    position: absolute;
    width: 100vw;
    height: 100vh;
    background: radial-gradient(circle, rgba(255, 51, 102, 0.1) 0%, transparent 70%);
    animation: pulse 3s infinite;
  }

  @keyframes pulse {
    0%, 100% { opacity: 0.4; }
    50% { opacity: 1; }
  }
</style>
</head>
<body>

<div class="light"></div>
<div class="creator">✨ Created by Ariyan ✨</div>
<div class="ring"></div>
<div class="heart"></div>
<h1>💍 I Proposed You 💞</h1>

</body>
</html>
