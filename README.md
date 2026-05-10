<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For The Beaches | Home - Sustainable Swimwear</title>
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
            padding-bottom: calc(var(--footer-height) + 20px);
            padding-top: var(--header-height);
            line-height: 1.6;
            color: #333;
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

        /* Fixed Top Header & Title */
        header {
            position: fixed;
            top: 0; left: 0; width: 100%; height: var(--header-height);
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
            letter-spacing: 2px;
        }

        nav ul {
            list-style: none;
            display: flex;
            padding: 0; margin: 0;
            background-color: var(--brand-dark);
            width: 100%;
            justify-content: center;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            padding: 12px 20px;
            display: flex;
            align-items: center;
            min-height: 48px; /* Requirement: Mobile touch target */
        }

        /* Home Content Section */
        .home-container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 40px 20px;
            text-align: center;
            position: relative;
            z-index: 1;
        }

        .hero-image-wrapper {
            width: 100%;
            border: 8px solid var(--brand-pink);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            margin-bottom: 30px;
        }

        .hero-image-wrapper img {
            width: 100%;
            height: auto;
            display: block;
            /* Using a high-quality placeholder representing inclusive swimwear groups */
            aspect-ratio: 16 / 9;
            object-fit: cover;
        }

        .welcome-statement {
            font-size: 1.5rem;
            color: var(--brand-dark);
            font-weight: 500;
            max-width: 800px;
            margin: 0 auto 30px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
        }

        .cta-shop-now {
            display: inline-block;
            background-color: var(--brand-border);
            color: white;
            padding: 15px 40px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 50px;
            font-size: 1.2rem;
            transition: background 0.3s;
        }

        .cta-shop-now:hover {
            background-color: var(--brand-dark);
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
        <h1>For The Beaches</h1>
        <nav>
            <ul>
                <li><a href="#home" style="background: var(--brand-border);">HOME</a></li>
                <li><a href="#bikinis">BIKINIS</a></li>
                <li><a href="#sale">SALE</a></li>
            </ul>
        </nav>
    </header>

    <main class="home-container" id="home">
        
        <div class="hero-image-wrapper">
            <img src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?auto=format&fit=crop&w=1200&q=80" 
                 alt="A diverse group of women with different body types smiling and wearing various colorful swimsuits on a sunny beach.">
        </div>

        <p class="welcome-statement">
            Welcome to the Beachfront! Here, you will find all the swimsuits you need to look nice for your next summer getaway. Find your next fit today!
        </p>

        <a href="#bikinis" class="cta-shop-now">Explore the Collection</a>

    </main>

    <footer>
        <p>&copy; 2026 For The Beaches | All Bodies Are Beach Bodies</p>
    </footer>

</body>
</html>
