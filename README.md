<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Greeting for Annanya Nandi Miss</title>
  <style>
    :root {
      --primary-color: #4a90e2;
      --secondary-color: #50e3c2;
      --bg-color: #f7f9fc;
      --card-bg: #ffffff;
      --text-color: #333333;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #a1c4fd 0%, #c2e9fb 100%);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 20px;
      color: var(--text-color);
    }

    .container {
      background: var(--card-bg);
      max-width: 650px;
      width: 100%;
      border-radius: 20px;
      padding: 40px;
      box-shadow: 0 15px 35px rgba(0, 0, 0, 0.15);
      text-align: center;
      animation: fadeIn 1s ease-in-out;
      border: 2px solid #84fab0;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .school-tag {
      display: inline-block;
      background: #84fab0;
      color: #1a5336;
      padding: 6px 16px;
      border-radius: 20px;
      font-size: 0.85rem;
      font-weight: bold;
      letter-spacing: 1px;
      margin-bottom: 15px;
      text-transform: uppercase;
    }

    h1 {
      font-size: 2.2rem;
      color: #2c3e50;
      margin-bottom: 10px;
    }

    p.subtitle {
      font-size: 1.05rem;
      color: #555;
      margin-bottom: 25px;
    }

    .quote-box {
      background: #f0f4f8;
      border-left: 5px solid var(--primary-color);
      padding: 15px 20px;
      margin-bottom: 25px;
      border-radius: 8px;
      font-style: italic;
      color: #444;
    }

    button {
      background: linear-gradient(135deg, #4481eb, #04b6e5);
      color: white;
      border: none;
      padding: 14px 30px;
      font-size: 1rem;
      font-weight: bold;
      border-radius: 25px;
      cursor: pointer;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    button:hover {
      transform: translateY(-2px);
      box-shadow: 0 5px 15px rgba(4, 182, 229, 0.4);
    }

    .message-card {
      display: none;
      margin-top: 25px;
      padding: 25px;
      background: #f4fbf7;
      border: 1px solid #a3e4d7;
      border-radius: 12px;
      animation: fadeIn 0.8s ease-in-out;
      text-align: left;
    }

    .message-card h2 {
      color: #1b4f72;
      margin-bottom: 10px;
    }

    .signature {
      margin-top: 20px;
      text-align: right;
      font-weight: bold;
      color: #2e4053;
      border-top: 1px dashed #ccc;
      padding-top: 10px;
    }

    .footer {
      margin-top: 35px;
      font-size: 0.85rem;
      color: #777;
    }
  </style>
</head>
<body>

  <div class="container">
    <div class="school-tag">St. Mary's School • CBSE Class 12</div>
    <h1>Dear Annanya Nandi Miss 💐</h1>
    <p class="subtitle">A special card created with gratitude for your constant guidance and support.</p>

    <div class="quote-box" id="quote-display">
      "A great teacher takes a hand, opens a mind, and touches a heart."
    </div>

    <button onclick="revealMessage()">Click to Open Note</button>

    <div class="message-card" id="hidden-message">
      <h2>Respected Miss,</h2>
      <p style="margin-top: 10px; line-height: 1.6; color: #34495e;">
        Thank you for being an exceptional mentor and for making our learning journey so insightful and inspiring. Your constant encouragement and guidance mean a lot to us as we navigate through Class 12.
      </p>
      <p style="margin-top: 15px; font-weight: bold; color: #117a65;">
        Wishing you happiness, health, and success always! ✨
      </p>
      <div class="signature">
        — Warm regards,<br>
        <strong>Somshirsha Mukherjee</strong><br>
        <span style="font-weight: normal; font-size: 0.9rem; color: #666;">Class 12, CBSE</span>
      </div>
    </div>

    <div class="footer">
      Designed with respect & gratitude by Somshirsha
    </div>
  </div>

  <script>
    const quotes = [
      "\"A great teacher takes a hand, opens a mind, and touches a heart.\"",
      "\"Education is not the filling of a pail, but the lighting of a fire.\" – W.B. Yeats",
      "\"Teachers plant seeds that grow forever.\"",
      "\"Technology is just a tool. In terms of getting the kids working together and motivating them, the teacher is the most important.\" – Bill Gates"
    ];

    // Select random quote on load
    const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
    document.getElementById('quote-display').innerText = randomQuote;

    function revealMessage() {
      const msg = document.getElementById('hidden-message');
      if (msg.style.display === "block") {
        msg.style.display = "none";
      } else {
        msg.style.display = "block";
      }
    }
  </script>

</body>
</html>
