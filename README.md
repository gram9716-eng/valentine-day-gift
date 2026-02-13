<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Will You Handle My Miscellaneous Expenses?</title>

<style>
body{
    text-align:center;
    font-family:Arial, sans-serif;
    background:#ffccd5;
    margin-top:100px;
}

h1{
    color:#b30059;
}

button{
    padding:12px 25px;
    font-size:18px;
    border:none;
    border-radius:8px;
    cursor:pointer;
    margin:10px;
}

#yes{
    background-color:green;
    color:white;
}

#no{
    background-color:red;
    color:white;
    position:absolute;
}
#videoBox{
    display:none;
    margin-top:30px;
}
</style>
</head>

<body>

<h1>Will You Handle My Miscellaneous Expenses? 💸😜</h1>

<button id="yes" onclick="playVideo()">Yes 😍</button>
<button id="no" onmouseover="moveNo()">No 🙈</button>

<div id="videoBox">
    <h2>I knew you would say YES ❤️</h2>
    <video width="400" controls autoplay>
        <source src="video.mp4" type="video/mp4">
    </video>
</div>

<script>
function moveNo(){
    let btn = document.getElementById("no");
    let x = Math.random() * (window.innerWidth - 100);
    let y = Math.random() * (window.innerHeight - 100);
    btn.style.left = x + "px";
    btn.style.top = y + "px";
}

function playVideo(){
    document.getElementById("videoBox").style.display="block";
}
</script>

</body>
</html>
