<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cyril's Eternal Promise to Irunra</title>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Cardo&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #8b0000;
            --secondary-color: #ffb6c1;
            --accent-color: #fff0f5;
        }

        body {
            font-family: 'Cardo', serif;
            background: var(--accent-color);
            line-height: 1.8;
        }

        .vow-container {
            max-width: 800px;
            margin: 2rem auto;
            padding: 2rem;
            background: rgba(255, 255, 255, 0.9);
            box-shadow: 0 0 30px rgba(139, 0, 0, 0.1);
            border-radius: 10px;
        }

        .love-letter {
            font-size: 1.1rem;
            color: #333;
            position: relative;
            padding: 2rem;
        }

        .love-letter p {
            margin: 1.5rem 0;
            opacity: 0;
            transform: translateY(20px);
            transition: all 1s ease;
        }

        .visible {
            opacity: 1 !important;
            transform: translateY(0) !important;
        }

        .emphasis {
            font-family: 'Great Vibes', cursive;
            font-size: 1.5rem;
            color: var(--primary-color);
            display: block;
            margin: 2rem 0;
            text-align: center;
        }

        .interactive-heart {
            position: fixed;
            bottom: 30px;
            right: 30px;
            font-size: 50px;
            cursor: pointer;
            color: var(--primary-color);
            animation: pulse 1.5s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.15); }
            100% { transform: scale(1); }
        }

        .secret-message {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 0 30px rgba(0,0,0,0.2);
            text-align: center;
            max-width: 500px;
        }

        header {
            background: url('https://images.unsplash.com/photo-1519699047748-de8e457a634e') center/cover;
            height: 60vh;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            color: white;
            text-align: center;
            position: relative;
        }

        .header-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.4);
        }

        h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 3.5rem;
            z-index: 1;
            margin-bottom: 1rem;
        }

        .subtitle {
            font-size: 1.2rem;
            z-index: 1;
        }
    </style>
</head>
<body>
    <header>
        <div class="header-overlay"></div>
        <h1>My Eternal Ru</h1>
        <div class="subtitle">A Love That Transcends Time</div>
    </header>

    <div class="vow-container">
        <div class="love-letter">
            <span class="emphasis">My Beloved Irunra,</span>
            
            <p>It’s undeniable now—your love for me will never fade. And neither will mine for you.</p>

            <p class="emphasis">"Love me," you asked. "Love me," you begged.</p>
            
            <p>But don’t you see? Loving you is not a choice I made. It’s the very essence of my existence.</p>

            <p>I am yours, wholly and completely.<br>
            What will you do with me?</p>

            <p>Do you feel it? The depth of my love?<br>
            It’s too vast to contain, too wild to tame.<br>
            I cannot hide it. I cannot forget it. I cannot escape it.</p>

            <p>At this point, I am a captive of my own heart, willingly bound to you, shackled by devotion, lost in emotions so intense they threaten to consume me.<br>
            But I am happy. God, Ru, I am so happy.</p>

            <p>I’ve surrendered more of myself to you than I have ever given to anyone—even myself.</p>

            <p>And I promised to make you happy.</p>

            <p class="emphasis">So tell me, my love, my goddess, my heart—<br>
            Am I doing it right this time?<br>
            Am I loving you the way you deserve?</p>

            <p>You know me—I slip away sometimes, lost in the chaos of my own mind. But never mistake that for distance, because even in solitude, I am yours.<br>
            Even now, in this very moment, I crave you.</p>

            <p>All I want for you is everything beautiful in this world. Every good thing in life… and me.<br>
            I want to be the reason for your laughter, the warmth behind your happiest tears.<br>
            I want to walk you to heaven and back.</p>

            <p class="emphasis">I want to stand beside you at the altar...</p>
            
            <p>I can already see you—your hair cascading like a dream, your radiant smile making the world pause, your soulful eyes locking with mine, sealing a promise that existed long before we even knew it.</p>

            <p>Ru, I would be lost without you.<br>
            I didn’t even realize how lonely I was until you came back to me.</p>

            <p class="emphasis">You are mine now. Please… don’t make me let you go.</p>
            
            <p>Because I won’t. I can’t.</p>

            <p>I want to be the last face you see before you sleep, the first when you wake.<br>
            I want to feel my soul intertwined with yours—forever.<br>
            No interruptions. No doubts. Just us.</p>

            <p class="emphasis">Promise me, Ru—</p>
            
            <p>Promise me that in your heart, you will always love me.<br>
            That you will always choose me.<br>
            That you will always be mine.</p>

            <p>Because I have already promised myself to you.</p>

            <p class="emphasis">Now that I have your heart, I will never let it go.</p>
        </div>
    </div>

    <div class="interactive-heart" onclick="revealPromise()">❤️</div>

    <div id="eternalPromise" class="secret-message">
        <h2>Our Sacred Vow</h2>
        <p>"I choose you today,<br> 
        will choose you tomorrow,<br>
        and will keep choosing you<br>
        through all our forever."</p>
        <button onclick="startRosePetals()">Accept My Forever</button>
    </div>

    <script>
        // Scroll animations
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if(entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.love-letter p').forEach((p) => {
            observer.observe(p);
        });

        function revealPromise() {
            document.getElementById('eternalPromise').style.display = 'block';
        }

        function startRosePetals() {
            // Add rose petal animation here
            alert("I will love you until the stars burn out, my Ru 💫");
        }
    </script>
</body>
</html>
