# gizlibilgi
cokgizlibilgi
<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<title>Video</title>
<style>
    body {
        margin: 0;
        background-color: black;
    }
    #scare {
        display: none;
        width: 100vw;
        height: 100vh;
        object-fit: cover;
    }
</style>
</head>
<body>

<!-- Başta boş ekran -->
<h1 style="color:white; text-align:center; margin-top:40vh; font-family:sans-serif;">
    Loading...
</h1>

<!-- Jumpscare görüntüsü -->
<img id="scare" src="https://i.imgur.com/hzFJf1q.png">

<!-- Jumpscare sesi -->
<audio id="sound">
    <source src="https://www.myinstants.com/media/sounds/scream_1.mp3" type="audio/mpeg">
</audio>

<script>
    // 2 saniye sonra jumpscare tetikleniyor
    setTimeout(() => {
        document.querySelector("h1").style.display = "none";
        document.getElementById("scare").style.display = "block";
        document.getElementById("sound").play();
    }, 2000);
</script>

</body>
</html>
