# Ex.08 Design of Interactive Image Gallery

## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
```
<html>
<head>
    <title> IMAGE GALLERY</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Anton&family=Bebas+Neue&family=Edu+AU+VIC+WA+NT+Arrows:wght@400..700&family=Josefin+Sans:ital,wght@0,100..700;1,100..700&family=Montserrat:ital,wght@0,100..900;1,100..900&family=Raleway:ital,wght@0,100..900;1,100..900&family=Shadows+Into+Light&display=swap" rel="stylesheet">
</head>

<body>
    <div class="first"><CENTER></CENTER>
    <h1 class="heading">
       IMAGE GALLERY
    </h1>
    </div>
    </CENTER>
    <div>
        <center>
        <img src="kamal.jpg" class="img">
        <h3>Kamal Haasan</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="Rajnikanth.webp" class="img">
        <h3>Nayanthara</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="vijayactor.webp" class="img">
        <h3>Vijay</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="ajith.webp" class="img">
        <h3>Ajith Kumar</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="surya.webp" class="img">
        <h3>Surya</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="vikram.webp" class="img">
        <h3>Vikram</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="simbu.webp" class="img">
        <h3>Silambarasan</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="dhanush.jpg" class="img">
        <h3>dhanush</h3>
        </center>
    </div>
    
    <div class="action">
        <img src="" alt="" class="action-image">
        <button class="btn">X</button>
    </div>
    <footer>
        Designed and Developed by YUARAJ M &reg;
    </footer>
    <script>
        const action = document.querySelector('.action');
        const actionImage = document.querySelector('.action-image');
        const closeButton = document.querySelector('.btn');
        const images = document.querySelectorAll('.img');

        images.forEach((image) => {
            image.addEventListener('click', () => {
                actionImage.src = image.src;
                action.classList.add('visible'); 
            });
        });

        closeButton.addEventListener('click', () => {
            action.classList.remove('visible'); 
        });

       action.addEventListener('click', (e) => {
            if (e.target === action) {
                action.classList.remove('visible'); 
            }
        });
    </script>
</body>
</html>
```

## OUTPUT
![alt text](image.png)


## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
