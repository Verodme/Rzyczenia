<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wesołych Świąt</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: url('https://source.unsplash.com/1600x900/?christmas,holiday') no-repeat center center fixed;
            background-size: cover;
            color: #fff;
            overflow: hidden;
        }
        .overlay {
            background-color: rgba(0, 0, 0, 0.6);
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
        }
        .container {
            max-width: 800px;
            margin: 50px auto;
            text-align: center;
            background-color: rgba(255, 255, 255, 0.2);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }
        .header {
            font-size: 32px;
            font-weight: bold;
            margin-bottom: 20px;
            animation: fadeIn 2s;
        }
        .message {
            font-size: 20px;
            line-height: 1.8;
            margin-bottom: 20px;
            animation: fadeIn 2.5s;
        }
        .footer {
            font-size: 18px;
            margin-top: 20px;
            font-style: italic;
            animation: fadeIn 3s;
        }
        .footer span {
            font-weight: bold;
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }
        .snowflake {
            position: fixed;
            top: -50px;
            color: #fff;
            font-size: 1.5em;
            user-select: none;
            z-index: 1000;
            animation: snow 10s linear infinite;
        }
        @keyframes snow {
            0% {
                transform: translateY(0) rotate(0deg);
            }
            100% {
                transform: translateY(100vh) rotate(360deg);
            }
        }
        @keyframes drift {
            0% {
                transform: translateX(0);
            }
            50% {
                transform: translateX(20px);
            }
            100% {
                transform: translateX(0);
            }
        }
    </style>
</head>
<body>
    <div class="overlay"></div>
    <div class="container">
        <div class="header">
            Wesołych Świąt!
        </div>
        <div class="message">
            Z okazji Świąt Bożego Narodzenia składamy najserdeczniejsze życzenia: <br>
            Niech ten magiczny czas napełni Wasze serca radością, a dom ciepłem rodzinnych spotkań. <br>
            Niech zdrowie, szczęście i spokój towarzyszą Wam każdego dnia, <br>
            a Nowy Rok przyniesie spełnienie marzeń i nowe możliwości.
        </div>
        <div class="footer">
            Z najlepszymi życzeniami, <br>
            <span>Sławomir i Maria Mering z rodziną</span>
        </div>
        <!-- Odtwarzacz muzyczny -->
        <audio controls autoplay loop style="margin-top: 20px;">
            <source src="https://www.bensound.com/bensound-music/bensound-thejazzpiano.mp3" type="audio/mpeg">
            Twoja przeglądarka nie obsługuje odtwarzacza audio.
        </audio>
    </div>
    <!-- Śnieżynki -->
    <div class="snowflake" style="left: 10%; animation-delay: 0s;">❄</div>
    <div class="snowflake" style="left: 30%; animation-delay: 2s;">❄</div>
    <div class="snowflake" style="left: 50%; animation-delay: 4s;">❄</div>
    <div class="snowflake" style="left: 70%; animation-delay: 1s;">❄</div>
    <div class="snowflake" style="left: 90%; animation-delay: 3s;">❄</div> szybko
</body>
</html>
