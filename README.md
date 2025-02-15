<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Special Message</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: url('https://love-romance-image.blogspot.com/2017/01/romantic-couple-with-pink-background.html') no-repeat center center fixed;
            background-size: cover;
            color: white;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 500px;
            margin: 50px auto;
            padding: 20px;
            background: rgba(0, 0, 0, 0.7);
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
        }
        h1 {
            font-size: 30px;
            font-weight: bold;
            text-transform: uppercase;
            color: #ff4d4d;
        }
        button {
            background-color: #ff4d4d;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 18px;
            margin-top: 20px;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #e60000;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>

    <div class="container" id="step1">
        <h1>HI, HASINI ❤️</h1>
        <p>I have something special for you!</p>
        <button onclick="nextStep(1)">Next</button>
    </div>

    <div class="container hidden" id="step2">
        <h2>Hasini, you make my world brighter every day. ❤️</h2>
        <p>Do you want to continue?</p>
        <button onclick="nextStep(2)">Yes</button>
    </div>

    <div class="container hidden" id="step3">
        <p>Guess who secretly adores you?</p>
        <button onclick="nextStep(3)">Your Best Friend</button>
        <button onclick="nextStep(3)">A Secret Admirer</button>
        <button onclick="nextStep(3)">Someone Special</button>
    </div>

    <div class="container hidden" id="step4">
        <h2>❤️ Hasini, I have something to tell you ❤️</h2>
        <p>I have been in love with you for 3 years. You are my happiness, my dream, and my favorite person.</p>
        <h3>Will you be mine? 🥰</h3>
        <button onclick="showLove()">Yes</button>
        <button onclick="showLove()">Of course, Yes!</button>
    </div>

    <div class="container hidden" id="final">
        <h2>🎉 Yay! You made me the happiest person alive! 🎉</h2>
        <p>Let’s celebrate our new journey together! ❤️</p>
        <audio id="loveSong" autoplay>
            <source src="YOUR_MP3_LINK_HERE.mp3" type="audio/mpeg">
        </audio>
    </div>

    <script>
        function nextStep(step) {
            document.getElementById("step" + step).classList.add("hidden");
            document.getElementById("step" + (step + 1)).classList.remove("hidden");
        }

        function showLove() {
            document.getElementById("step4").classList.add("hidden");
            document.getElementById("final").classList.remove("hidden");

            // Change the background to the proposal image
            document.body.style.background = "url('https://www.freepik.com/premium-vector/happy-propose-day-boy-bending-his-knees-proposing-girl-with-rose-blue-background_64321482.htm') no-repeat center center fixed";
            document.body.style.backgroundSize = "cover";

            // Play the song
            document.getElementById("loveSong").play();
        }
    </script>

</body>
</html>
