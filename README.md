<!DOCTYPE html>
<html>
<head>
    <title>My Valentine ❤️</title>
    <style>
        body {
            text-align: center;
            font-family: 'Arial', sans-serif;
            margin-top: 100px;
            background-color: #fff0f5;
        }

        h1 { color: #ff3366; }

        button {
            padding: 15px 30px;
            font-size: 18px;
            margin: 20px;
            cursor: pointer;
            border-radius: 12px;
            border: none;
        }

        #yes {
            background-color: #ff4d88;
            color: white;
        }

        #no {
            background-color: #ccc;
            position: absolute;
        }

        img {
            width: 200px;
            margin-top: 20px;
            border-radius: 10px;
        }
    </style>
</head>
<body>

<h1>Will you be my Valentine? ❤️</h1>

<button id="yes" onclick="yesClicked()">Yes 💖</button>
<button id="no" onclick="moveNo()">No 🙈</button>

<script>
function yesClicked(){
    document.body.innerHTML = `
        <h1>Yay! ❤️</h1>
        <p>I wanted to tell you something honestly — I still care deeply, and I’ll always wish you happiness.  
        If someday you walk toward me, I’ll meet you with love and growth.  
        If not, I’ll carry our memories with gratitude and keep becoming the best version of myself.  
        Either way, you’re always special to me.</p>
        <img src="YOUR_IMAGE_URL_HERE" alt="memory">
    `;
}

function moveNo(){
    const btn = document.getElementById("no");
    btn.style.top = Math.random() * (window.innerHeight - 50) + "px";
    btn.style.left = Math.random() * (window.innerWidth - 100) + "px";
}
</script>

</body>
</html>

