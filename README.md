# TootCoin
TootCoin is a super silly money coin that loves to make funny fart noises!
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TootCoin - The Funniest Cryptocurrency</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f8ff;
            color: #333;
            text-align: center;
        }
        header {
            background-color: #ffd700;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        header h1 {
            font-size: 3rem;
            margin: 0;
        }
        .tagline {
            font-size: 1.5rem;
            margin: 10px 0;
        }
        .toot-coin-image {
            max-width: 200px;
            margin: 20px auto;
        }
        .main-content {
            padding: 20px;
        }
        .main-content h2 {
            font-size: 2rem;
            color: #555;
        }
        .main-content p {
            font-size: 1.2rem;
            line-height: 1.6;
            max-width: 700px;
            margin: 10px auto;
        }
        .cta-button {
            background-color: #ff6347;
            color: white;
            padding: 10px 20px;
            font-size: 1rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
        }
        .cta-button:hover {
            background-color: #e5533d;
        }
        footer {
            margin-top: 20px;
            padding: 10px;
            background-color: #ffd700;
            color: #333;
            font-size: 0.9rem;
        }
        .toot-game {
            margin-top: 30px;
        }
        .toot-text {
            font-size: 2rem;
            color: #ff6347;
        }
        .social-links {
            margin-top: 20px;
        }
        .social-links a {
            color: #1DA1F2;
            text-decoration: none;
            font-size: 1.2rem;
        }
        .social-links a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>TootCoin</h1>
        <p class="tagline">The cryptocurrency that’s full of laughs!</p>
    </header>
    <main class="main-content">
        <img src="tootcoin-image.png" alt="TootCoin Logo" class="toot-coin-image">
        <h2>What is TootCoin?</h2>
        <p>TootCoin is the world’s funniest cryptocurrency! It’s not just money; it’s a fart-tastic journey of giggles and fun. Perfect for those who love to trade with a sense of humor.</p>

        <h2>Why Choose TootCoin?</h2>
        <p>Because life’s too short for boring coins. TootCoin comes with giggles guaranteed. Every transaction is powered by fun!</p>

        <h2>How Does TootCoin Work?</h2>
        <p>To keep the fun going and the value rising, every time the market cap reaches $500,000, 10,000 tokens are burned! This helps reduce supply and makes each TootCoin more special.</p>

        <button class="cta-button">Get Started with TootCoin</button>

        <div class="toot-game">
            <p class="toot-text" id="toot-text">Click anywhere to make a toot!</p>
        </div>

        <div class="social-links">
            <p>Follow us on Twitter: <a href="https://x.com/tootcoins?s=21&t=leobGK6bTy7QJAK1HNhWGQ" target="_blank">@TootCoins</a></p>
        </div>
    </main>
    <footer>
        <p>&copy; 2024 TootCoin Inc. All rights reserved. Powered by laughs and farts.</p>
    </footer>

    <audio id="toot-sound" src="toot-sound.mp3"></audio>
    <script>
        document.body.addEventListener('click', () => {
            const tootSound = document.getElementById('toot-sound');
            tootSound.play();

            const tootText = document.getElementById('toot-text');
            tootText.textContent = "Toot!";

            setTimeout(() => {
                tootText.textContent = "Click anywhere to make a toot!";
            }, 1000);
        });
    </script>
</body>
</html>
