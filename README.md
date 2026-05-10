<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For The Beaches | Women's Bikinis</title>
    <style>
        :root {
            --brand-pink: #FFC0CB;
            --brand-border: #D02090;
            --brand-dark: #800040;
            --footer-height: 60px;
            --header-height: 130px;
        }

        body {
            margin: 0;
            font-family: 'Helvetica Neue', Arial, sans-serif;
            background-color: #ffffff;
            padding-bottom: calc(var(--footer-height) + 40px);
            padding-top: var(--header-height);
            line-height: 1.5;
        }

        /* Fixed Background Logo */
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
            opacity: 0.2;
        }

        /* Fixed Top Header & Title */
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
            font-size: 2.2rem;
            color: var(--brand-dark);
            margin: 5px 0;
            text-transform: uppercase;
        }

        nav ul {
            list-style: none;
            display: flex;
            padding: 0;
            margin: 0;
            background-color: var(--brand-dark);
            width: 100%;
            justify-content: center;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            padding: 12px 20px;
            display: block;
            min-height: 48px;
        }

        /* Size Selection Section */
        .size-filter {
            background: white;
            padding: 15px;
            text-align: center;
            border-bottom: 2px solid #eee;
            margin-bottom: 20px;
        }

        .size-filter span {
            font-weight: bold;
            margin-right: 10px;
            color: var(--brand-dark);
        }

        .size-btn {
            display: inline-block;
            padding: 8px 15px;
            margin: 3px;
            border: 1px solid var(--brand-border);
            border-radius: 4px;
            text-decoration: none;
            color: var(--brand-dark);
            font-size: 14px;
            background: #fff;
        }

        .size-btn:hover {
            background-color: var(--brand-pink);
        }

        /* Bikini Product Grid */
        .content-wrapper {
            max-width: 1100px;
            margin: 0 auto;
            padding: 20px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .product-card {
            background: white;
            border: 1px solid #ddd;
            border-radius: 10px;
            overflow: hidden;
            text-align: center;
            padding-bottom: 20px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .product-card img {
            width: 100%;
            height: 400px;
            object-fit: cover;
        }

        .product-card h3 {
            color: var(--brand-dark);
            margin: 15px 0 5px;
        }

        .price {
            font-size: 1.2rem;
            color: #555;
            margin-bottom: 15px;
        }

        /* Fixed Bottom Footer */
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
                <li><a href="index.html">HOME</a></li>
                <li><a href="#bikinis" style="background: var(--brand-border);">BIKINIS</a></li>
                <li><a href="#sale">SALE</a></li>
            </ul>
        </nav>
    </header>

    <div class="size-filter">
        <span>Filter by Size:</span>
        <a href="#" class="size-btn">Small</a>
        <a href="#" class="size-btn">Medium</a>
        <a href="#" class="size-btn">Large</a>
        <a href="#" class="size-btn">XL</a>
        <a href="#" class="size-btn">XXL</a>
        <a href="#" class="size-btn">3XL</a>
    </div>

    <div class="content-wrapper">
        <main class="product-grid" id="bikinis">
            
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1596435707700-62645849f05a?auto=format&fit=crop&w=600&q=80" alt="Two-piece turquoise bikini set with adjustable straps">
                <h3>Coral Reef Bikini</h3>
                <p class="price">$48.00</p>
                <p>Sizes: S - 3XL</p>
                <button style="background: var(--brand-border); color: white; border: none; padding: 10px 20px; border-radius: 5px; cursor: pointer;">Add to Cart</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1582533561751-ef6f6ab93a2e?auto=format&fit=crop&w=600&q=80" alt="High-waisted black sporty bikini">
                <h3>Midnight Wave Bikini</h3>
                <p class="price">$52.00</p>
                <p>Sizes: S - 3XL</p>
                <button style="background: var(--brand-border); color: white; border: none; padding: 10px 20px; border-radius: 5px; cursor: pointer;">Add to Cart</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1590650213165-c1fef80648c4?auto=format&fit=crop&w=600&q=80" alt="Floral print bikini with ruffled edges">
                <h3>Paradise Floral Set</h3>
                <p class="price">$55.00</p>
                <p>Sizes: S - 3XL</p>
                <button style="background: var(--brand-border); color: white; border: none; padding: 10px 20px; border-radius: 5px; cursor: pointer;">Add to Cart</button>
            </div>

        </main>
    </div>

    <footer>
        <p>&copy; 2026 For The Beaches | Sizes S to 3XL Available</p>
    </footer>

</body>
</html>
</body>
</html>
