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
            background-color: #ff69b4; /* Fun hot pink */
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
            background-color: #ff1493; /* Bright pink for hover effect */
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
        <a href="#" data-tab="toot-shooter">Toot Shooter</a>
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
            <img width="779" alt="tooting burning image" src="https://github.com/user-attachments/assets/24958245-b53b-484e-8fa8-6534e3c41861" />
        </section>
        <section id="socials" class="section">
            <h2>Follow Us</h2>
            <p>Follow us on Twitter: <a href="https://x.com/tootcoins?s=21&t=leobGK6bTy7QJAK1HNhWGQ" target="_blank">@TootCoins</a></p>
            <p>Contact Address: DxproJfPzgPh3Z4YdEmXQNWFbh5atFCyZEuhkjDmpump</p>
        </section>
            <section id="toot-shooter" class="section">
            <h2>Toot Shooter Game</h2>
            <canvas id="tootCanvas" width="800" height="400" style="background-color: lightblue; border: 2px solid #00796b;"></canvas>
            <p>Use the arrow keys to move and press SPACE to toot!</p>
            <p id="toot-score">Score: 0</p>
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
            "Believe it or not, toots can travel at speeds of 10 feet per second!",
            "Elephants are known to toot loudly due to their size and diet!",
            "A toot can be silent but deadly — it's all about air turbulence!",
            "Did you know? Even astronauts toot in space!",
            "Tooting is a sign of healthy digestion!",
            "Toots can be caused by swallowing air while eating or drinking!",
            "Did you know? Some people can toot on command!",
            "Birds don't toot because they don't have the same digestive system!",
            "Fun Fact: Toots can smell differently depending on your diet!",
            "A single toot can be made up of 5-10 different gases!",
            "Humans aren’t the only mammals that toot — cows are major contributors to methane toots!",
            "Toots have been referenced in ancient humor scripts!",
            "The loudness of a toot depends on the speed and pressure of the gas!",
            "Toots can travel up to 10 feet in 1 second!",
            "Fish can toot too, often to communicate with each other!",
            "Beans contain oligosaccharides, which are notorious for causing toots!",
            "A healthy gut microbiome produces more frequent but less smelly toots!",
            "Toots are made mostly of nitrogen (59%) and carbon dioxide (21%)!",
            "Some reptiles, like snakes, toot to ward off predators!",
            "Your position while sitting or lying down can affect how loud a toot sounds!",
            "Some foods, like dairy, can cause louder toots in lactose-intolerant people!",
            "Toots were once considered a sign of good health in some ancient cultures!",
            "Guinness World Records has categories for the longest and loudest toots!",
            "Termites toot methane gas, contributing to global greenhouse effects!",
            "Tooting can be a byproduct of carbonated drinks!",
            "Chewing gum can lead to extra toots due to swallowed air!",
            "Certain medications can alter the frequency or smell of toots!",
            "Silent toots occur when the muscles around the anus are relaxed!",
            "Artificial sweeteners like sorbitol can lead to more frequent toots!",
            "Some cultures believe tooting brings good luck!",
            "Certain fish use toots as part of their mating calls!",
            "Toots are typically denser after eating fibrous foods!",
            "Dogs often toot in their sleep due to their relaxed state!",
            "Did you know? The sound of a toot comes from vibrations of the anal opening!",
            "Onions can cause both tears and toots!",
            "Toots can sometimes be used to diagnose digestive health issues!",
            "Spicy foods may increase the intensity of toots!",
            "Whales release massive underwater toots that create bubbles!",
            "The bacteria in your gut are the main producers of toots!",
            "Toots are odorless unless sulfur compounds are present!",
            "Lentils are a popular toot-triggering food!",
            "Holding in a toot doesn’t make it disappear — it just reabsorbs into your body!",
            "Yoga poses like "Wind-Relieving Pose" help release toots intentionally!",
            "People toot more while flying due to cabin pressure changes!",
            "Toots can contain traces of hydrogen sulfide, giving them a distinctive smell!",
            "You toot while sleeping, though you rarely notice!"
        ];

        funFactButton.addEventListener('click', () => {
            const randomFact = funFacts[Math.floor(Math.random() * funFacts.length)];
            tootFact.textContent = randomFact;
        });
    </script>
    <script>
        const shooterTab = document.querySelector('[data-tab="toot-shooter"]');
        const shooterSection = document.getElementById('toot-shooter');

        let canvas = document.getElementById('tootCanvas');
        let ctx = canvas.getContext('2d');
        let player = { x: canvas.width / 2, y: canvas.height - 30, width: 50, height: 20 };
        let bullets = [];
        let targets = [];
        let score = 0;
        let isGameRunning = true;

        function drawPlayer() {
            ctx.fillStyle = '#00796b';
            ctx.fillRect(player.x, player.y, player.width, player.height);
        }

        function drawBullets() {
            ctx.fillStyle = '#ff6347';
            bullets.forEach((bullet) => {
                ctx.fillRect(bullet.x, bullet.y, 5, 10);
                bullet.y -= 5;
            });
            bullets = bullets.filter((bullet) => bullet.y > 0);
        }

        function drawTargets() {
            ctx.fillStyle = '#ffa500';
            targets.forEach((target) => {
                ctx.fillRect(target.x, target.y, target.width, target.height);
                target.y += 2;
            });
            targets = targets.filter((target) => target.y < canvas.height);
        }

        function detectCollisions() {
            bullets.forEach((bullet, bIndex) => {
                targets.forEach((target, tIndex) => {
                    if (
                        bullet.x < target.x + target.width &&
                        bullet.x + 5 > target.x &&
                        bullet.y < target.y + target.height &&
                        bullet.y + 10 > target.y
                    ) {
                        bullets.splice(bIndex, 1);
                        targets.splice(tIndex, 1);
                        score += 10;
                        document.getElementById('toot-score').textContent = `Score: ${score}`;
                    }
                });
            });
        }

        function spawnTarget() {
            const target = {
                x: Math.random() * (canvas.width - 30),
                y: 0,
                width: 30,
                height: 30
            };
            targets.push(target);
        }

        function gameLoop() {
            if (!isGameRunning) return;
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            drawPlayer();
            drawBullets();
            drawTargets();
            detectCollisions();
            requestAnimationFrame(gameLoop);
        }

        document.addEventListener('keydown', (e) => {
            if (e.code === 'ArrowLeft' && player.x > 0) player.x -= 10;
            if (e.code === 'ArrowRight' && player.x < canvas.width - player.width) player.x += 10;
            if (e.code === 'Space') {
                bullets.push({ x: player.x + player.width / 2 - 2.5, y: player.y });
            }
        });

        setInterval(spawnTarget, 1000);
        gameLoop();
    </script>
</body>
</html>
