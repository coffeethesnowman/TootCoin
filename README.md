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
            background: url('https://github.com/user-attachments/assets/a1ea6935-c93d-4fa0-952b-6afda5bf2959') no-repeat center center fixed;
            background-size: cover;
            color: #333;
            text-align: center;
        }
        header {
            background-color: rgba(0, 188, 212, 0.9);
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
        #toot-fact {
            font-size: 1.2rem;
            margin-top: 20px;
            color: #004d40;
        }
    </style>
</head>
<body>
    <header>
        <h1>TootCoin</h1>
        <p class="tagline">The cryptocurrency that’s full of laughs!</p>
        <img width="593" alt="tootcoin" src="https://github.com/user-attachments/assets/1ed4fa07-0ae4-4c58-a5e0-ff2e148be840" />
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
            <button class="cta-button" id="fun-fact-button">Click Here for a Fun Toot Fact!</button>
            <p id="toot-fact">Press the button to learn something funny about tooting!</p>
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

        // Display a random fun fact
        const funFactButton = document.getElementById('fun-fact-button');
        const tootFact = document.getElementById('toot-fact');
        const funFacts = [
            "Did you know? The average person toots 14 times a day!",
            "Fun Fact: Tooting helps relieve pressure and keeps your intestines healthy!",
            "Here's a fact: Some foods, like beans, are famous for making you toot!",
            "Guess what? Toots are mostly made of nitrogen and hydrogen!",
            "Believe it or not, toots can travel at speeds of 10 feet per second!"
        ];

        funFactButton.addEventListener('click', () => {
            const randomFact = funFacts[Math.floor(Math.random() * funFacts.length)];
            tootFact.textContent = randomFact;
        });
    </script>
</body>
</html>
