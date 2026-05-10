<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For The Beaches | Tropical Swimwear</title>
    <style>
        :root {
            --brand-pink: #FFC0CB;
            --brand-border: #D02090;
            --brand-dark: #800040;
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

        /* NEW: Tropical Beach Island Fixed Background */
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
            opacity: 0.25; /* Subtle enough to see the island without distracting */
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

        /* Content Wrapper */
        .main-content {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
            text-align: center;
            position: relative;
            z-index: 1;
        }

        .welcome-box {
            background: rgba(255, 255, 255, 0.9);
            padding: 30px;
            border-radius: 15px;
            border: 2px solid var(--brand-border);
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
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
                <li><a href="#sale">SALE</a></li>
            </ul>
        </nav>
    </header>

    <main class="main-content" id="home">
        <div class="welcome-box">
            <h2 style="color: var(--brand-dark);">Welcome to the Beachfront!</h2>
            <p style="font-size: 1.2rem;">
                Here, you will find all the swimsuits you need to look nice for your next summer getaway. Find your next fit today!
            </p>
        </div>
        
        <div style="height: 1000px; margin-top: 50px;">
            <p>Scroll down to see our collections...</p>
        </div>
    </main>

    <footer>
        <p>For the Beaches 2026.</p>
    </footer>

</body>
</html>
