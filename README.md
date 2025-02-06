<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Valentine's Day💕</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f9f9f9;
            color: #333;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            margin: auto;
            background: lightpink;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        img {
            width: 100%;
            border-radius: 10px;
            margin-top: 10px;
        }
        .hidden-message {
            display: none;
            margin-top: 20px;
            font-size: 20px;
            color: #e44d4d;
            opacity: 0;
            transition: opacity 1s ease-in-out;
        }
        button {
            padding: 10px 20px;
            border: none;
            background-color: #ff7eb3;
            color: white;
            font-size: 16px;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
            transition: transform 0.1s;
        }
        button:hover {
            background-color: #ff4d94;
        }
        button:active {
            transform: scale(0.95);
        }
#youtubePlayer {
    width: 1px;
    height: 1px;
    visibility: hidden;
}
    </style>
</head>
<body>
    <div class="container">
        <h1>HAPPY VALENTINE'S DAY💖</h1>
        <p>MY BENJI🥰</p>
        
      
        <img src="https://drive.google.com/uc?export=view&id=1aK2ILSo9HMmdPnLdNaEzlihjc0gG3wEI" alt="Our Memory">
        
        <p>OPEN TO SEE THE SECRET!💌</p>
        <button onclick="showMessage()">OPEN</button>
        <p class="hidden-message" id="secretMessage">Thanks for being mine, love chu bibi💕</p>

        <p> Music: <button onclick="toggleMusic()">Play / Pause</button></p>
    </div>


    <iframe id="youtubePlayer" width="0" height="0" src="https://www.youtube.com/embed/XShaIZs7J7M?autoplay=1&loop=1&playlist=XShaIZs7J7M&mute=1" frameborder="0" allow="autoplay"></iframe>

    <script>
        function showMessage() {
            var message = document.getElementById('secretMessage');
            message.style.display = 'block';
            setTimeout(() => { message.style.opacity = 1; }, 10);
        }

        function toggleMusic() {
            var iframe = document.getElementById("youtubePlayer");
            var src = iframe.src;
            if (src.includes("mute=1")) {
                iframe.src = src.replace("mute=1", "mute=0");
            } else {
                iframe.src = src.replace("mute=0", "mute=1");
            }
        }
    </script>
</body>
</html>
