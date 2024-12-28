<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TootCoin - Clean and Fun</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background: #f7f9fc;
            color: #333;
        }
        header {
            background: #4a90e2;
            padding: 40px 20px;
            text-align: center;
            color: white;
        }
        header h1 {
            font-size: 3rem;
            margin: 0;
        }
        header p {
            font-size: 1.2rem;
            margin-top: 10px;
        }
        nav {
            display: flex;
            justify-content: center;
            gap: 20px;
            background: #fff;
            padding: 15px 0;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        nav a {
            color: #4a90e2;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #0366d6;
        }
        main {
            padding: 40px 20px;
        }
        .section {
            margin: 20px auto;
            max-width: 800px;
            background: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 30px;
        }
        .section h2 {
            font-size: 2rem;
            margin-bottom: 15px;
        }
        footer {
            text-align: center;
            background: #4a90e2;
            color: white;
            padding: 20px;
            margin-top: 40px;
        }
    </style>
</head>
<body>
    <header>
        <h1>TootCoin</h1>
        <p>The Cryptocurrency That’s Full of Laughs!</p>
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
        </section>
        <section id="how-it-works" class="section">
            <h2>How It Works</h2>
            <p>With every $500,000 market cap milestone, 10,000 TootCoins are burned, making your coins more valuable. Plus, every trade is a chance to share a laugh and spread joy.</p>
            <button id="toot-counter-btn" class="cta-button" style="background: #4caf50; font-size: 1.2rem; margin-top: 20px;">Make a Toot!</button>
            <p id="toot-counter" style="font-size: 1.2rem; margin-top: 10px;">Toots Made: 0</p>
            <button id="fun-facts-btn" class="cta-button" style="background: #ff5722; font-size: 1.2rem; margin-top: 20px;">Get a Fun Toot Fact!</button>
            <p id="fun-fact-display" style="font-size: 1.2rem; font-weight: bold; margin-top: 10px;">Click the button to learn something funny about tooting!</p>
        </section>
        <section id="join" class="section">
            <h2>Join Us</h2>
            <p>Be part of the TootCoin revolution today! Follow us on Twitter or join our community on Discord.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 TootCoin Inc. All rights reserved.</p>
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
