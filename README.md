# Ex-7: Interactive Image Gallery
## Date: 09-11-2024

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:

### index.html
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Photo Gallery</title>
  <link rel="stylesheet" href="style.css">
</head>

<body>
  <h1>Interactive Photo Gallery</h1>
  <div id="image">Hover over an image below to display here.</div>

  <div class="gallery">
    <img class="preview" alt="White Dog" src="https://images.pexels.com/photos/3196887/pexels-photo-3196887.jpeg?auto=compress&cs=tinysrgb&w=600" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" alt="blonde Dog" src="https://images.pexels.com/photos/14730839/pexels-photo-14730839.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" src="https://images.pexels.com/photos/11683755/pexels-photo-11683755.jpeg?auto=compress&cs=tinysrgb&w=600" alt="Dogs" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" alt="Cap" src="https://images.pexels.com/photos/4588052/pexels-photo-4588052.jpeg?auto=compress&cs=tinysrgb&w=600" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" alt="Couples" src="https://images.pexels.com/photos/6291572/pexels-photo-6291572.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover="upDate(this)" onmouseout="unDo()">
    <img class="preview" src="https://images.pexels.com/photos/8192220/pexels-photo-8192220.jpeg?auto=compress&cs=tinysrgb&w=600" alt="Cuties" onmouseover="upDate(this)" onmouseout="unDo()">
  </div>
  <script src="script.js"></script>
</body>

</html>
```

### gallery.css
```
body {
  margin: 2%;
  border: 1px solid black;
  background-color: #b3b3b3;
}
#image {
  line-height: 650px;
  width: 575px;
  height: 650px;
  border: 5px solid black;
  margin: 0 auto;
  background-color: #8e68ff;
  background-image: url("");
  background-repeat: no-repeat;
  color: #ffffff;
  text-align: center;
  background-size: 100%;
  margin-bottom: 25px;
  font-size: 150%;
}
.preview {
  width: 10%;
  margin-left: 17%;
  border: 10px solid black;
}
img {
  width: 95%;
}

```

### gallery.js
```
// Reference to the image container
const imageDiv = document.getElementById("image");
const originalImageUrl = ""; // Set this to the URL of your original image
const originalText = "Hover over an image below to display here."; // Original text

function upDate(previewPic) {
  // Change the background image to the source of the hovered image
  imageDiv.style.backgroundImage = `url('${previewPic.src}')`;

  // Update the text to the alt text of the hovered image
  imageDiv.innerHTML = previewPic.alt;
}

function unDo() {
  // Reset the background image to the original URL
  imageDiv.style.backgroundImage = `url('${originalImageUrl}')`; // Use the original image URL here

  // Change the text back to the original text
  imageDiv.innerHTML = originalText;
}

```
## WEBSITE URL
```
https://codepen.io/Anbu-Selvan-the-looper/pen/WNVYzRX
```
## OUTPUT:

![Screenshot (66)](https://github.com/user-attachments/assets/0bc39570-100e-4b1d-a049-67f4eded1fa8)


![Screenshot (67)](https://github.com/user-attachments/assets/d4bb66dc-024a-4476-be54-7d4d8e6b9e38)





## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
