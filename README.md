<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For The Beaches | Women's Swimwear Shop</title>
    <meta name="description" content="Shop the latest in women's sustainable swimwear at For The Beaches. High-quality bikinis and one-pieces.">

    <style>
        :root {
            --brand-pink: #FFC0CB;
            --brand-border: #D02090;
            --brand-dark: #800040;
            --footer-height: 60px;
        }

        body {
            margin: 0;
            font-family: 'Helvetica Neue', Arial, sans-serif;
            line-height: 1.6;
            background-color: #ffffff;
            padding-bottom: var(--footer-height);
        }

        /* Fixed Background Logo (Entire Page) */
        .fixed-logo-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100vh;
            z-index: -1;
            background-image: url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            opacity: 0.3;
        }

        /* Navigation - Accessible 48px targets */
        nav {
            background-color: var(--brand-dark);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            margin: 0;
            padding: 0;
            flex-wrap: wrap;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            min-height: 48px;
            display: flex;
            align-items: center;
            padding: 0 20px;
        }

        /* Shopping Layout */
        .content-wrapper {
            margin-top: 60vh; /* Show top logo banner first */
            background-color: white;
            position: relative;
            z-index: 1;
            padding: 40px 20px;
            border-top: 8px solid var(--brand-border);
        }

        .shop-header {
            text-align: center;
            margin-bottom: 40px;
        }

        h1 {
            font-size: 3rem;
            color: var(--brand-dark);
            margin: 0;
            text-transform: uppercase;
        }

        /* Product Grid - Fluid for Mobile/Desktop */
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .product-card {
            border: 2px solid #eee;
            border-radius: 12px;
            overflow: hidden;
            text-align: center;
            padding-bottom: 20px;
            transition: transform 0.3s;
        }

        .product-card:hover {
            transform: translateY(-5px);
            border-color: var(--brand-pink);
        }

        .product-card img {
            width: 100%;
            height: 350px;
            object-fit: cover;
        }

        .product-title {
            font-size: 20px;
            font-weight: bold;
            margin: 15px 0 5px;
            color: var(--brand-dark);
        }

        .product-price {
            font-size: 18px;
            color: #666;
            margin-bottom: 15px;
        }

        /* CTA - Shop Button */
        .add-to-cart {
            background-color: var(--brand-border);
            color: white;
            padding: 12px 25px;
            border: none;
            border-radius: 50px;
            font-weight: bold;
            cursor: pointer;
            text-decoration: none;
            display: inline-block;
        }

        .add-to-cart:hover {
            background-color: var(--brand-dark);
        }

        /* Fixed Footer */
        footer {
            position: fixed;
            bottom: 0;
            width: 100%;
            height: var(--footer-height);
            background-color: var(--brand-dark);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 2000;
        }
    </style>
</head>
<body>

    <div class="fixed-logo-container"></div>

    <nav>
        <ul>
            <li><a href="#new">NEW ARRIVALS</a></li>
            <li><a href="#bikinis">BIKINIS</a></li>
            <li><a href="#one-pieces">ONE-PIECES</a></li>
            <li><a href="#sale">SALE</a></li>
        </ul>
    </nav>

    <div class="content-wrapper">
        <header class="shop-header">
            <h1>FOR THE BEACHES</h1>
            <p>Sustainable. Stylish. Women's Swimwear.</p>
        </header>

        <main class="product-grid">
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1596435707700-62645849f05a?auto=format&fit=crop&w=500&q=80" alt="Sustainable turquoise bikini set">
                <div class="product-title">Azure Two-Piece</div>
                <div class="product-price">$45.00</div>
                <button class="add-to-cart">Add to Cart</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1590650213165-c1fef80648c4?auto=format&fit=crop&w=500&q=80" alt="Floral print one-piece swimsuit">
                <div class="product-title">Tropical One-Piece</div>
                <div class="product-price">$65.00</div>
                <button class="add-to-cart">Add to Cart</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1582533561751-ef6f6ab93a2e?auto=format&fit=crop&w=500&q=80" alt="Sporty high-waisted black bikini">
                <div class="product-title">Midnight Sport Bikini</div>
                <div class="product-price">$50.00</div>
                <button class="add-to-cart">Add to Cart</button>
            </div>
        </main>
    </div>

    <footer>
        <p>&copy; 2026 For The Beaches | Secure Checkout Available</p>
    </footer>

</body>
</html>
