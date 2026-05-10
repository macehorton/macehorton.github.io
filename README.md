<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For The Beaches | Sale Event</title>
    <style>
        :root {
            --brand-pink: #FFC0CB;
            --brand-border: #D02090;
            --brand-dark: #800040;
            --sale-red: #E60000;
            --footer-height: 60px;
            --header-height: 180px; 
        }

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
            top: 0; 
            left: 0; 
            width: 100%; 
            height: 100vh;
            z-index: -2;
            /* Using a high-res tropical island aerial view */
            background-image: url('https://images.unsplash.com/photo-1544550581-5f7ceaf7f992?auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            opacity: 0.15; /* Subtle enough to see the island without distracting */
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

        /* Sale Page Content */
        .sale-container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
            text-align: center;
            position: relative;
            z-index: 1;
        }

        /* Today Only Callout Box */
        .promo-box {
            background-color: #ffffff;
            border: 6px solid var(--sale-red);
            padding: 30px;
            margin-bottom: 50px;
            box-shadow: 0 10px 20px rgba(230, 0, 0, 0.15);
            border-radius: 20px;
        }

        .promo-title {
            color: var(--sale-red);
            font-size: 3rem;
            margin: 0;
            text-transform: uppercase;
        }

        .promo-subtitle {
            color: var(--brand-dark);
            font-size: 1.8rem;
            margin: 10px 0 0;
            font-weight: bold;
        }

        /* Expanded Sale Gallery */
        .sale-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .sale-gallery img {
            width: 100%;
            height: 450px;
            object-fit: cover;
            border-radius: 12px;
            border: 4px solid var(--brand-pink);
            transition: transform 0.3s ease;
        }

        .sale-gallery img:hover {
            transform: scale(1.03);
            border-color: var(--brand-border);
        }

        /* Fixed Bottom Footer */
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
                <li><a href="#bikinis">BIKINIS</a></li>
                <li><a href="#sale" style="background: var(--brand-border);">SALE</a></li>
            </ul>
        </nav>
    </header>

    <main class="sale-container" id="sale">
        <section class="promo-box">
            <h2 class="promo-title">TODAY ONLY!!!</h2>
            <p class="promo-subtitle">30% OFF Your next order of $100 or more.</p>
        </section>

        <div class="sale-gallery">
            <img src="https://images.unsplash.com/photo-1596435707700-62645849f05a?auto=format&fit=crop&w=600&q=80" alt="Inclusive bikini model">
            <img src="https://images.unsplash.com/photo-1582533561751-ef6f6ab93a2e?auto=format&fit=crop&w=600&q=80" alt="Swimwear for all body types">
            <img src="https://images.unsplash.com/photo-1590650213165-c1fef80648c4?auto=format&fit=crop&w=600&q=80" alt="Sustainable beach fashion">
            <img src="https://images.unsplash.com/photo-1505118380757-91f5f5832de0?auto=format&fit=crop&w=600&q=80" alt="High-quality beachwear collection">
            <img src="https://images.unsplash.com/photo-1568480350417-7e6be952377b?auto=format&fit=crop&w=600&q=80" alt="Summer sale bikini selection">
            <img src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?auto=format&fit=crop&w=600&q=80" alt="Group of women on beach">
        </div>
    </main>

    <footer>
        <p>For the Beaches 2026.</p>
    </footer>

</body>
</html>
