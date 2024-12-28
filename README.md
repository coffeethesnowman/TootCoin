<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TootCoin - A Gassy Revolution</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: url('https://github.com/user-attachments/assets/1053aa22-1dc7-4d24-8f50-00ce9cb754cc') no-repeat center center fixed; background-size: cover;
            color: #333;
            text-align: center;
        }
        header {
            background: linear-gradient(135deg, #00796b, #004d40);
            padding: 30px;
            color: #ffffff;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }
        header h1 {
            font-size: 3.5rem;
            margin: 0;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }
        .tagline {
            font-size: 1.5rem;
            margin-top: 10px;
            font-style: italic;
        }
        nav {
            margin: 20px 0;
            padding: 10px;
            background: #80cbc4;
            display: flex;
            justify-content: center;
            gap: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        nav a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: bold;
            transition: transform 0.2s, color 0.3s;
        }
        nav a:hover {
            transform: scale(1.1);
            color: #660066;
        }
        main {
            padding: 20px;
        }
        .section {
            background: white;
            padding: 30px;
            margin: 20px auto;
            max-width: 800px;
            border-radius: 15px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
        }
        .cta-button {
            background: #00897b;
            color: white;
            font-size: 1.2rem;
            padding: 15px 30px;
            margin-top: 20px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.3s, background 0.3s;
        }
        .cta-button:hover {
            transform: translateY(-5px);
            background: #00695c;
        }
        .fun-graphic {
            animation: float 3s ease-in-out infinite;
        }
        @keyframes float {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }
        footer {
            background: #ff69b4;
            color: white;
            padding: 15px;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }
    </style>
</head>
<body>
    <header>
        <img width="1048" alt="tootcoin banner" src="https://github.com/user-attachments/assets/d4033203-ebb0-4f65-bbfe-80071d54df86" style="width: 100%; max-height: 300px; object-fit: cover;">
        <h1>TootCoin</h1>
        <p class="tagline">The cryptocurrency that’s full of laughs and gas!</p>
    </header>
    <nav>
        <a href="#about">About</a>
        <a href="#how-it-works">How It Works</a>
        <a href="#join">Join Us</a>
    </nav>
    <main>
        <section id="about" class="section">
            <h2>About TootCoin</h2>
            <p>TootCoin isn’t just another cryptocurrency; it’s a revolution powered by humor and toots! Trade with fun, laugh with friends, and be part of the gassiest community around.</p>
            <img width="593" alt="tootcoin" src="https://github.com/user-attachments/assets/2b416e94-3ac8-465b-b0a5-7b13db648a8e" class="fun-graphic" style="width: 200px;">
        </section>
        <section id="how-it-works" class="section">
            <h2>How It Works</h2>
            <p>With every $500,000 market cap milestone, 10,000 TootCoins are burned, making your coins more valuable. Plus, every trade is a chance to share a laugh and spread joy.</p>
            <button class="cta-button">Learn More</button>
        
            <img width="779" alt="tooting burning image" src="https://github.com/user-attachments/assets/167cb535-c8d2-4dfa-b9b4-a947e41a2a59" style="margin-top: 20px; border-radius: 10px; max-width: 100%;">
        </section>
        <section id="join" class="section">
            <h2>Join the Fun</h2>
            <p>Ready to toot your way to the top? Follow us on Twitter or join our Discord to become part of the TootCoin family.</p>
            <p>Contact Address: DxproJfPzgPh3Z4YdEmXQNWFbh5atFCyZEuhkjDmpump</p>
            <a href="https://x.com/TOOTCOINS" class="cta-button">Follow Us</a>
        </section>
    <section id="fun-section" class="section">
            <h2>Fun Interactive Buttons</h2>
            <button id="toot-counter-btn" class="cta-button">Make a Toot!</button>
            <p id="toot-counter">Toots Made: 0</p>
            <button id="fun-facts-btn" class="cta-button">Get a Fun Toot Fact!</button>
            <p id="fun-fact-display">Click the button to learn something funny about tooting!</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 TootCoin Inc. All rights reserved. Powered by laughter and toots.</p>
    </footer>
<script>
        let tootCount = 0;
        const tootCounterBtn = document.getElementById('toot-counter-btn');
        const tootCounterDisplay = document.getElementById('toot-counter');
        tootCounterBtn.addEventListener('click', () => {
            tootCount++;
            tootCounterDisplay.textContent = `Toots Made: ${tootCount}`;
        });

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
            "Yoga poses like \"Wind-Relieving Pose\" help release toots intentionally!",
            "People toot more while flying due to cabin pressure changes!",
            "Toots can contain traces of hydrogen sulfide, giving them a distinctive smell!",
            "You toot while sleeping, though you rarely notice!"
        ];

        const funFactsBtn = document.getElementById('fun-facts-btn');
        const funFactDisplay = document.getElementById('fun-fact-display');
        funFactsBtn.addEventListener('click', () => {
            const randomFact = funFacts[Math.floor(Math.random() * funFacts.length)];
            funFactDisplay.textContent = randomFact;
        });
    </script>
</body>
</html>
