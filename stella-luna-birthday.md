<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Birthday Mission | Maximum Reality</title>
  <style>
    /* Main vibe and colors */
    body { 
      background-color: #0b1021; 
      color: white; 
      font-family: -apple-system, BlinkMacSystemFont, sans-serif; 
      text-align: center; 
      padding: 15px; 
      margin: 0;
    }
    
    h1 { 
      color: #ffb6c1; 
      margin: 30px 0; 
      text-shadow: 0 0 10px rgba(255,182,193,0.5); 
      font-size: 1.6rem;
      letter-spacing: 2px;
    }

    /* Individual Image Frames */
    .scene-frame {
      width: 100%;
      height: auto;
      max-width: 500px; /* Keeps it sharp on the Pro Max */
      border-radius: 25px;
      border: 2px solid #ffb6c1;
      margin: 20px 0;
      box-shadow: 0 0 15px rgba(255, 182, 193, 0.2);
    }

    .story-text { 
      font-size: 1.15rem; 
      line-height: 1.6; 
      padding: 0 15px; 
      margin: 10px 0 40px 0; 
      color: #f0f0f0;
    }
    
    /* The Birthday Surprise Box */
    .birthday-box {
      border: 3px dashed #ffb6c1;
      border-radius: 35px;
      padding: 25px;
      margin: 40px 10px;
      background: rgba(255,182,193,0.05);
    }

    #birthday-surprise { 
      display: none; 
      font-size: 3.5rem; 
      animation: bounce 2s infinite; 
    }

    @keyframes bounce { 
      0%, 100% { transform: translateY(0); } 
      50% { transform: translateY(-15px); } 
    }

    .nav-link { 
      display: inline-block; 
      margin: 40px 0 60px 0; 
      padding: 15px 35px; 
      color: #ffb6c1; 
      border: 2px solid #ffb6c1; 
      border-radius: 50px; 
      text-decoration: none; 
      font-weight: bold;
    }
  </style>
</head>
<body>

  <h1>THE BIRTHDAY MISSION</h1>

  <img src="birthday_1.JPG" class="scene-frame" alt="Luna and Stella with Moon Cookie">
  <p class="story-text">
    Luna is turning <b>Two</b>! She found a giant Moon Cookie floating in the stars, but it needs a special birthday glow.
  </p>

  <img src="birthday_2.JPG" class="scene-frame" alt="The Glowing Library Tree">
  <p class="story-text">
    Stella, the Master Explorer, is leading the way to the <b>Maximum Reality Library</b> to find the missing stardust frosting.
  </p>

  <img src="birthday_3.JPG" class="scene-frame" alt="Guardians of the Archive">
  <p class="story-text">
    Deep in the stars, the <b>Guardians of the Archive</b> found the secret glow. Mission accomplished!
  </p>

  <div class="birthday-box">
    <div id="birthday-surprise">
      🧁<br>
      <span style="font-size: 1.2rem; color: #ffb6c1;">HAPPY 2nd BIRTHDAY LUNA!</span>
    </div>
    <p class="story-text" id="waiting-text">The stars are lining up... check back on January 15th for the final glow!</p>
  </div>

  <a href="library.html" class="nav-link">← BACK TO LIBRARY</a>

  <script>
    // Reveal the surprise on Jan 15th
    const today = new Date();
    const isJan = today.getMonth() === 0; // 0 is January
    const is15th = today.getDate() === 15;

    if (isJan && is15th) {
      document.getElementById('birthday-surprise').style.display = 'block';
      document.getElementById('waiting-text').style.display = 'none';
    }
  </script>

</body>
</html>
