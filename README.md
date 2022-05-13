
<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8">
  <title>Yukki Music Bot</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta http-equiv="X-UA-Compatible" content="ie=edge"><link rel="stylesheet" href="./style.css">

</head>
<body>
<!-- partial:index.partial.html -->
<script async defer src="https://buttons.github.io/buttons.js"></script>
<div class="container">
    <div class="card">
        <h1 align="center" class="card_title"><b>Yukki Music Bot</b></h1>
        <p align="center"><a class="github-button" href="https://github.com/TeamYukki/YukkiMusicBot/fork" data-color-scheme="no-preference: light; light: dark; dark: dark_dimmed;" data-size="large" data-show-count="true" aria-label="Fork NotReallyShikhar/YukkiMusicBot on GitHub">Fork</a></p>
        <p align="center">
            <a href="https://t.me/TeamYukki"> Channel </a> •
            <a href="https://notreallyshikhar.gitbook.io/yukkimusicbot/about/getting-started"> Documentation </a> •
            <a href="https://t.me/YukkiSupport"> Support </a> 
        </p>
        <p align="center" class="card_title-info">Deploy Yukki Music Bot to Heroku</p>
        <br>
        <form class="card_form">
            <div class="input">
                <input type="text" class="input_field" required id="myInput"/>
                <label class="input_label">Input Your Forked Repo Link</label>
            </div>
            <button class="card_button" onclick="getInputValue();">Deploy Now </button>
        </form>
    </div>
    <script> 
        function getInputValue(){
            var inputVal = document.getElementById("myInput").value;
            if (inputVal == "") {
                return alert("Provide your forked github repo link.");
            }
            if (inputVal.includes("TeamYukki")) {
                return alert("You can't deploy Yukki Music Bot Official Repo as it has been blacklisted by Heroku. Simply Fork the YukkiMusicBot Repo and Input your Fork Repo Link Here");
            } else {
                if (inputVal.includes("https://github.com/")) {
                    her = "https://dashboard.heroku.com/new?template=";
                    herokulink = her.concat(inputVal);
                    window.open(herokulink,"blank");
                } else {
                    return alert("Input Github Link starting with https only!");
                }
            }
        }
    </script>
    
<!-- partial -->
</div>
<script data-name="BMC-Widget" data-cfasync="false" src="https://cdnjs.buymeacoffee.com/1.0.0/widget.prod.min.js" data-id="notreallysY" data-description="Support me on Buy me a coffee!" data-message="" data-color="#ff813f" data-position="Right" data-x_margin="18" data-y_margin="18"></script>



</body>
</html>
