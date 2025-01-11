<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href=".styles.css">
    </head>
    <body>
        <div class="container">
          <div >
              <h1 class = "header_text">Hoai bubby c: ! Yes it is I, your girlfriend huehuehue... anywhooooo. I know this isn't my kind of thing but I wanted to do something for you!</h1>
              <h1 class = "header_text">Would you like to be my valentine's?</h1>
          </div>
          <div class="gif_animevalentine">
              <img src="https://tenor.com/view/anime-thanks-love-pink-gif-19009040">
          </div>
          <div class = "buttons">
              <button class="btn" id = "yesButton" onclick="nextPage()">Yes</button>
              <button class="btn" id ="noButton" onmouseover="moveButton()" onclick="moveButton()">No</button>
              <script>
                  function nextPage() {
                      window.location.href = "yes.html";
                  }
                  function moveButton() {
                      var x = Math.random() * (window.innerWidth - document.getElementById('noButton').offsetWidth) - 85;
                      var y = Math.random() * (window.innerHeight - document.getElementById('noButton').offsetHeight) - 48;
                      document.getElementById('noButton').style.left = '${x}px';
                      document.getElementById('noButton').style.top = '${y}px';
                  }
              </script>
          </div>

      </body>
  </html>             
