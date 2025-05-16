# Ex.08 Design of Interactive Image Gallery
## Date:

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
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <link rel="stylesheet" href="styles.css/css">
</head>
<body>
                            <style>
                                body {
                                    font-family: Arial, sans-serif;
                                    margin: 0;
                                    padding: 0;
                                    background-color: #f4f4f4;
                                }
                                header {
                                    background-color: #333;
                                    color: white;
                                    text-align: center;
                                    padding: 1rem;
                                }
                                footer {
                                    background-color: #333;
                                    color: white;
                                    padding: 10px 0;
                                    text-align: center;
                                    position: fixed;
                                    bottom: 0;
                                    width: 100%;
                                }
                                .gallery {
                                    display: grid;
                                    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
                                    gap: 10px;
                                    flex: 1;
                                    padding: 10px;
                                }
                                .gallery-item {
                                    position: relative;
                                    overflow: hidden;
                                    border-radius: 5px;
                                    cursor: pointer;
                                }
                                .gallery-item img {
                                    width: 100%;
                                    height: auto;
                                    transition: transform 0.3s ease;
                                }
                                .gallery-item:hover img {
                                    transform: scale(1.1);
                                }
                                .gallery-item .caption {
                                    position: absolute;
                                    bottom: 0;
                                    background: rgba(0, 0, 0, 0.7);
                                    color: white;
                                    width: 100%;
                                    text-align: center;
                                    padding: 0.5rem;
                                    opacity: 0;
                                    transition: opacity 0.3s ease;
                                }
                                .gallery-item:hover .caption {
                                    opacity: 1;
                                }
                                #modal {
                                    display: none;
                                    position: fixed;
                                    top: 0;
                                    left: 0;
                                    width: 100%;
                                    height: 100%;
                                    background: rgba(0, 0, 0, 0.8);
                                    justify-content: center;
                                    align-items: center;
                                    z-index: 1000;
                                }
                                #modal img {
                                    max-width: 90%;
                                    max-height: 90%;
                                }
                                #modal.close {
                                    position: absolute;
                                    top: 20px;
                                    right: 20px;
                                    font-size: 1.5rem;
                                    color: white;
                                    cursor: pointer;
                                }
                            </style>
                        </head>
                        <body>
                            <header>
                                <h1>7 Wonders Gallery</h1>
                            </header>
                            <div class="gallery">
                                <div class="gallery-item" onclick="openModal('image1.jpg')">
                                    <img src="c:\\Users\\admin\\Desktop\\image gallery\\colosseum-202004-1587656297.avif" alt="Image 1">
                                    <div class="caption">Colosseum</div>
                                </div>
                                <div class="gallery-item" onclick="openModal('image2.jpg')">
                                    <img src="c:\\Users\\admin\\Desktop\\image gallery\\itza_461.avif" alt="Image 2">
                                    <div class="caption">Itza</div>
                                </div>
                                <div class="gallery-item" onclick="openModal('image3.jpg')">
                                    <img src="c:\\Users\\admin\\Desktop\\image gallery\\Petra-1200x853.jpg" alt="Image 3">
                                    <div class="caption">Petra</div>
                                </div>
                                <div class="gallery-item" onclick="openModal('image4.jpg')">
                                    <img src="c:\\Users\\admin\\Desktop\\image gallery\\taj-mahal-202004-1587656298.avif" alt="Image 4">
                                    <div class="caption">Taj Mahal</div>
                                </div>
                                <div class="gallery-item" onclick="openModal('image4.jpg')">
                                    <img src="C:\Users\admin\Desktop\image gallery\360-christ-superJumbo.jpg" alt="Image 5">
                                    <div class="caption">Christ</div>
                                </div>
                                <!-- Add more gallery items here -->
                            </div>
                        
                            <div id="modal">
                                <span class="close" onclick="closeModal()">&times;</span>
                                <img id="modal-image" src="" alt="">
                            </div>

                            <footer>
                               <h3> &copy; 2024.   7 Wonders Gallery.    All rights reserved.</h3>
                            </footer>
                        
                            <script>
                                function openModal(imageSrc) {
                                    const modal = document.getElementById('modal');
                                    const modalImage = document.getElementById('modal-image');
                                    modal.style.display = 'flex';
                                    modalImage.src = imageSrc;
                                }
                        
                                function closeModal() {
                                    const modal = document.getElementById('modal');
                                    modal.style.display = 'none';
                                }
                            </script>
</body>
</html>
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/02a13ba4-83b1-4daf-b2c8-97b76fa2a5ed)
![image](https://github.com/user-attachments/assets/2c5fab80-e6fa-47e5-b63d-d103b0beac47)
![image](https://github.com/user-attachments/assets/234c3448-409b-448f-853f-e7b934e148ee)
![image](https://github.com/user-attachments/assets/ef7a0a68-9f9d-4308-b8f4-f21fa7ef56b7)





## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully..
