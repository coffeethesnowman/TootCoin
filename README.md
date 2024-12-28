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
            background-color: #e0f7fa; /* Light cyan background for easy readability */
            color: #333;
            text-align: center;
        }
        header {
            background-color: rgba(0, 188, 212, 0.9); /* Soothing teal */
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        header h1 {
            font-size: 3rem;
            margin: 0;
            color: #ffffff;
        }
        .tagline {
            font-size: 1.5rem;
            margin: 10px 0;
            color: #ffffff;
        }
        .toot-coin-image {
            max-width: 150px;
            margin: 20px auto;
        }
        nav {
            margin: 20px 0;
            background-color: rgba(224, 247, 250, 0.9);
            padding: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #00796b;
            font-size: 1.2rem;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #004d40;
        }
        .section {
            display: none;
            background-color: rgba(255, 255, 255, 0.9);
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
            background-color: #00796b;
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
            background-color: #004d40;
        }
        footer {
            margin-top: 20px;
            padding: 10px;
            background-color: rgba(0, 188, 212, 0.9);
            color: #ffffff;
            font-size: 0.9rem;
        }
        #toot-counter {
            font-size: 1.5rem;
            margin-top: 20px;
            color: #00796b;
        }
    </style>
</head>
<body>
    <header>
        <h1>TootCoin</h1>
        <p class="tagline">The cryptocurrency that’s full of laughs!</p>
        <img src="tootcoin.png" alt="TootCoin Logo" class="toot-coin-image">
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
            <p id="toot-counter">Toots Made: 0</p>
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

        // Play toot sound and update counter
        const tootButton = document.getElementById('toot-game');
        const tootSound = document.getElementById('toot-sound');
        const tootCounter = document.getElementById('toot-counter');
        let tootCount = 0;

        tootButton.addEventListener('click', () => {
            tootSound.currentTime = 0; // Restart sound if already playing
            tootSound.play();

            tootCount++;
            tootCounter.textContent = `Toots Made: ${tootCount}`;
        });
    </script>
</body>
</html>
