# happy-birthday-card
happy birthday to my best friend
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            font-family: Arial, sans-serif;
            flex-direction: column;
        }
        .card {
            background: white;
            width: 300px;
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        .card h1 {
            color: #ff4f8b;
        }
        .cake {
            font-size: 50px;
        }
        .btn {
            margin-top: 20px;
            padding: 10px 20px;
            background: #ff4f8b;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
        }
        .btn:hover {
            background: #e03e73;
        }
        .hidden-message {
            display: none;
            color: #e03e73;
            font-size: 18px;
            margin-top: 15px;
        }
        .video-container {
            display: none;
            margin-top: 20px;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: rgba(0, 0, 0, 0.8);
            padding: 20px;
            border-radius: 10px;
        }
        .video-container video {
            width: 80vw;
            height: auto;
            max-width: 800px;
        }
    </style>
</head>
<body>
    <div class="card">
        <h1>Happy Birthday 🎉</h1>
        <p>Dear Bestie,</p>
        <p>Wishing you a day filled with love, joy, and cake! 🍰</p>
        <div class="cake">🎂</div>
        <button class="btn" onclick="showMessage()">Click for a Surprise!</button>
        <p class="hidden-message" id="message">You're the best friend ever! 💖</p>
    </div>
    
    <div class="video-container" id="videoContainer">
        <video controls>
            <source src="Kids birthday slideshow - Made with Clipchamp (2).mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
    
    <script>
        function showMessage() {
            document.getElementById("message").style.display = "block";
            document.getElementById("videoContainer").style.display = "block";
        }
    </script>
</body>
</html>
