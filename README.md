# Ex.08 Design of Interactive Image Gallery
## Date: 07.10.2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
gallery.html

<html>
    <head>
        <title>
            Interactive Image Gallery
        </title>
        <link rel="stylesheet" href="gallery.css">
    </head>
    <body>
        <h1>My Gallery</h1>
        <h2>Janesha S (25018817)</h2>
        <br><br><br><br><br><br><br>
        <div class="gallery">
            <div class="photos">
                <img src="me.png" >
                <h3>Me!</h3>
            </div>
            <div class="photos">
                <img src="mdu.jpg">
                <h3>My Home</h3>
            </div>
            <div class="photos">
                <img src="food.jpg">
                <h3>Fav Food</h3>
            </div>
            <div class="photos">
                <img src="school.jpg">
                <h3>My School</h3>
            </div>
            <div class="photos">
                <img id="Image" src="clg.jpg" onmouseover="highlight()" onmouseout="removehighlight()">
                <h3>My College</h3>
            </div>
        </div>
        <script type="text/javascript" src="gallery.js"></script>
    </body>
</html>

gallery.css

body{
    background-color: rgb(0, 0, 0);
    color:rgb(254, 131, 17);
    align-items: center;
    text-align: center;
}
body h2{
    color: rgb(255, 206, 137);
    font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif
}
.gallery{
    align-items: center;
    display: grid;
    grid-template-columns: repeat(5,1fr);
    max-width: 1300px;
    margin: 0 auto;
    gap: 10px;
    padding: 20px;
    background-size: 500px;
}
.photos{
    background-color: rgba(216, 126, 52, 0.41);
    background-size: 500px;
    padding: 1px;
    border-radius: 5px;
    text-align: center;
    border: 3px solid #cd7a05;
}
.photos img {
  width: 95%;
  height: auto;
  margin-bottom: 5px;
}
.photos h3 {
  margin: 0;
  font-size: 20px;
  color: #cbffaf;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

gallery.js

function highlight(){
    document.getElementById("Image").style.transform="scale(1.5)";
    document.getElementById("Image").style.trasition="transform 0.5px ease"
    document.getElementById("Image").style.boxShadow="0 0 20px rgba(254, 118, 46, 0.74)";
}
function removehighlight(){
    document.getElementById("Image").style.transform="scale(1)";
    document.getElementById("Image").style.boxShadow="none";
}
```
## OUTPUT:
![alt text](<Screenshot (89).png>)
![alt text](<Screenshot (90).png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
