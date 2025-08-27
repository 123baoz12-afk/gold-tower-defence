<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Tower Defense</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1 class="title">🔥 My Tower Defense 🔥</h1>
  <p>Click chuột vào bản đồ để đặt tháp (chọn loại tháp trước).</p>

  <div class="toolbar">
    <button onclick="selectTower('basic')">🟦 Basic (100g)</button>
    <button onclick="selectTower('fast')">🌀 Fast (120g)</button>
    <button onclick="selectTower('sniper')">🎯 Sniper (150g)</button>
  </div>

  <canvas id="game" width="900" height="600"></canvas>

  <!-- Dev Panel -->
  <div class="dev-panel" id="devPanel">
    <h3>⚙️ Dev Panel (Hack)</h3>
    Gold: <input type="number" id="setGold" value="200"><br>
    Ruby: <input type="number" id="setRuby" value="50"><br>
    Lives: <input type="number" id="setLives" value="10"><br>
    <button onclick="applyDevSettings()">✔ Apply</button>
  </div>

  <script src="game.js"></script>
</body>
</html>
