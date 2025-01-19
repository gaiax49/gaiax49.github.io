<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Valentine's Surprise</title>
        <link rel="stylesheet" href="./styles.css">
        <style>
            /* Inline CSS for dynamic button positioning */
            #noButton {
                position: absolute; /* Required for dynamic positioning */
            }
        </style>
    </head>
    <body>
        <div class="container">
            <div>
                <h1 class="header_text">
                    Hoai bubby c: ! Yes it is I, your girlfriend huehuehue...
                    anywhooooo. I know this isn't my kind of thing but I wanted to do something for you!
                </h1>
                <h1 class="header_text">Would you like to be my valentine's?</h1>
            </div>
            <div class="gif_animevalentine">
                <img src="https://c.tenor.com/u-WBOLnVe1IAAAAC/anime-thanks-love.gif" 
                     alt="A cute anime character blushing and saying thanks with love hearts" 
                     width="300" />
            </div>
            <div class="buttons">
                <button class="btn" id="yesButton" onclick="nextPage()">Yes</button>
                <button class="btn" id="noButton" 
                        onmouseover="moveButton()" 
                        onclick="moveButton()">No</button>
            </div>
        </div>
        <script>
            // Navigate to the "Yes" page when the "Yes" button is clicked
            function nextPage() {
                window.location.href = "yes.html";
            }

            // Move the "No" button to a random position within the viewport
            function moveButton() {
                // Reference the "No" button
                var noButton = document.getElementById('noButton');
                
                // Get the maximum allowed coordinates
                var maxX = window.innerWidth - noButton.offsetWidth;
                var maxY = window.innerHeight - noButton.offsetHeight;
                
                // Randomly generate new positions within the boundaries
                var x = Math.random() * maxX;
                var y = Math.random() * maxY;

                // Apply the new positions to the button
                noButton.style.left = `${x}px`;
                noButton.style.top = `${y}px`;
            }
        </script>
    </body>
</html>
