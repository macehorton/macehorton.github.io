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

       .fixed-logo-container {
            position: fixed; /* Keeps it in one place while scrolling */
            top: 0;
            left: 0;
            width: 100%;
            height: 100vh; /* Covers the full height of the viewport */
            z-index: -1;   /* Places it behind the text content */
            
            /* Visuals */
            background-image: url('https://via.placeholder.com/1920x1080/FFC0CB/800040?text=FOR+THE+BEACHES');
            background-size: cover;      /* Ensures it spans the entire width */
            background-position: center;
            background-repeat: no-repeat;
            opacity: 0.6; /* Lightened so text remains legible over it */
        }

        /* Navigation remains at the top */
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

        /* Content needs a background so it covers the logo as you scroll */
        .content-wrapper {
            margin-top: 100vh; /* Pushes content down so logo is seen first */
            background-color: white;
            position: relative;
            z-index: 1;
            padding: 50px 20px;
            border-top: 10px solid var(--brand-border);
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
        }

        h1, h2 {
            color: var(--brand-dark);
            text-transform: uppercase;
        }

        .spacer {
            height: 1000px; /* Temporary height to demonstrate the scroll effect */
        }
    </style>
</head>
<body>

    <div class="fixed-logo-container" aria-hidden="true"></div>

    <nav>
        <ul>
            <li><a href="#home">HOME</a></li>
            <li><a href="#gallery">GALLERY</a></li>
            <li><a href="#resources">RESOURCES</a></li>
        </ul>
    </nav>

    <div class="content-wrapper">
        <main class="container" id="home">

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
