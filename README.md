<!DOCTYPE html>
<head>
    <title>The Latte Library - Coffee and Bookstore</title>
    <style>
        body {
            font-family: 'Georgia', serif;
            background-color: #f7f1e3;
            color: #4b3f35;
            margin: 0;
            padding: 0;
            background-image: url('https://wallpaperaccess.com/full/9524787.jpg');
            background-size: cover;
            background-attachment: fixed;
            background-repeat: no-repeat;
        }

        header {
            background-color: rgba(245, 233, 215, 0.95);
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 50px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        header img {
            height: 60px;
        }

        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #4b3f35;
            font-weight: bold;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #8a6e4b;
        }

        section {
            text-align: center;
            padding: 80px 20px;
            background-color: rgba(255, 255, 255, 0.8);
            margin: 40px;
            border-radius: 12px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        h1, h2 {
            color: #3c2f2f;
        }

        .menu-item, .book-item {
            display: inline-block;
            width: 250px;
            margin: 15px;
            padding: 20px;
            background-color: #f1e3d3;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .see-more-btn {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 20px;
            background-color: #8a6e4b;
            color: white;
            border-radius: 8px;
            text-decoration: none;
            transition: background-color 0.3s;
        }

        .see-more-btn:hover {
            background-color: #b8996e;
        }

        footer {
            background-color: #e9dcc9;
            text-align: center;
            padding: 25px;
            color: #4b3f35;
        }
    </style>
</head>
<body>

    <header>
        <img src="https://uploads.onecompiler.io/43xg44j4q/444bsj7zz/LatteLibraryLogo.png" alt="The Latte Library Logo">
        <nav>
            <a href="#about">About</a>
            <a href="#menu">Menu</a>
            <a href="#catalog">Catalog</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section id="about">
        <h1>Welcome to The Latte Library</h1>
        <p>
            The Latte Library is your cozy nook in the city — a place where the aroma of fresh coffee blends 
            with the warmth of turning pages. Whether you’re here for a comforting cup or your next great 
            read, we invite you to sit back, sip, and stay awhile. <br>

<br><br> Latte Library was born from a cozy afternoon of caffeine and conversation when four friends, bonded by their shared love for books and coffee, decided to turn their favorite pastime into something bigger. What began as a dream over steaming mugs soon became a space where stories and aromas blend seamlessly. At Latte Library, every sip pairs perfectly with a new chapter — whether you’re diving into a mystery novel or just the foam of your cappuccino. The store also hosts its own book club, where lively discussions and laughter spill over like a well-poured latte. It’s not just a café or a bookstore — it’s a home for readers, dreamers, and anyone who believes that the best stories are brewed together.

        </p>
    </section>

    <section id="menu">
        <h2>Our Coffee Menu</h2>
        <div class="menu-item">
	    <img src="https://uploads.onecompiler.io/43xg44j4q/43xg42p3j/FRAPCRE_StrawberriesandCreamFrappuccino.jpg" alt="Coffee Image" width="200" height="190">
            <h3>Caramel Latte</h3>
            <p>Rich espresso with smooth caramel and steamed milk.</p>
        </div>
        <div class="menu-item">
	    <img src="https://uploads.onecompiler.io/43xg44j4q/43xg42p3j/FRAPCRE_GreenTeaCreamFrappuccino.jpg" alt="Coffee Image" width="200" height="190">
            <h3>Hazelnut Mocha</h3>
            <p>A delightful blend of chocolate, hazelnut, and espresso.</p>
        </div>
        <div class="menu-item">
	    <img src="https://uploads.onecompiler.io/43xg44j4q/43xg42p3j/FRAPCRE_ChocolateCreamFrappuccino.jpg" alt="Coffee Image" width="200" height="190">
            <h3>Vanilla Cold Brew</h3>
            <p>Slow-steeped perfection with a hint of vanilla.</p>
        </div>
        <a href="file:///C:/Users/Acer/Desktop/Cruz,%20Paolo%20Gabriel/C++%20&%20HTML/group%204%20menu%20real.html" class="see-more-btn">See More</a>
    </section>

    <section id="catalog">
        <h2>Book Catalog</h2>
        <div class="book-item">
	    <img src="https://cdn2.penguin.com.au/covers/original/9781446468265.jpg" alt="Book Image" width="160" height="250">
            <h3>The Night Circus</h3>
            <p>by Erin Morgenstern</p>
        </div>
        <div class="book-item">
	    <img src="https://m.media-amazon.com/images/I/81XuBDUvMaL._SL1500_.jpg" alt="Book Image" width="160" height="230">
            <h3>Before the Coffee Gets Cold</h3>
            <p>by Toshikazu Kawaguchi</p>
        </div>
        <div class="book-item">
	    <img src="https://imgix.bustle.com/uploads/image/2018/12/26/fa3d106d-8f15-4108-9b1e-feef8b7da0f5-circe.jpg?w=400&h=604&fit=crop&crop=faces&auto=format%2Ccompress&q=50&dpr=2" alt="Book Image" width="160" height="250">
            <h3>Circe</h3>
            <p>by Madeline Miller</p>
        </div>
        <a href="file:///C:/Users/Acer/Desktop/Cruz,%20Paolo%20Gabriel/C++%20&%20HTML/group%204%20menu%20real.html" class="see-more-btn">See More</a>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <p>📍 211B Baker Street, Manila, Philippines</p>
        <p>📞 (02) 123-4567</p>
        <p>📧 hello@thelattelibrary.com</p>
    </section>

    <footer>
        <p>&copy; 2025 The Latte Library Coffee and Bookstore | All Rights Reserved</p>
    </footer>

</body>
</html>
