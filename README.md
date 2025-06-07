# for-Rita
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
      font-size: 4rem;
      letter-spacing: 2px;
      margin-bottom: 2rem;
      text-shadow: 0 0 12px rgba(255, 0, 0, 0.6);
    }

    /* PAGE 2 */
    #page2 {
      display: none;
      background-color: #1e2d5a; /* navy blue */
      color: white;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100%;
      width: 100%;
      max-width: 700px;
      padding: 2rem;
      font-weight: bold;
      font-size: 1.5rem;       /* smaller font size */
      line-height: 1.5;
      text-align: center;
      border-radius: 15px;
      overflow: hidden;
      box-sizing: border-box;
    }

    #page2 > div {
      max-height: 60vh;        /* limit height */
      overflow-y: auto;        /* scroll if needed */
      margin-bottom: 2rem;
      padding-right: 10px;     /* for scrollbar spacing */
    }

    #page2 button {
      margin-top: 0;
      flex-shrink: 0;
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

    #page2 button:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 15px rgba(0, 0, 0, 0.3);
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
      padding: 3rem 4rem;
      border-radius: 25px;
      text-align: center;
      box-shadow: 0 8px 20px rgba(0,0,0,0.2);
      max-width: 500px;
      width: 90%;
      font-family: 'Arial', sans-serif;
      color: black;
    }

    .coupon h2 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    .coupon p {
      font-size: 1.2rem;
      margin: 0.5rem 0;
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
      <h2>🎀 COUPON FOR 🎀</h2>
      <p style="font-weight: bold; font-size: 1.5rem;">HUGS and KISSES</p>
      <p>maximum use: infinite</p>
      <p>expiry date: forever</p>
    </div>
  </div>

  <script>
    function goToLetter() {
      // Hide page 1, show page 2, update bg
      document.getElementById('page1').style.display = 'none';
      document.getElementById('page2').style.display = 'flex';
      document.body.style.backgroundColor = '#1e2d5a'; // navy blue
    }

    function goToCoupon() {
      // Hide page 2, show page 3, update bg
      document.getElementById('page2').style.display = 'none';
      document.getElementById('page3').style.display = 'flex';
      document.body.style.backgroundColor = 'white';
    }
  </script>
</body>
</html>
