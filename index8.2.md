1. HTML file — index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>My Photo Gallery</h1>
        <p>A beautiful responsive image collection</p>
    </header>

    <main class="gallery">

        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?auto=format&fit=crop&w=800&q=80" alt="Mountain landscape">
            <h3>Mountain View</h3>
        </div>

        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?auto=format&fit=crop&w=800&q=80" alt="Lake and mountains">
            <h3>Beautiful Lake</h3>
        </div>

        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=800&q=80" alt="Nature scenery">
            <h3>Nature</h3>
        </div>

        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1470252649378-9c29740c9fa8?auto=format&fit=crop&w=800&q=80" alt="Sunrise landscape">
            <h3>Sunrise</h3>
        </div>

        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?auto=format&fit=crop&w=800&q=80" alt="Green forest">
            <h3>Green Forest</h3>
        </div>

        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=800&q=80" alt="Beach and ocean">
            <h3>Beach</h3>
        </div>

        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1518837695005-2083093ee35b?auto=format&fit=crop&w=800&q=80" alt="Ocean waves">
            <h3>Ocean Waves</h3>
        </div>

        <div class="gallery-item">
            <img src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?auto=format&fit=crop&w=800&q=80" alt="Snowy mountains">
            <h3>Snowy Mountains</h3>
        </div>

    </main>

    <footer>
        <p>Created for Assignment 8.2 | Responsive Image Gallery</p>
    </footer>

</body>
</html>



2. CSS file — style.css

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f1f5f9;
    color: #1e293b;
}

/* Header */
header {
    text-align: center;
    background-color: #1d4ed8;
    color: white;
    padding: 30px 15px;
}

header h1 {
    margin-bottom: 10px;
    font-size: 32px;
}

/* Responsive Gallery */
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    padding: 25px;
    max-width: 1400px;
    margin: auto;
}

/* Gallery Items */
.gallery-item {
    background-color: white;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 4px 10px #00000015;
    transition: transform 0.3s ease;
}

.gallery-item:hover {
    transform: translateY(-5px);
}

/* Images */
.gallery-item img {
    width: 100%;
    height: 220px;
    object-fit: cover;
    display: block;
}

.gallery-item h3 {
    text-align: center;
    padding: 15px;
    font-size: 18px;
}

/* Footer */
footer {
    text-align: center;
    background-color: #1e293b;
    color: white;
    padding: 20px;
    margin-top: 20px;
}

/* Mobile Screens */
@media (max-width: 500px) {
    .gallery {
        grid-template-columns: 1fr;
        padding: 15px;
        gap: 15px;
    }

    header h1 {
        font-size: 25px;
    }

    .gallery-item img {
        height: 200px;
    }
}



3. How to run your assignment
1. Create a folder named Assignment-8.2.
2. Create index.html and style.css inside it.
3. Copy the HTML code into index.html.
4. Copy the CSS code into style.css.
5. Save both files and open index.html in Chrome.
6. Ensure you have an internet connection because the images load from online URLs.
4. Expected gallery design




















8








5. Assignment checklist
- [x] At least 8 images included.
- [x] Each image placed inside a gallery item.
- [x] grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)) used.
- [x] Images use width: 100% and object-fit: cover.
- [x] Consistent spacing with gap.
- [x] Mobile-friendly layout added.
- [ ] Test the gallery at desktop and mobile widths.
- [ ] Capture desktop and mobile screenshots.