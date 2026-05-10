<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For The Beaches | Women's Swimwear Shop</title>
    <style>
        :root {
            --brand-pink: #FFC0CB;
            --brand-border: #D02090;
            --brand-dark: #800040;
            --footer-height: 60px;
            --header-height: 120px;
        }

        body {
            margin: 0;
            font-family: 'Helvetica Neue', Arial, sans-serif;
            background-color: #ffffff;
            padding-bottom: var(--footer-height);
            /* Adds space so the top title doesn't cover content */
            padding-top: var(--header-height); 
        }

        /* Fixed Background Logo (Across entire page) */
        .fixed-logo-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100vh;
            z-index: -2;
            background-image: url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            opacity: 0.3;
        }

        /* Fixed Header at the Top */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: var(--header-height);
            background-color: var(--brand-pink);
            border-bottom: 5px solid var(--brand-border);
            z-index: 3000;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        h1 {
            font-size: 2.5rem;
            color: var(--brand-dark);
            margin: 0;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        /* Navigation sits right below the title */
        nav {
            width: 100%;
            background-color: var(--brand-dark);
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            margin: 0;
            padding: 0;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            min-height: 48px; /* Requirement: 46px+ for mobile */
            display: flex;
            align-items: center;
            padding: 0 20px;
        }

        /* Main Shopping Content */
        .content-wrapper {
            position: relative;
            z-index: 1;
            padding: 40px 20px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .product-card {
            background: white;
            border: 2px solid #eee;
            border-radius: 12px;
            overflow: hidden;
            text-align: center;
            padding-bottom: 20px;
        }

        .product-card img {
            width: 100%;
            height: 350px;
            object-fit: cover;
        }

        .add-to-cart {
            background-color: var(--brand-border);
            color: white;
            padding: 12px 25px;
            border: none;
            border-radius: 50px;
            font-weight: bold;
            cursor: pointer;
        }

        /* Fixed Footer at the bottom */
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
            z-index: 4000;
        }
    </style>
</head>
<body>

    <div class="fixed-logo-container"></div>

    <header>
        <h1>For The Beaches</h1>
        <nav>
            <ul>
                <li><a href="#bikinis">BIKINIS</a></li>
                <li><a href="#one-pieces">ONE-PIECES</a></li>
                <li><a href="#sale">SALE</a></li>
            </ul>
        </nav>
    </header>

    <div class="content-wrapper">
        <main class="product-grid">
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1596435707700-62645849f05a?auto=format&fit=crop&w=500&q=80" alt="Azure Bikini Set">
                <h3>Azure Two-Piece</h3>
                <p>$45.00</p>
                <button class="add-to-cart">Add to Cart</button>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1590650213165-c1fef80648c4?auto=format&fit=crop&w=500&q=80" alt="Tropical One-Piece">
                <h3>Tropical One-Piece</h3>
                <p>$65.00</p>
                <button class="add-to-cart">Add to Cart</button>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1582533561751-ef6f6ab93a2e?auto=format&fit=crop&w=500&q=80" alt="Midnight Sport Bikini">
                <h3>Midnight Bikini</h3>
                <p>$50.00</p>
                <button class="add-to-cart">Add to Cart</button>
            </div>
        </main>
    </div>

    <footer>
        <p>&copy; 2026 For The Beaches | Professional Swimwear</p>
    </footer>

</body>
</html>
