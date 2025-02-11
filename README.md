<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #ffebee;
            font-family: Arial, sans-serif;
            text-align: center;
        }
        h1 {
            color: #d32f2f;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 10px;
        }
        .yes {
            background-color: #4caf50;
            color: white;
        }
        .no {
            background-color: #d32f2f;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>Would you be my Valentine? 💖</h1>
    <div class="buttons">
        <button class="yes" onclick="alert('Yay! I love you! 💕')">Yes</button>
        <button class="no" onmouseover="moveButton()">No</button>
    </div>

    <script>
        function moveButton() {
            const button = document.querySelector('.no');
            const x = Math.random() * (window.innerWidth - 100);
            const y = Math.random() * (window.innerHeight - 50);
            button.style.left = `${x}px`;
            button.style.top = `${y}px`;
        }
    </script>
</body>
</html>
