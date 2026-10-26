<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>H Sports Live</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #0a0f1a;
      color: white;
      min-height: 100vh;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 40px;
      background: rgba(0, 0, 0, 0.35);
      border-bottom: 1px solid rgba(255, 255, 255, 0.08);
      flex-wrap: wrap;
    }

    .logo {
      font-size: 1.6rem;
      font-weight: bold;
      color: #38bdf8;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .live-dot {
      width: 10px;
      height: 10px;
      background: #ef4444;
      border-radius: 50%;
      animation: pulse 1.5s infinite;
    }

    @keyframes pulse {
      0% { opacity: 1; }
      50% { opacity: 0.4; }
      100% { opacity: 1; }
    }

    .nav-links {
      display: flex;
      gap: 25px;
    }

    .nav-links a {
      color: #cbd5e1;
      text-decoration: none;
      font-size: 0.95rem;
      transition: color 0.2s;
    }

    .nav-links a:hover {
      color: #38bdf8;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 30px 20px;
    }

    .hero {
      text-align: center;
      margin-bottom: 40px;
    }

    .hero h1 {
      font-size: 2.8rem;
      color: #38bdf8;
      margin-bottom: 10px;
    }

    .hero p {
      font-size: 1.1rem;
      color: #94a3b8;
    }

    .live-channel-box {
      background: rgba(255, 255, 255, 0.04);
      border: 1px solid rgba(255, 255, 255, 0.08);
      border-radius: 12px;
      padding: 30px;
      text-align: center;
      margin-bottom: 30px;
    }

    .live-channel-box h2 {
      color: #ef4444;
      margin-bottom: 15px;
      font-size: 1.8rem;
    }

    .stream-placeholder {
      background: #111827;
      border: 1px solid #38bdf8;
      border-radius: 10px;
      padding: 60px 20px;
      color: #94a3b8;
      font-size: 1.1rem;
      margin-bottom: 20px;
    }

    .watch-btn {
      display: inline-block;
      background: #ef4444;
      color: white;
      padding: 14px 32px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      font-size: 1rem;
      transition: background 0.3s;
    }

    .watch-btn:hover {
      background: #dc2626;
    }

    .section {
      margin-top: 40px;
    }

    .section h2 {
      font-size: 1.4rem;
      color: #e2e8f0;
      margin-bottom: 25px;
      text-align: center;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
      gap: 15px;
    }

    .sport-card {
      background: rgba(255, 255, 255, 0.04);
      border: 1px solid rgba(255, 255, 255, 0.08);
      border-radius: 10px;
      padding: 25px 15px;
      text-align: center;
      transition: all 0.3s ease;
    }

    .sport-card:hover {
      border-color: #38bdf8;
      background: rgba(56, 189, 248, 0.05);
    }

    .sport-card span {
      font-size: 2rem;
      margin-bottom: 10px;
      display: block;
    }

    .sport-card h3 {
      font-size: 1rem;
      color: #e2e8f0;
    }

    footer {
      text-align: center;
      padding: 40px 20px;
      color: #64748b;
      font-size: 0.85rem;
    }

    @media (max-width: 768px) {
      nav {
        flex-direction: column;
        gap: 15px;
      }

      .hero h1 {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>

  <nav>
    <div class="logo">
      <span class="live-dot"></span>
      H Sports Live
    </div>
    <div class="nav-links">
      <a href="/">Home</a>
      <a href="/live">Live Channel</a>
      <a href="/scores">Live Scores</a>
      <a href="/schedule">Schedule</a>
      <a href="/news">News</a>
    </div>
  </nav>

  <div class="container">
    <div class="hero">
      <h1>H Sports Live</h1>
      <p>Watch live sports channels, scores, and updates in one place.</p>
    </div>

    <div class="live-channel-box">
      <h2>🔴 LIVE CHANNEL</h2>
      <div class="stream-placeholder">
        Live stream player will appear here
      </div>
      <a href="#" class="watch-btn">Watch Live Now</a>
    </div>

    <div class="section">
      <h2>🏆 Sports Coverage</h2>
      <div class="cards">
        <div class="sport-card">
          <span>⚽</span>
          <h3>Football</h3>
        </div>
        <div class="sport-card">
          <span>🏀</span>
          <h3>NBA</h3>
        </div>
        <div class="sport-card">
          <span>🏈</span>
          <h3>NFL</h3>
        </div>
        <div class="sport-card">
          <span>🎾</span>
          <h3>Tennis</h3>
        </div>
        <div class="sport-card">
          <span>🥊</span>
          <h3>Boxing</h3>
        </div>
        <div class="sport-card">
          <span>🏎️</span>
          <h3>F1</h3>
        </div>
      </div>
    </div>
  </div>

  <footer>
    <p>H Sports Live — Fast, Reliable Sports Updates</p>
  </footer>

</body>
</html>

