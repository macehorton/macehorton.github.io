<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For The Beaches | Full Collection</title>
    <style>
        :root {
            --brand-pink: #FFC0CB;
            --brand-border: #D02090;
            --brand-dark: #800040;
            --footer-height: 60px;
            --header-height: 180px; 
        }

        /* Fluid Layout */
        body {
            margin: 0;
            font-family: 'Arial Black', sans-serif;
            background-color: #ffffff;
            padding-bottom: calc(var(--footer-height) + 40px);
            padding-top: var(--header-height);
            line-height: 1.6;
        }

        /* Fixed Background Logo Overlay */
        .fixed-logo-container {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100vh;
            z-index: -2;
            background-image: url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            opacity: 0.1;
        }

        /* Fixed Top Header (Massive Title) */
        header {
            position: fixed;
            top: 0; left: 0; width: 100%; height: var(--header-height);
            background-color: var(--brand-pink);
            border-bottom: 8px solid var(--brand-border);
            z-index: 3000;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        h1 {
            font-size: clamp(2rem, 8vw, 4.5rem); 
            color: var(--brand-dark);
            margin: 0;
            text-transform: uppercase;
            letter-spacing: 15px; 
            font-weight: 900;
            text-align: center;
        }

        nav {
            width: 100%;
            background-color: var(--brand-dark);
            margin-top: 10px;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            margin: 0; padding: 0;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            min-height: 48px;
            display: flex;
            align-items: center;
            padding: 0 25px;
        }

        /* Product Gallery Section */
        .collection-container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
            text-align: center;
            position: relative;
            z-index: 1;
        }

        .section-headline {
            color: var(--brand-dark);
            text-transform: uppercase;
            font-size: 2.5rem;
            margin-bottom: 40px;
            background: rgba(255, 192, 203, 0.3);
            display: inline-block;
            padding: 10px 30px;
            border-radius: 50px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .product-card {
            background: white;
            border: 3px solid var(--brand-pink);
            border-radius: 15px;
            overflow: hidden;
            padding-bottom: 20px;
            box-shadow: 0 8px 15px rgba(0,0,0,0.1);
        }

        .product-card img {
            width: 100%;
            height: 400px;
            object-fit: cover;
            border-bottom: 3px solid var(--brand-pink);
        }

        .product-title {
            font-size: 1.4rem;
            margin: 15px 0 5px;
            color: var(--brand-dark);
        }

        .product-price {
            font-size: 1.2rem;
            color: var(--brand-border);
            font-weight: bold;
            margin-bottom: 10px;
        }

        .product-sizes {
            font-family: sans-serif;
            font-size: 0.9rem;
            font-weight: bold;
            color: #555;
            margin-bottom: 15px;
        }

        .buy-button {
            background-color: var(--brand-dark);
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 50px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.2s;
        }

        .buy-button:hover {
            transform: scale(1.05);
            background-color: var(--brand-border);
        }

        /* Fixed Footer */
        footer {
            position: fixed;
            bottom: 0; left: 0; width: 100%;
            height: var(--footer-height);
            background-color: var(--brand-dark);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 4000;
            border-top: 3px solid var(--brand-border);
        }
    </style>
</head>
<body>

    <div class="fixed-logo-container"></div>

    <header>
        <h1>FOR THE BEACHES</h1>
        <nav>
            <ul>
                <li><a href="#home">HOME</a></li>
                <li><a href="#collection">COLLECTION</a></li>
                <li><a href="#sale">SALE</a></li>
            </ul>
        </nav>
    </header>

    <main class="collection-container" id="collection">
        <h2 class="section-headline">Explore The Collection</h2>

        <div class="product-grid">
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1596435707700-62645849f05a?auto=format&fit=crop&w=600&q=80" alt="Azure Blue Bikini">
                <div class="product-title">Azure Sky Bikini</div>
                <div class="product-price">$45.00</div>
                <div class="product-sizes">SIZES: S, M, L, XL, XXL, 3XL</div>
                <button class="buy-button">ADD TO CART</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1582533561751-ef6f6ab93a2e?auto=format&fit=crop&w=600&q=80" alt="Midnight Sport Bikini">
                <div class="product-title">Midnight Sport Bikini</div>
                <div class="product-price">$52.00</div>
                <div class="product-sizes">SIZES: S, M, L, XL, XXL, 3XL</div>
                <button class="buy-button">ADD TO CART</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1590650213165-c1fef80648c4?auto=format&fit=crop&w=600&q=80" alt="Paradise Floral Bikini">
                <div class="product-title">Paradise Floral Set</div>
                <div class="product-price">$58.00</div>
                <div class="product-sizes">SIZES: S, M, L, XL, XXL, 3XL</div>
                <button class="buy-button">ADD TO CART</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1568480350417-7e6be952377b?auto=format&fit=crop&w=600&q=80" alt="Classic Coral Bikini">
                <div class="product-title">Classic Coral Two-Piece</div>
                <div class="product-price">$48.00</div>
                <div class="product-sizes">SIZES: S, M, L, XL, XXL, 3XL</div>
                <button class="buy-button">ADD TO CART</button>
            </div>
        </div>
    </main>

    <footer>
        <p>For the Beaches 2026.</p>
    </footer>

</body>
</html>
