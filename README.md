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
      padding: 2rem;
      transition: background-color 0.5s ease-in-out;
    }

    /* PAGE 1 */
    #page1 {
      background-color: black;
      flex-direction: column;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100%;
      width: 100%;
      text-align: center;
    }

    #page1 h1 {
      color: red;
      font-size: 2.5rem;
      letter-spacing: 2px;
      margin-bottom: 2rem;
      text-shadow: 0 0 12px rgba(255, 0, 0, 0.6);
    }

    /* PAGE 2 */
    #page2 {
      display: none;
      background-color: #1e2d5a;
      color: white;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100%;
      width: 100%;
      max-width: 700px;
      padding: 2rem;
      font-weight: bold;
      font-size: 1.2rem;
      line-height: 1.6;
      text-align: center;
      border-radius: 15px;
      overflow: hidden;
      box-sizing: border-box;
    }

    #page2 > div {
      max-height: 60vh;
      overflow-y: auto;
      margin-bottom: 2rem;
      padding-right: 10px;
    }

    #page2 button {
      margin-top: 0;
      flex-shrink: 0;
    }

    /* PAGE 3 */
    #page3 {
      display: none;
      background-color: white;
      height: 100%;
      width: 100%;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 2rem;
    }

    .coupon {
      background-color: #ffc0cb;
      padding: 2rem;
      border-radius: 25px;
      text-align: center;
      box-shadow: 0 8px 20px rgba(0,0,0,0.2);
      max-width: 500px;
      width: 100%;
      font-family: 'Arial', sans-serif;
      color: black;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    .coupon h2 {
      font-size: 2rem;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 0.5rem;
      margin-bottom: 0.2rem;
      word-spacing: 4px;
    }

    .coupon p {
      font-size: 1.1rem;
      margin: 0.4rem 0;
      word-break: break-word;
    }

    /* BUTTONS shared style */
    button {
      background-color: white;
      color: black;
      font-size: 1.3rem;
      padding: 15px 30px;
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

    @media (max-width: 600px) {
      #page1 h1 {
        font-size: 2rem;
      }

      #page2 {
        font-size: 1rem;
      }

      .coupon h2 {
        font-size: 1.7rem;
      }

      .coupon p {
        font-size: 1rem;
      }

      button {
        font-size: 1rem;
        padding: 12px 20px;
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
      <p style="font-size: 1.1rem; margin-top: 0.5rem;">FOR</p>
      <p style="font-weight: bold; font-size: 1.8rem; margin: 0.5rem 0;">HUGS and KISSES</p>
      <p>maximum use: <strong>infinite</strong></p>
      <p>expiry date: <strong>forever</strong></p>
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
