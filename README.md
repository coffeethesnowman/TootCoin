
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
            background: url('tootcoin_wallpaper.png') no-repeat center center fixed;
            background-size: cover;
            color: #333;
            text-align: center;
        }
        header {
            background-color: rgba(255, 215, 0, 0.9);
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
            max-width: 150px;
            margin: 20px auto;
        }
        nav {
            margin: 20px 0;
            background-color: rgba(255, 239, 130, 0.9);
            padding: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #333;
            font-size: 1.2rem;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #ff6347;
        }
        .section {
            display: none;
            background-color: rgba(255, 255, 255, 0.8);
            padding: 20px;
            margin: 20px auto;
            width: 80%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .section.active {
            display: block;
        }
        .cta-button {
            background-color: #ff6347;
            color: white;
            padding: 10px 20px;
            font-size: 1.2rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
            margin: 20px auto;
            display: inline-block;
        }
        .cta-button:hover {
            background-color: #e5533d;
        }
        footer {
            margin-top: 20px;
            padding: 10px;
            background-color: rgba(255, 215, 0, 0.9);
            color: #333;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>TootCoin</h1>
        <p class="tagline">The cryptocurrency that’s full of laughs!</p>
        <img src="tootcoin_logo.png" alt="TootCoin Logo" class="toot-coin-image">
    </header>
    <nav>
        <a href="#" data-tab="about">About</a>
        <a href="#" data-tab="token-burning">Token Burning</a>
        <a href="#" data-tab="socials">Socials</a>
    </nav>
    <main>
        <section id="about" class="section active">
            <h2>What is TootCoin?</h2>
            <p>TootCoin is the world’s funniest cryptocurrency! It’s not just money; it’s a fart-tastic journey of giggles and fun. Perfect for those who love to trade with a sense of humor.</p>
            <button class="cta-button" id="toot-game">Click Here to Make a Toot!</button>
        </section>
        <section id="token-burning" class="section">
            <h2>How Does TootCoin Work?</h2>
            <p>To keep the fun going and the value rising, every time the market cap reaches $500,000, 10,000 tokens are burned! This helps reduce supply and makes each TootCoin more special.</p>
        </section>
        <section id="socials" class="section">
            <h2>Follow Us</h2>
            <p>Follow us on Twitter: <a href="https://x.com/tootcoins?s=21&t=leobGK6bTy7QJAK1HNhWGQ" target="_blank">@TootCoins</a></p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 TootCoin Inc. All rights reserved. Powered by laughs and farts.</p>
    </footer>
    <audio id="toot-sound" src="videoplayback.m4a"></audio>
    <script>
        const tabs = document.querySelectorAll('nav a');
        const sections = document.querySelectorAll('.section');

        tabs.forEach(tab => {
            tab.addEventListener('click', (e) => {
                e.preventDefault();
                const target = tab.getAttribute('data-tab');

                sections.forEach(section => {
                    section.classList.remove('active');
                });

                document.getElementById(target).classList.add('active');
            });
        });

        // Play toot sound on button click
        document.getElementById('toot-game').addEventListener('click', (e) => {
            e.preventDefault();
            const tootSound = document.getElementById('toot-sound');
            tootSound.play();
        });
    </script>
</body>
</html>
