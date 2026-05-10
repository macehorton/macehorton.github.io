<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For The Beaches | Women's Swimwear</title>
    <meta name="description" content="Find your perfect swimsuit for that perfect summer getaway.">

    <style>
        :root {
            --brand-pink: #FFC0CB;
            --brand-border: #D02090;
            --brand-dark: #800040;
            --text-main: #333333;
            /* Font styles - consistent sizes */
            --font-size-body: 18px;
            --font-size-h2: 28px;
        }

        body {
            line-height: 1.6;
            font-size: var(--font-size-body);
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            margin: 0;
            background-color: #f9f9f9;
            color: var(--text-main);
        }

        /* Typography Legibility - All forms (Bold, Italics, Caps) */
        h1, h2, h3 { 
            color: var(--brand-dark); 
            text-transform: uppercase; /* Testing all caps legibility */
            letter-spacing: 1px;
        }

        .emphasis-text {
            font-style: italic;
            font-weight: bold;
            color: var(--brand-border);
        }

        /* Header & Logo */
        .header-banner {
            background-color: var(--brand-pink);
            border-bottom: 8px solid var(--brand-border);
            padding: 40px 20px;
            text-align: center;
        }

        /* Navigation - 46px+ Touch Target */
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

        /* Container & Content */
        .container {
            max-width: 900px;
            margin: 40px auto;
            padding: 0 20px;
        }

        .resource-list {
            margin: 20px 0;
            padding: 0;
            list-style-type: none;
        }

        .resource-list li {
            background: white;
            margin-bottom: 10px;
            padding: 15px;
            border-left: 5px solid var(--brand-border);
            border-radius: 4px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }

        .external-link {
            color: #005A9C;
            font-weight: bold;
            text-decoration: underline;
        }

        footer {
            text-align: center;
            padding: 40px;
            background: #eee;
        }
    </style>
</head>
<body>

    <nav>
        <ul>
            <li><a href="#home">HOME</a></li>
            <li><a href="#swimsuits">SWIMSUITS</a></li>
            <li><a href="#gallery">GALLERY</a></li>
        </ul>
    </nav>

    <header class="header-banner">
        <a href="#home">
            <img src="https://via.placeholder.com/60/D02090/FFFFFF?text=FTB" alt="For The Beaches Logo" style="border-radius: 50%;">
        </a>
        <h1>For The Beaches</h1>
    </header>

    <main class="container">
        <section id="home">
            <h2>Welcome to the Beachline!</h2>
            <p>Our mission is to provide <span class="emphasis-text">stylish, high-quality, and fitted</span> swimsuits to our customers. Whether you are a size 3XL <strong>BOLD</strong>, <em>SMALL</em>, or MEDIUM, we have swimsuits that are tailored to fit all sizes.</p>
        </section>

        <section id="swimsuits">
            <h2>Swimewear</h2>
            <p>To learn more about beach conservation, please visit these official organizations:</p>
            <ul class="resource-list">
                <li>
                    <a href="https://www.surfrider.org" class="external-link" target="_blank" rel="noopener">Surfrider Foundation</a> - Dedicated to the protection and enjoyment of the world’s ocean and beaches.
                </li>
                <li>
                    <a href="https://oceana.org" class="external-link" target="_blank" rel="noopener">Oceana</a> - The largest international advocacy organization focused solely on ocean conservation.
                </li>
                <li>
                    <a href="https://www.oceanconservancy.org" class="external-link" target="_blank" rel="noopener">Ocean Conservancy</a> - Working to protect the ocean from today’s greatest global challenges.
                </li>
            </ul>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 For The Beaches.</p>
    </footer>

</body>
</html>
