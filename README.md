<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy 22nd Birthday Kamilya </title>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Pacifico&family=Fredoka+One&display=swap" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'Pacifico', cursive;
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
            background: #0a0015;
        }

        .space-background {
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: linear-gradient(180deg, 
                #0a0015 0%, #1a0030 20%, #2d0052 40%, 
                #1a0030 60%, #0d001a 80%, #050010 100%);
            z-index: 0;
            overflow: hidden;
        }

        .space-background::before {
            content: '';
            position: absolute;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: 
                radial-gradient(ellipse at 20% 30%, rgba(138, 43, 226, 0.15) 0%, transparent 50%),
                radial-gradient(ellipse at 80% 70%, rgba(75, 0, 130, 0.2) 0%, transparent 50%),
                radial-gradient(ellipse at 50% 50%, rgba(128, 0, 128, 0.1) 0%, transparent 60%);
            animation: nebulaShift 20s ease-in-out infinite;
        }

        @keyframes nebulaShift {
            0%, 100% { opacity: 0.7; transform: scale(1); }
            50% { opacity: 1; transform: scale(1.1); }
        }

        .star {
            position: absolute;
            background: white;
            border-radius: 50%;
            animation: twinkle 3s ease-in-out infinite;
        }

        @keyframes twinkle {
            0%, 100% { opacity: 0.3; transform: scale(1); }
            50% { opacity: 1; transform: scale(1.3); }
        }

        .kamilya-name {
            position: absolute;
            font-family: 'Great Vibes', cursive;
            color: rgba(155, 89, 182, 0.25);
            text-shadow: 0 0 10px rgba(155, 89, 182, 0.3);
            pointer-events: none;
            animation: nameFloat 8s ease-in-out infinite;
            white-space: nowrap;
        }

        @keyframes nameFloat {
            0%, 100% { transform: translateY(0) rotate(0deg); opacity: 0.25; }
            50% { transform: translateY(-20px) rotate(5deg); opacity: 0.4; }
        }

        .planet {
            position: absolute;
            border-radius: 50%;
            pointer-events: none;
            animation: planetFloat 15s ease-in-out infinite;
        }

        @keyframes planetFloat {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-30px) rotate(10deg); }
        }

        .planet-purple {
            background: radial-gradient(circle at 30% 30%, #d8b4fe 0%, #a855f7 30%, #7c3aed 60%, #4c1d95 100%);
            box-shadow: 0 0 30px rgba(168, 85, 247, 0.6), 0 0 60px rgba(168, 85, 247, 0.3), inset -10px -10px 20px rgba(0, 0, 0, 0.5);
        }

        .planet-blue {
            background: radial-gradient(circle at 30% 30%, #93c5fd 0%, #3b82f6 30%, #1d4ed8 60%, #1e3a8a 100%);
            box-shadow: 0 0 30px rgba(59, 130, 246, 0.6), 0 0 60px rgba(59, 130, 246, 0.3), inset -10px -10px 20px rgba(0, 0, 0, 0.5);
        }

        .planet-red {
            background: radial-gradient(circle at 30% 30%, #fca5a5 0%, #ef4444 30%, #dc2626 60%, #7f1d1d 100%);
            box-shadow: 0 0 30px rgba(239, 68, 68, 0.6), 0 0 60px rgba(239, 68, 68, 0.3), inset -10px -10px 20px rgba(0, 0, 0, 0.5);
        }

        .planet-ring {
            position: absolute;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%) rotateX(75deg);
            width: 160%; height: 160%;
            border: 3px solid rgba(255, 255, 255, 0.3);
            border-radius: 50%;
            pointer-events: none;
        }

        .container {
            position: relative;
            z-index: 10;
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        .main-title {
            text-align: center;
            margin-bottom: 40px;
            background: rgba(0, 0, 0, 0.5);
            padding: 30px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 3px solid rgba(255, 215, 0, 0.6);
        }

        .main-title h1 {
            font-family: 'Fredoka One', cursive;
            font-size: 5.5em;
            background: linear-gradient(135deg, #ffd700 0%, #ff69b4 25%, #9b59b6 50%, #00d2ff 75%, #ffd700 100%);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: rainbowText 5s ease infinite, bounce 2s ease-in-out infinite;
            margin-bottom: 10px;
            letter-spacing: 3px;
        }

        @keyframes rainbowText {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
        }

        .subtitle {
            color: #fff;
            font-size: 1.6em;
            margin-top: 10px;
            text-shadow: 0 0 20px rgba(255, 255, 255, 0.8);
        }

        .nickname {
            font-family: 'Fredoka One', cursive;
            color: #ffd700;
            font-size: 2.2em;
            margin-top: 15px;
            text-shadow: 0 0 20px rgba(255, 215, 0, 0.8), 0 0 40px rgba(255, 105, 180, 0.6);
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { text-shadow: 0 0 20px rgba(255, 215, 0, 0.8); }
            to { text-shadow: 0 0 40px rgba(255, 105, 180, 1), 0 0 60px rgba(255, 215, 0, 0.8); }
        }

        .age-number {
            text-align: center;
            margin: 30px 0;
            background: rgba(0, 0, 0, 0.5);
            padding: 20px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 3px solid rgba(255, 215, 0, 0.6);
        }

        .age-number span {
            font-family: 'Fredoka One', cursive;
            font-size: 9em;
            background: linear-gradient(135deg, #ffd700 0%, #ff69b4 50%, #00d2ff 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            display: inline-block;
            animation: float 3s ease-in-out infinite, rainbowText 4s ease infinite;
            filter: drop-shadow(0 0 40px rgba(255, 215, 0, 0.8));
            background-size: 300% 300%;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) rotate(-2deg); }
            50% { transform: translateY(-25px) rotate(2deg); }
        }

        .namjoon-bg {
            position: fixed;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            width: 600px; height: 800px;
            opacity: 0.08;
            z-index: 1;
            pointer-events: none;
            filter: blur(2px);
        }

        .namjoon-bg img {
            width: 100%; height: 100%;
            object-fit: cover;
            border-radius: 20px;
        }

        .calendar-section {
            margin: 60px auto;
            max-width: 400px;
            text-align: center;
            background: rgba(0, 0, 0, 0.5);
            padding: 30px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 3px solid rgba(255, 215, 0, 0.6);
        }

        .calendar-month {
            font-family: 'Great Vibes', cursive;
            font-size: 3em;
            color: #fff;
            text-shadow: 0 0 30px rgba(255, 255, 255, 0.8);
            margin-bottom: 10px;
        }

        .calendar-year {
            font-family: 'Fredoka One', cursive;
            font-size: 1.5em;
            color: #ffd700;
            margin-bottom: 20px;
            text-shadow: 0 0 20px rgba(255, 215, 0, 0.8);
        }

        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 8px;
            text-align: center;
            background: rgba(255, 255, 255, 0.15);
            padding: 20px;
            border-radius: 15px;
        }

        .calendar-day-header {
            font-size: 1em;
            color: #ffd700;
            font-weight: bold;
            padding: 8px;
            font-family: 'Fredoka One', cursive;
        }

        .calendar-day {
            font-size: 1.1em;
            color: #fff;
            padding: 10px;
            border-radius: 50%;
            transition: all 0.3s ease;
            font-weight: bold;
        }

        .calendar-day.birthday {
            background: linear-gradient(135deg, #ffd700 0%, #ff69b4 100%);
            color: #fff;
            font-weight: bold;
            font-size: 1.4em;
            box-shadow: 0 0 25px rgba(255, 215, 0, 1);
            animation: birthdayPulse 1.5s ease-in-out infinite;
        }

        @keyframes birthdayPulse {
            0%, 100% { transform: scale(1); box-shadow: 0 0 25px rgba(255, 215, 0, 1); }
            50% { transform: scale(1.3); box-shadow: 0 0 35px rgba(255, 105, 180, 1); }
        }

        .calendar-day:hover:not(.birthday) {
            background: rgba(255, 215, 0, 0.4);
            transform: scale(1.2);
        }

        .asma-message {
            margin: 60px auto;
            max-width: 500px;
            text-align: center;
            padding: 50px 40px;
            background: rgba(0, 0, 0, 0.6);
            border: 4px solid rgba(255, 215, 0, 0.8);
            border-radius: 25px;
            backdrop-filter: blur(15px);
            box-shadow: 0 20px 60px rgba(255, 105, 180, 0.5), 0 0 100px rgba(255, 215, 0, 0.3);
            position: relative;
            overflow: hidden;
            cursor: pointer;
            transition: all 0.4s ease;
        }

        .asma-message::before {
            content: '';
            position: absolute;
            top: -50%; left: -50%;
            width: 200%; height: 200%;
            background: 
                radial-gradient(circle at 20% 30%, rgba(255, 105, 180, 0.4) 0%, transparent 40%),
                radial-gradient(circle at 80% 70%, rgba(255, 215, 0, 0.3) 0%, transparent 40%);
            animation: shimmer 8s ease-in-out infinite;
            z-index: 0;
        }

        @keyframes shimmer {
            0%, 100% { transform: translate(0, 0) rotate(0deg); }
            33% { transform: translate(30px, -30px) rotate(5deg); }
            66% { transform: translate(-20px, 20px) rotate(-5deg); }
        }

        .asma-message:hover {
            transform: scale(1.05) rotate(-1deg);
            box-shadow: 0 30px 80px rgba(255, 105, 180, 0.7), 0 0 120px rgba(255, 215, 0, 0.5);
        }

        .asma-text {
            font-family: 'Great Vibes', cursive;
            font-size: 3.5em;
            background: linear-gradient(135deg, #ffd700 0%, #ff69b4 50%, #fff 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            position: relative;
            z-index: 1;
            text-shadow: 0 0 40px rgba(255, 215, 0, 0.5);
            line-height: 1.4;
        }

        .asma-hearts {
            position: absolute;
            width: 100%; height: 100%;
            top: 0; left: 0;
            pointer-events: none;
            overflow: hidden;
        }

        .floating-heart {
            position: absolute;
            font-size: 2em;
            animation: heartFloat 4s ease-in-out infinite;
            opacity: 0.7;
        }

        @keyframes heartFloat {
            0%, 100% { transform: translateY(0) rotate(0deg); opacity: 0.7; }
            50% { transform: translateY(-20px) rotate(15deg); opacity: 1; }
        }

        .floating-note {
            position: absolute;
            font-size: 1.8em;
            animation: noteFloat 3s ease-in-out infinite;
            opacity: 0.6;
        }

        @keyframes noteFloat {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-15px) rotate(-15deg); }
        }

        .gallery-section { margin: 50px 0; }

        .polaroid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            padding: 20px;
        }

        .polaroid {
            background: white;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            transform: rotate(-3deg);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .polaroid:nth-child(even) { transform: rotate(3deg); }

        .polaroid:hover {
            transform: rotate(0deg) scale(1.1);
            box-shadow: 0 20px 50px rgba(255, 105, 180, 0.8);
        }

        .polaroid-img {
            width: 100%; height: 280px;
            background: linear-gradient(135deg, #ff6ec7 0%, #9b59b6 100%);
            border-radius: 5px;
            overflow: hidden;
        }

        .polaroid-img img {
            width: 100%; height: 100%;
            object-fit: cover;
        }

        .floating-elements {
            position: fixed;
            width: 100%; height: 100%;
            top: 0; left: 0;
            pointer-events: none;
            z-index: 5;
        }

        .floating-item {
            position: absolute;
            font-size: 3em;
            animation: floatAround 12s ease-in-out infinite;
            opacity: 0.85;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        @keyframes floatAround {
            0%, 100% { transform: translate(0, 0) rotate(0deg); }
            25% { transform: translate(100px, -100px) rotate(90deg); }
            50% { transform: translate(200px, 0) rotate(180deg); }
            75% { transform: translate(100px, 100px) rotate(270deg); }
        }

        .guitar {
            font-size: 2.5em;
            filter: drop-shadow(0 0 10px currentColor);
            animation: guitarGlow 2s ease-in-out infinite alternate;
        }

        @keyframes guitarGlow {
            from { filter: drop-shadow(0 0 8px currentColor); transform: scale(1); }
            to { filter: drop-shadow(0 0 15px currentColor); transform: scale(1.1); }
        }

        .guitar-red { color: #ff3333; filter: hue-rotate(0deg) drop-shadow(0 0 12px #ff3333); }
        .guitar-electric { color: #00d4ff; filter: hue-rotate(180deg) drop-shadow(0 0 15px #00d4ff); animation: electricPulse 1s ease-in-out infinite alternate; }

        @keyframes electricPulse {
            from { filter: hue-rotate(180deg) drop-shadow(0 0 10px #00d4ff); }
            to { filter: hue-rotate(200deg) drop-shadow(0 0 25px #00d4ff) brightness(1.3); }
        }

        .guitar-acoustic { color: #d4a574; filter: drop-shadow(0 0 10px #d4a574); }
        .guitar-bass { color: #2c2c2c; filter: drop-shadow(0 0 10px #666); }
        .guitar-pink { color: #ff69b4; filter: hue-rotate(300deg) drop-shadow(0 0 12px #ff69b4); }
        .guitar-purple { color: #9b59b6; filter: hue-rotate(270deg) drop-shadow(0 0 12px #9b59b6); }
        .guitar-gold { color: #ffd700; filter: drop-shadow(0 0 15px #ffd700); animation: goldShine 1.5s ease-in-out infinite alternate; }

        @keyframes goldShine {
            from { filter: drop-shadow(0 0 10px #ffd700); }
            to { filter: drop-shadow(0 0 25px #ffd700) brightness(1.4); }
        }

        .army-bomb {
            width: 50px; height: 75px;
            position: relative;
            display: flex;
            flex-direction: column;
            align-items: center;
            animation: bombGlow 2s ease-in-out infinite alternate;
        }

        @keyframes bombGlow {
            from { filter: drop-shadow(0 0 8px rgba(100, 100, 255, 0.6)); }
            to { filter: drop-shadow(0 0 20px rgba(100, 100, 255, 1)); }
        }

        .army-bomb .ball {
            width: 45px; height: 45px;
            border-radius: 50%;
            background: radial-gradient(circle at 30% 30%, 
                rgba(255, 255, 255, 0.9) 0%, 
                rgba(200, 220, 255, 0.6) 30%, 
                rgba(100, 100, 255, 0.3) 70%, 
                rgba(50, 50, 150, 0.2) 100%);
            border: 2px solid rgba(255, 255, 255, 0.6);
            box-shadow: 0 0 20px rgba(100, 100, 255, 0.8), 0 0 40px rgba(100, 100, 255, 0.5), inset 0 0 15px rgba(100, 100, 255, 0.4);
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
        }

        .army-bomb .ball::before {
            content: '';
            position: absolute;
            top: 8px; left: 10px;
            width: 12px; height: 8px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 50%;
            transform: rotate(-30deg);
        }

        .army-bomb .bts-logo {
            width: 22px; height: 22px;
            position: relative;
            z-index: 2;
        }

        .army-bomb .bts-logo svg {
            width: 100%; height: 100%;
            filter: drop-shadow(0 0 5px #4169E1);
        }

        .army-bomb .handle {
            width: 14px; height: 25px;
            background: linear-gradient(to bottom, #444 0%, #222 50%, #111 100%);
            border-radius: 0 0 6px 6px;
            margin-top: -3px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.5);
            position: relative;
        }

        .army-bomb .handle::before {
            content: '';
            position: absolute;
            top: 3px; left: 50%;
            transform: translateX(-50%);
            width: 6px; height: 6px;
            background: #ff3333;
            border-radius: 50%;
            box-shadow: 0 0 5px #ff3333;
        }

        .music-note {
            font-size: 2em;
            color: #fff;
            text-shadow: 0 0 15px #ff69b4, 0 0 25px #9b59b6;
            animation: noteDance 2s ease-in-out infinite;
        }

        @keyframes noteDance {
            0%, 100% { transform: rotate(-10deg) scale(1); }
            50% { transform: rotate(10deg) scale(1.2); }
        }

        .purple-heart-float {
            font-size: 2.2em;
            color: #9b59b6;
            text-shadow: 0 0 15px #9b59b6;
            animation: heartBeat 1.5s ease-in-out infinite;
        }

        @keyframes heartBeat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }

        .simple-message {
            text-align: center;
            margin: 60px 0;
            padding: 40px;
            background: rgba(0, 0, 0, 0.5);
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 3px solid rgba(255, 215, 0, 0.6);
        }

        .simple-message p {
            font-family: 'Great Vibes', cursive;
            font-size: 3em;
            color: #fff;
            text-shadow: 0 0 30px rgba(255, 215, 0, 0.8);
            line-height: 1.8;
        }

        .simple-message .date {
            font-family: 'Fredoka One', cursive;
            font-size: 1.5em;
            color: #ffd700;
            margin: 20px 0;
        }

        .simple-message .birthday-text {
            font-family: 'Pacifico', cursive;
            font-size: 2em;
            color: #fff;
            margin: 20px 0;
        }

        .simple-message .kami-name {
            font-family: 'Great Vibes', cursive;
            font-size: 3.5em;
            color: #ffd700;
            text-shadow: 0 0 40px rgba(255, 215, 0, 1);
        }

        .simple-message .borahae {
            font-family: 'Fredoka One', cursive;
            font-size: 2.5em;
            color: #ff69b4;
            text-shadow: 0 0 30px rgba(255, 105, 180, 0.8);
            margin-top: 30px;
        }

        footer {
            text-align: center;
            padding: 30px;
            color: #fff;
            margin-top: 50px;
            border-top: 3px solid rgba(255, 215, 0, 0.5);
            font-family: 'Pacifico', cursive;
            background: rgba(0, 0, 0, 0.5);
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }

        footer p { font-size: 1.3em; }

        .borahae-footer {
            color: #ffd700;
            font-size: 1.8em;
            margin-top: 10px;
            text-shadow: 0 0 20px rgba(255, 215, 0, 0.8);
        }

        .moon-modal-overlay {
            display: none;
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: radial-gradient(ellipse at center, 
                rgba(10, 0, 21, 0.97) 0%, 
                rgba(5, 0, 10, 0.99) 100%);
            z-index: 1000;
            justify-content: center;
            align-items: center;
            animation: modalFadeIn 1s ease;
            overflow: hidden;
        }

        .moon-modal-overlay.active { display: flex; }

        @keyframes modalFadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .giant-moon {
            position: relative;
            width: 700px;
            height: 700px;
            border-radius: 50%;
            background: radial-gradient(circle at 35% 35%, 
                #f5f5f5 0%, 
                #d4d4d4 20%, 
                #a8a8a8 40%, 
                #7a7a7a 60%, 
                #4a4a4a 80%, 
                #2a2a2a 100%);
            box-shadow: 
                0 0 80px rgba(255, 255, 255, 0.6),
                0 0 150px rgba(200, 200, 255, 0.4),
                0 0 250px rgba(155, 89, 182, 0.3),
                inset -30px -30px 80px rgba(0, 0, 0, 0.8),
                inset 20px 20px 60px rgba(255, 255, 255, 0.3);
            animation: moonAppear 2s cubic-bezier(0.68, -0.55, 0.265, 1.55), moonGlow 4s ease-in-out infinite alternate;
            overflow: hidden;
        }

        @keyframes moonAppear {
            0% { transform: scale(0) rotate(-180deg); opacity: 0; }
            60% { transform: scale(1.1) rotate(10deg); }
            100% { transform: scale(1) rotate(0deg); opacity: 1; }
        }

        @keyframes moonGlow {
            from {
                box-shadow: 
                    0 0 80px rgba(255, 255, 255, 0.6),
                    0 0 150px rgba(200, 200, 255, 0.4),
                    0 0 250px rgba(155, 89, 182, 0.3),
                    inset -30px -30px 80px rgba(0, 0, 0, 0.8),
                    inset 20px 20px 60px rgba(255, 255, 255, 0.3);
            }
            to {
                box-shadow: 
                    0 0 100px rgba(200, 200, 255, 0.8),
                    0 0 200px rgba(155, 89, 182, 0.6),
                    0 0 300px rgba(100, 100, 255, 0.4),
                    inset -30px -30px 80px rgba(0, 0, 0, 0.8),
                    inset 20px 20px 60px rgba(255, 255, 255, 0.4);
            }
        }

        .crater {
            position: absolute;
            border-radius: 50%;
            background: radial-gradient(circle at 40% 40%, 
                rgba(0, 0, 0, 0.3) 0%, 
                rgba(0, 0, 0, 0.5) 50%, 
                rgba(0, 0, 0, 0.2) 100%);
            box-shadow: 
                inset 3px 3px 8px rgba(0, 0, 0, 0.6),
                inset -2px -2px 5px rgba(255, 255, 255, 0.1);
        }

        .crater-1 { width: 80px; height: 80px; top: 15%; left: 20%; }
        .crater-2 { width: 50px; height: 50px; top: 60%; left: 15%; }
        .crater-3 { width: 100px; height: 100px; top: 25%; right: 15%; }
        .crater-4 { width: 60px; height: 60px; bottom: 20%; right: 25%; }
        .crater-5 { width: 40px; height: 40px; top: 50%; left: 45%; }
        .crater-6 { width: 70px; height: 70px; bottom: 30%; left: 30%; }
        .crater-7 { width: 35px; height: 35px; top: 10%; left: 55%; }
        .crater-8 { width: 45px; height: 45px; bottom: 15%; right: 15%; }

        .moon-content {
            position: absolute;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            width: 80%; height: 80%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 40px;
            text-align: center;
            z-index: 10;
            overflow-y: auto;
        }

        .moon-content::-webkit-scrollbar { width: 6px; }
        .moon-content::-webkit-scrollbar-track { background: rgba(0, 0, 0, 0.3); border-radius: 10px; }
        .moon-content::-webkit-scrollbar-thumb { background: rgba(255, 255, 255, 0.3); border-radius: 10px; }

        .moon-title {
            font-family: 'Great Vibes', cursive;
            font-size: 3.5em;
            color: #e0e0e0;
            text-shadow: 
                0 0 10px rgba(255, 255, 255, 0.8),
                0 0 20px rgba(200, 200, 255, 0.6),
                0 0 30px rgba(155, 89, 182, 0.5),
                2px 2px 4px rgba(0, 0, 0, 0.8),
                -1px -1px 2px rgba(255, 255, 255, 0.3);
            margin-bottom: 20px;
            animation: titleShine 3s ease-in-out infinite;
            letter-spacing: 2px;
        }

        @keyframes titleShine {
            0%, 100% { 
                color: #e0e0e0;
                text-shadow: 
                    0 0 10px rgba(255, 255, 255, 0.8),
                    0 0 20px rgba(200, 200, 255, 0.6),
                    0 0 30px rgba(155, 89, 182, 0.5),
                    2px 2px 4px rgba(0, 0, 0, 0.8),
                    -1px -1px 2px rgba(255, 255, 255, 0.3);
            }
            50% { 
                color: #ffd700;
                text-shadow: 
                    0 0 15px rgba(255, 215, 0, 1),
                    0 0 30px rgba(255, 215, 0, 0.8),
                    0 0 45px rgba(255, 105, 180, 0.6),
                    2px 2px 4px rgba(0, 0, 0, 0.8),
                    -1px -1px 2px rgba(255, 255, 255, 0.5);
            }
        }

        .moon-body {
            color: #d0d0d0;
            font-size: 1.1em;
            line-height: 1.8;
            text-shadow: 
                1px 1px 2px rgba(0, 0, 0, 0.9),
                -1px -1px 1px rgba(255, 255, 255, 0.2),
                0 0 10px rgba(200, 200, 255, 0.3);
            margin-bottom: 15px;
            font-family: 'Pacifico', cursive;
        }

        .moon-body .kami-name {
            font-family: 'Great Vibes', cursive;
            color: #ffd700;
            font-size: 2.2em;
            text-shadow: 
                0 0 15px rgba(255, 215, 0, 1),
                0 0 30px rgba(255, 215, 0, 0.8),
                2px 2px 4px rgba(0, 0, 0, 0.9);
            display: block;
            margin: 10px 0;
        }

        .moon-body .highlight {
            color: #ffd700;
            font-weight: bold;
            font-size: 1.3em;
            font-family: 'Fredoka One', cursive;
            text-shadow: 
                0 0 15px rgba(255, 215, 0, 1),
                0 0 30px rgba(255, 215, 0, 0.8),
                2px 2px 4px rgba(0, 0, 0, 0.9);
        }

        .moon-body .date-info {
            background: rgba(0, 0, 0, 0.4);
            padding: 12px;
            border-radius: 15px;
            margin: 15px 0;
            border: 2px solid rgba(255, 215, 0, 0.6);
            box-shadow: 
                inset 0 0 20px rgba(0, 0, 0, 0.5),
                0 0 15px rgba(255, 215, 0, 0.3);
        }

        .moon-footer {
            margin-top: 15px;
            padding-top: 15px;
            border-top: 2px solid rgba(255, 255, 255, 0.3);
        }

        .moon-footer .borahae-text {
            font-family: 'Fredoka One', cursive;
            font-size: 2em;
            color: #ffd700;
            text-shadow: 
                0 0 20px rgba(255, 215, 0, 1),
                0 0 40px rgba(255, 215, 0, 0.8),
                2px 2px 4px rgba(0, 0, 0, 0.9);
            margin-bottom: 10px;
        }

        .moon-footer p {
            color: #d0d0d0;
            font-size: 0.9em;
            margin: 5px 0;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.9);
        }

        .moon-close {
            position: absolute;
            top: 20px; right: 30px;
            width: 50px; height: 50px;
            background: rgba(0, 0, 0, 0.5);
            border: 3px solid rgba(255, 215, 0, 0.8);
            border-radius: 50%;
            color: #ffd700;
            font-size: 1.8em;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
            z-index: 100;
            backdrop-filter: blur(10px);
            text-shadow: 0 0 10px rgba(255, 215, 0, 0.8);
        }

        .moon-close:hover {
            background: rgba(255, 105, 180, 0.4);
            transform: rotate(90deg) scale(1.1);
            box-shadow: 0 0 30px rgba(255, 215, 0, 0.8);
        }

        .moon-stars {
            position: absolute;
            width: 100%; height: 100%;
            top: 0; left: 0;
            pointer-events: none;
        }

        .moon-star {
            position: absolute;
            background: white;
            border-radius: 50%;
            animation: moonStarTwinkle 2s ease-in-out infinite;
        }

        @keyframes moonStarTwinkle {
            0%, 100% { opacity: 0.3; transform: scale(1); }
            50% { opacity: 1; transform: scale(1.5); }
        }

        .moon-halo {
            position: absolute;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            width: 900px; height: 900px;
            border-radius: 50%;
            background: radial-gradient(circle, 
                rgba(155, 89, 182, 0.2) 0%, 
                rgba(100, 100, 255, 0.1) 40%, 
                transparent 70%);
            animation: haloPulse 4s ease-in-out infinite;
            pointer-events: none;
            z-index: 1;
        }

        @keyframes haloPulse {
            0%, 100% { transform: translate(-50%, -50%) scale(1); opacity: 0.6; }
            50% { transform: translate(-50%, -50%) scale(1.1); opacity: 0.9; }
        }

        @media (max-width: 768px) {
            .main-title h1 { font-size: 3em; }
            .age-number span { font-size: 5em; }
            .calendar-grid { padding: 15px; gap: 5px; }
            .calendar-month { font-size: 2.2em; }
            .nickname { font-size: 1.5em; }
            .music-control { bottom: 20px; right: 20px; width: 65px; height: 65px; }
            .simple-message p { font-size: 2em; }
            .simple-message .kami-name { font-size: 2.5em; }
            .namjoon-bg { width: 400px; height: 600px; }
            .asma-text { font-size: 2.5em; }
            .asma-message { padding: 40px 30px; }
            
            .giant-moon { width: 350px; height: 350px; }
            .moon-title { font-size: 2em; }
            .moon-body { font-size: 0.85em; }
            .moon-body .kami-name { font-size: 1.5em; }
            .moon-halo { width: 450px; height: 450px; }
            .crater-1 { width: 40px; height: 40px; }
            .crater-2 { width: 25px; height: 25px; }
            .crater-3 { width: 50px; height: 50px; }
            .crater-4 { width: 30px; height: 30px; }
            .crater-5 { width: 20px; height: 20px; }
            .crater-6 { width: 35px; height: 35px; }
            .crater-7 { width: 18px; height: 18px; }
            .crater-8 { width: 22px; height: 22px; }
            .moon-close { width: 40px; height: 40px; font-size: 1.4em; top: 10px; right: 15px; }
        }

        .music-control {
            position: fixed;
            bottom: 30px; right: 30px;
            z-index: 100;
            background: linear-gradient(135deg, #ff69b4 0%, #9b59b6 100%);
            border: 3px solid #ffd700;
            border-radius: 50%;
            width: 75px; height: 75px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            box-shadow: 0 10px 30px rgba(255, 105, 180, 0.8);
            transition: all 0.3s ease;
            animation: musicPulse 2s ease-in-out infinite;
        }

        @keyframes musicPulse {
            0%, 100% { transform: scale(1); box-shadow: 0 10px 30px rgba(255, 105, 180, 0.8); }
            50% { transform: scale(1.1); box-shadow: 0 15px 40px rgba(255, 215, 0, 0.8); }
        }

        .music-control:hover {
            transform: scale(1.2);
            box-shadow: 0 20px 50px rgba(255, 215, 0, 0.8);
        }

        .music-control.playing { animation: spin 3s linear infinite; }

        @keyframes spin {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .music-control span { font-size: 2.2em; }

        .music-tooltip {
            position: absolute;
            bottom: 85px; right: 0;
            background: rgba(155, 89, 182, 0.95);
            color: #ffd700;
            padding: 10px 15px;
            border-radius: 10px;
            border: 2px solid #ffd700;
            white-space: nowrap;
            font-size: 0.9em;
            opacity: 0;
            transition: opacity 0.3s ease;
            pointer-events: none;
            font-family: 'Fredoka One', cursive;
        }

        .music-control:hover .music-tooltip { opacity: 1; }
    </style>
</head>
<body>
    <div class="space-background" id="spaceBackground"></div>
    
    <div class="namjoon-bg">
        <img src="./images/namjoon.jpg" alt="RM Namjoon">
    </div>
    
    <div class="floating-elements" id="floatingElements"></div>

    <!-- مشغل الموسيقى - Happy Birthday -->
    <audio id="bgMusic" loop>
        <source src="./music/happy-birthday.mp3" type="audio/mpeg">
    </audio>

    <div class="music-control" id="musicControl">
        <span id="musicIcon"></span>
        <div class="music-tooltip">Happy Birthday Song (Click to play/pause)</div>
    </div>

    <div class="container">
        <div class="main-title">
            <h1>Happy Birthday Kamilya</h1>
            <p class="subtitle">Wishing you all the happiness in the world 💜</p>
            <p class="nickname">✨ My Dear Kami ✨</p>
        </div>

        <div class="age-number">
            <span>22</span>
        </div>

        <div class="calendar-section">
            <div class="calendar-month">September</div>
            <div class="calendar-year">2026</div>
            <div class="calendar-grid">
                <div class="calendar-day-header">S</div>
                <div class="calendar-day-header">M</div>
                <div class="calendar-day-header">T</div>
                <div class="calendar-day-header">W</div>
                <div class="calendar-day-header">T</div>
                <div class="calendar-day-header">F</div>
                <div class="calendar-day-header">S</div>
                
                <div class="calendar-day"></div>
                <div class="calendar-day"></div>
                <div class="calendar-day"></div>
                <div class="calendar-day"></div>
                <div class="calendar-day">1</div>
                <div class="calendar-day birthday">2</div>
                <div class="calendar-day">3</div>
                <div class="calendar-day">4</div>
                <div class="calendar-day">5</div>
                <div class="calendar-day">6</div>
                <div class="calendar-day">7</div>
                <div class="calendar-day">8</div>
                <div class="calendar-day">9</div>
                <div class="calendar-day">10</div>
                <div class="calendar-day">11</div>
                <div class="calendar-day">12</div>
                <div class="calendar-day">13</div>
                <div class="calendar-day">14</div>
                <div class="calendar-day">15</div>
                <div class="calendar-day">16</div>
                <div class="calendar-day">17</div>
                <div class="calendar-day">18</div>
                <div class="calendar-day">19</div>
                <div class="calendar-day">20</div>
                <div class="calendar-day">21</div>
                <div class="calendar-day">22</div>
                <div class="calendar-day">23</div>
                <div class="calendar-day">24</div>
                <div class="calendar-day">25</div>
                <div class="calendar-day">26</div>
                <div class="calendar-day">27</div>
                <div class="calendar-day">28</div>
                <div class="calendar-day">29</div>
                <div class="calendar-day">30</div>
            </div>
        </div>

        <div class="asma-message" id="parchmentBtn">
            <div class="asma-hearts">
                <div class="floating-heart" style="top: 10%; left: 10%; animation-delay: 0s;">💜</div>
                <div class="floating-heart" style="top: 20%; right: 15%; animation-delay: 0.5s;"></div>
                <div class="floating-heart" style="bottom: 15%; left: 20%; animation-delay: 1s;">💖</div>
                <div class="floating-heart" style="bottom: 25%; right: 10%; animation-delay: 1.5s;"></div>
                <div class="floating-note" style="top: 15%; left: 50%; animation-delay: 0.3s;">🎵</div>
                <div class="floating-note" style="bottom: 20%; left: 40%; animation-delay: 0.8s;">🎶</div>
                <div class="floating-note" style="top: 50%; right: 20%; animation-delay: 1.2s;">🎸</div>
                <div class="floating-note" style="top: 40%; left: 15%; animation-delay: 1.7s;">🎤</div>
            </div>
            <div class="asma-text">to my kami<br>from Asma 💜</div>
        </div>

        <div class="gallery-section">
            <div class="polaroid-container">
                <div class="polaroid">
                    <div class="polaroid-img">
                        <img src="./images/photo1.jpg" alt="Memory 1">
                    </div>
                </div>
                <div class="polaroid">
                    <div class="polaroid-img">
                        <img src="./images/photo2.jpg" alt="Memory 2">
                    </div>
                </div>
                <div class="polaroid">
                    <div class="polaroid-img">
                        <img src="./images/photo3.jpg" alt="Memory 3">
                    </div>
                </div>
                <div class="polaroid">
                    <div class="polaroid-img">
                        <img src="./images/photo4.jpg" alt="Memory 4">
                    </div>
                </div>
            </div>
        </div>

        <div class="simple-message">
            <p class="date">September 2, 2004 - September 2, 2026</p>
            <p class="birthday-text">Happy Birthday to the most precious friend</p>
            <p class="kami-name">My dear Kami 💜</p>
            <p class="borahae">Borahae Kamilya 💜</p>
        </div>

        <footer>
            <p>Made with 💜 for Kami's 22nd Birthday</p>
            <p class="borahae-footer">Borahae Kamilya - I Purple You 💜</p>
            <p style="margin-top: 20px; font-size: 1em; opacity: 0.9;">
                BTS Forever | ARMY Forever | Kami Forever 💜
            </p>
        </footer>
    </div>

    <!-- MOON MODAL -->
    <div class="moon-modal-overlay" id="moonModal">
        <div class="moon-halo"></div>
        <div class="moon-stars" id="moonStars"></div>
        <button class="moon-close" id="moonClose"></button>
        
        <div class="giant-moon">
            <div class="crater crater-1"></div>
            <div class="crater crater-2"></div>
            <div class="crater crater-3"></div>
            <div class="crater crater-4"></div>
            <div class="crater crater-5"></div>
            <div class="crater crater-6"></div>
            <div class="crater crater-7"></div>
            <div class="crater crater-8"></div>
            
            <div class="moon-content">
                <h2 class="moon-title">Happy 22nd Birthday Kamilya!</h2>
                
                <div class="moon-body">
                    <p>My dearest <span class="kami-name">Kami</span>,</p>
                    
                    <p>Today marks a special day - the day the world became brighter because you were born! </p>
                    
                    <div class="date-info">
                        <p class="highlight">September 2, 2004 → September 2, 2026</p>
                        <p>22 years of pure magic ✨</p>
                    </div>
                    
                    <p>On your twenty-second birthday, I want you to know how much you mean to me. You are not just a friend, you are family. 💜</p>
                    
                    <p>Like RM always says: <em>"You are born to shine"</em> - and shine you do, Kami! Your light makes everyone around you happier. 🌸</p>
                    
                    <p>May this year bring you:</p>
                    <p>🎸 Beautiful melodies from your guitar</p>
                    <p>🎵 Endless music in your soul</p>
                    <p>💜 True love and friendship</p>
                    <p>👑 Success in everything you do</p>
                    
                    <p>You deserve all the good things in this world, Kamilya. Never forget how special you are! 💜</p>
                    
                    <p class="highlight">Happy Birthday, my dear Kami! </p>
                </div>
                
                <div class="moon-footer">
                    <div class="borahae-text">Borahae Kamilya 💜</div>
                    <p>I Purple You - Today and Always</p>
                    <p>BTS Forever | ARMY Forever | Kami Forever</p>
                </div>
            </div>
        </div>
    </div>

    <script>
        function createSpaceBackground() {
            const bg = document.getElementById('spaceBackground');
            
            for (let i = 0; i < 150; i++) {
                const star = document.createElement('div');
                star.className = 'star';
                const size = Math.random() * 3 + 1;
                star.style.width = size + 'px';
                star.style.height = size + 'px';
                star.style.left = Math.random() * 100 + '%';
                star.style.top = Math.random() * 100 + '%';
                star.style.animationDelay = Math.random() * 3 + 's';
                star.style.animationDuration = (Math.random() * 3 + 2) + 's';
                bg.appendChild(star);
            }
            
            for (let i = 0; i < 15; i++) {
                const name = document.createElement('div');
                name.className = 'kamilya-name';
                name.textContent = 'Kamilya';
                const fontSize = Math.random() * 1.5 + 0.8;
                name.style.fontSize = fontSize + 'em';
                name.style.left = Math.random() * 90 + '%';
                name.style.top = Math.random() * 100 + '%';
                name.style.animationDelay = Math.random() * 8 + 's';
                name.style.animationDuration = (Math.random() * 6 + 6) + 's';
                name.style.transform = `rotate(${Math.random() * 30 - 15}deg)`;
                bg.appendChild(name);
            }
            
            const planetColors = ['purple', 'blue', 'red'];
            const planetSizes = [
                { min: 40, max: 80 },
                { min: 80, max: 130 },
                { min: 130, max: 200 }
            ];
            
            for (let i = 0; i < 12; i++) {
                const planet = document.createElement('div');
                const colorClass = planetColors[Math.floor(Math.random() * planetColors.length)];
                const sizeClass = planetSizes[Math.floor(Math.random() * planetSizes.length)];
                const size = Math.random() * (sizeClass.max - sizeClass.min) + sizeClass.min;
                
                planet.className = `planet planet-${colorClass}`;
                planet.style.width = size + 'px';
                planet.style.height = size + 'px';
                planet.style.left = Math.random() * 90 + '%';
                planet.style.top = Math.random() * 100 + '%';
                planet.style.animationDelay = Math.random() * 10 + 's';
                planet.style.animationDuration = (Math.random() * 10 + 10) + 's';
                
                if (Math.random() > 0.6 && size > 60) {
                    const ring = document.createElement('div');
                    ring.className = 'planet-ring';
                    planet.appendChild(ring);
                }
                
                bg.appendChild(planet);
            }
        }

        function createMoonStars() {
            const container = document.getElementById('moonStars');
            for (let i = 0; i < 100; i++) {
                const star = document.createElement('div');
                star.className = 'moon-star';
                const size = Math.random() * 2 + 1;
                star.style.width = size + 'px';
                star.style.height = size + 'px';
                star.style.left = Math.random() * 100 + '%';
                star.style.top = Math.random() * 100 + '%';
                star.style.animationDelay = Math.random() * 2 + 's';
                container.appendChild(star);
            }
        }

        function createArmyBomb() {
            const bomb = document.createElement('div');
            bomb.className = 'army-bomb';
            bomb.innerHTML = `
                <div class="ball">
                    <div class="bts-logo">
                        <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
                            <path d="M50 10 L75 35 L75 70 L50 90 L25 70 L25 35 Z" 
                                  fill="none" stroke="#4169E1" stroke-width="4"/>
                            <path d="M50 20 L65 38 L65 65 L50 80 L35 65 L35 38 Z" 
                                  fill="#4169E1" opacity="0.6"/>
                            <path d="M50 30 L58 42 L58 60 L50 70 L42 60 L42 42 Z" 
                                  fill="#6495ED"/>
                        </svg>
                    </div>
                </div>
                <div class="handle"></div>
            `;
            return bomb;
        }

        function createGuitar(type) {
            const guitar = document.createElement('div');
            guitar.className = `guitar guitar-${type}`;
            guitar.textContent = '🎸';
            return guitar;
        }

        function createMusicNote() {
            const note = document.createElement('div');
            note.className = 'music-note';
            const notes = ['', '🎶', '♪', ''];
            note.textContent = notes[Math.floor(Math.random() * notes.length)];
            return note;
        }

        function createPurpleHeart() {
            const heart = document.createElement('div');
            heart.className = 'purple-heart-float';
            const hearts = ['💜', '💗', '💖', '💝'];
            heart.textContent = hearts[Math.floor(Math.random() * hearts.length)];
            return heart;
        }

        function createFloatingElements() {
            const container = document.getElementById('floatingElements');
            const guitarTypes = ['red', 'electric', 'acoustic', 'bass', 'pink', 'purple', 'gold'];

            setInterval(() => {
                const element = document.createElement('div');
                element.className = 'floating-item';
                const rand = Math.random();
                
                if (rand < 0.40) {
                    const randomType = guitarTypes[Math.floor(Math.random() * guitarTypes.length)];
                    element.appendChild(createGuitar(randomType));
                } else if (rand < 0.65) {
                    element.appendChild(createArmyBomb());
                } else if (rand < 0.85) {
                    element.appendChild(createMusicNote());
                } else {
                    element.appendChild(createPurpleHeart());
                }
                
                element.style.left = Math.random() * 100 + '%';
                element.style.top = '100vh';
                element.style.animationDuration = (Math.random() * 8 + 10) + 's';
                element.style.animationDelay = Math.random() * 2 + 's';
                container.appendChild(element);
                
                setTimeout(() => { element.remove(); }, 18000);
            }, 700);
        }

        // ===== التحكم في الموسيقى =====
        const musicControl = document.getElementById('musicControl');
        const musicIcon = document.getElementById('musicIcon');
        const bgMusic = document.getElementById('bgMusic');
        let isPlaying = false;

        musicControl.addEventListener('click', () => {
            if (isPlaying) {
                bgMusic.pause();
                musicIcon.textContent = '🎵';
                musicControl.classList.remove('playing');
            } else {
                bgMusic.play();
                musicIcon.textContent = '⏸️';
                musicControl.classList.add('playing');
            }
            isPlaying = !isPlaying;
        });

        document.addEventListener('click', () => {
            if (!isPlaying && bgMusic.paused) {
                bgMusic.play().then(() => {
                    isPlaying = true;
                    musicIcon.textContent = '⏸️';
                    musicControl.classList.add('playing');
                }).catch(error => {
                    console.log('Autoplay prevented by browser');
                });
            }
        }, { once: true });

        window.addEventListener('load', () => {
            createSpaceBackground();
            createFloatingElements();
            createMoonStars();
        });

        document.querySelectorAll('.polaroid').forEach((polaroid, index) => {
            polaroid.addEventListener('click', () => {
                polaroid.style.transform = 'rotate(0deg) scale(1.15)';
                setTimeout(() => {
                    polaroid.style.transform = `rotate(${index % 2 === 0 ? -3 : 3}deg)`;
                }, 300);
            });
        });

        const parchmentBtn = document.getElementById('parchmentBtn');
        const moonModal = document.getElementById('moonModal');
        const moonClose = document.getElementById('moonClose');

        parchmentBtn.addEventListener('click', () => {
            moonModal.classList.add('active');
            document.body.style.overflow = 'hidden';
        });

        moonClose.addEventListener('click', () => {
            moonModal.classList.remove('active');
            document.body.style.overflow = 'auto';
        });

        moonModal.addEventListener('click', (e) => {
            if (e.target === moonModal) {
                moonModal.classList.remove('active');
                document.body.style.overflow = 'auto';
            }
        });

        document.addEventListener('keydown', (e) => {
            if (e.key === 'Escape' && moonModal.classList.contains('active')) {
                moonModal.classList.remove('active');
                document.body.style.overflow = 'auto';
            }
        });

        console.log('%c💜 Happy 22nd Birthday Kamilya! 💜', 'font-size: 30px; color: #ff69b4; font-weight: bold;');
        console.log('%cBorahae Kami - I Purple You', 'font-size: 20px; color: #ffd700;');
        console.log('%cBTS Forever | ARMY Forever', 'font-size: 15px; color: #9b59b6;');
    </script>
</body>
</html>
