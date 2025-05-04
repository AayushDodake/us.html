
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fun Redirect</title>
    <style>
        /* Basic Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Comic Sans MS', cursive, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            color: #fff;
            flex-direction: column;
            overflow: hidden;
            text-align: center;
        }
        h1 {
            font-size: 3.5em;
            margin-bottom: 20px;
            color: #ff6b81;
            animation: bounceIn 2s ease;
        }
        p {
            font-size: 1.5em;
            margin-bottom: 40px;
            color: #6a1b9a;
            animation: fadeIn 3s ease-in-out;
        }
        .redirect-btn {
            padding: 20px 50px;
            font-size: 1.5em;
            background: radial-gradient(circle, #ff5f6d, #ffc3a0);
            border: none;
            border-radius: 50px;
            cursor: pointer;
            outline: none;
            box-shadow: 0 10px 30px rgba(255, 95, 109, 0.4);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            font-weight: bold;
        }
        .redirect-btn:hover {
            transform: scale(1.1);
            box-shadow: 0 15px 40px rgba(255, 95, 109, 0.6);
        }
        .redirect-btn:active {
            transform: scale(0.95);
        }
        .cloud {
            position: absolute;
            top: 10%;
            left: 50%;
            transform: translateX(-50%);
            background: url('https://cdn.pixabay.com/photo/2017/08/30/00/58/cloud-2695367_960_720.png') no-repeat;
            width: 150px;
            height: 90px;
            animation: cloudMove 5s infinite linear;
        }
        /* Animations */
        @keyframes fadeIn {
            0% {
                opacity: 0;
                transform: translateY(20px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @keyframes bounceIn {
            0% {
                opacity: 0;
                transform: translateY(-100px);
            }
            60% {
                opacity: 1;
                transform: translateY(30px);
            }
            100% {
                transform: translateY(0);
            }
        }
        @keyframes cloudMove {
            0% {
                transform: translateX(-50%);
            }
            50% {
                transform: translateX(30%);
            }
            100% {
                transform: translateX(-50%);
            }
        }
    </style>
</head>
<body>

    <div class="cloud"></div>
    
    <h1>Yay, You're Here!</h1>
    <p>Click below to go to our special page!</p>
    <button class="redirect-btn" onclick="redirectToPage()">Go to us.html</button>

    <script>
        function redirectToPage() {
            // Redirect to us.html when the button is clicked
            window.location.href = "us.html";
        }
    </script>

</body>
</html>
