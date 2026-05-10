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

        /* Home Content Grid */
        .home-container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
            text-align: center;
            position: relative;
            z-index: 1;
        }

        .hero-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .hero-gallery img {
            width: 100%;
            height: 500px;
            object-fit: cover;
            border-radius: 15px;
            border: 5px solid var(--brand-pink);
            box-shadow: 0 8px 20px rgba(0,0,0,0.1);
        }

        .welcome-box {
            background: rgba(255, 255, 255, 0.9);
            padding: 30px;
            border-radius: 15px;
            border: 2px solid var(--brand-border);
            margin-top: 20px;
        }

        .welcome-text {
            font-size: 1.5rem;
            color: var(--brand-dark);
            font-weight: bold;
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
    <main class="shop-container" id="bikinis">
        <h2 class="section-title">Shop Our Bikinis</h2>
        
        <div class="product-grid">
            <div class="product-card">
                <img src="https://www.bing.com/images/search?view=detailV2&ccid=%2FcFswSFS&id=5C44CDF02F92E8CC858375D680D4BDA24560C619&thid=OIP._cFswSFSLPj82QttQzMOJAHaLH&mediaurl=https%3A%2F%2Fcdn.shopify.com%2Fs%2Ffiles%2F1%2F0293%2F9277%2Ffiles%2F01-24-24_S9_10_2280FN_Jade_RA_RL_11-15-01_1647_PXF.jpg%3Fv%3D1706638810%26width%3D801%26height%3D1202%26crop%3Dcenter&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.fdc16cc121522cf8fcd90b6d43330e24%3Frik%3DGcZgRaK91IDWdQ%26pid%3DImgRaw%26r%3D0&exph=1202&expw=801&q=turquoise+high+waist+bikini&form=IRPRST&ck=663D7593B35C01E4962E7040D5187BF5&selectedindex=10&itb=0&cw=1405&ch=667&ajaxhist=0&ajaxserp=0&pivotparams=insightsToken%3Dccid_cT0NX4yn*cp_BBCBD9316E95DDCCE3788D10A3712962*mid_CD0891431B9E090BBC7C1AE70AD70799953DF8CC*thid_OIP.cT0NX4yn7a3h!_NvfAJW0QQHaLJ&vt=0&sim=11&iss=VSI&ajaxhist=0&ajaxserp=0" alt="Turquoise high-waisted bikini">
                <div class="product-name">Azure Coast Two-Piece</div>
                <div class="product-price">$48.00</div>
                <div class="product-sizes">SIZES: S, M, L, XL, XXL, 3XL</div>
                <button class="btn-add">Add to Cart</button>
            </div>

            <div class="product-card">
                <img src="https://www.bing.com/images/search?view=detailV2&ccid=3exuHXDg&id=3AD0E2EB2AB20246B6C04C38DC53094E1ED2B34B&thid=OIP.3exuHXDgGyN4QyLlBt4DlwHaLH&mediaurl=https%3A%2F%2Fimage.ezshopcarts.com%2F3f580679b590fc75cc6046914c1e1852%2F2024011502%2F7c3a6769e240d36845cc07d2bbb09ed0.jpg&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.ddec6e1d70e01b23784322e506de0397%3Frik%3DS7PSHk4JU9w4TA%26pid%3DImgRaw%26r%3D0&exph=1200&expw=800&q=black+sporty+bikini&FORM=IRPRST&ck=DEEB6AEA000D9133A9238631B5C80768&selectedIndex=11&itb=0&adtq=1&cw=1405&ch=667&ajaxhist=0&ajaxserp=0" alt="Sleek black sporty bikini">
                <div class="product-name">Midnight Wave Bikini</div>
                <div class="product-price">$52.00</div>
                <div class="product-sizes">SIZES: S, M, L, XL, XXL, 3XL</div>
                <button class="btn-add">Add to Cart</button>
            </div>

            <div class="product-card">
                <img src="https://www.bing.com/images/search?view=detailV2&ccid=BtO8ieFW&id=03B76D2031937F5504F1951810A78CD06429BD15&thid=OIP.BtO8ieFWiMZGvuKo6AJq8AAAAA&mediaurl=https%3A%2F%2Fm.media-amazon.com%2Fimages%2FI%2F71oc3-LWrWL.__AC_SY445_SX342_QL70_ML2_.jpg&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.06d3bc89e15688c646bee2a8e8026af0%3Frik%3DFb0pZNCMpxAYlQ%26pid%3DImgRaw%26r%3D0&exph=445&expw=333&q=floral+patterned+ruffled+bikini+plus+sized&FORM=IRPRST&ck=DC50E39FDF5C07A22E7784224EF6C362&selectedIndex=4&itb=0&cw=1405&ch=667&ajaxhist=0&ajaxserp=0" alt="Floral patterned ruffled bikini">
                <div class="product-name">Paradise Bloom Bikini</div>
                <div class="product-price">$55.00</div>
                <div class="product-sizes">SIZES: S, M, L, XL, XXL, 3XL</div>
                <button class="btn-add">Add to Cart</button>
            </div>
        </div>
    </main>
    <main class="sale-container" id="sale">
        <section class="promo-box">
            <h2 class="promo-title">TODAY ONLY!!!</h2>
            <p class="promo-subtitle">30% OFF Your next order of $100 or more.</p>
        </section>

        <div class="sale-gallery">
            <img src="[https://images.unsplash.com/photo-1596435707700-62645849f05a?auto=format&fit=crop&w=600&q=80](https://www.bing.com/images/search?view=detailV2&ccid=gtCpTlsN&id=C342BA141CD313CDF2D6265AD7A01C1EFBA0E061&thid=OIP.gtCpTlsNOeGOIdVQA1AlQwHaKQ&mediaurl=https%3A%2F%2Fwww.arkswimwear.com%2Fmedia%2Fcatalog%2Fproduct%2Fr%2Fe%2Fred_string_bralette_1.jpg%3Foptimize%3Dmedium%26height%3D2660%26width%3D1920&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.82d0a94e5b0d39e18e21d55003502543%3Frik%3DYeCg%252bx4coNdaJg%26pid%3DImgRaw%26r%3D0&exph=1995&expw=1440&q=bikini&FORM=IRPRST&ck=3EA9EAE0FB01933A6A14BDE67C1D14C1&selectedIndex=10&itb=0&cw=1405&ch=667&ajaxhist=0&ajaxserp=0)" alt="Inclusive bikini model">
            <img src="[https://images.unsplash.com/photo-1582533561751-ef6f6ab93a2e?auto=format&fit=crop&w=600&q=80](https://www.bing.com/images/search?view=detailV2&ccid=wAmffkRx&id=7DC5B589B7C81CEC8548B87995BC48E79EB2DA5F&thid=OIP.wAmffkRxmCHy_y8FfMWk-wHaIV&mediaurl=https%3A%2F%2Fphotos.cdn-outlet.com%2Fphotos%2Foptions%2F8164469-56046-1A-zoomin.jpg&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.c0099f7e44719821f2ff2f057cc5a4fb%3Frik%3DX9qynudIvJV5uA%26pid%3DImgRaw%26r%3D0&exph=1176&expw=1044&q=swimwear+plus+size&FORM=IRPRST&ck=B44F955AE6B6E010227C081CC96E092C&selectedIndex=4&itb=0&cw=1405&ch=667&ajaxhist=0&ajaxserp=0)" alt="Swimwear for all body types">
            <img src="[https://images.unsplash.com/photo-1590650213165-c1fef80648c4?auto=format&fit=crop&w=600&q=80](https://www.bing.com/images/search?view=detailV2&ccid=NmxNz5aa&id=5473EED23B071A6BBF8F5DE6DD66060B5A04FF70&thid=OIP.NmxNz5aavYbqFINpiiQ2BgHaKq&mediaurl=https%3A%2F%2Fwww.emoswimsuits.com%2Fcdn%2Fshop%2Ffiles%2F10003_20240604163208_2_665x.jpg%3Fv%3D1718099564&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.366c4dcf969abd86ea1483698a243606%3Frik%3DcP8EWgsGZt3mXQ%26pid%3DImgRaw%26r%3D0&exph=958&expw=665&q=Extra+Plus+Size+Swimwear&FORM=IRPRST&ck=A51975F55D1F46D2AE7CB268588C5C37&selectedIndex=41&itb=0&cw=1405&ch=667&ajaxhist=0&ajaxserp=0)" alt="Sustainable beach fashion">
            <img src="[https://images.unsplash.com/photo-1505118380757-91f5f5832de0?auto=format&fit=crop&w=600&q=80](https://www.bing.com/images/search?view=detailV2&ccid=d5BVqt2Q&id=6FB369E33F4FDE9CB7028D096D7A59882E5F8EAA&thid=OIP.d5BVqt2QHU11KJam8TB6NQHaHa&mediaurl=https%3A%2F%2Fi5.walmartimages.com%2Fseo%2FWREESH-Womens-Plus-Size-One-Piece-Swimsuit-Short-Sleeve-Surfing-Swimsuit-Sun-Protection-Swimwear-Fashion-Printed-Zipper-Bathing-Suit-Black_713fed9c-a71b-4a02-9f34-426e6018d6ed.dba62303ac9c1fe1cf8e7960f740a6f0.jpeg&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.779055aadd901d4d752896a6f1307a35%3Frik%3Dqo5fLohZem0JjQ%26pid%3DImgRaw%26r%3D0&exph=1600&expw=1600&q=Swimsuit+Plus+Size+Swimwear&FORM=IRPRST&ck=C22F3A30FBB375CFF6950082B003F35E&selectedIndex=118&itb=0&cw=1405&ch=667&ajaxhist=0&ajaxserp=0)" alt="High-quality beachwear collection">
            <img src="[https://images.unsplash.com/photo-1568480350417-7e6be952377b?auto=format&fit=crop&w=600&q=80](https://www.bing.com/images/search?view=detailV2&ccid=RL%2F1%2BYZq&id=5227A6A6205689A9331666314DD5BA2D5B36845C&thid=OIP.RL_1-YZqecbM4eNSt4pkMQHaJ2&mediaurl=https%3A%2F%2Fimg.ltwebstatic.com%2Fimages3_pi%2F2024%2F02%2F12%2Fd9%2F1707702853bed01d02c40b3d9c4d76591c487e6692_thumbnail_900x.jpg&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.44bff5f9866a79c6cce1e352b78a6431%3Frik%3DXIQ2Wy261U0xZg%26pid%3DImgRaw%26r%3D0&exph=1198&expw=900&q=Swimsuit+Plus+Size+Swimwear&form=IRPRST&ck=13FA00842687DEF443A3339F4845BBDB&selectedindex=14&itb=0&cw=1405&ch=667&ajaxhist=0&ajaxserp=0&pivotparams=insightsToken%3Dccid_d5BVqt2Q*cp_C22F3A30FBB375CFF6950082B003F35E*mid_6FB369E33F4FDE9CB7028D096D7A59882E5F8EAA*thid_OIP.d5BVqt2QHU11KJam8TB6NQHaHa&vt=0&sim=11&iss=VSI&ajaxhist=0&ajaxserp=0)" alt="Summer sale bikini selection">
            <img src="[https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?auto=format&fit=crop&w=600&q=80](https://www.bing.com/images/search?view=detailV2&ccid=JIIvVqr6&id=4B3AC27D777FAB76E039CA8C9171922DFEE398BB&thid=OIP.JIIvVqr6rgngSI19CYnnzgHaE7&mediaurl=https%3A%2F%2Fmedia.istockphoto.com%2Fid%2F1477196908%2Fphoto%2Fyoung-multiracial-women-having-fun-together-during-summer-vacation-on-the-beach.jpg%3Fs%3D170667a%26w%3D0%26k%3D20%26c%3DxlCMOwqgJA7evWuCsAPOkVln_HWnMSyg15GKoqlWLuo%3D&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.24822f56aafaae09e0488d7d0989e7ce%3Frik%3Du5jj%252fi2ScZGMyg%26pid%3DImgRaw%26r%3D0&exph=339&expw=509&q=group+of+women+on+beach+wearing+swimsuits&form=IRPRST&ck=95922FE77642CE599E76B071E8AF8C26&selectedindex=2&itb=0&cw=1405&ch=667&ajaxhist=0&ajaxserp=0&pivotparams=insightsToken%3Dccid_7L9BBVYP*cp_B87677E34BC498D3296BDD6C35FE5DE9*mid_7DA05D3731356BFD48ABC964747F21E1F0FC3279*thid_OIP.7L9BBVYPo6mgETDhp8C0eQHaE8&vt=0&sim=11&iss=VSI&ajaxhist=0&ajaxserp=0)" alt="Group of women on beach">
        </div>
    </main>

    <footer>
        <p>For the Beaches 2026.</p>
    </footer>

</body>
</html>
