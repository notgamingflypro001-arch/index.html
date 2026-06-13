# index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Neon Retro Clicker</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>👾 NEON ARCADE 👾</h1>
        <p>A completely serverless, free cloud-synced clicker game.</p>
    </header>

    <div class="main-layout">
        <!-- Sidebar Segment -->
        <aside class="sidebar">
            <div id="auth-box" class="card">
                <h3><span class="icon">🎮</span> Claim Token</h3>
                <input type="text" id="username-input" placeholder="Enter Player Tag...">
                <button onclick="handleLogin()">Join Arena</button>
            </div>

            <div class="card">
                <h3><span class="icon">🏆</span> Global Leaderboard</h3>
                <ul id="leaderboard-list">
                    <li class="loading">Loading live ranks...</li>
                </ul>
            </div>
        </aside>

        <!-- Main Gameplay Window -->
        <main class="game-window card">
            <div class="game-header">
                <h2>Target Smasher Matrix</h2>
                <div class="score-container">Score: <span id="score-counter">0</span></div>
            </div>
            
            <div id="game-arena">
                <div id="game-target" onclick="targetClicked()">🎯</div>
            </div>
        </main>
    </div>

    <script src="game.js"></script>
</body>
</html>
