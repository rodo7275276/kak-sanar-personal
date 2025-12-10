[deepseek_html_20251209_2035d6.html](https://github.com/user-attachments/files/24067717/deepseek_html_20251209_2035d6.html)
<!DOCTYPE html>
<html lang="ckb" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UK Pizza Erbil - مێنیو</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --soft-white: #f9f9f9;
            --soft-blue: #e6f2ff;
            --soft-red: #ffe6e6;
            --accent-blue: #1e3a8a;
            --accent-red: #dc2626;
            --text-dark: #1f2937;
            --text-light: #6b7280;
            --shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--soft-white);
            color: var(--text-dark);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        /* Header Styles - UPDATED WITH UK PIZZA ERBIL LOGO */
        header {
            background-color: white;
            box-shadow: var(--shadow);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }

        .logo-container {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-img {
            height: 50px;
            width: 50px;
            background: linear-gradient(135deg, var(--accent-blue), var(--accent-red));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
            font-size: 18px;
            box-shadow: var(--shadow);
        }

        .logo-text {
            font-size: 28px;
            font-weight: 800;
            line-height: 1.1;
        }

        .uk {
            color: var(--accent-blue);
        }

        .pizza {
            color: var(--accent-red);
        }

        .erbil {
            display: block;
            font-size: 14px;
            color: #666;
            font-weight: 600;
            margin-top: 2px;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--text-dark);
            font-weight: 500;
            transition: var(--transition);
            position: relative;
        }

        nav ul li a:hover {
            color: var(--accent-blue);
        }

        nav ul li a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background-color: var(--accent-blue);
            transition: var(--transition);
        }

        nav ul li a:hover::after {
            width: 100%;
        }

        .cart-icon {
            position: relative;
            cursor: pointer;
            font-size: 22px;
            color: var(--text-dark);
            transition: var(--transition);
        }

        .cart-icon:hover {
            color: var(--accent-blue);
        }

        .cart-count {
            position: absolute;
            top: -8px;
            right: -8px;
            background-color: var(--accent-red);
            color: white;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 12px;
            font-weight: bold;
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 24px;
            cursor: pointer;
            color: var(--text-dark);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1081&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
            margin-bottom: 40px;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 20px;
            max-width: 700px;
            margin: 0 auto;
        }

        /* Menu Categories */
        .categories {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 40px;
            padding: 0 10px;
        }

        .category-btn {
            background-color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 30px;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            box-shadow: var(--shadow);
            font-size: 15px;
        }

        .category-btn:hover {
            background-color: var(--soft-blue);
            transform: translateY(-3px);
        }

        .category-btn.active {
            background-color: var(--accent-blue);
            color: white;
        }

        /* Menu Items */
        .menu-section {
            margin-bottom: 60px;
        }

        .section-title {
            text-align: center;
            margin-bottom: 30px;
            font-size: 32px;
            color: var(--text-dark);
            position: relative;
            padding-bottom: 15px;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background-color: var(--accent-blue);
        }

        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
        }

        .menu-item {
            background-color: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            cursor: pointer;
        }

        .menu-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }

        .item-image {
            height: 180px;
            width: 100%;
            background-size: cover;
            background-position: center;
        }

        .item-content {
            padding: 18px;
        }

        .item-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 10px;
        }

        .item-name {
            font-size: 18px;
            font-weight: 600;
        }

        .item-price {
            font-size: 16px;
            font-weight: 700;
            color: var(--accent-red);
        }

        .item-description {
            color: var(--text-light);
            margin-bottom: 15px;
            font-size: 14px;
            line-height: 1.5;
        }

        .add-to-cart {
            background-color: var(--accent-blue);
            color: white;
            border: none;
            padding: 8px 16px;
            border-radius: 6px;
            cursor: pointer;
            font-weight: 600;
            transition: var(--transition);
            display: flex;
            align-items: center;
            gap: 6px;
            font-size: 14px;
            width: 100%;
            justify-content: center;
        }

        .add-to-cart:hover {
            background-color: #152c6b;
        }

        /* Product Detail Modal */
        .product-modal {
            display: none;
            position: fixed;
            top: 0;
            right: -100%;
            width: 100%;
            max-width: 500px;
            height: 100vh;
            background-color: white;
            box-shadow: -5px 0 25px rgba(0, 0, 0, 0.15);
            z-index: 1001;
            transition: right 0.4s ease;
            overflow-y: auto;
        }

        .product-modal.active {
            right: 0;
            display: block;
        }

        .product-modal-content {
            padding: 20px;
            height: 100%;
            display: flex;
            flex-direction: column;
        }

        .product-modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 15px;
            border-bottom: 1px solid #eee;
        }

        .product-modal-title {
            font-size: 24px;
            font-weight: 700;
            color: var(--text-dark);
        }

        .close-product-modal {
            background: none;
            border: none;
            font-size: 22px;
            cursor: pointer;
            color: var(--text-light);
            transition: var(--transition);
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
        }

        .close-product-modal:hover {
            background-color: var(--soft-red);
            color: var(--accent-red);
        }

        .product-image {
            width: 100%;
            height: 250px;
            background-size: cover;
            background-position: center;
            border-radius: 12px;
            margin-bottom: 20px;
        }

        .product-details {
            flex: 1;
        }

        .product-price {
            font-size: 24px;
            font-weight: 700;
            color: var(--accent-red);
            margin-bottom: 15px;
        }

        .product-description {
            color: var(--text-light);
            margin-bottom: 20px;
            line-height: 1.6;
        }

        .product-info-section {
            margin-bottom: 25px;
        }

        .product-info-title {
            font-size: 18px;
            font-weight: 600;
            color: var(--accent-blue);
            margin-bottom: 10px;
            padding-bottom: 5px;
            border-bottom: 2px solid var(--soft-blue);
        }

        .ingredients-list {
            list-style: none;
            padding: 0;
        }

        .ingredients-list li {
            padding: 8px 0;
            border-bottom: 1px solid #f0f0f0;
            display: flex;
            align-items: center;
        }

        .ingredients-list li:before {
            content: "•";
            color: var(--accent-blue);
            font-weight: bold;
            margin-left: 10px;
        }

        .calories-info {
            background-color: var(--soft-blue);
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            margin-top: 10px;
        }

        .calories-amount {
            font-size: 20px;
            font-weight: 700;
            color: var(--accent-blue);
        }

        .modal-add-to-cart {
            background-color: var(--accent-blue);
            color: white;
            border: none;
            padding: 15px;
            border-radius: 8px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            width: 100%;
            margin-top: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }

        .modal-add-to-cart:hover {
            background-color: #152c6b;
        }

        /* Background blur container */
        .main-content {
            transition: filter 0.3s ease;
        }

        .main-content.blur-background {
            filter: blur(5px);
            pointer-events: none;
        }

        /* Cart Modal */
        .cart-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 1000;
            justify-content: center;
            align-items: center;
        }

        .cart-content {
            background-color: white;
            width: 95%;
            max-width: 500px;
            border-radius: 12px;
            padding: 20px;
            max-height: 80vh;
            overflow-y: auto;
        }

        .cart-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 1px solid #eee;
        }

        .cart-title {
            font-size: 22px;
            font-weight: 700;
        }

        .close-cart {
            background: none;
            border: none;
            font-size: 22px;
            cursor: pointer;
            color: var(--text-light);
            transition: var(--transition);
        }

        .close-cart:hover {
            color: var(--accent-red);
        }

        .cart-items {
            margin-bottom: 15px;
        }

        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 0;
            border-bottom: 1px solid #eee;
        }

        .cart-item-info {
            display: flex;
            align-items: center;
            gap: 12px;
            flex: 1;
        }

        .cart-item-image {
            width: 50px;
            height: 50px;
            border-radius: 8px;
            background-size: cover;
            background-position: center;
            flex-shrink: 0;
        }

        .cart-item-details {
            flex: 1;
        }

        .cart-item-name {
            font-weight: 600;
            font-size: 15px;
        }

        .cart-item-price {
            color: var(--accent-red);
            font-weight: 600;
            font-size: 14px;
        }

        .cart-item-controls {
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .quantity-btn {
            background-color: var(--soft-blue);
            border: none;
            width: 28px;
            height: 28px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            transition: var(--transition);
            font-size: 12px;
        }

        .quantity-btn:hover {
            background-color: var(--accent-blue);
            color: white;
        }

        .cart-item-quantity {
            font-weight: 600;
            min-width: 25px;
            text-align: center;
            font-size: 15px;
        }

        .remove-item {
            background: none;
            border: none;
            color: var(--accent-red);
            cursor: pointer;
            font-size: 16px;
            margin-right: 5px;
            transition: var(--transition);
        }

        .remove-item:hover {
            color: #b91c1c;
        }

        .cart-total {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: 12px;
            border-top: 2px solid #eee;
            font-size: 18px;
            font-weight: 700;
        }

        .total-price {
            color: var(--accent-red);
        }

        .checkout-btn {
            background-color: var(--accent-blue);
            color: white;
            border: none;
            padding: 12px;
            border-radius: 8px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            width: 100%;
            margin-top: 15px;
        }

        .checkout-btn:hover {
            background-color: #152c6b;
        }

        .empty-cart {
            text-align: center;
            padding: 30px 0;
            color: var(--text-light);
        }

        .empty-cart i {
            font-size: 40px;
            margin-bottom: 10px;
            color: #ddd;
        }

        /* Footer */
        footer {
            background-color: white;
            padding: 30px 0;
            margin-top: 50px;
            box-shadow: 0 -4px 12px rgba(0, 0, 0, 0.05);
        }

        .footer-content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 25px;
        }

        .footer-section {
            flex: 1;
            min-width: 200px;
        }

        .footer-section h3 {
            margin-bottom: 15px;
            font-size: 18px;
            color: var(--accent-blue);
        }

        .footer-section p, .footer-section a {
            color: var(--text-light);
            margin-bottom: 8px;
            display: block;
            text-decoration: none;
            transition: var(--transition);
            font-size: 14px;
        }

        .footer-section a:hover {
            color: var(--accent-blue);
        }

        .social-icons {
            display: flex;
            gap: 12px;
            margin-top: 12px;
        }

        .social-icons a {
            background-color: var(--soft-blue);
            width: 36px;
            height: 36px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            transition: var(--transition);
        }

        .social-icons a:hover {
            background-color: var(--accent-blue);
            color: white;
        }

        .copyright {
            text-align: center;
            margin-top: 30px;
            padding-top: 15px;
            border-top: 1px solid #eee;
            color: var(--text-light);
            font-size: 14px;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: row;
                justify-content: space-between;
                gap: 10px;
                padding: 10px 0;
            }

            .logo-text {
                font-size: 24px;
            }

            .logo-img {
                height: 45px;
                width: 45px;
                font-size: 16px;
            }

            .mobile-menu-btn {
                display: block;
            }

            .cart-icon {
                order: 3;
            }

            nav ul {
                gap: 10px;
                flex-wrap: wrap;
                justify-content: center;
            }

            nav ul li {
                margin-left: 0;
            }

            .hero {
                padding: 70px 15px;
            }

            .hero h1 {
                font-size: 32px;
            }

            .hero p {
                font-size: 16px;
            }

            .categories {
                gap: 8px;
            }

            .category-btn {
                padding: 8px 16px;
                font-size: 14px;
            }

            .menu-items {
                grid-template-columns: 1fr;
            }

            .section-title {
                font-size: 26px;
            }

            .cart-content {
                width: 95%;
                padding: 15px;
            }

            nav {
                display: none;
                width: 100%;
                position: absolute;
                top: 100%;
                left: 0;
                background: white;
                box-shadow: var(--shadow);
            }

            nav.active {
                display: block;
            }

            nav ul {
                flex-direction: column;
                gap: 0;
                width: 100%;
            }

            nav ul li {
                width: 100%;
                text-align: center;
                padding: 10px 0;
                border-bottom: 1px solid #eee;
            }

            .product-modal {
                max-width: 100%;
            }
        }

        @media (max-width: 480px) {
            .hero {
                padding: 50px 10px;
            }

            .hero h1 {
                font-size: 28px;
            }

            .menu-items {
                gap: 15px;
            }

            .item-content {
                padding: 15px;
            }

            .footer-section {
                min-width: 100%;
            }

            .product-image {
                height: 200px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <button class="mobile-menu-btn" id="mobileMenuBtn">
                    <i class="fas fa-bars"></i>
                </button>
                <div class="logo-container">
                    <div class="logo-img">
                        UK
                    </div>
                    <div class="logo-text">
                        <span class="uk">UK</span> <span class="pizza">Pizza</span>
                        <span class="erbil">هەولێر</span>
                    </div>
                </div>
                <div class="cart-icon" id="cartIcon">
                    <i class="fas fa-shopping-cart"></i>
                    <span class="cart-count">0</span>
                </div>
                <nav id="mainNav">
                    <ul>
                        <li><a href="#home">سەرەکی</a></li>
                        <li><a href="#menu">مێنیو</a></li>
                        <li><a href="#about">دەربارە</a></li>
                        <li><a href="#contact">پەیوەندی</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Main Content (this gets blurred) -->
    <div class="main-content" id="mainContent">
        <!-- Hero Section -->
        <section class="hero" id="home">
            <div class="container">
                <h1>باشترین پیتزا لە شاری هەولێر</h1>
                <p>پیتزای تایبەتی ئێمە بە باشترین پێکهاتە دروست دەکرێت و بە جوانترین شێوە پێشکەشت دەکرێت</p>
            </div>
        </section>

        <!-- Menu Categories -->
        <section class="container" id="menu">
            <div class="categories">
                <button class="category-btn active" data-category="all">هەموو</button>
                <button class="category-btn" data-category="pizza">پیتزا</button>
                <button class="category-btn" data-category="burgers">بێرگەر</button>
                <button class="category-btn" data-category="drinks">خواردنەوە</button>
                <button class="category-btn" data-category="appetizers">پێش خواردن</button>
                <button class="category-btn" data-category="desserts">دێزرت</button>
            </div>
        </section>

        <!-- Menu Items -->
        <section class="container">
            <!-- Pizza Section -->
            <div class="menu-section" id="pizza">
                <h2 class="section-title">پیتزا</h2>
                <div class="menu-items">
                    <!-- Pizza items will be added by JavaScript -->
                </div>
            </div>

            <!-- Burgers Section -->
            <div class="menu-section" id="burgers">
                <h2 class="section-title">بێرگەر</h2>
                <div class="menu-items">
                    <!-- Burger items will be added by JavaScript -->
                </div>
            </div>

            <!-- Drinks Section -->
            <div class="menu-section" id="drinks">
                <h2 class="section-title">خواردنەوە</h2>
                <div class="menu-items">
                    <!-- Drink items will be added by JavaScript -->
                </div>
            </div>

            <!-- Appetizers Section -->
            <div class="menu-section" id="appetizers">
                <h2 class="section-title">پێش خواردن</h2>
                <div class="menu-items">
                    <!-- Appetizer items will be added by JavaScript -->
                </div>
            </div>

            <!-- Desserts Section -->
            <div class="menu-section" id="desserts">
                <h2 class="section-title">دێزرت</h2>
                <div class="menu-items">
                    <!-- Dessert items will be added by JavaScript -->
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer>
            <div class="container">
                <div class="footer-content">
                    <div class="footer-section">
                        <h3>دەربارەی ئێمە</h3>
                        <p>UK Pizza هەولێر باشترین شوێنی پیتزا لە هەولێرە کە پیتزای تایبەتی پێشکەش دەکات</p>
                    </div>
                    <div class="footer-section">
                        <h3>پەیوەندی</h3>
                        <p><i class="fas fa-map-marker-alt"></i> هەولێر، کوردستان</p>
                        <p><i class="fas fa-phone"></i> ٠٧٥٠ ١٢٣ ٤٥٦٧</p>
                        <p><i class="fas fa-envelope"></i> info@ukpizza-erbil.com</p>
                    </div>
                    <div class="footer-section">
                        <h3>کاتەکانی کار</h3>
                        <p>هەینی - پێنجشەممە: ١٠:٠٠ بەیانی - ١١:٠٠ شەو</p>
                        <p>هەینی - یەکشەممە: ١٠:٠٠ بەیانی - ١٢:٠٠ شەو</p>
                    </div>
                    <div class="footer-section">
                        <h3>شوێنی ئێمە</h3>
                        <div class="social-icons">
                            <a href="#"><i class="fab fa-facebook-f"></i></a>
                            <a href="#"><i class="fab fa-instagram"></i></a>
                            <a href="#"><i class="fab fa-twitter"></i></a>
                        </div>
                    </div>
                </div>
                <div class="copyright">
                    <p>© ٢٠٢٣ UK Pizza هەولێر. هەموو مافەکان پارێزراون.</p>
                </div>
            </div>
        </footer>
    </div>

    <!-- Product Detail Modal -->
    <div class="product-modal" id="productModal">
        <div class="product-modal-content">
            <div class="product-modal-header">
                <h2 class="product-modal-title" id="productModalTitle">ناوی بەرهەم</h2>
                <button class="close-product-modal" id="closeProductModal">
                    <i class="fas fa-times"></i>
                </button>
            </div>
            <div class="product-image" id="productModalImage"></div>
            <div class="product-details">
                <div class="product-price" id="productModalPrice">٠ دینار</div>
                <p class="product-description" id="productModalDescription">وەسفی بەرهەم</p>
                
                <div class="product-info-section">
                    <h3 class="product-info-title">پێکهاتەکان</h3>
                    <ul class="ingredients-list" id="productModalIngredients">
                        <!-- Ingredients will be added by JavaScript -->
                    </ul>
                </div>
                
                <div class="product-info-section">
                    <h3 class="product-info-title">کالۆری</h3>
                    <div class="calories-info">
                        <div class="calories-amount" id="productModalCalories">٠ کالۆری</div>
                    </div>
                </div>
                
                <button class="modal-add-to-cart" id="modalAddToCart">
                    <i class="fas fa-plus"></i> زیادکردن بە سەبەتە
                </button>
            </div>
        </div>
    </div>

    <!-- Cart Modal -->
    <div class="cart-modal" id="cartModal">
        <div class="cart-content">
            <div class="cart-header">
                <h2 class="cart-title">سەبەتەی خواردن</h2>
                <button class="close-cart" id="closeCart">
                    <i class="fas fa-times"></i>
                </button>
            </div>
            <div class="cart-items" id="cartItems">
                <div class="empty-cart">
                    <i class="fas fa-shopping-cart"></i>
                    <p>سەبەتەکەت بەتاڵە</p>
                </div>
            </div>
            <div class="cart-total">
                <span>کۆی گشتی:</span>
                <span class="total-price" id="totalPrice">٠ دینار</span>
            </div>
            <button class="checkout-btn" id="checkoutBtn">پارەدان</button>
        </div>
    </div>

    <script>
        // KEEPING ALL ORIGINAL MENU DATA - ONLY CHANGING THE LOGO
        const menuData = {
            pizza: [
                { 
                    id: 1, 
                    name: "پیتزای مەرگەنزا", 
                    price: 15000, 
                    image: "https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?ixlib=rb-4.0.3&auto=format&fit=crop&w=1081&q=80", 
                    description: "پیتزایەکی کلاسیک بە سۆسی تەماتە، موزەرێلا، بەنێوشکە و ڕەزەنە",
                    ingredients: ["سۆسی تەماتە", "پەنیری موزەرێلا", "بەنێوشکە", "ڕەزەنە", "زەیتوون", "بەهارات"],
                    calories: "٣٢٠"
                },
                { 
                    id: 2, 
                    name: "پیتزای پێپەرۆنی", 
                    price: 18000, 
                    image: "https://images.unsplash.com/photo-1574071318508-1cdbab80d002?ixlib=rb-4.0.3&auto=format&fit=crop&w=1169&q=80", 
                    description: "پیتزایەکی بەناوبانگ بە سۆسی تەماتە، موزەرێلا و پێپەرۆنی",
                    ingredients: ["سۆسی تەماتە", "پەنیری موزەرێلا", "پێپەرۆنی", "زەیتوون", "بەهارات"],
                    calories: "٣٥٠"
                },
                { 
                    id: 3, 
                    name: "پیتزای ڤێجی", 
                    price: 16000, 
                    image: "https://images.unsplash.com/photo-1595708684082-a173bb3a06c5?ixlib=rb-4.0.3&auto=format&fit=crop&w=1046&q=80", 
                    description: "پیتزایەکی تایبەت بۆ خواردنی گیایی بە کەرەس و فلفل و زەیتوون و قیاز",
                    ingredients: ["سۆسی تەماتە", "پەنیری موزەرێلا", "کەرەس", "فلفلی سەوز", "زەیتوون", "قیاز", "کەرەوی بروکلی"],
                    calories: "٢٨٠"
                },
                { 
                    id: 4, 
                    name: "پیتزای چیکن", 
                    price: 17000, 
                    image: "https://images.unsplash.com/photo-1593560708920-61dd98c46a4e?ixlib=rb-4.0.3&auto=format&fit=crop&w=1035&q=80", 
                    description: "پیتزایەکی تایبەت بە مەرغ و سەوزە و سۆسی تایبەت",
                    ingredients: ["سۆسی تەماتە", "پەنیری موزەرێلا", "مەرغ", "فلفل", "قیاز", "سۆسی تایبەت"],
                    calories: "٣٦٠"
                },
                { 
                    id: 5, 
                    name: "پیتزای سیفیود", 
                    price: 22000, 
                    image: "https://images.unsplash.com/photo-1593504049359-74330189a345?ixlib=rb-4.0.3&auto=format&fit=crop&w=1027&q=80", 
                    description: "پیتزایەکی تایبەت بە ماسی و مەڕووی دەریایی",
                    ingredients: ["سۆسی تەماتە", "پەنیری موزەرێلا", "ماسی", "مەڕووی دەریایی", "زەیتوون", "لیمۆ"],
                    calories: "٣٢٠"
                },
                { 
                    id: 6, 
                    name: "پیتزای BBQ", 
                    price: 19000, 
                    image: "https://images.unsplash.com/photo-1571407970349-bc81e7e96d47?ixlib=rb-4.0.3&auto=format&fit=crop&w=1025&q=80", 
                    description: "پیتزایەکی تایبەت بە سۆسی BBQ و گۆشت",
                    ingredients: ["سۆسی BBQ", "پەنیری موزەرێلا", "گۆشتی بەفێ", "پیاز", "فلفل"],
                    calories: "٤٠٠"
                },
                { 
                    id: 7, 
                    name: "پیتزای هاواای", 
                    price: 25000, 
                    image: "https://images.unsplash.com/photo-1552539618-7eec9b4d1796?ixlib=rb-4.0.3&auto=format&fit=crop&w=1052&q=80", 
                    description: "پیتزایەکی تایبەت بە هەموو جۆرە پێکهاتەکان",
                    ingredients: ["سۆسی تەماتە", "پەنیری موزەرێلا", "پێپەرۆنی", "مەرغ", "بەنێوشکە", "زەیتوون", "فلفل"],
                    calories: "٤٥٠"
                }
            ],
            burgers: [
                { 
                    id: 8, 
                    name: "بێرگەری کلاسیک", 
                    price: 12000, 
                    image: "https://images.unsplash.com/photo-1568901346375-23c9450c58cd?ixlib=rb-4.0.3&auto=format&fit=crop&w=1098&q=80", 
                    description: "بێرگەرێکی کلاسیک بە گۆشتی بەفێ، سەوزە و سۆسی تایبەت",
                    ingredients: ["گۆشتی بەفێ", "نانی بێرگەر", "سەلاد", "تیکا", "پیاز", "سۆسی تایبەت"],
                    calories: "٥٦٠"
                },
                { 
                    id: 9, 
                    name: "بێرگەری پنێر", 
                    price: 14000, 
                    image: "https://images.unsplash.com/photo-1553979459-d2229ba7433b?ixlib=rb-4.0.3&auto=format&fit=crop&w=1068&q=80", 
                    description: "بێرگەرێکی تایبەت بە پنێر و سەوزە و سۆسی تایبەتی رێستۆرانت",
                    ingredients: ["گۆشتی بەفێ", "پەنیری چێدار", "نانی بێرگەر", "سەلاد", "تیکا", "سۆسی تایبەت"],
                    calories: "٦٢٠"
                },
                { 
                    id: 10, 
                    name: "بێرگەری چیکن", 
                    price: 13000, 
                    image: "https://images.unsplash.com/photo-1606755962773-d324e3833248?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "بێرگەرێکی تایبەت بە مەرغ و سەوزە و سۆسی تایبەت",
                    ingredients: ["مەرغ", "نانی بێرگەر", "سەلاد", "تیکا", "پیاز", "سۆسی مایۆ"],
                    calories: "٤٨٠"
                },
                { 
                    id: 11, 
                    name: "بێرگەری ڤێجی", 
                    price: 11000, 
                    image: "https://images.unsplash.com/photo-1525059696034-4967a7290044?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "بێرگەرێکی تایبەت بۆ خواردنی گیایی بە سەوزە",
                    ingredients: ["پەتاتە", "نانی بێرگەر", "سەلاد", "تیکا", "پیاز", "سۆسی ڤێجی"],
                    calories: "٣٨٠"
                },
                { 
                    id: 12, 
                    name: "بێرگەری دووبڵ", 
                    price: 18000, 
                    image: "https://images.unsplash.com/photo-1572802419224-296b0aeee0d9?ixlib=rb-4.0.3&auto=format&fit=crop&w=1115&q=80", 
                    description: "بێرگەرێکی گەورە بە دوو پارچە گۆشت",
                    ingredients: ["٢ پارچە گۆشتی بەفێ", "نانی بێرگەر", "سەلاد", "تیکا", "پیاز", "سۆسی تایبەت"],
                    calories: "٨٥٠"
                }
            ],
            drinks: [
                { 
                    id: 13, 
                    name: "کۆلا", 
                    price: 2500, 
                    image: "https://images.unsplash.com/photo-1544145945-f90425340c7e?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "خواردنەوەیەکی گازی بەتام و خوێشەویست بۆ هاوپێچی خواردن",
                    ingredients: ["ئاوە سۆدا", "شەکر", "رەنگ و تامی تایبەت"],
                    calories: "١٤٠"
                },
                { 
                    id: 14, 
                    name: "لیمۆناد", 
                    price: 3000, 
                    image: "https://images.unsplash.com/photo-1437418747212-8d9709afab22?ixlib=rb-4.0.3&auto=format&fit=crop&w=1064&q=80", 
                    description: "خواردنەوەیەکی تازە و سارد بە لیمۆ و شەکر",
                    ingredients: ["لیمۆ", "شەکر", "ئاو"],
                    calories: "١٢٠"
                },
                { 
                    id: 15, 
                    name: "ئەیسی تی", 
                    price: 2000, 
                    image: "https://images.unsplash.com/photo-1513558161293-cdaf765ed2fd?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "خواردنەوەیەکی سارد و خوێشەویست بە تی و لیمۆ",
                    ingredients: ["تی", "لیمۆ", "شەکر"],
                    calories: "٩٠"
                },
                { 
                    id: 16, 
                    name: "ئاوەڕێ", 
                    price: 1500, 
                    image: "https://images.unsplash.com/photo-1544145945-f90425340c7e?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "خواردنەوەیەکی گازی بەتام و خوێشەویست",
                    ingredients: ["ئاوە سۆدا", "شەکر", "رەنگ و تامی تایبەت"],
                    calories: "١٥٠"
                },
                { 
                    id: 17, 
                    name: "ئاوەمیوە", 
                    price: 3500, 
                    image: "https://images.unsplash.com/photo-1621506289937-a8e4df240d0b?ixlib=rb-4.0.3&auto=format&fit=crop&w=1035&q=80", 
                    description: "خواردنەوەیەکی تازە بە میوەی جیاواز",
                    ingredients: ["میوەی تازە", "شەکر", "ئاو"],
                    calories: "١٨٠"
                },
                { 
                    id: 18, 
                    name: "سەربستە", 
                    price: 4000, 
                    image: "https://images.unsplash.com/photo-1572442388796-11668a67e53d?ixlib=rb-4.0.3&auto=format&fit=crop&w=1035&q=80", 
                    description: "خواردنەوەیەکی تایبەت بە سەربستە",
                    ingredients: ["شیر", "سەربستە", "شەکر"],
                    calories: "٢٢٠"
                }
            ],
            appetizers: [
                { 
                    id: 19, 
                    name: "فلافڵ", 
                    price: 6000, 
                    image: "https://images.unsplash.com/photo-1563379926898-05f4575a45d8?ixlib=rb-4.0.3&auto=format&fit=crop&w=1170&q=80", 
                    description: "فلافڵێکی تازە و خۆشبەرز بە هەنگوین و سەوزە",
                    ingredients: ["نیکۆڵە", "سەوزە", "هەنگوین", "بەهارات"],
                    calories: "٣٢٠"
                },
                { 
                    id: 20, 
                    name: "سەلاد", 
                    price: 5000, 
                    image: "https://images.unsplash.com/photo-1626700051175-6818013e0571?ixlib=rb-4.0.3&auto=format&fit=crop&w=1064&q=80", 
                    description: "سەلادێکی تازە بە کەرەس و گوێز و سەوزە و سۆسی تایبەت",
                    ingredients: ["کەرەس", "گوێز", "سەلاد", "سۆسی تایبەت"],
                    calories: "١٨٠"
                },
                { 
                    id: 21, 
                    name: "فرێنچ فرای", 
                    price: 4000, 
                    image: "https://images.unsplash.com/photo-1573080496219-bb080dd4f877?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "فرێنچ فرایێکی تازە و خۆشبەرز",
                    ingredients: ["پەتاتە", "روون", "خوێ"],
                    calories: "٣٦٠"
                },
                { 
                    id: 22, 
                    name: "چیکن وینگ", 
                    price: 8000, 
                    image: "https://images.unsplash.com/photo-1567620832903-9fc6debc209f?ixlib=rb-4.0.3&auto=format&fit=crop&w=1080&q=80", 
                    description: "چیکن وینگێکی تازە و خۆشبەرز بە سۆسی تایبەت",
                    ingredients: ["مەرغ", "سۆسی تایبەت", "بەهارات"],
                    calories: "٤٢٠"
                },
                { 
                    id: 23, 
                    name: "ئۆنیان ڕینگ", 
                    price: 5000, 
                    image: "https://images.unsplash.com/photo-1631452180519-c014fe946bc7?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "ئۆنیان ڕینگێکی تازە و خۆشبەرز",
                    ingredients: ["پیاز", "آرد", "روون"],
                    calories: "٣٠٠"
                },
                { 
                    id: 24, 
                    name: "مۆزارێلا ستیک", 
                    price: 7000, 
                    image: "https://images.unsplash.com/photo-1594489573857-4d0cafe979bc?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "مۆزارێلا ستیکێکی تازە و خۆشبەرز",
                    ingredients: ["پەنیری موزەرێلا", "آرد", "روون"],
                    calories: "٣٨٠"
                }
            ],
            desserts: [
                { 
                    id: 25, 
                    name: "چیزکەیک", 
                    price: 8000, 
                    image: "https://images.unsplash.com/photo-1563729784474-d77dbb933a9e?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "چیزکەیکی تایبەت بە سۆسی چێژلە و چۆکلەت",
                    ingredients: ["پەنیر", "شەکر", "چێژلە", "چۆکلەت"],
                    calories: "٤٨٠"
                },
                { 
                    id: 26, 
                    name: "ئایس کریم", 
                    price: 4000, 
                    image: "https://images.unsplash.com/photo-1483695028939-5bb13f8648b0?ixlib=rb-4.0.3&auto=format&fit=crop&w=1170&q=80", 
                    description: "ئایس کریمێکی تازە بە چێژلە و ڤەنیلا و چۆکلەت",
                    ingredients: ["شیر", "شەکر", "چێژلە", "ڤەنیلا", "چۆکلەت"],
                    calories: "٢٨٠"
                },
                { 
                    id: 27, 
                    name: "براونی", 
                    price: 6000, 
                    image: "https://images.unsplash.com/photo-1599599810769-bcde5a160d32?ixlib=rb-4.0.3&auto=format&fit=crop&w=1092&q=80", 
                    description: "براونیێکی تازە و نەرم بە چۆکلەت",
                    ingredients: ["چۆکلەت", "شەکر", "آرد", "هێلکە"],
                    calories: "٤٢٠"
                },
                { 
                    id: 28, 
                    name: "کووکی", 
                    price: 3000, 
                    image: "https://images.unsplash.com/photo-1576618148400-f54bed99fcfd?ixlib=rb-4.0.3&auto=format&fit=crop&w=1160&q=80", 
                    description: "کووکیێکی تازە و خۆشبەرز بە چۆکلەت",
                    ingredients: ["آرد", "شەکر", "چۆکلەت", "هێلکە"],
                    calories: "٢٠٠"
                },
                { 
                    id: 29, 
                    name: "دۆنات", 
                    price: 2500, 
                    image: "https://images.unsplash.com/photo-1551024506-0bccd828d307?ixlib=rb-4.0.3&auto=format&fit=crop&w=1064&q=80", 
                    description: "دۆناتێکی تازە و خۆشبەرز بە چێژلە",
                    ingredients: ["آرد", "شەکر", "چێژلە", "روون"],
                    calories: "٢٤٠"
                },
                { 
                    id: 30, 
                    name: "مافین", 
                    price: 3500, 
                    image: "https://images.unsplash.com/photo-1576618148400-f54bed99fcfd?ixlib=rb-4.0.3&auto=format&fit=crop&w=1160&q=80", 
                    description: "مافینێکی تازە و نەرم بە چۆکلەت",
                    ingredients: ["آرد", "شەکر", "چۆکلەت", "هێلکە"],
                    calories: "٣٢٠"
                },
                { 
                    id: 31, 
                    name: "پای", 
                    price: 7000, 
                    image: "https://images.unsplash.com/photo-1535920527002-b35e96722206?ixlib=rb-4.0.3&auto=format&fit=crop&w=987&q=80", 
                    description: "پایێکی تازە بە میوە",
                    ingredients: ["آرد", "شەکر", "میوە", "هێلکە"],
                    calories: "٣٦٠"
                },
                { 
                    id: 32, 
                    name: "وافی", 
                    price: 5000, 
                    image: "https://images.unsplash.com/photo-1624353365286-3f8d62daad51?ixlib=rb-4.0.3&auto=format&fit=crop&w=1170&q=80", 
                    description: "وافیێکی تازە و خۆشبەرز بە سۆسی چۆکلەت",
                    ingredients: ["آرد", "شەکر", "چۆکلەت", "کەرە"],
                    calories: "٣٨٠"
                }
            ]
        };

        // Cart functionality
        let cart = [];
        const cartIcon = document.getElementById('cartIcon');
        const cartModal = document.getElementById('cartModal');
        const closeCart = document.getElementById('closeCart');
        const cartItems = document.getElementById('cartItems');
        const totalPrice = document.getElementById('totalPrice');
        const checkoutBtn = document.getElementById('checkoutBtn');
        const cartCount = document.querySelector('.cart-count');
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mainNav = document.getElementById('mainNav');

        // Product modal elements
        const productModal = document.getElementById('productModal');
        const closeProductModal = document.getElementById('closeProductModal');
        const productModalTitle = document.getElementById('productModalTitle');
        const productModalImage = document.getElementById('productModalImage');
        const productModalPrice = document.getElementById('productModalPrice');
        const productModalDescription = document.getElementById('productModalDescription');
        const productModalIngredients = document.getElementById('productModalIngredients');
        const productModalCalories = document.getElementById('productModalCalories');
        const modalAddToCart = document.getElementById('modalAddToCart');
        const mainContent = document.getElementById('mainContent');

        let currentProduct = null;

        // Initialize menu items
        function initializeMenu() {
            for (const category in menuData) {
                const container = document.querySelector(`#${category} .menu-items`);
                container.innerHTML = '';
                
                menuData[category].forEach(item => {
                    const menuItem = document.createElement('div');
                    menuItem.className = 'menu-item';
                    menuItem.setAttribute('data-id', item.id);
                    menuItem.innerHTML = `
                        <div class="item-image" style="background-image: url('${item.image}')"></div>
                        <div class="item-content">
                            <div class="item-header">
                                <h3 class="item-name">${item.name}</h3>
                                <span class="item-price">${formatPrice(item.price)} دینار</span>
                            </div>
                            <p class="item-description">${item.description}</p>
                            <button class="add-to-cart" data-id="${item.id}" data-name="${item.name}" data-price="${item.price}" data-image="${item.image}">
                                <i class="fas fa-plus"></i> زیادکردن بە سەبەتە
                            </button>
                        </div>
                    `;
                    container.appendChild(menuItem);
                });
            }
            
            // Add event listeners to all add-to-cart buttons
            document.querySelectorAll('.add-to-cart').forEach(button => {
                button.addEventListener('click', addToCart);
            });

            // Add event listeners to menu items for product detail view
            document.querySelectorAll('.menu-item').forEach(item => {
                item.addEventListener('click', (e) => {
                    // Don't open product modal if clicking the add to cart button
                    if (!e.target.closest('.add-to-cart')) {
                        const productId = parseInt(item.getAttribute('data-id'));
                        openProductModal(getProductById(productId));
                    }
                });
            });
        }

        // Get product by ID
        function getProductById(id) {
            for (const category in menuData) {
                const product = menuData[category].find(item => item.id === id);
                if (product) return product;
            }
            return null;
        }

        // Open product modal
        function openProductModal(product) {
            if (!product) return;
            
            currentProduct = product;
            
            // Update modal content
            productModalTitle.textContent = product.name;
            productModalImage.style.backgroundImage = `url('${product.image}')`;
            productModalPrice.textContent = `${formatPrice(product.price)} دینار`;
            productModalDescription.textContent = product.description;
            
            // Update ingredients
            productModalIngredients.innerHTML = '';
            product.ingredients.forEach(ingredient => {
                const li = document.createElement('li');
                li.textContent = ingredient;
                productModalIngredients.appendChild(li);
            });
            
            // Update calories
            productModalCalories.textContent = `${product.calories} کالۆری`;
            
            // Add blur to main content only (not header or modal)
            mainContent.classList.add('blur-background');
            
            // Show modal with slide animation
            productModal.style.display = 'block';
            setTimeout(() => {
                productModal.classList.add('active');
            }, 10);
        }

        // Close product modal
        function closeProductModalFunc() {
            productModal.classList.remove('active');
            mainContent.classList.remove('blur-background');
            
            // Reset after animation
            setTimeout(() => {
                productModal.style.display = 'none';
            }, 400);
        }

        // Add to cart functionality
        function addToCart(e) {
            e.stopPropagation(); // Prevent triggering the product modal
            
            const button = e.currentTarget;
            const id = button.getAttribute('data-id');
            const name = button.getAttribute('data-name');
            const price = parseInt(button.getAttribute('data-price'));
            const image = button.getAttribute('data-image');

            // Check if item already in cart
            const existingItem = cart.find(item => item.id === id);
            
            if (existingItem) {
                existingItem.quantity += 1;
            } else {
                cart.push({
                    id,
                    name,
                    price,
                    image,
                    quantity: 1
                });
            }

            updateCartCount();
            showAddedToCartMessage(name);
        }

        // Add to cart from modal
        modalAddToCart.addEventListener('click', () => {
            if (currentProduct) {
                // Check if item already in cart
                const existingItem = cart.find(item => item.id === currentProduct.id.toString());
                
                if (existingItem) {
                    existingItem.quantity += 1;
                } else {
                    cart.push({
                        id: currentProduct.id.toString(),
                        name: currentProduct.name,
                        price: currentProduct.price,
                        image: currentProduct.image,
                        quantity: 1
                    });
                }

                updateCartCount();
                showAddedToCartMessage(currentProduct.name);
                closeProductModalFunc();
            }
        });

        // Update cart count in header
        function updateCartCount() {
            const totalItems = cart.reduce((total, item) => total + item.quantity, 0);
            cartCount.textContent = totalItems;
        }

        // Show "added to cart" message
        function showAddedToCartMessage(itemName) {
            // Create a temporary notification
            const notification = document.createElement('div');
            notification.textContent = `${itemName} زیادکرا بە سەبەتە`;
            notification.style.position = 'fixed';
            notification.style.bottom = '20px';
            notification.style.left = '50%';
            notification.style.transform = 'translateX(-50%)';
            notification.style.backgroundColor = 'var(--accent-blue)';
            notification.style.color = 'white';
            notification.style.padding = '10px 20px';
            notification.style.borderRadius = '5px';
            notification.style.zIndex = '1000';
            notification.style.boxShadow = '0 4px 12px rgba(0,0,0,0.15)';
            notification.style.fontSize = '14px';
            
            document.body.appendChild(notification);
            
            // Remove after 2 seconds
            setTimeout(() => {
                document.body.removeChild(notification);
            }, 2000);
        }

        // Update cart display
        function updateCartDisplay() {
            if (cart.length === 0) {
                cartItems.innerHTML = `
                    <div class="empty-cart">
                        <i class="fas fa-shopping-cart"></i>
                        <p>سەبەتەکەت بەتاڵە</p>
                    </div>
                `;
                totalPrice.textContent = '٠ دینار';
                return;
            }

            let cartHTML = '';
            let total = 0;

            cart.forEach(item => {
                const itemTotal = item.price * item.quantity;
                total += itemTotal;

                cartHTML += `
                    <div class="cart-item">
                        <div class="cart-item-info">
                            <div class="cart-item-image" style="background-image: url('${item.image}')"></div>
                            <div class="cart-item-details">
                                <div class="cart-item-name">${item.name}</div>
                                <div class="cart-item-price">${formatPrice(item.price)} دینار</div>
                            </div>
                        </div>
                        <div class="cart-item-controls">
                            <button class="quantity-btn decrease" data-id="${item.id}">
                                <i class="fas fa-minus"></i>
                            </button>
                            <span class="cart-item-quantity">${item.quantity}</span>
                            <button class="quantity-btn increase" data-id="${item.id}">
                                <i class="fas fa-plus"></i>
                            </button>
                            <button class="remove-item" data-id="${item.id}">
                                <i class="fas fa-trash"></i>
                            </button>
                        </div>
                    </div>
                `;
            });

            cartItems.innerHTML = cartHTML;
            totalPrice.textContent = `${formatPrice(total)} دینار`;

            // Add event listeners to quantity buttons
            document.querySelectorAll('.increase').forEach(button => {
                button.addEventListener('click', () => {
                    const id = button.getAttribute('data-id');
                    const item = cart.find(item => item.id === id);
                    item.quantity += 1;
                    updateCartDisplay();
                    updateCartCount();
                });
            });

            document.querySelectorAll('.decrease').forEach(button => {
                button.addEventListener('click', () => {
                    const id = button.getAttribute('data-id');
                    const item = cart.find(item => item.id === id);
                    if (item.quantity > 1) {
                        item.quantity -= 1;
                    } else {
                        cart = cart.filter(item => item.id !== id);
                    }
                    updateCartDisplay();
                    updateCartCount();
                });
            });

            document.querySelectorAll('.remove-item').forEach(button => {
                button.addEventListener('click', () => {
                    const id = button.getAttribute('data-id');
                    cart = cart.filter(item => item.id !== id);
                    updateCartDisplay();
                    updateCartCount();
                });
            });
        }

        // Format price with commas
        function formatPrice(price) {
            return price.toString().replace(/\B(?=(\d{3})+(?!\d))/g, "،");
        }

        // Checkout button
        checkoutBtn.addEventListener('click', () => {
            if (cart.length === 0) {
                alert('سەبەتەکەت بەتاڵە!');
                return;
            }
            
            alert('سوپاس بۆ داواکاریەکەت! داواکاریەکەت وەرگیرا و لە ماوەی ٣٠ خولەکدا ئامادەیە.');
            cart = [];
            updateCartDisplay();
            updateCartCount();
            cartModal.style.display = 'none';
        });

        // Category filtering
        const categoryButtons = document.querySelectorAll('.category-btn');
        const menuSections = document.querySelectorAll('.menu-section');

        categoryButtons.forEach(button => {
            button.addEventListener('click', () => {
                const category = button.getAttribute('data-category');
                
                // Update active button
                categoryButtons.forEach(btn => btn.classList.remove('active'));
                button.classList.add('active');
                
                // Show/hide sections
                if (category === 'all') {
                    menuSections.forEach(section => section.style.display = 'block');
                } else {
                    menuSections.forEach(section => {
                        if (section.id === category) {
                            section.style.display = 'block';
                        } else {
                            section.style.display = 'none';
                        }
                    });
                }
                
                // Scroll to menu
                document.getElementById('menu').scrollIntoView({ behavior: 'smooth' });
            });
        });

        // Mobile menu toggle
        mobileMenuBtn.addEventListener('click', () => {
            mainNav.classList.toggle('active');
        });

        // Close mobile menu when clicking outside
        document.addEventListener('click', (e) => {
            if (!mainNav.contains(e.target) && !mobileMenuBtn.contains(e.target)) {
                mainNav.classList.remove('active');
            }
        });

        // Open cart modal
        cartIcon.addEventListener('click', () => {
            cartModal.style.display = 'flex';
            updateCartDisplay();
        });

        // Close cart modal
        closeCart.addEventListener('click', () => {
            cartModal.style.display = 'none';
        });

        // Close product modal
        closeProductModal.addEventListener('click', closeProductModalFunc);

        // Close modal when clicking outside
        window.addEventListener('click', (e) => {
            if (e.target === cartModal) {
                cartModal.style.display = 'none';
            }
        });

        // Initialize the page
        document.addEventListener('DOMContentLoaded', () => {
            initializeMenu();
        });
    </script>
</body>
</html>
