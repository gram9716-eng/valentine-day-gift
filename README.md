<!DOCTYPE html>
<html>
<head>
    <title>Will You Handle My Miscellaneous Expenses? 😜</title>

    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background: linear-gradient(to right, #ff9a9e, #fad0c4);
            margin-top: 100px;
            overflow: hidden;
        }

        h1 {
            color: white;
            font-size: 35px;
        }

        button {
            padding: 12px 25px;
            font-size: 18px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            margin: 10px;
        }

        #yesBtn {
            background-color: #28a745;
            color: white;
        }

        #noBtn {
            background-color: #dc3545;
            color: white;
            position: absolute;
        }

        #videoSection {
            display: none;
            margin-top: 30px;
        }

        video {
            width: 400px;
            border-radius: 15px;
        }
    </style>
</head>

<body>

    <h1>Will You Handle My Miscellaneous Expenses? 💸😜</h1>

    <button id="yesBtn" onclick="showVideo()">Yes 😍</button>
    <button id="noBtn" onmouseover="moveButton()">No 🙈</button>

    <div id="videoSection">
        <h2>Hehe… I knew it! ❤️</h2>
        <video controls autoplay>
            <source src="love.mp4" type="video/mp4">
        </video>
    </div>

<script>
    function moveButton() {
        var button = document.getElementById("noBtn");
        var x = Math.random() * (window.innerWidth - 100);
        var y = Math.random() * (window.innerHeight - 100);
        button.style.left = x + "px";
        button.style.top = y + "px";
    }

    function showVideo() {
        document.getElementById("videoSection").style.display = "block";
    }
</script>

</body>
</html>