<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Valentine's Surprise</title>
        <!-- Link to external CSS -->
        <link rel="stylesheet" href="styles.css">
    </head>
    <body>
        <!-- Container for all content -->
        <div class="container">
            <!-- Text section -->
            <div>
                <h1 class="header_text">
                    Hoai bubby c: ! Yes it is I, your girlfriend huehuehue...
                    anywhooooo. I know this isn't my kind of thing but I wanted to do something for you!
                </h1>
                <h1 class="header_text">Would you like to be my valentine's?</h1>
            </div>

            <!-- GIF section -->
            <div class="gif_container">
                <img src="https://c.tenor.com/u-WBOLnVe1IAAAAC/anime-thanks-love.gif" 
                     alt="An anime character blushing and saying thanks with love hearts" 
                     width="300">
            </div>

            <!-- Buttons section -->
            <div class="buttons">
                <button class="btn" id="yesButton" onclick="nextPage()">Yes</button>
                <button class="btn" id="noButton" 
                        onmouseover="moveButton()" 
                        onclick="moveButton()">No</button>
            </div>
        </div>

        <!-- JavaScript functionality -->
        <script>
            // Redirect to "Yes" page when the Yes button is clicked
            function nextPage() {
                window.location.href = "yes.html";
            }

            // Move the "No" button to a random position on hover or click
            function moveButton() {
                var noButton = document.getElementById('noButton');
                var maxX = window.innerWidth - noButton.offsetWidth;
                var maxY = window.innerHeight - noButton.offsetHeight;
                var x = Math.random() * maxX;
                var y = Math.random() * maxY;
                noButton.style.left = `${x}px`;
                noButton.style.top = `${y}px`;
            }
        </script>
    </body>
</html>
