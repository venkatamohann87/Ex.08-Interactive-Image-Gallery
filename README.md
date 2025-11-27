# Ex.08 Interactive Image Gallery
## Date: 22.11.2025

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
<!DOCTYPE html>
<html>
<head>
    <title>Superbikes Image Gallery</title>

    <style>
        body{
            background:#111;
            font-family:Arial, Helvetica, sans-serif;
            color:white;
            text-align:center;
        }

        h1{
            margin-top:20px;
            font-size:40px;
        }

        /* small images row */
        .gallery{
            width:80%;
            margin:auto;
            margin-top:30px;
            display:flex;
            flex-wrap:wrap;
            justify-content:center;
            gap:15px;
        }

        .gallery img{
            width:220px;
            height:220px;
            border-radius:10px;
            cursor:pointer;
            transition:0.3s;
            object-fit:cover;
        }

        .gallery img:hover{
            transform:scale(1.05);
        }

        /* big preview */
        .preview{
            margin-top:25px;
            display:none;
        }

        .preview img{
            width:500px;
            max-width:90%;
            border-radius:10px;
            object-fit:cover;
        }

        footer{
            margin-top:40px;
            padding:10px;
        }
    </style>
</head>
<body>

    <h1>SUPERBIKES GALLERY</h1>

    <!-- Thumbnails -->
    <div class="gallery">
        <!-- Replace these filenames with your own superbike images -->
        <img src="r1.jpg"      alt="Yamaha R1"        onclick="show(this)">
        <img src="panigale.jpg" alt="Ducati Panigale" onclick="show(this)">
        <img src="ninja-h2r.jpg" alt="Kawasaki Ninja H2R" onclick="show(this)">
        <img src="s1000rr.jpg" alt="BMW S1000RR"     onclick="show(this)">
        <img src="rc390.jpg"   alt="KTM RC390"       onclick="show(this)">
    </div>

    <!-- Big image -->
    <div class="preview" id="bigbox">
        <img id="bigimg">
    </div>

    <footer>
        DESIGNED &amp; DEVELOPED BY <b>VENKATA MOHAN N</b>
    </footer>

    <script>
        function show(img){
            // show big preview box
            document.getElementById("bigbox").style.display = "block";
            // set big image src to clicked image
            document.getElementById("bigimg").src = img.src;
        }
    </script>

</body>
</html>


```
## OUTPUT:

![WhatsApp Image 2025-11-27 at 11 52 01_9d185eea](https://github.com/user-attachments/assets/9f7cdc98-2254-44c0-bf63-3f58d1c27ebc)



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
