<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Creative Redirect</title>
    <style>
        /* Basic Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #282c34;
            color: white;
            flex-direction: column;
        }
        .container {
            text-align: center;
        }
        h1 {
            font-size: 3em;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-in-out;
        }
        p {
            font-size: 1.2em;
            margin-bottom: 30px;
            color: #aaa;
            animation: fadeIn 3s ease-in-out;
        }
        .redirect-btn {
            padding: 15px 30px;
            font-size: 1.2em;
            color: white;
            background: linear-gradient(45deg, #6a11cb, #2575fc);
            border: none;
            border-radius: 30px;
            cursor: pointer;
            outline: none;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transition: all 0.3s ease;
        }
        .redirect-btn:hover {
            background: linear-gradient(45deg, #2575fc, #6a11cb);
            transform: scale(1.1);
        }
        /* Animation for fade-in effect */
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
    </style>
</head>
<body>

    <div class="container">
        <h1>Welcome to Our Website!</h1>
        <p>Click the button below to visit another page</p>
        <button class="redirect-btn" onclick="redirectToPage()">Go to us.html</button>
    </div>

    <script>
        function redirectToPage() {
            // Redirect to us.html when the button is clicked
            window.location.href = "us.html";
        }
    </script>

</body>
</html>
