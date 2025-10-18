<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zexin Oyunları</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #FF69B4, #FFB6C1);
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
            position: relative;
        }
        header {
            background: rgba(255, 105, 180, 0.9);
            color: #fff;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 6px 25px rgba(0, 0, 0, 0.2);
            animation: shimmer 3s infinite;
        }
        @keyframes shimmer {
            0% { background-position: -300px 0; }
            100% { background-position: 300px 0; }
        }
        header h1 {
            font-size: 3.5rem;
            animation: fadeIn 2s ease-in, sparkle 1.5s infinite;
            text-shadow: 0 0 20px #fff, 0 0 40px #9370DB;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes sparkle {
            0% { text-shadow: 0 0 10px #fff; }
            50% { text-shadow: 0 0 25px #9370DB, 0 0 40px #fff; }
            100% { text-shadow: 0 0 10px #fff; }
        }
        nav {
            margin-top: 1.5rem;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 25px;
            font-size: 1.3rem;
            transition: color 0.3s, text-shadow 0.3s;
        }
        nav a:hover {
            color: #9370DB;
            text-shadow: 0 0 20px #fff;
        }
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 40px;
        }
        .games-section {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        .game-card {
            background: #fff;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.15);
            transition: transform 0.4s, box-shadow 0.4s;
            position: relative;
            overflow: hidden;
        }
        .game-card::before {
            content: '';
            position: absolute;
            top: -60%;
            left: -60%;
            width: 220%;
            height: 220%;
            background: radial-gradient(circle, rgba(255, 182, 193, 0.5) 0%, transparent 70%);
            animation: glitter 6s infinite;
            z-index: 0;
        }
        @keyframes glitter {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        .game-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 40px rgba(147, 112, 219, 0.7);
        }
        .game-card iframe {
            width: 100%;
            height: 300px;
            border: none;
            border-radius: 20px 20px 0 0;
            position: relative;
            z-index: 1;
        }
        .game-card h3 {
            padding: 20px;
            color: #FF69B4;
            font-size: 1.4rem;
            position: relative;
            z-index: 1;
            background: rgba(255,
