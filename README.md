<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TootCoin - The Funniest Cryptocurrency</title>
    <style>
        body {
            font-family: 'Comic Sans MS', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom right, #ffefba, #ffffff);
            color: #333;
            text-align: center;
        }
        header {
            background-color: #ff69b4;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            color: white;
        }
        header h1 {
            font-size: 3.5rem;
            margin: 0;
        }
        .tagline {
            font-size: 1.8rem;
            margin: 10px 0;
        }
        nav {
            margin: 20px 0;
            background-color: #ffb6c1;
            padding: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #ffffff;
            font-size: 1.4rem;
            font-weight: bold;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #660066;
        }
        main {
            padding: 20px;
        }
        .section {
            background-color: #ffffff;
            padding: 30px;
            margin: 20px auto;
            width: 90%;
            max-width: 800px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .cta-button {
            background-color: #ff69b4;
            color: white;
            padding: 15px 30px;
            font-size: 1.2rem;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
        }
        .cta-button:hover {
            background-color: #ff1493;
        }
        footer {
            margin-top: 30px;
            padding: 15px;
            background-color: #ff69b4;
            color: white;
            font-size: 1rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>TootCoin</h1>
        <p class="tagline">The cryptocurrency that’s full of laughs and farts!</p>
    </header>
    <nav>
        <a href="#about">About</a>
        <a href="#token-burning">Token Burning</a>
        <a href="#socials">Socials</a>
    </nav>
    <main>
        <section id="about" class="section">
            <h2>What is TootCoin?</h2>
            <p>TootCoin is the world’s funniest cryptocurrency! With TootCoin, every trade comes with a giggle. It’s perfect for those who love to mix fun with finance!</p>
            <button class="cta-button" id="toot-game">Click Here to Make a Toot!</button>
            <p id="toot-counter">Toots Made: 0</p>
        </section>
        <section id="token-burning" class="section">
            <h2>How Does TootCoin Work?</h2>
            <p>Every time our market cap hits $500,000, 10,000 tokens are burned! This reduces supply and makes every TootCoin extra special.</p>
        </section>
        <section id="socials" class="section">
            <h2>Follow Us</h2>
            <p>Follow us on Twitter: <a href="https://x.com/tootcoins?s=21&t=leobGK6bTy7QJAK1HNhWGQ" target="_blank">@TootCoins</a></p>
            <p>Contact Address: DxproJfPzgPh3Z4YdEmXQNWFbh5atFCyZEuhkjDmpump</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 TootCoin Inc. All rights reserved. Powered by laughs and toots.</p>
    </footer>
    <script>
        const tootButton = document.getElementById('toot-game');
        const tootCounter = document.getElementById('toot-counter');
        let tootCount = 0;

        tootButton.addEventListener('click', () => {
            tootCount++;
            tootCounter.textContent = `Toots Made: ${tootCount}`;
        });
</body>
</html>
