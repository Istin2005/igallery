# Ex.08 Design of Interactive Image Gallery
## Date:1-11-2024

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
##HTML
```
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Satisfy&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="{% static 'css/style.css' %}">
</head>
<body>
    <h1 style="font-family: 'Satisfy', cursive; text-align: center; margin-bottom: 20px;">Interactive Image Gallery</h1>
    
    <div class="gallery">
        <div class="gallery-item">
            <img src="{% static 'img/i1.jpg' %}" alt="">
            <p>Blue Jay</p>
        </div>
        <div class="gallery-item">
            <img src="{% static 'img/i2.jpg' %}" alt="">
            <p>Ara macao</p>
        </div>
        <div class="gallery-item">
            <img src="{% static 'img/i3.jpg' %}" alt="">
            <p>Arafed red bird</p>
        </div>
        <div class="gallery-item">
            <img src="{% static 'img/i4.jpg' %}" alt="">
            <p>Bright Exotic Bird</p>
        </div>
        <div class="gallery-item">
            <img src="{% static 'img/i5.jpg' %}" alt="">
            <p>Humming Bird</p>
        </div>
        <div class="gallery-item">
            <img src="{% static 'img/i6.jpg' %}" alt="">
            <p>Blue Birds</p>
        </div>
        <div class="gallery-item">
            <img src="{% static 'img/i7.jpg' %}" alt="">
            <p>Parrot</p>
        </div>
        <div class="gallery-item">
            <img src="{% static 'img\i9.jpg' %}" alt="">
            <p>Cockatoo</p>
        </div>
    </div>
</body>
</html>

```

##css
```
body {
    font-family: 'Satisfy', cursive;
    margin: 0;
    padding: 0;
    background-color: #f8f8f8;
    color: #333;
}

h1 {
    font-size: 10rem;
    margin-top: 250px;
    margin-bottom: 1000px;
}

.gallery {
    display: flex;
    flex-wrap: wrap; /* Allows images to wrap to the next row if they don’t fit */
    gap: 100px; /* Adds space between gallery items */
    justify-content: center; /* Center the gallery in the window */
    padding: 20px;
}

.gallery-item {
    position: relative;
    width: 20%; /* 3 images per row */
    height: auto; /* Allow height to be automatic based on image aspect ratio */
    overflow: hidden; /* Hide parts of the image that overflow */
    border-radius: 10px; /* Smooth corners */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease-in-out;
    margin-bottom: 15px; /* Space between rows */
}

.gallery-item:hover {
    transform: scale(1.1); /* Slight zoom effect on hover */
}

.gallery-item img {
    width: 100%; /* Make the image fit the gallery item */
    height: 100%; /* Ensure the image stretches vertically to fill the space */
    object-fit: cover; /* Crop the image to fill the area */
    border-radius: 10px;
}

.gallery-item p {
    position: absolute;
    bottom: 10px;
    left: 0;
    right: 0;
    text-align: center;
    font-size: 2.5rem;
    color: #fff;
    background: rgba(0, 0, 0, 0.6); /* Semi-transparent background */
    padding: 5px;
    margin: 0;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
}

```

## OUTPUT:
![Screenshot (334)](https://github.com/user-attachments/assets/6e009e2e-59e0-4cdd-8afe-9956ea87a07b)
![Screenshot (340)](https://github.com/user-attachments/assets/a28805dc-7f41-4fd4-a6d2-fd9ebdc8a750)






## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
