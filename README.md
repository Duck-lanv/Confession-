<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tỏ tình</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            background: linear-gradient(to right, #ff9a9e, #fad0c4);
        }
        .container {
            margin-top: 100px;
        }
        h1 {
            color: #ff6f61;
        }
        .button {
            display: inline-block;
            margin: 10px;
            padding: 15px 30px;
            font-size: 16px;
            color: white;
            background-color: #ff6f61;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .button:hover {
            background-color: #ff3e30;
        }
        .runaway {
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Chị có đồng ý làm bạn gái em không?</h1>
        <button id="agree" class="button">Đồng ý</button>
        <button id="disagree" class="button runaway">Không đồng ý</button>
    </div>

    <script>
        const agreeButton = document.getElementById("agree");
        const disagreeButton = document.getElementById("disagree");

        // Sự kiện khi bấm nút đồng ý
        agreeButton.addEventListener("click", function () {
            alert("Yay! yêu chị Châm nhất luôn 🥰🥰🥰");
        });

        // Sự kiện khi bấm nút không đồng ý
        disagreeButton.addEventListener("mouseover", function () {
            const x = Math.random() * (window.innerWidth - 100);
            const y = Math.random() * (window.innerHeight - 50);
            disagreeButton.style.left = x + "px";
            disagreeButton.style.top = y + "px";
        });
    </script>
</body>
</html>
