<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy 19th Birthday Soha! 💕</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;500;600;700&family=Poppins:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .dancing-script {
            font-family: 'Dancing Script', cursive;
        }
        
        /* Floating hearts animation */
        .heart {
            position: fixed;
            color: #ff69b4;
            font-size: 20px;
            animation: float 6s ease-in-out infinite;
            pointer-events: none;
            z-index: 1000;
        }
        
        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        /* Sparkle animation */
        .sparkle {
            position: fixed;
            color: #ffd700;
            font-size: 16px;
            animation: sparkle 3s ease-in-out infinite;
            pointer-events: none;
            z-index: 1000;
        }
        
        @keyframes sparkle {
            0%, 100% { opacity: 0; transform: scale(0); }
            50% { opacity: 1; transform: scale(1); }
        }
        
        /* Pulse animation for main title */
        .pulse-love {
            animation: pulse-love 2s ease-in-out infinite;
        }
        
        @keyframes pulse-love {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }
        
        /* Gradient text */
        .gradient-text {
            background: linear-gradient(45deg, #ff69b4, #ff1493, #dc143c);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        /* Card hover effects */
        .memory-card {
            transition: all 0.3s ease;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .memory-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
            background: rgba(255, 255, 255, 0.2);
        }
        
        /* Countdown styles */
        .countdown-item {
            background: linear-gradient(135deg, #ff69b4, #ff1493);
            border-radius: 15px;
            padding: 20px;
            margin: 10px;
            text-align: center;
            color: white;
            box-shadow: 0 8px 25px rgba(255, 105, 180, 0.3);
            animation: bounce 2s ease-in-out infinite;
        }
        
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-10px); }
            60% { transform: translateY(-5px); }
        }
        
        /* Button animations */
        .love-button {
            background: linear-gradient(45deg, #ff69b4, #ff1493);
            border: none;
            color: white;
            padding: 15px 30px;
            border-radius: 50px;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 8px 25px rgba(255, 105, 180, 0.3);
        }
        
        .love-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 35px rgba(255, 105, 180, 0.4);
        }
        
        /* Photo gallery styles */
        .photo-container {
            position: relative;
            overflow: hidden;
            border-radius: 20px;
            transition: all 0.3s ease;
        }
        
        .photo-container:hover {
            transform: scale(1.05);
        }
        
        .photo-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(45deg, rgba(255, 105, 180, 0.8), rgba(255, 20, 147, 0.8));
            opacity: 0;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 600;
        }
        
        .photo-container:hover .photo-overlay {
            opacity: 1;
        }
        
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 10px;
        }
        
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        
        ::-webkit-scrollbar-thumb {
            background: linear-gradient(45deg, #ff69b4, #ff1493);
            border-radius: 10px;
        }
        
        ::-webkit-scrollbar-thumb:hover {
            background: linear-gradient(45deg, #ff1493, #dc143c);
        }
        
        /* Message popup styles */
        .message-popup {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%) scale(0);
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            z-index: 2000;
            text-align: center;
            transition: all 0.3s ease;
            max-width: 90%;
            width: 400px;
        }
        
        .message-popup.show {
            transform: translate(-50%, -50%) scale(1);
        }
        
        .popup-overlay {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.5);
            z-index: 1999;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }
        
        .popup-overlay.show {
            opacity: 1;
            visibility: visible;
        }
    </style>
</head>
<body>
    <!-- Floating hearts and sparkles will be added by JavaScript -->
    
    <!-- Hero Section -->
    <section class="min-h-screen flex items-center justify-center text-center px-4 relative">
        <div class="max-w-4xl mx-auto">
            <div class="mb-8">
                <h1 class="text-6xl md:text-8xl font-bold dancing-script gradient-text pulse-love mb-4">
                    Happy Birthday!
                </h1>
                <h2 class="text-4xl md:text-6xl font-bold text-white mb-6 dancing-script">
                    Sweet Soha
                </h2>
                <div class="text-2xl md:text-3xl text-pink-200 mb-8">
                    <i class="fas fa-heart text-pink-400"></i>
                    Turning 19 on October 12, 2025
                    <i class="fas fa-heart text-pink-400"></i>
                </div>
            </div>
            
            <!-- Countdown Timer -->
            <div class="flex flex-wrap justify-center mb-12" id="countdown">
                <div class="countdown-item">
                    <div class="text-3xl font-bold" id="days">0</div>
                    <div class="text-sm">Days</div>
                </div>
                <div class="countdown-item">
                    <div class="text-3xl font-bold" id="hours">0</div>
                    <div class="text-sm">Hours</div>
                </div>
                <div class="countdown-item">
                    <div class="text-3xl font-bold" id="minutes">0</div>
                    <div class="text-sm">Minutes</div>
                </div>
                <div class="countdown-item">
                    <div class="text-3xl font-bold" id="seconds">0</div>
                    <div class="text-sm">Seconds</div>
                </div>
            </div>
            
            <button class="love-button" onclick="showLoveMessage()">
                <i class="fas fa-heart"></i> Click for a Special Message <i class="fas fa-heart"></i>
            </button>
        </div>
    </section>
    
    <!-- Photo Gallery Section -->
    <section class="py-20 px-4">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-5xl font-bold text-center text-white dancing-script mb-16">
                <i class="fas fa-camera text-pink-400"></i>
                Beautiful Memories
                <i class="fas fa-camera text-pink-400"></i>
            </h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="photo-container">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/dbe72746-998b-42db-8f13-0f7f017605e9.png" alt="Beautiful young woman with flowing dark hair smiling warmly in golden hour sunlight with soft bokeh background" class="w-full h-64 object-cover rounded-20">
                    <div class="photo-overlay">
                        <span>Your Beautiful Smile</span>
                    </div>
                </div>
                
                <div class="photo-container">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/ea2307c6-22dd-4aac-ba53-1f5ecb54afd3.png" alt="Romantic couple holding hands walking on a beach at sunset with pink and orange sky reflecting on water" class="w-full h-64 object-cover rounded-20">
                    <div class="photo-overlay">
                        <span>Our Perfect Moments</span>
                    </div>
                </div>
                
                <div class="photo-container">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/dade7e0a-3a11-45fe-90c3-568e353d54ac.png" alt="Elegant birthday cake with 19 candles glowing in a dark room with pink and purple decorations" class="w-full h-64 object-cover rounded-20">
                    <div class="photo-overlay">
                        <span>Birthday Dreams</span>
                    </div>
                </div>
                
                <div class="photo-container">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/778f0ddd-0fa3-4ba9-896d-5aebf2b5ef9f.png" alt="Pink roses bouquet with soft lighting and romantic atmosphere on vintage wooden table" class="w-full h-64 object-cover rounded-20">
                    <div class="photo-overlay">
                        <span>Flowers for You</span>
                    </div>
                </div>
                
                <div class="photo-container">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/7631b522-d174-4674-b6d5-2f3b656c98c4.png" alt="Cozy coffee date setup with two cups heart-shaped foam art and fairy lights in background" class="w-full h-64 object-cover rounded-20">
                    <div class="photo-overlay">
                        <span>Coffee Dates</span>
                    </div>
                </div>
                
                <div class="photo-container">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/70954519-8939-4f5e-bfe6-f288ca79e9a8.png" alt="Night sky filled with stars and shooting star over silhouette of couple sitting together" class="w-full h-64 object-cover rounded-20">
                    <div class="photo-overlay">
                        <span>Stargazing Together</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Wishes and Memories Section -->
    <section class="py-20 px-4">
        <div class="max-w-4xl mx-auto">
            <h2 class="text-5xl font-bold text-center text-white dancing-script mb-16">
                <i class="fas fa-heart text-pink-400"></i>
                My Wishes for You
                <i class="fas fa-heart text-pink-400"></i>
            </h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="memory-card rounded-3xl p-8">
                    <div class="text-4xl text-pink-400 mb-4">
                        <i class="fas fa-star"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4">Dreams Come True</h3>
                    <p class="text-pink-100 leading-relaxed">
                        May this new year of your life bring you endless joy, success in everything you pursue, 
                        and all the happiness your beautiful heart deserves. You're incredible, Soha!
                    </p>
                </div>
                
                <div class="memory-card rounded-3xl p-8">
                    <div class="text-4xl text-pink-400 mb-4">
                        <i class="fas fa-heart"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4">Forever Young</h3>
                    <p class="text-pink-100 leading-relaxed">
                        19 looks absolutely perfect on you! May you always keep that sparkle in your eyes 
                        and that amazing spirit that makes everyone around you smile.
                    </p>
                </div>
                
                <div class="memory-card rounded-3xl p-8">
                    <div class="text-4xl text-pink-400 mb-4">
                        <i class="fas fa-gift"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4">Precious Moments</h3>
                    <p class="text-pink-100 leading-relaxed">
                        Every moment with you is a gift. Thank you for being the amazing person you are. 
                        Here's to creating many more beautiful memories together!
                    </p>
                </div>
                
                <div class="memory-card rounded-3xl p-8">
                    <div class="text-4xl text-pink-400 mb-4">
                        <i class="fas fa-infinity"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-4">Endless Love</h3>
                    <p class="text-pink-100 leading-relaxed">
                        My love for you grows stronger with each passing day. May this birthday mark 
                        the beginning of the most amazing chapter of your life!
                    </p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Interactive Birthday Cake Section -->
    <section class="py-20 px-4">
        <div class="max-w-2xl mx-auto text-center">
            <h2 class="text-5xl font-bold text-white dancing-script mb-12">
                <i class="fas fa-birthday-cake text-pink-400"></i>
                Make a Wish!
                <i class="fas fa-birthday-cake text-pink-400"></i>
            </h2>
            
            <div class="birthday-cake mb-12">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/89954f33-d9a9-43b9-92f4-f007c6de77c1.png" alt="Gorgeous three-layer birthday cake with pink frosting, 19 glowing candles, and decorated with edible flowers and gold accents" class="w-full max-w-md mx-auto rounded-3xl shadow-2xl">
            </div>
            
            <button class="love-button mb-8" onclick="blowCandles()">
                <i class="fas fa-wind"></i> Blow the Candles! <i class="fas fa-wind"></i>
            </button>
            
            <div id="wish-message" class="text-2xl text-pink-200 dancing-script hidden">
                <i class="fas fa-star text-yellow-400"></i>
                Your wish has been sent to the stars!
                <i class="fas fa-star text-yellow-400"></i>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer class="py-16 text-center">
        <div class="max-w-2xl mx-auto px-4">
            <h2 class="text-4xl font-bold text-white dancing-script mb-6">
                Happy 19th Birthday, My Love!
            </h2>
            <p class="text-xl text-pink-200 mb-8">
                October 12, 2025 - A day to celebrate the most wonderful person in my life
            </p>
            <div class="text-6xl">
                <i class="fas fa-heart text-pink-400 animate-pulse"></i>
            </div>
        </div>
    </footer>
    
    <!-- Message Popup -->
    <div class="popup-overlay" id="popupOverlay" onclick="closeLoveMessage()"></div>
    <div class="message-popup" id="messagePopup">
        <div class="text-6xl text-pink-500 mb-4">
            <i class="fas fa-heart"></i>
        </div>
        <h3 class="text-2xl font-bold text-gray-800 mb-4">For My Beautiful Soha</h3>
        <p class="text-gray-600 mb-6 leading-relaxed">
            Every day with you feels like a celebration, but today is extra special! 
            You bring so much joy, love, and light into my life. Happy 19th Birthday, 
            my amazing girlfriend! May this year be filled with all the love, 
            laughter, and dreams coming true that you deserve. I love you more than words can express!
        </p>
        <button class="love-button" onclick="closeLoveMessage()">
            <i class="fas fa-heart"></i> I Love You Too! <i class="fas fa-heart"></i>
        </button>
    </div>
    
    <script>
        // Countdown Timer
        function updateCountdown() {
            const birthday = new Date('2025-10-12T00:00:00').getTime();
            const now = new Date().getTime();
            const distance = birthday - now;
            
            if (distance > 0) {
                const days = Math.floor(distance / (1000 * 60 * 60 * 24));
                const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((distance % (1000 * 60)) / 1000);
                
                document.getElementById('days').textContent = days;
                document.getElementById('hours').textContent = hours;
                document.getElementById('minutes').textContent = minutes;
                document.getElementById('seconds').textContent = seconds;
            } else {
                document.getElementById('countdown').innerHTML = '<div class="countdown-item text-4xl">🎉 It\'s Soha\'s Birthday! 🎉</div>';
            }
        }
        
        // Update countdown every second
        setInterval(updateCountdown, 1000);
        updateCountdown();
        
        // Create floating hearts
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = (Math.random() * 3 + 3) + 's';
            document.body.appendChild(heart);
            
            setTimeout(() => {
                if (heart.parentNode) {
                    heart.parentNode.removeChild(heart);
                }
            }, 6000);
        }
        
        // Create sparkles
        function createSparkle() {
            const sparkle = document.createElement('div');
            sparkle.classList.add('sparkle');
