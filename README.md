# Ex.07 Restaurant Website
## Date:07.10.2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dindigul Thalappakatti Biriyani - Since 1957</title>
    <style>
        /* Basic Styling to suggest the look (for this HTML file only) */
        body {
            font-family: 'Times New Roman', serif;
            margin: 0;
            padding: 0;
            color: #13068f;
            background-color: #c58b3a; /* Cream background */
        }
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }
        header {
            background-color: #faabed; /* Deep Maroon color */
            color: rgb(50, 3, 71);
            padding: 10px 0;
        }
        header h1 {
            font-size: 2.5em;
            text-align: center;
            margin: 10px 0;
            letter-spacing: 2px;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            justify-content: center;
        }
        nav ul li a {
            color: #660a0a; /* Gold/Saffron for links */
            text-decoration: none;
            padding: 10px 20px;
            display: block;
            font-weight: bold;
            text-transform: uppercase;
        }
        .hero-section {
            background: url('biriyani_image_placeholder.jpg') no-repeat center center/cover;
            height: 400px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            margin-bottom: 30px;
            position: relative;
        }
        .hero-overlay {
            background-color: rgba(0, 0, 0, 0.6);
            padding: 40px;
            color: rgb(21, 199, 15);
        }
        .hero-overlay h2 {
            font-size: 3em;
            color: #ffcc00;
            margin-top: 0;
        }
        .hero-overlay p {
            font-size: 1.2em;
        }
        .section-title {
            text-align: center;
            color: #566805;
            font-size: 2em;
            margin: 40px 0 20px;
            border-bottom: 2px solid #ffcc00;
            padding-bottom: 10px;
        }
        .menu-grid {
            display: flex;
            justify-content: space-between;
            gap: 20px;
            margin-bottom: 50px;
        }
        .menu-category {
            flex: 1;
            background-color: rgb(159, 219, 141);
            padding: 20px;
            border: 1px solid #e0e0e0;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .menu-category h3 {
            color: #480af3;
            border-bottom: 1px dashed #ffcc00;
            padding-bottom: 10px;
            margin-top: 0;
        }
        .item-name {
            font-weight: bold;
            color: #333;
            margin-top: 10px;
        }
        .item-description {
            font-size: 0.9em;
            color: #666;
            margin-bottom: 15px;
        }
        .cta-button {
            display: block;
            width: 250px;
            margin: 20px auto 50px;
            padding: 15px;
            background-color: #ffcc00;
            color: #cc690d;
            text-align: center;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .cta-button:hover {
            background-color: #95dab4;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 30px;
        }
    </style>
</head>
<body>

    <header>
        <div class="container">
            <h1>DINDIGUL THALAPPAKATTI</h1>
            <img src="ul.png" width="600" height="600">
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#story">Our Story</a></li>
                    <li><a href="#menu">Full Menu</a></li>
                    <li><a href="#locations">Locations</a></li>
                    <li><a href="#order">Order Online</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">

        <section id="home" class="hero-section" style="background-image: url(' deepika/foodapp/static/ul.png ');">
            <div class="hero-overlay">
                <h2>Legendary Biriyani, Since 1957</h2>
                <p>Taste the authentic flavor of Seeraga Samba rice and hand-ground spices that started a tradition.</p>
                <a href="#order" class="cta-button">Order Your Biriyani Now</a>
            </div>
        </section>

        <section id="story">
            <h2 class="section-title">Our Legendary Story</h2>
            <p style="text-align: center; line-height: 1.6;">
                The roots of Thalappakatti trace back to 1957 in Dindigul. Our founder, Mr. Nagasamy Naidu,
                always wore a traditional turban called a 'Thalappa,' which became synonymous with his unique
                cooking style and the restaurant's name. We carry forward his legacy, using a secret recipe
                and traditional 'DUM' style of cooking to deliver the world's most aromatic biriyani.
            </p>
        </section>

        <section id="menu">
            <h2 class="section-title">The Star Attractions</h2>

            <div class="menu-grid">
                
                <div class="menu-category">
                    <h3>Signature Biriyanis</h3>
                    
                    <div class="menu-item">
                    <img src="mb.png" width="400" height="200">

                        <div class="item-name">Thalappakatti Naidu Mutton Biriyani</div>
                        <div class="item-description">Succulent pieces of baby goat meat cooked with fragrant Seeraga Samba rice.</div>
                    </div>
                    
                    <div class="menu-item">
                    <img src="cb.png" width="400" height="200">
                        <div class="item-name">Thalappakatti Chicken Biriyani</div>
                        <div class="item-description">The iconic chicken biriyani, served with raita and gravy.</div>
                    </div>
                    
                    <div class="menu-item">
                    <img src="pb.png" width="400" height="200">
                        <div class="item-name">Kuska (Plain Biriyani Rice)</div>
                        <div class="item-description">Aromatic seeraga samba rice cooked to perfection, without the meat.</div>
                    </div>
                </div>

                <div class="menu-category">
                    <h3>Must-Try Starters</h3>
                    
                    <div class="menu-item">
                    <img src="ko.png" width="400" height="200">
                        <div class="item-name">Mutton Kola Urundai (Meatballs)</div>
                        <div class="item-description">Spicy minced lamb meatballs, a famous South Indian starter.</div>
                    </div>
                    
                    <div class="menu-item">
                    <img src="c65.png" width="400" height="200">
                        <div class="item-name">Chicken 65</div>
                        <div class="item-description">Crispy fried chicken chunks marinated in a special mix of spices.</div>
                    </div>
                    
                    <div class="menu-item">
                    <img src="ff.png" width="400" height="200">
                        <div class="item-name">Fish Fry (Vanjaram)</div>
                        <div class="item-description">King Fish slices marinated and shallow-fried in traditional masala.</div>
                    </div>
                </div>

                <div class="menu-category">
                    <h3>Curries & Combos</h3>
                    
                    <div class="menu-item">
                    <img src="mp.png" width="400" height="200">
                        <div class="item-name">Nellai Mutton Paya (Trotters)</div>
                        <div class="item-description">A rich, comforting curry best paired with Idiyappam or Parotta.</div>
                    </div>
                    
                    <div class="menu-item">
                    <img src="cg.png" width="400" height="200">
                        <div class="item-name">Chicken Gravy</div>
                        <div class="item-description">A spicy side dish to complement the Biriyani experience.</div>
                    </div>
                    
                    <div class="menu-item">
                    <img src="bh.png" width="400" height="200">
                        <div class="item-name">Bread Halwa</div>
                        <div class="item-description">A traditional, rich bread-based dessert.</div>
                    </div>
                </div>

            </div>

        </section>

        <section id="locations">
            <h2 class="section-title">Global Presence</h2>
            <p style="text-align: center;">With over 105+ outlets globally, including locations across India, Sri Lanka, Singapore, and UAE, we are bringing the taste of Dindigul to the world.</p>
            
            <address style="text-align: center; margin-top: 20px;">
                <strong>Headquarters:</strong> Chennai, Tamil Nadu, India<br>
                <strong>Customer Care:</strong> 1800-XXX-XXXX<br>
                <strong>Email:</strong> <a href="mailto:info@thalappakatti.com" style="color: #0e1b8f;">info@thalappakatti.com</a>
            </address>s
        </section>

    </main>

    <footer>
        <p>&copy; 2025 Dindigul Thalappakatti Restaurant. All rights reserved. | Legendary Biriyani Since 1957.</p>
    </footer>

</body>
</html>

```

## OUTPUT:
![alt text](<Screenshot 2025-10-07 222431.png>)  
![alt text](<Screenshot 2025-10-07 222515.png>)
<img width="1272" height="187" alt="Screenshot 2025-10-07 223826" src="https://github.com/user-attachments/assets/792c9b35-19a6-42b8-bfc1-3db1d012414a" />
![alt text](<Screenshot 2025-10-07 222554.png>)
![alt text](<Screenshot 2025-10-07 222617.png>)
![alt text](<Screenshot 2025-10-07 222657.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
