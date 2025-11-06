<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cookie.fun + Kaito Banner</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #1a1a2e;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            padding: 20px;
        }
        
        .banner-container {
            width: 100%;
            max-width: 1200px;
            overflow: hidden;
            border-radius: 12px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
        }
        
        .banner {
            position: relative;
            width: 100%;
            height: 300px;
            display: flex;
            overflow: hidden;
        }
        
        /* Bagian Kiri - Cookie.fun Style */
        .cookie-side {
            flex: 1;
            background: linear-gradient(135deg, #ff9a9e 0%, #fad0c4 100%);
            position: relative;
            padding: 20px;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        
        .cookie-bg {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            opacity: 0.7;
        }
        
        .cookie {
            position: absolute;
            width: 60px;
            height: 60px;
            background: #d4a574;
            border-radius: 50%;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        
        .cookie::before {
            content: '';
            position: absolute;
            width: 10px;
            height: 10px;
            background: #8b5a2b;
            border-radius: 50%;
            top: 20px;
            left: 15px;
        }
        
        .cookie::after {
            content: '';
            position: absolute;
            width: 8px;
            height: 8px;
            background: #8b5a2b;
            border-radius: 50%;
            top: 35px;
            left: 40px;
        }
        
        .bubble {
            position: absolute;
            background: rgba(255, 255, 255, 0.7);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 20px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        
        /* Bagian Kanan - Kaito Style */
        .kaito-side {
            flex: 1;
            background: linear-gradient(135deg, #0f2027 0%, #203a43 50%, #2c5364 100%);
            position: relative;
            padding: 20px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            overflow: hidden;
        }
        
        .grid-lines {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: 
                linear-gradient(rgba(0, 255, 255, 0.1) 1px, transparent 1px),
                linear-gradient(90deg, rgba(0, 255, 255, 0.1) 1px, transparent 1px);
            background-size: 20px 20px;
        }
        
        .neon-circle {
            position: absolute;
            width: 100px;
            height: 100px;
            border: 2px solid rgba(0, 255, 255, 0.5);
            border-radius: 50%;
            box-shadow: 0 0 10px rgba(0, 255, 255, 0.7);
        }
        
        .neon-line {
            position: absolute;
            height: 2px;
            background: rgba(0, 255, 255, 0.7);
            box-shadow: 0 0 5px rgba(0, 255, 255, 0.7);
        }
        
        /* Bagian Tengah - Teks Utama */
        .center-text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            z-index: 10;
            width: 80%;
        }
        
        .main-title {
            font-size: 48px;
            font-weight: 800;
            background: linear-gradient(to right, #ff0000, #ff8000, #ffff00, #00ff00, #00ffff, #0000ff, #8000ff);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 10px;
            text-shadow: 0 0 15px rgba(255, 255, 255, 0.3);
            letter-spacing: 1px;
        }
        
        .subtitle {
            font-size: 22px;
            color: white;
            margin-bottom: 8px;
            font-weight: 600;
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
        }
        
        .tagline {
            font-size: 16px;
            color: rgba(255, 255, 255, 0.8);
            font-style: italic;
            text-shadow: 0 0 5px rgba(255, 255, 255, 0.3);
        }
        
        /* Efek Cahaya Web3 */
        .web3-glow {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at center, rgba(123, 104, 238, 0.2) 0%, transparent 70%);
            pointer-events: none;
        }
        
        /* Animasi */
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        @keyframes glow {
            0%, 100% { opacity: 0.5; }
            50% { opacity: 1; }
        }
        
        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        .cookie, .bubble {
            animation: float 4s ease-in-out infinite;
        }
        
        .neon-circle, .neon-line {
            animation: glow 3s ease-in-out infinite alternate;
        }
    </style>
</head>
<body>
    <div class="banner-container">
        <div class="banner">
            <!-- Bagian Kiri - Cookie.fun -->
            <div class="cookie-side">
                <div class="cookie-bg">
                    <!-- Cookie Elements -->
                    <div class="cookie" style="top: 20%; left: 15%;"></div>
                    <div class="cookie" style="top: 60%; left: 25%;"></div>
                    <div class="cookie" style="top: 40%; left: 70%;"></div>
                    
                    <!-- Bubble Elements dengan Emoji -->
                    <div class="bubble" style="width: 50px; height: 50px; top: 15%; left: 60%;">🍪</div>
                    <div class="bubble" style="width: 40px; height: 40px; top: 70%; left: 10%;">✨</div>
                    <div class="bubble" style="width: 45px; height: 45px; top: 30%; left: 40%;">😊</div>
                </div>
            </div>
            
            <!-- Bagian Kanan - Kaito -->
            <div class="kaito-side">
                <div class="grid-lines"></div>
                <div class="neon-circle" style="top: 10%; left: 20%;"></div>
                <div class="neon-circle" style="bottom: 15%; right: 25%; width: 70px; height: 70px;"></div>
                <div class="neon-line" style="top: 40%; left: 10%; width: 80%;"></div>
                <div class="neon-line" style="top: 70%; left: 5%; width: 70%;"></div>
            </div>
            
            <!-- Teks Utama di Tengah -->
            <div class="center-text">
                <div class="main-title">peng || Web3</div>
                <div class="subtitle">Kaito Yapping • Cookie.fun Yapping</div>
                <div class="tagline">Turning noise into alpha</div>
            </div>
            
            <!-- Efek Cahaya Web3 -->
            <div class="web3-glow"></div>
        </div>
    </div>

    <script>
        // Menambahkan elemen dinamis untuk efek yang lebih hidup
        document.addEventListener('DOMContentLoaded', function() {
            const cookieSide = document.querySelector('.cookie-side');
            const kaitoSide = document.querySelector('.kaito-side');
            
            // Tambahkan lebih banyak elemen cookie
            for (let i = 0; i < 5; i++) {
                const cookie = document.createElement('div');
                cookie.className = 'cookie';
                cookie.style.top = `${Math.random() * 80 + 10}%`;
                cookie.style.left = `${Math.random() * 80 + 10}%`;
                cookie.style.animationDelay = `${Math.random() * 2}s`;
                cookieSide.querySelector('.cookie-bg').appendChild(cookie);
            }
            
            // Tambahkan lebih banyak bubble dengan emoji acak
            const emojis = ['🍪', '✨', '🌟', '😊', '🚀', '🌈', '⭐', '💫'];
            for (let i = 0; i < 4; i++) {
                const bubble = document.createElement('div');
                bubble.className = 'bubble';
                const size = Math.random() * 20 + 30;
                bubble.style.width = `${size}px`;
                bubble.style.height = `${size}px`;
                bubble.style.top = `${Math.random() * 80 + 10}%`;
                bubble.style.left = `${Math.random() * 80 + 10}%`;
                bubble.style.animationDelay = `${Math.random() * 2}s`;
                bubble.textContent = emojis[Math.floor(Math.random() * emojis.length)];
                cookieSide.querySelector('.cookie-bg').appendChild(bubble);
            }
            
            // Tambahkan lebih banyak elemen neon
            for (let i = 0; i < 3; i++) {
                const neonLine = document.createElement('div');
                neonLine.className = 'neon-line';
                neonLine.style.top = `${Math.random() * 80 + 10}%`;
                neonLine.style.left = `${Math.random() * 20}%`;
                neonLine.style.width = `${Math.random() * 50 + 30}%`;
                neonLine.style.animationDelay = `${Math.random() * 2}s`;
                kaitoSide.appendChild(neonLine);
            }
        });
    </script>
</body>
</html>
