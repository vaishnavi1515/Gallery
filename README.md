# Ex.08 Design of Interactive Image Gallery
# Date:
# AIM:15/11/2024
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
~~~
<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width , initial-scale=1.0">
    <title>Image Gallery</title>
    <link rel="stylesheet" href="image gallery.css">
</head>
<body>
    <div class="full-img" id="fullImgBox">
        <img src="img gallery-1.jpg" id="fullImg">
        <span onclick="closeFullImg()">X</span>
    </div>

    <div class="img-gallery">
        <img src="c:\Users\admin\Documents\restaraunt\peacock.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Documents\dog.jpeg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Documents\flower.jpeg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Documents\butterflies.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Documents\baby.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Documents\restaraunt\mojito.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Documents\restaraunt\rabbit.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Documents\restaraunt\tiger.jpg" onclick="openFullImg(this.src)">
        <img src=" c:\Users\admin\Documents\girll.jpg" onclick="openFullImg(this.src)">
    </div>

<script>
    var fullImgBox = document.getElementById("fullImgBox");
    var fullImg = document.getElementById("fullImg");

    function openFullImg(pic){
        fullImgBox.style.display="flex";
        fullImg.src = pic;
    }

    function closeFullImg(){
        fullImgBox.style.display="none";

    }
</script>
</body>
</html>


*{
    margin: 0;
    padding: 0;
    font-family:sans-serif;
}
body{
    background: #ecf4fb;
}
.img-gallery{
    width: 70%;
    margin: 100px auto 50px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
    grid-gap:30px;
}
.img-gallery img{
    width: 300px;
    height: 300px;
    cursor:pointer;
}
.img-gallery img:hover{
    transform: scale(0.8) rotate(-25deg);
    border-radius: 20px;
    box-shadow: 0 32px 75px rgba(68,77,136,0.2);

}
.full-img{
    width: 100%;
    height: 100vh;
    background: rgba(0,0,0,0.9);
    position: fixed;
    top: 0;
    left: 0;
    display: none;
    align-items: center;
    justify-content: center;
    z-index: 100;

}
.full-img img{
    width: 90%;
    max-width: 500px;
}
.full-img span{
    position: absolute;
    top: 5%;
    right: 5%;
    font-size: 30px;
    color: #fff;
    cursor:pointer;

}
~~~
# OUTPUT:
![Screenshot (44)](https://github.com/user-attachments/assets/f0063f7d-69f7-4443-8a53-fa98c16aa00f)
![Screenshot 2024-12-27 233933](https://github.com/user-attachments/assets/01c9acd8-cb36-4838-9a82-ca30e87bfb93)
![Screenshot 2024-12-27 234015](https://github.com/user-attachments/assets/57b842ee-b0b9-45b2-96aa-1f933e98d585)
![Screenshot 2024-12-27 234047](https://github.com/user-attachments/assets/70192ef0-e3f5-4f87-8e44-3f1bef3d6947)
![Screenshot 2024-12-27 234117](https://github.com/user-attachments/assets/349ea5f3-0da5-4c98-83a1-0ce5532f659e)
![Screenshot 2024-12-27 234138](https://github.com/user-attachments/assets/35d94721-db1c-497b-929f-cc0b872146f3)
![Screenshot 2024-12-27 234204](https://github.com/user-attachments/assets/712e036e-23e9-4bc5-9d35-de4396ec8d30)
![Screenshot 2024-12-27 234235](https://github.com/user-attachments/assets/1bb50097-0ca5-40d4-900f-ae5815dabb44)
![Screenshot (45)](https://github.com/user-attachments/assets/56647f24-0d76-4a06-913d-2a1845860c19)
![Screenshot (47)](https://github.com/user-attachments/assets/37492c71-5406-45ab-9dc8-ef4f0e879a8b)

# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
