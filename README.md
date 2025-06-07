<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>For Rita 💘</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Arial', sans-serif;
    }

    body {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 1rem;
      transition: background-color 0.5s ease-in-out;
    }

    #page1, #page2, #page3 {
      display: none;
      height: 100%;
      width: 100%;
      max-width: 600px;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 1.5rem;
      border-radius: 15px;
    }

    #page1 {
      display: flex;
      background-color: black;
    }

    #page1 h1 {
      color: red;
      font-size: 2.5rem;
      margin-bottom: 2rem;
      text-shadow: 0 0 12px rgba(255, 0, 0, 0.6);
    }

    #page2 {
      background-color: #1e2d5a;
      color: white;
      font-weight: bold;
      font-size: 1.2rem;
      line-height: 1.5;
    }

    #page2 > div {
      max-height: 60vh;
      overflow-y: auto;
      margin-bottom: 2rem;
      padding-right: 10px;
    }

    #page3 {
      background-color: white;
    }

    .coupon {
      background-color: #ffc0cb;
      padding: 2rem;
      border-radius: 20px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.2);
      width: 100%;
      max-width: 400px;
      color: black;
    }

    .coupon h2 {
      font-size: 2.2rem;
      margin-bottom: 0.5rem;
    }

    .coupon p {
      font-size: 1.1rem;
      margin: 0.4rem 0;
    }

    .coupon .main-line {
      font-size: 1.6rem;
      font-weight: bold;
      margin: 0.5rem 0 1rem;
    }

    button {
      background-color: white;
      color: black;
      font-size: 1.2rem;
      padding: 12px 24px;
      border: none;
      border-radius: 10px;
      box-shadow: 0 4px 0 #aaa;
      cursor: pointer;
      transition: all 0.2s ease-in-out;
      font-weight: bold;
    }

    button:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 15px rgba(0, 0, 0, 0.3);
    }

    @media (max-width: 480px) {
      #page1 h1 {
        font-size: 2rem;
      }

      button {
        font-size: 1rem;
        padding: 10px 20px;
      }

      .coupon h2 {
        font-size: 1.8rem;
      }

      .coupon .main-line {
        font-size: 1.3rem;
      }
    }
  </style>
</head>
<body>
  <!-- PAGE 1 -->
  <div id="page1">
    <h1>FOR MY BABY GIRL RITA</h1>
    <button onclick="goToLetter()">READ ME</button>
  </div>

  <!-- PAGE 2 -->
  <div id="page2">
    <div>
      I LOVE YOU SO SO MUCH BABYYY 💘<br><br>
      Every day with you is a blessing. You are my everything — my sunshine, my joy.<br><br>  
      I can't imagine my life without you. You make me a better person, and I’m so grateful for every moment  
      we share. You are the love of my life, and I promise to cherish you forever.<br><br>  
      I love you more than words can express. You are my heart, my soul, my everything.<br><br>  
      I love you to the moon and back, and I’ll always be here for you.<br><br>  
      You are my forever and always, my love, my Rita.
    </div>
    <button onclick="goToCoupon()">REDEEM NOW !!!</button>
  </div>

  <!-- PAGE 3 -->
  <div id="page3">
    <div class="coupon">
      <h2>🎀 COUPON 🎀</h2>
      <p>FOR</p>
      <p class="main-line">HUGS and KISSES</p>
      <p>maximum use: infinite</p>
      <p>expiry date: forever</p>
    </div>
  </div>

  <script>
    function goToLetter() {
      document.getElementById('page1').style.display = 'none';
      document.getElementById('page2').style.display = 'flex';
      document.body.style.backgroundColor = '#1e2d5a';
    }

    function goToCoupon() {
      document.getElementById('page2').style.display = 'none';
      document.getElementById('page3').style.display = 'flex';
      document.body.style.backgroundColor = 'white';
    }
  </script>
</body>
</html>
