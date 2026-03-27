# Apology
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>💕 I'm Sorry 💕 - Heartfelt Apology</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 50%, #fecfef 100%);
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
        }

        /* Floating hearts animation */
        .hearts {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .heart {
            position: absolute;
            font-size: 20px;
            color: #ff69b4;
            animation: float 6s infinite linear;
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

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
            z-index: 2;
        }

        .header {
            text-align: center;
            margin-bottom: 40px;
            animation: bounceIn 1s ease-out;
        }

        @keyframes bounceIn {
            0% { transform: scale(0.3); opacity: 0; }
            50% { transform: scale(1.05); }
            70% { transform: scale(0.9); }
            100% { transform: scale(1); opacity: 1; }
        }

        .header h1 {
            font-size: 3em;
            background: linear-gradient(45deg, #ff6b9d, #c44569);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .editor {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 25px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            border: 2px solid rgba(255, 255, 255, 0.3);
        }

        .form-group {
            margin-bottom: 25px;
        }

        label {
            display: block;
            font-weight: 600;
            color: #c44569;
            margin-bottom: 8px;
            font-size: 1.1em;
        }

        input, textarea, select {
            width: 100%;
            padding: 15px 20px;
            border: 2px solid #ffe4e6;
            border-radius: 15px;
            font-size: 1.1em;
            font-family: 'Poppins', sans-serif;
            transition: all 0.3s ease;
            background: rgba(255, 255, 255, 0.9);
        }

        input:focus, textarea:focus, select:focus {
            outline: none;
            border-color: #ff6b9d;
            box-shadow: 0 0 20px rgba(255, 107, 157, 0.3);
            transform: translateY(-2px);
        }

        textarea {
            resize: vertical;
            min-height: 120px;
        }

        .theme-selector {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 15px;
            margin-top: 10px;
        }

        .theme-btn {
            height: 60px;
            border: none;
            border-radius: 15px;
            font-size: 0.9em;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .preview {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 25px;
            padding: 40px;
            margin-top: 30px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            border: 2px solid rgba(255, 255, 255, 0.3);
            animation: slideUp 0.8s ease-out;
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .apology-card {
            text-align: center;
            max-width: 500px;
            margin: 0 auto;
        }

        .apology-card h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .apology-name {
            font-size: 1.5em;
            color: #ff6b9d;
            margin-bottom: 30px;
            font-weight: 600;
        }

        .apology-message {
            font-size: 1.3em;
            line-height: 1.6;
            color: #555;
            margin-bottom: 30px;
            font-style: italic;
        }

        .love-note {
            background: linear-gradient(135deg, #ff9a9e, #fecfef);
            color: white;
            padding: 20px;
            border-radius: 20px;
            font-size: 1.2em;
            font-weight: 600;
            margin-top: 20px;
        }

        .generate-btn {
            background: linear-gradient(45deg, #ff6b9d, #c44569);
            color: white;
            border: none;
            padding: 18px 40px;
            font-size: 1.2em;
            font-weight: 600;
            border-radius: 25px;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
            margin-top: 20px;
        }

        .generate-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 30px rgba(255, 107, 157, 0.4);
        }

        .share-links {
            margin-top: 20px;
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
        }

        .share-btn {
            padding: 12px 20px;
            border: none;
            border-radius: 20px;
            color: white;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .copy-btn { background: #ff6b9d; }
        .twitter-btn { background: #1da1f2; }
        .whatsapp-btn { background: #25d366; }

        .copy-btn:hover, .twitter-btn:hover, .whatsapp-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }

        @media (max-width: 768px) {
            .header h1 { font-size: 2em; }
            .container { padding: 15px; }
        }
    </style>
</head>
<body>
    <div class="hearts" id="hearts"></div>
    
    <div class="container">
        <div class="header">
            <h1>💕 I'm Really Sorry 💕</h1>
            <p>Create a heartfelt apology they'll never forget!</p>
        </div>

        <div class="editor">
            <div class="form-group">
                <label>Recipient's Name ✨</label>
                <input type="text" id="recipientName" placeholder="e.g., My Sweetheart" value="My Love">
            </div>

            <div class="form-group">
                <label>Your Heartfelt Message 💌</label>
                <textarea id="apologyMessage" placeholder="Tell them exactly how you feel...">I'm truly sorry for hurting you. You mean the world to me and I never meant to make you feel this way. Please forgive me? I promise to be better. 💕</textarea>
            </div>

            <div class="form-group">
                <label>Love Promise 🌹</label>
                <textarea id="lovePromise" placeholder="What you'll do to make it right...">I'll listen better, communicate more openly, and cherish every moment with you. You're my everything! 💖</textarea>
            </div>

            <div class="form-group">
                <label>Theme 🎨</label>
                <div class="theme-selector">
                    <button class="theme-btn theme-pink active" data-theme="pink">🌸 Pink</button>
                    <button class="theme-btn theme-purple" data-theme="purple">💜 Purple</button>
                    <button class="theme-btn theme-blue" data-theme="blue">🌊 Blue</button>
                    <button class="theme-btn theme-green" data-theme="green">🍃 Mint</button>
                </div>
            </div>

            <button class="generate-btn" onclick="generateApology()">✨ Generate Heartfelt Apology ✨</button>
        </div>

        <div class="preview" id="preview" style="display: none;">
            <div class="apology-card" id="apologyCard">
                <!-- Preview content generated here -->
            </div>
            <div class="share-links" id="shareLinks" style="display: none;">
                <a href="#" class="share-btn copy-btn" onclick="copyLink()">📋 Copy Link</a>
                <a href="#" class="share-btn twitter-btn" id="twitterLink">🐦 Twitter</a>
                <a href="#" class="share-btn whatsapp-btn" id="whatsappLink">💬 WhatsApp</a>
            </div>
        </div>
    </div>

    <script>
        let currentTheme = 'pink';
        let apologyLink = '';

        // Theme switching
        document.querySelectorAll('.theme-btn').forEach(btn => {
            btn.addEventListener('click', function() {
                document.querySelector('.theme-btn.active').classList.remove('active');
                this.classList.add('active');
                currentTheme = this.dataset.theme;
                applyTheme(currentTheme);
            });
        });

        function applyTheme(theme) {
            const themes = {
                pink: { bg: 'linear-gradient(135deg, #ff9a9e 0%, #fecfef 50%, #fecfef 100%)', accent: '#ff6b9d' },
                purple: { bg: 'linear-gradient(135deg, #a8edea 0%, #fed6e3 50%, #fed6e3 100%)', accent: '#9b59b6' },
                blue: { bg: 'linear-gradient(135deg, #a1c4fd 0%, #c2e9fb 50%, #c2e9fb 100%)', accent: '#3498db' },
                green: { bg: 'linear-gradient(135deg, #d299c2 0%, #fef9d7 50%, #fef9d7 100%)', accent: '#27ae60' }
            };
            
            document.body.style.background = themes[theme].bg;
        }

        function generateApology() {
            const recipient = document.getElementById('recipientName').value || 'My Love';
            const message = document.getElementById('apologyMessage').value || '';
            const promise = document.getElementById('lovePromise').value || '';

            const card = document.getElementById('apologyCard');
            card.innerHTML = `
                <div class="apology-name">${recipient}</div>
                <h2>💔 I'm So Sorry 💔</h2>
                <div class="apology-message">${message}</div>
                <div class="love-note">
                    <strong>💕 My Promise to You:</strong><br>
                    ${promise}
                </div>
                <p style="margin-top: 25px; font-size: 1.1em; color: #777;">
                    Will you forgive me? 🥺💖
                </p>
            `;

            document.getElementById('preview').style.display = 'block';
            document.getElementById('shareLinks').style.display = 'flex';
            
            // Generate shareable link
            const params = new URLSearchParams({
                recipient: encodeURIComponent(recipient),
                message: encodeURIComponent(message),
                promise: encodeURIComponent(promise),
                theme: currentTheme
            });
            apologyLink = `${window.location.href.split('?')[0]}?${params.toString()}`;
            
            createHearts();
            slideUpAnimation();
        }

        function createHearts() {
            const heartsContainer = document.getElementById('hearts');
            heartsContainer.innerHTML = '';
            
            for (let i = 0; i < 10; i++) {
                setTimeout(() => {
                    const heart = document.createElement('div');
                    heart.className = 'heart';
                    heart.innerHTML = ['💕', '💖', '💗', '💓', '💞'][Math.floor(Math.random() * 5)];
                    heart.style.left = Math.random() *
