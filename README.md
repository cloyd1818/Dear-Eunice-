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
            padding: 15px;
        }

        .container {
            max-width: 95%;
            width: 100%;
            background-color: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
            padding: 25px;
            text-align: center;
            position: relative;
            z-index: 10;
            animation: fadeIn 0.8s ease-out;
            border: 2px solid #ff758f;
            margin: 10px;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(15px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h1 {
            color: #ff477e;
            font-size: clamp(1.8rem, 5vw, 2.5rem);
            margin-bottom: 15px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.1);
            line-height: 1.2;
        }

        .name-highlight {
            color: #ff2e63;
            font-weight: 700;
            text-decoration: underline;
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { text-shadow: 0 0 3px #ffafcc; }
            to { text-shadow: 0 0 8px #ff477e, 0 0 15px #ff477e; }
        }

        .subtitle {
            color: #ff758f;
            font-size: clamp(1rem, 3vw, 1.2rem);
            margin-bottom: 20px;
            font-weight: 500;
            line-height: 1.4;
        }

        .question {
            color: #ff2e63;
            font-size: clamp(1.5rem, 4vw, 2rem);
            margin: 25px 0;
            font-weight: 700;
            animation: pulse 2s infinite;
            line-height: 1.3;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.03); }
            100% { transform: scale(1); }
        }

        .buttons-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 35px 0;
            flex-wrap: wrap;
        }

        .button {
            padding: 14px 30px;
            font-size: clamp(1.2rem, 3vw, 1.5rem);
            font-weight: 600;
            border: none;
            border-radius: 40px;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
            z-index: 5;
            min-width: 140px;
            flex: 1;
            max-width: 200px;
        }

        .yes-button {
            background: linear-gradient(135deg, #ff758f 0%, #ff477e 100%);
            color: white;
        }

        .yes-button:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(255, 71, 126, 0.3);
        }

        .no-button {
            background: linear-gradient(135deg, #c4c4c4 0%, #a0a0a0 100%);
            color: white;
            position: relative;
            transition: all 0.3s ease;
        }

        .no-button:hover {
            transform: scale(0.95);
        }

        .message {
            font-size: clamp(1rem, 2.5vw, 1.2rem);
            color: #ff477e;
            margin-top: 20px;
            min-height: 45px;
            font-weight: 600;
            transition: all 0.5s ease;
            line-height: 1.4;
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
            color: rgba(255, 71, 126, 0.6);
            font-size: clamp(16px, 3vw, 22px);
            animation: float 6s ease-in-out infinite;
            user-select: none;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-15px) rotate(8deg); }
        }

        .result {
            display: none;
            margin-top: 30px;
            animation: fadeIn 1s ease-out;
        }

        .result h2 {
            color: #ff477e;
            font-size: clamp(1.5rem, 4vw, 2rem);
            margin-bottom: 15px;
            line-height: 1.2;
        }

        .result p {
            font-size: clamp(1rem, 2.5vw, 1.2rem);
            color: #ff758f;
            margin-bottom: 20px;
            line-height: 1.4;
        }

        .result-image {
            font-size: clamp(3rem, 8vw, 5rem);
            color: #ff477e;
            margin: 20px 0;
            animation: bounce 1s infinite alternate;
        }

        @keyframes bounce {
            from { transform: translateY(0); }
            to { transform: translateY(-10px); }
        }

        .footer {
            margin-top: 30px;
            color: #ff758f;
            font-size: 0.9rem;
        }

        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background-color: #ff477e;
            top: 0;
            opacity: 0;
        }

        .personal-note {
            background: rgba(255, 175, 204, 0.15);
            border-radius: 12px;
            padding: 15px;
            margin: 20px 0;
            border-left: 4px solid #ff477e;
            text-align: left;
        }

        .personal-note p {
            color: #ff2e63;
            font-size: clamp(0.9rem, 2.5vw, 1rem);
            line-height: 1.5;
            margin-bottom: 8px;
        }

        /* Extra small devices */
        @media (max-width: 576px) {
            .container {
                padding: 20px 15px;
                border-radius: 15px;
            }
            
            .buttons-container {
                gap: 15px;
                margin: 25px 0;
            }
            
            .button {
                padding: 12px 20px;
                min-width: 120px;
                font-size: 1.1rem;
            }
            
            .personal-note {
                padding: 12px;
                margin: 15px 0;
            }
            
            .heart {
                font-size: 18px;
            }
        }

        /* Small tablets and large phones */
        @media (min-width: 577px) and (max-width: 768px) {
            .container {
                max-width: 90%;
                padding: 30px;
            }
            
            .button {
                min-width: 150px;
            }
        }

        /* Tablets and small laptops */
        @media (min-width: 769px) and (max-width: 1024px) {
            .container {
                max-width: 85%;
                padding: 35px;
            }
        }

        /* Large screens */
        @media (min-width: 1025px) {
            .container {
                max-width: 800px;
                padding: 40px;
            }
        }

        /* Very small screens (like old phones) */
        @media (max-width: 360px) {
            .container {
                padding: 15px 10px;
                margin: 5px;
            }
            
            h1 {
                font-size: 1.5rem;
            }
            
            .question {
                font-size: 1.3rem;
            }
            
            .button {
                padding: 10px 15px;
                min-width: 100px;
                font-size: 1rem;
            }
            
            .buttons-container {
                flex-direction: column;
                align-items: center;
            }
            
            .button {
                width: 90%;
                max-width: 250px;
            }
        }

        /* Prevent text overflow on very small screens */
        .break-word {
            overflow-wrap: break-word;
            word-wrap: break-word;
            hyphens: auto;
        }
    </style>
</head>
<body>
    <div class="hearts-container" id="heartsContainer"></div>
    
    <div class="container">
        <h1 class="break-word">Happy Valentine's Day, <span class="name-highlight">Eunice</span>! 💝</h1>
        <p class="subtitle break-word">You make every day brighter, and today I have a special question for you...</p>
        
        <div class="personal-note">
            <p class="break-word">Dear Eunice,</p>
            <p class="break-word">From the moment I met you, you've brought so much joy and light into my life. Your smile brightens my day, your laughter is music to my ears, and your presence makes everything better.</p>
            <p class="break-word">Today, on this special day of love, I want to ask you something very important...</p>
        </div>
        
        <div class="question break-word">Eunice, will you be my Valentine? 💌</div>
        
        <div class="buttons-container">
            <button class="button yes-button" id="yesButton">YES! 💕</button>
            <button class="button no-button" id="noButton">No ❤️</button>
        </div>
        
        <div class="message break-word" id="message"></div>
        
        <div class="result" id="result">
            <h2 class="break-word">You've Made Me So Happy! 🥰</h2>
            <div class="result-image">💖🎉💕</div>
            <p class="break-word">Thank you for saying YES, Eunice! ❤️</p>
            <p class="break-word">I'm so excited to be your Valentine! Let's make this day unforgettable!</p>
            <p class="break-word">You mean the world to me! 💝</p>
        </div>
        
        <div class="footer break-word">
            Made with <i class="fas fa-heart" style="color:#ff477e;"></i> especially for Eunice
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Create floating hearts - fewer on mobile
            const heartsContainer = document.getElementById('heartsContainer');
            const heartCount = window.innerWidth < 768 ? 20 : 30;
            
            for (let i = 0; i < heartCount; i++) {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.innerHTML = '❤️';
                heart.style.left = `${Math.random() * 100}%`;
                heart.style.top = `${Math.random() * 100}%`;
                heart.style.fontSize = `${Math.random() * 15 + 15}px`;
                heart.style.animationDuration = `${Math.random() * 3 + 3}s`;
                heart.style.animationDelay = `${Math.random() * 2}s`;
                heart.style.opacity = `${Math.random() * 0.4 + 0.2}`;
                heartsContainer.appendChild(heart);
            }
            
            // No button texts - personalized for Eunice
            const noTexts = [
                "No ❤️",
                "Are you sure? 😢",
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
                message.style.fontSize = "clamp(1.2rem, 3vw, 1.5rem)";
                
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
                const maxX = window.innerWidth - buttonWidth - 10;
                const maxY = window.innerHeight - buttonHeight - 10;
                
                // Generate random position
                const randomX = Math.random() * maxX;
                const randomY = Math.random() * maxY;
                
                // Apply new position with smooth transition
                noButton.style.position = "fixed";
                noButton.style.left = `${randomX}px`;
                noButton.style.top = `${randomY}px`;
                noButton.style.transition = "all 0.4s ease";
                
                // Make button smaller as user continues to click no
                const scale = 1 - (noIndex * 0.04);
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
                const confettiCount = window.innerWidth < 768 ? 100 : 150;
                
                for (let i = 0; i < confettiCount; i++) {
                    const confetti = document.createElement('div');
                    confetti.className = 'confetti';
                    confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
                    confetti.style.left = `${Math.random() * 100}%`;
                    confetti.style.width = `${Math.random() * 8 + 4}px`;
                    confetti.style.height = `${Math.random() * 8 + 4}px`;
                    confetti.style.borderRadius = Math.random() > 0.5 ? '50%' : '0';
                    
                    document.body.appendChild(confetti);
                    
                    // Animate confetti
                    const animation = confetti.animate([
                        { top: '0px', opacity: 1, transform: 'rotate(0deg)' },
                        { top: `${Math.random() * 80 + 80}%`, opacity: 0.7, transform: `rotate(${Math.random() * 720}deg)` }
                    ], {
                        duration: Math.random() * 1500 + 800,
                        easing: 'cubic-bezier(0.215, 0.61, 0.355, 1)'
                    });
                    
                    // Remove confetti after animation
                    animation.onfinish = () => {
                        confetti.remove();
                    };
                }
            }
            
            // Re-position button on window resize
            window.addEventListener('resize', () => {
                if (!answered) {
                    moveNoButton();
                }
            });
            
            // Initialize the no button position
            setTimeout(() => {
                moveNoButton();
            }, 300);
            
            // Add heartbeat effect to Eunice's name
            setInterval(() => {
                const nameHighlight = document.querySelector('.name-highlight');
                if (nameHighlight) {
                    nameHighlight.style.transform = nameHighlight.style.transform === 'scale(1.05)' ? 'scale(1)' : 'scale(1.05)';
                }
            }, 1000);
            
            // Adjust for touch devices
            if ('ontouchstart' in window) {
                // Reduce animation intensity on mobile
                document.querySelectorAll('.heart').forEach(heart => {
                    heart.style.animationDuration = `${Math.random() * 4 + 4}s`;
                });
            }
        });
    </script>
</body>
</html>
