<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <link rel="stylesheet" href="./styles/css/style.css">
</head>
<body>
    <div class="container">
        <div class="text" >
            <h1 class = "header_text">Ты будешь моей валентинкой?</h1>
        </div>
        <div class="gif_container">
            <img src="https://media.giphy.com/media/LnKonfpQ44fNvuGLkA/giphy.gif" alt="Cute animated illustration">
        </div>
        <div class = "buttons">
            <button class="btn" id = "yesButton" onclick="nextPage()">Да</button>
            <button class="btn" id="noButton" onmouseover="moveButton()">Нет</button>
            <script>
                function nextPage() {
                    window.location.href = "yes.html";
                }

                function moveButton() {
                    let x = Math.random() * (window.innerWidth - document.getElementById('noButton').offsetWidth);
                    let y = Math.random() * (window.innerHeight - document.getElementById('noButton').offsetHeight);
                    document.getElementById('noButton').style.left = ${x}px;
                    document.getElementById('noButton').style.top = ${y}px;
                }
            </script>
        </div>
    </div>
</body>
</html>
