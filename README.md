<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water World - Pure & Refreshing</title>
    <style>
        /* Full CSS code embedded here for easy use */
        body {
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            font-family: 'Arial', sans-serif;
            background-color: #000;
            overflow-x: hidden;
            color: white;
        }

        .ripple-background {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            background: radial-gradient(circle, #1e90ff, #4682b4);
            overflow: hidden;
            z-index: -1;
        }

        .ripple {
            position: absolute;
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.2);
            animation: ripple-animation 6s infinite;
            opacity: 0;
        }

        @keyframes ripple-animation {
            0% {
                transform: scale(0.5);
                opacity: 0.8;
            }
            50% {
                transform: scale(2);
                opacity: 0.4;
            }
            100% {
                transform: scale(4);
                opacity: 0;
            }
        }

        .ripple:nth-child(1) {
            animation-delay: 0s;
            left: 30%;
            top: 40%;
        }
        .ripple:nth-child(2) {
            animation-delay: 1.5s;
            left: 60%;
            top: 50%;
        }
        .ripple:nth-child(3) {
            animation-delay: 3s;
            left: 50%;
            top: 30%;
        }
        .ripple:nth-child(4) {
            animation-delay: 4.5s;
            left: 70%;
            top: 60%;
        }

        .content {
            text-align: center;
            padding: 2rem;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            max-width: 600px;
            margin: 2rem;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
        }

        h1 {
            font-size: 3rem;
            background: linear-gradient(45deg, #ffffff, #e0f7ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin: 0 0 1rem;
            text-shadow: 0 0 20px rgba(255, 255, 255, 0.5);
        }

        p {
            font-size: 1.2rem;
            line-height: 1.6;
            margin-bottom: 2rem;
        }

        .cta-button {
            display: inline-block;
            padding: 1rem 2rem;
            background: linear-gradient(45deg, #00bfff, #1e90ff);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: transform 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 191, 255, 0.4);
        }

        .cta-button:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 20px rgba(0, 191, 255, 0.6);
        }

        .features {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-top: 2rem;
        }

        .feature {
            background: rgba(255, 255, 255, 0.1);
            padding: 1rem;
            margin: 0.5rem;
            border-radius: 10px;
            min-width: 150px;
        }
    </style>
</head>
<body>
    <div class="ripple-background">
        <div class="ripple"></div>
        <div class="ripple"></div>
        <div class="ripple"></div>
        <div class="ripple"></div>
    </div>

    <div class="content">
        <h1>🌊 Water World</h1>
        <p>Experience the purity of nature's most essential element. Refreshing, clean, and delivered to your door.</p>
        <a href="#" class="cta-button">Order Now</a>
        
        <div class="features">
            <div class="feature">💧 Pure Spring Water</div>
            <div class="feature">🚚 Fast Delivery</div>
            <div class="feature">♻️ Eco-Friendly</div>
        </div>
    </div>
</body>
</html>
