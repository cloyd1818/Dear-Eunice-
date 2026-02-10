        <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For Eunice - Will You Be My Valentine? 💖</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #ffafcc 0%, #ff758f 50%, #ff477e 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            position: relative;
            padding: 20px;
        }

        .container {
            max-width: 800px;
            width: 100%;
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 25px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            padding: 40px;
            text-align: center;
            position: relative;
            z-index: 10;
            animation: fadeIn 1s ease-out;
            border: 3px solid #ff758f;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h1 {
            color: #ff477e;
            font-size: 3rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
        }

        .name-highlight {
            color: #ff2e63;
            font-weight: 800;
            text-decoration: underline;
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { text-shadow: 0 0 5px #ffafcc, 0 0 10px #ffafcc; }
            to { text-shadow: 0 0 10px #ff477e, 0 0 20px #ff477e, 0 0 30px #ff477e; }
        }

        .subtitle {
            color: #ff758f;
            font-size: 1.5rem;
            margin-bottom: 30px;
            font-weight: 500;
        }

        .question {
            color: #ff2e63;
            font-size: 2.5rem;
            margin: 40px 0;
            font-weight: 700;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        .buttons-container {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin: 50px 0;
            flex-wrap: wrap;
        }

        .button {
            padding: 18px 40px;
            font-size: 1.8rem;
            font-weight: 700;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
            position: relative;
            overflow: hidden;
            z-index: 5;
            min-width: 180px;
        }

        .yes-button {
            background: linear-gradient(135deg, #ff758f 0%, #ff477e 100%);
            color: white;
        }

        .yes-button:hover {
            transform: scale(1.1);
            box-shadow: 0 12px 25px rgba(255, 71, 126, 0.4);
        }

        .no-button {
            background: linear-gradient(135deg, #c4c4c4 0%, #a0a0a0 100%);
            color: white;
            position: relative;
            transition: all 0.3s ease;
        }

        .no-button:hover {
            transform: scale(0.9);
        }

        .message {
            font-size: 1.5rem;
            color: #ff477e;
            margin-top: 30px;
            min-height: 60px;
            font-weight: 600;
            transition: all 0.5s ease;
        }

        .hearts-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .heart {
            position: absolute;
            color: rgba(255, 71, 126, 0.7);
            font-size: 24px;
            animation: float 6s ease-in-out infinite;
            user-select: none;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(10deg); }
        }

        .result {
            display: none;
            margin-top: 40px;
            animation: fadeIn 1s ease-out;
        }

        .result h2 {
            color: #ff477e;
            font-size: 3rem;
            margin-bottom: 20px;
        }

        .result p {
            font-size: 1.8rem;
            color: #ff758f;
            margin-bottom: 30px;
        }

        .result-image {
            font-size: 8rem;
            color: #ff477e;
            margin: 30px 0;
            animation: bounce 1s infinite alternate;
        }

        @keyframes bounce {
            from { transform: translateY(0); }
            to { transform: translateY(-20px); }
        }

        .footer {
            margin-top: 40px;
            color: #ff758f;
            font-size: 1.2rem;
        }

        .confetti {
            position: absolute;
            width: 15px;
            height: 15px;
            background-color: #ff477e;
            top: 0;
            opacity: 0;
        }

        .personal-note {
            background: rgba(255, 175, 204, 0.2);
            border-radius: 15px;
            padding: 20px;
            margin: 30px 0;
            border-left: 5px solid #ff477e;
            text-align: left;
        }

        .personal-note p {
            color: #ff2e63;
            font-size: 1.3rem;
            line-height: 1.6;
            margin-bottom: 10px;
        }

        @media (max-width: 768px) {
            .container {
                padding: 25px;
            }
            
            h1 {
                font-size: 2.2rem;
            }
            
            .question {
                font-size: 2rem;
            }
            
            .button {
                padding: 15px 30px;
                font-size: 1.5rem;
                min-width: 140px;
            }
            
            .buttons-container {
                gap: 20px;
            }
            
            .personal-note p {
                font-size: 1.1rem;
            }
        }

        @media (max-width: 480px) {
            h1 {
                font-size: 1.8rem;
            }
            
            .question {
                font-size: 1.6rem;
            }
            
            .button {
                padding: 12px 25px;
                font-size: 1.3rem;
                min-width: 120px;
            }
            
            .buttons-container {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="hearts-container" id="heartsContainer"></div>
    
    <div class="container">
        <h1>Happy Valentine's Day, <span class="name-highlight">Eunice</span>! 💝</h1>
        <p class="subtitle">You make every day brighter, and today I have a special question for you...</p>
        
        <div class="personal-note">
            <p>Dear Eunice,</p>
            <p>From the moment I met you, you've brought so much joy and light into my life. Your smile brightens my day, your laughter is music to my ears, and your presence makes everything better.</p>
            <p>Today, on this special day of love, I want to ask you something very important...</p>
        </div>
        
        <div class="question">Eunice, will you be my Valentine? 💌</div>
        
        <div class="buttons-container">
            <button class="button yes-button" id="yesButton">YES! 💕</button>
            <button class="button no-button" id="noButton">No ❤️</button>
        </div>
        
        <div class="message" id="message"></div>
        
        <div class="result" id="result">
            <h2>You've Made Me So Happy! 🥰</h2>
            <div class="result-image">💖🎉💕</div>
            <p>Thank you for saying YES, Eunice! ❤️</p>
            <p>I'm so excited to be your Valentine! Let's make this day unforgettable!</p>
            <p>You mean the world to me! 💝</p>
        </div>
        
        <div class="footer">
            Made with <i class="fas fa-heart" style="color:#ff477e;"></i> especially for Eunice
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Create floating hearts
            const heartsContainer = document.getElementById('heartsContainer');
            const heartCount = 35;
            
            for (let i = 0; i < heartCount; i++) {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.innerHTML = '❤️';
                heart.style.left = `${Math.random() * 100}%`;
                heart.style.top = `${Math.random() * 100}%`;
                heart.style.fontSize = `${Math.random() * 20 + 20}px`;
                heart.style.animationDuration = `${Math.random() * 4 + 4}s`;
                heart.style.animationDelay = `${Math.random() * 2}s`;
                heart.style.opacity = `${Math.random() * 0.5 + 0.3}`;
                heartsContainer.appendChild(heart);
            }
            
            // No button texts - personalized for Eunice
            const noTexts = [
                "No ❤️",
                "Are you sure, Eunice? 😢",
                "Really sure? 🤔",
                "Think again! 💡",
                "Pls say yes? 😞",
                "Don't do this 🚫",
                "I'll be so sad 😭",
                "Pretty please? 😍",
                "Just say yes! 😊",
                "You're breaking my heart 😭",
                "I'll cry... 😭",
                "Okay fine... YES! 🥺"
            ];
            
            // DOM elements
            const yesButton = document.getElementById('yesButton');
            const noButton = document.getElementById('noButton');
            const message = document.getElementById('message');
            const result = document.getElementById('result');
            
            let noIndex = 0;
            let answered = false;
            
            // Handle YES button click
            yesButton.addEventListener('click', function() {
                if (answered) return;
                
                answered = true;
                message.textContent = "Yay! You've made me the happiest person, Eunice! 🥰💖";
                message.style.color = "#ff477e";
                message.style.fontSize = "2rem";
                
                // Show result
                result.style.display = "block";
                
                // Create confetti
                createConfetti();
                
                // Hide buttons
                yesButton.style.display = "none";
                noButton.style.display = "none";
                
                // Change all Eunice mentions in result to glowing
                const euniceElements = document.querySelectorAll('.result p, .result h2');
                euniceElements.forEach(el => {
                    el.innerHTML = el.innerHTML.replace(/Eunice/g, '<span class="name-highlight">Eunice</span>');
                });
            });
            
            // Handle NO button interactions
            noButton.addEventListener('click', handleNoClick);
            noButton.addEventListener('mouseenter', handleNoHover);
            noButton.addEventListener('touchstart', handleNoHover);
            
            function handleNoClick() {
                if (answered) return;
                
                const nextIndex = noIndex + 1;
                
                if (nextIndex >= noTexts.length) {
                    // If we've gone through all texts, trigger YES
                    yesButton.click();
                    return;
                }
                
                noIndex = nextIndex;
                noButton.textContent = noTexts[noIndex];
                
                // Personalized messages for Eunice
                const euniceMessages = [
                    "Eunice, are you really sure about that? 🤔",
                    "Eunice, my heart is breaking a little... 💔",
                    "Eunice, please reconsider! I'll be so sad without you! 😭",
                    "Eunice, I'm getting desperate here... 🥺",
                    "Eunice, you know we're perfect together! 💖",
                    "Eunice, I'll do anything for you! 🌹",
                    "Eunice, you're the best thing in my life! ✨",
                    "Eunice, please don't make me beg... 🙏",
                    "Eunice, I can't imagine Valentine's without you! 😢",
                    "Eunice, just say yes already! 💕",
                    "Eunice, you win! But say YES anyway! 😄"
                ];
                
                // Update message with personalized text
                const messageIndex = Math.min(noIndex, euniceMessages.length - 1);
                message.textContent = euniceMessages[messageIndex];
                
                // Move button to random position
                moveNoButton();
            }
            
            function handleNoHover() {
                if (answered) return;
                
                // Move button away from cursor on hover
                moveNoButton();
            }
            
            function moveNoButton() {
                if (answered) return;
                
                const buttonWidth = noButton.offsetWidth;
                const buttonHeight = noButton.offsetHeight;
                
                // Calculate max positions to keep button fully visible
                const maxX = window.innerWidth - buttonWidth - 20;
                const maxY = window.innerHeight - buttonHeight - 20;
                
                // Generate random position
                const randomX = Math.random() * maxX;
                const randomY = Math.random() * maxY;
                
                // Apply new position with smooth transition
                noButton.style.position = "fixed";
                noButton.style.left = `${randomX}px`;
                noButton.style.top = `${randomY}px`;
                noButton.style.transition = "all 0.5s ease";
                
                // Make button smaller as user continues to click no
                const scale = 1 - (noIndex * 0.05);
                noButton.style.transform = `scale(${scale})`;
                
                // Change button color based on desperation level
                if (noIndex > 5) {
                    noButton.style.background = "linear-gradient(135deg, #ffafcc 0%, #ff758f 100%)";
                    noButton.style.color = "white";
                }
                
                // Add Eunice's name to button when desperate
                if (noIndex > 8) {
                    noButton.textContent = `Eunice, ${noTexts[noIndex]}`;
                }
            }
            
            function createConfetti() {
                const colors = ['#ff477e', '#ff758f', '#ffafcc', '#ff2e63', '#ff1493'];
                
                for (let i = 0; i < 200; i++) {
                    const confetti = document.createElement('div');
                    confetti.className = 'confetti';
                    confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
                    confetti.style.left = `${Math.random() * 100}%`;
                    confetti.style.width = `${Math.random() * 10 + 5}px`;
                    confetti.style.height = `${Math.random() * 10 + 5}px`;
                    confetti.style.borderRadius = Math.random() > 0.5 ? '50%' : '0';
                    
                    document.body.appendChild(confetti);
                    
                    // Animate confetti
                    const animation = confetti.animate([
                        { top: '0px', opacity: 1, transform: 'rotate(0deg)' },
                        { top: `${Math.random() * 100 + 100}%`, opacity: 0.7, transform: `rotate(${Math.random() * 720}deg)` }
                    ], {
                        duration: Math.random() * 2000 + 1000,
                        easing: 'cubic-bezier(0.215, 0.61, 0.355, 1)'
                    });
                    
                    // Remove confetti after animation
                    animation.onfinish = () => {
                        confetti.remove();
                    };
                }
            }
            
            // Initial positioning of the no button
            window.addEventListener('resize', () => {
                if (!answered) {
                    moveNoButton();
                }
            });
            
            // Initialize the no button position
            setTimeout(() => {
                moveNoButton();
            }, 500);
            
            // Add heartbeat effect to Eunice's name
            setInterval(() => {
                const nameHighlight = document.querySelector('.name-highlight');
                if (nameHighlight) {
                    nameHighlight.style.transform = nameHighlight.style.transform === 'scale(1.1)' ? 'scale(1)' : 'scale(1.1)';
                }
            }, 1000);
        });
    </script>
</body>
</html>yes-button {
            background: linear-gradient(135deg, #ff758f 0%, #ff477e 100%);
            color: white;
        }

        .yes-button:hover {
            transform: scale(1.1);
            box-shadow: 0 12px 25px rgba(255, 71, 126, 0.4);
        }

        .no-button {
            background: linear-gradient(135deg, #c4c4c4 0%, #a0a0a0 100%);
            color: white;
            position: relative;
            transition: all 0.3s ease;
        }

        .no-button:hover {
            transform: scale(0.9);
        }

        .message {
            font-size: 1.5rem;
            color: #ff477e;
            margin-top: 30px;
            min-height: 60px;
            font-weight: 600;
            transition: all 0.5s ease;
        }

        .hearts-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .heart {
            position: absolute;
            color: rgba(255, 71, 126, 0.7);
            font-size: 24px;
            animation: float 6s ease-in-out infinite;
            user-select: none;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(10deg); }
        }

        .result {
            display: none;
            margin-top: 40px;
            animation: fadeIn 1s ease-out;
        }

        .result h2 {
            color: #ff477e;
            font-size: 3rem;
            margin-bottom: 20px;
        }

        .result p {
            font-size: 1.8rem;
            color: #ff758f;
            margin-bottom: 30px;
        }

        .result-image {
            font-size: 8rem;
            color: #ff477e;
            margin: 30px 0;
            animation: bounce 1s infinite alternate;
        }

        @keyframes bounce {
            from { transform: translateY(0); }
            to { transform: translateY(-20px); }
        }

        .footer {
            margin-top: 40px;
            color: #ff758f;
            font-size: 1.2rem;
        }

        .confetti {
            position: absolute;
            width: 15px;
            height: 15px;
            background-color: #ff477e;
            top: 0;
            opacity: 0;
        }

        .personal-note {
            background: rgba(255, 175, 204, 0.2);
            border-radius: 15px;
            padding: 20px;
            margin: 30px 0;
            border-left: 5px solid #ff477e;
            text-align: left;
        }

        .personal-note p {
            color: #ff2e63;
            font-size: 1.3rem;
            line-height: 1.6;
            margin-bottom: 10px;
        }

        @media (max-width: 768px) {
            .container {
                padding: 25px;
            }
            
            h1 {
                font-size: 2.2rem;
            }
            
            .question {
                font-size: 2rem;
            }
            
            .button {
                padding: 15px 30px;
                font-size: 1.5rem;
                min-width: 140px;
            }
            
            .buttons-container {
                gap: 20px;
            }
            
            .personal-note p {
                font-size: 1.1rem;
            }
        }

        @media (max-width: 480px) {
            h1 {
                font-size: 1.8rem;
            }
            
            .question {
                font-size: 1.6rem;
            }
            
            .button {
                padding: 12px 25px;
                font-size: 1.3rem;
                min-width: 120px;
            }
            
            .buttons-container {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="hearts-container" id="heartsContainer"></div>
    
    <div class="container">
        <h1>Happy Valentine's Day, <span class="name-highlight">Eunice</span>! 💝</h1>
        <p class="subtitle">You make every day brighter, and today I have a special question for you...</p>
        
        <div class="personal-note">
            <p>Dear Eunice,</p>
            <p>From the moment I met you, you've brought so much joy and light into my life. Your smile brightens my day, your laughter is music to my ears, and your presence makes everything better.</p>
            <p>Today, on this special day of love, I want to ask you something very important...</p>
        </div>
        
        <div class="question">Eunice, will you be my Valentine? 💌</div>
        
        <div class="buttons-container">
            <button class="button yes-button" id="yesButton">YES! 💕</button>
            <button class="button no-button" id="noButton">No ❤️</button>
        </div>
        
        <div class="message" id="message"></div>
        
        <div class="result" id="result">
            <h2>You've Made Me So Happy! 🥰</h2>
            <div class="result-image">💖🎉💕</div>
            <p>Thank you for saying YES, Eunice! ❤️</p>
            <p>I'm so excited to be your Valentine! Let's make this day unforgettable!</p>
            <p>You mean the world to me! 💝</p>
        </div>
        
        <div class="footer">
            Made with <i class="fas fa-heart" style="color:#ff477e;"></i> especially for Eunice
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Create floating hearts
            const heartsContainer = document.getElementById('heartsContainer');
            const heartCount = 35;
            
            for (let i = 0; i < heartCount; i++) {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.innerHTML = '❤️';
                heart.style.left = `${Math.random() * 100}%`;
                heart.style.top = `${Math.random() * 100}%`;
                heart.style.fontSize = `${Math.random() * 20 + 20}px`;
                heart.style.animationDuration = `${Math.random() * 4 + 4}s`;
                heart.style.animationDelay = `${Math.random() * 2}s`;
                heart.style.opacity = `${Math.random() * 0.5 + 0.3}`;
                heartsContainer.appendChild(heart);
            }
            
            // No button texts - personalized for Eunice
            const noTexts = [
                "No ❤️",
                "Are you sure, Eunice? 😢",
                "Really sure? 🤔",
                "Think again! 💡",
                "Pls say yes? 😞",
                "Don't do this 🚫",
                "I'll be so sad 😭",
                "Pretty please? 😍",
                "Just say yes! 😊",
                "You're breaking my heart 😭",
                "I'll cry... 😭",
                "Okay fine... YES! 🥺"
            ];
            
            // DOM elements
            const yesButton = document.getElementById('yesButton');
            const noButton = document.getElementById('noButton');
            const message = document.getElementById('message');
            const result = document.getElementById('result');
            
            let noIndex = 0;
            let answered = false;
            
            // Handle YES button click
            yesButton.addEventListener('click', function() {
                if (answered) return;
                
                answered = true;
                message.textContent = "Yay! You've made me the happiest person, Eunice! 🥰💖";
                message.style.color = "#ff477e";
                message.style.fontSize = "2rem";
                
                // Show result
                result.style.display = "block";
                
                // Create confetti
                createConfetti();
                
                // Hide buttons
                yesButton.style.display = "none";
                noButton.style.display = "none";
                
                // Change all Eunice mentions in result to glowing
                const euniceElements = document.querySelectorAll('.result p, .result h2');
                euniceElements.forEach(el => {
                    el.innerHTML = el.innerHTML.replace(/Eunice/g, '<span class="name-highlight">Eunice</span>');
                });
            });
            
            // Handle NO button interactions
            noButton.addEventListener('click', handleNoClick);
            noButton.addEventListener('mouseenter', handleNoHover);
            noButton.addEventListener('touchstart', handleNoHover);
            
            function handleNoClick() {
                if (answered) return;
                
                const nextIndex = noIndex + 1;
                
                if (nextIndex >= noTexts.length) {
                    // If we've gone through all texts, trigger YES
                    yesButton.click();
                    return;
                }
                
                noIndex = nextIndex;
                noButton.textContent = noTexts[noIndex];
                
                // Personalized messages for Eunice
                const euniceMessages = [
                    "Eunice, are you really sure about that? 🤔",
                    "Eunice, my heart is breaking a little... 💔",
                    "Eunice, please reconsider! I'll be so sad without you! 😭",
                    "Eunice, I'm getting desperate here... 🥺",
                    "Eunice, you know we're perfect together! 💖",
                    "Eunice, I'll do anything for you! 🌹",
                    "Eunice, you're the best thing in my life! ✨",
                    "Eunice, please don't make me beg... 🙏",
                    "Eunice, I can't imagine Valentine's without you! 😢",
                    "Eunice, just say yes already! 💕",
                    "Eunice, you win! But say YES anyway! 😄"
                ];
                
                // Update message with personalized text
                const messageIndex = Math.min(noIndex, euniceMessages.length - 1);
                message.textContent = euniceMessages[messageIndex];
                
                // Move button to random position
                moveNoButton();
            }
            
            function handleNoHover() {
                if (answered) return;
                
                // Move button away from cursor on hover
                moveNoButton();
            }
            
            function moveNoButton() {
                if (answered) return;
                
                const buttonWidth = noButton.offsetWidth;
                const buttonHeight = noButton.offsetHeight;
                
                // Calculate max positions to keep button fully visible
                const maxX = window.innerWidth - buttonWidth - 20;
                const maxY = window.innerHeight - buttonHeight - 20;
                
                // Generate random position
                const randomX = Math.random() * maxX;
                const randomY = Math.random() * maxY;
                
                // Apply new position with smooth transition
                noButton.style.position = "fixed";
                noButton.style.left = `${randomX}px`;
                noButton.style.top = `${randomY}px`;
                noButton.style.transition = "all 0.5s ease";
                
                // Make button smaller as user continues to click no
                const scale = 1 - (noIndex * 0.05);
                noButton.style.transform = `scale(${scale})`;
                
                // Change button color based on desperation level
                if (noIndex > 5) {
                    noButton.style.background = "linear-gradient(135deg, #ffafcc 0%, #ff758f 100%)";
                    noButton.style.color = "white";
                }
                
                // Add Eunice's name to button when desperate
                if (noIndex > 8) {
                    noButton.textContent = `Eunice, ${noTexts[noIndex]}`;
                }
            }
            
            function createConfetti() {
                const colors = ['#ff477e', '#ff758f', '#ffafcc', '#ff2e63', '#ff1493'];
                
                for (let i = 0; i < 200; i++) {
                    const confetti = document.createElement('div');
                    confetti.className = 'confetti';
                    confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
                    confetti.style.left = `${Math.random() * 100}%`;
                    confetti.style.width = `${Math.random() * 10 + 5}px`;
                    confetti.style.height = `${Math.random() * 10 + 5}px`;
                    confetti.style.borderRadius = Math.random() > 0.5 ? '50%' : '0';
                    
                    document.body.appendChild(confetti);
                    
                    // Animate confetti
                    const animation = confetti.animate([
                        { top: '0px', opacity: 1, transform: 'rotate(0deg)' },
                        { top: `${Math.random() * 100 + 100}%`, opacity: 0.7, transform: `rotate(${Math.random() * 720}deg)` }
                    ], {
                        duration: Math.random() * 2000 + 1000,
                        easing: 'cubic-bezier(0.215, 0.61, 0.355, 1)'
                    });
                    
                    // Remove confetti after animation
                    animation.onfinish = () => {
                        confetti.remove();
                    };
                }
            }
            
            // Initial positioning of the no button
            window.addEventListener('resize', () => {
                if (!answered) {
                    moveNoButton();
                }
            });
            
            // Initialize the no button position
            setTimeout(() => {
                moveNoButton();
            }, 500);
            
            // Add heartbeat effect to Eunice's name
            setInterval(() => {
                const nameHighlight = document.querySelector('.name-highlight');
                if (nameHighlight) {
                    nameHighlight.style.transform = nameHighlight.style.transform === 'scale(1.1)' ? 'scale(1)' : 'scale(1.1)';
                }
            }, 1000);
        });
    </script>
</body>
</html>
