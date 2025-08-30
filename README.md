# minhtuancybersecurity.com
Minh Tuan Cyber Security Company
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minh Tuan Cyber Security - Shop</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #0066cc;
            --secondary: #003366;
            --accent: #00cc99;
            --light: #f8f9fa;
            --dark: #212529;
            --sophos: #ff6600;
            --trendmicro: #00a9e0;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo-icon {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, var(--primary), var(--accent));
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            position: relative;
            overflow: hidden;
        }
        
        .logo-icon::before {
            content: "";
            position: absolute;
            width: 20px;
            height: 20px;
            border: 3px solid white;
            border-radius: 50%;
        }
        
        .logo-icon::after {
            content: "";
            position: absolute;
            width: 10px;
            height: 10px;
            background: white;
            border-radius: 50%;
            bottom: 8px;
            right: 8px;
        }
        
        .logo-text {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
        }
        
        .logo-text span {
            color: var(--accent);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 25px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: color 0.3s;
            position: relative;
        }
        
        nav ul li a:hover {
            color: var(--primary);
        }
        
        nav ul li a::after {
            content: "";
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 3px;
            background-color: var(--primary);
            transition: width 0.3s;
        }
        
        nav ul li a:hover::after {
            width: 100%;
        }
        
        .active a {
            color: var(--primary);
        }
        
        .active a::after {
            width: 100%;
        }
        
        .mobile-menu-btn {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        /* Cart Icon */
        .cart-icon {
            position: relative;
            margin-left: 25px;
            cursor: pointer;
        }
        
        .cart-count {
            position: absolute;
            top: -10px;
            right: -10px;
            background-color: var(--accent);
            color: white;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.8rem;
            font-weight: bold;
        }
        
        /* Page Styles */
        .page {
            display: none;
            padding: 60px 0;
            min-height: calc(100vh - 200px);
        }
        
        .page.active {
            display: block;
            animation: fadeIn 0.5s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 51, 102, 0.8), rgba(0, 102, 204, 0.8)), url('https://images.unsplash.com/photo-1563013544-824ae1b704d3?ixlib=rb-4.0.3') no-repeat center center/cover;
            color: white;
            text-align: center;
            padding: 100px 0;
            border-radius: 10px;
            margin-bottom: 40px;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: white;
            padding: 12px 25px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            border: 2px solid var(--accent);
            cursor: pointer;
        }
        
        .btn:hover {
            background-color: transparent;
            color: var(--accent);
        }
        
        .btn-outline {
            background-color: transparent;
            color: white;
            border: 2px solid white;
        }
        
        .btn-outline:hover {
            background-color: white;
            color: var(--primary);
        }
        
        /* Section Styles */
        .section-title {
            text-align: center;
            margin-bottom: 40px;
            color: var(--secondary);
            position: relative;
        }
        
        .section-title::after {
            content: "";
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(to right, var(--primary), var(--accent));
            border-radius: 2px;
        }
        
        /* Partners Section */
        .partners {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 40px;
            margin: 40px 0;
        }
        
        .partner-logo {
            height: 80px;
            filter: grayscale(100%);
            opacity: 0.7;
            transition: all 0.3s;
        }
        
        .partner-logo:hover {
            filter: grayscale(0%);
            opacity: 1;
        }
        
        .sophos-logo {
            color: var(--sophos);
            font-size: 2.5rem;
            font-weight: 700;
        }
        
        .trendmicro-logo {
            color: var(--trendmicro);
            font-size: 1.8rem;
            font-weight: 700;
        }
        
        /* Services Section */
        .services {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }
        
        .service-card {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
            text-align: center;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .service-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        /* About Page */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
            margin: 40px 0;
        }
        
        .team-photo {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        /* Contact Page */
        .contact-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }
        
        .contact-card {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            text-align: center;
        }
        
        .contact-icon {
            font-size: 2rem;
            color: var(--primary);
            margin-bottom: 15px;
        }
        
        .map {
            width: 100%;
            height: 400px;
            border-radius: 10px;
            overflow: hidden;
            margin: 40px 0;
        }
        
        .map iframe {
            width: 100%;
            height: 100%;
            border: none;
        }
        
        /* E-commerce Styles */
        .products {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }
        
        .product-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .product-image {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .product-info {
            padding: 20px;
        }
        
        .product-title {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: var(--secondary);
        }
        
        .product-price {
            font-size: 1.3rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 15px;
        }
        
        .product-description {
            color: #666;
            margin-bottom: 15px;
            font-size: 0.9rem;
        }
        
        .add-to-cart {
            width: 100%;
            padding: 10px;
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
            font-weight: 600;
        }
        
        .add-to-cart:hover {
            background-color: var(--secondary);
        }
        
        /* Cart Page */
        .cart-container {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            margin: 40px 0;
        }
        
        .cart-item {
            display: grid;
            grid-template-columns: 100px 1fr auto auto auto;
            gap: 20px;
            align-items: center;
            padding: 20px 0;
            border-bottom: 1px solid #eee;
        }
        
        .cart-item-image {
            width: 100px;
            height: 80px;
            object-fit: cover;
            border-radius: 5px;
        }
        
        .cart-item-quantity {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .quantity-btn {
            width: 30px;
            height: 30px;
            background-color: #f0f0f0;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        
        .remove-item {
            color: #ff4d4d;
            cursor: pointer;
            font-size: 1.2rem;
        }
        
        .cart-summary {
            margin-top: 30px;
            text-align: right;
        }
        
        .cart-total {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        /* Checkout Page */
        .checkout-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            margin: 40px 0;
        }
        
        .checkout-form {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }
        
        .form-input {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
        
        .payment-methods {
            display: flex;
            gap: 20px;
            margin: 20px 0;
        }
        
        .payment-method {
            flex: 1;
            text-align: center;
            padding: 15px;
            border: 2px solid #ddd;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s;
        }
        
        .payment-method.active {
            border-color: var(--primary);
            background-color: rgba(0, 102, 204, 0.1);
        }
        
        .payment-icon {
            font-size: 2rem;
            margin-bottom: 10px;
        }
        
        .checkout-summary {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            align-self: start;
        }
        
        .summary-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 15px;
        }
        
        .summary-total {
            display: flex;
            justify-content: space-between;
            font-size: 1.2rem;
            font-weight: 700;
            color: var(--primary);
            padding-top: 15px;
            border-top: 1px solid #eee;
            margin-top: 15px;
        }
        
        /* Footer */
        footer {
            background-color: var(--secondary);
            color: white;
            padding: 40px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }
        
        .footer-logo {
            font-size: 1.8rem;
            font-weight: 700;
            margin-bottom: 15px;
            color: white;
        }
        
        .footer-links h3 {
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-links h3::after {
            content: "";
            position: absolute;
            bottom: 0;
            left: 0;
            width: 40px;
            height: 3px;
            background-color: var(--accent);
        }
        
        .footer-links ul {
            list-style: none;
        }
        
        .footer-links ul li {
            margin-bottom: 10px;
        }
        
        .footer-links ul li a {
            color: #ccc;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links ul li a:hover {
            color: white;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
            color: #ccc;
        }
        
        /* Responsive Design */
        @media (max-width: 992px) {
            .about-content, .checkout-container {
                grid-template-columns: 1fr;
            }
            
            .cart-item {
                grid-template-columns: 80px 1fr;
                grid-template-rows: repeat(3, auto);
                gap: 10px;
            }
            
            .cart-item-price, .cart-item-quantity, .cart-item-total {
                justify-self: end;
            }
        }
        
        @media (max-width: 768px) {
            .header-container {
                padding: 15px 20px;
            }
            
            nav {
                position: fixed;
                top: 80px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 80px);
                background-color: white;
                transition: left 0.3s;
                z-index: 99;
            }
            
            nav.active {
                left: 0;
            }
            
            nav ul {
                flex-direction: column;
                padding: 20px;
            }
            
            nav ul li {
                margin: 0 0 20px 0;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .partners {
                flex-direction: column;
                gap: 20px;
            }
            
            .payment-methods {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <div class="logo-icon"></div>
                <div class="logo-text">Minh Tuan <span>Cyber Security</span></div>
            </div>
            
            <nav id="nav">
                <ul>
                    <li class="active"><a href="#home">Home</a></li>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#shop">Shop</a></li>
                    <li><a href="#partners">Partners</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
            
            <div class="cart-icon" id="cart-icon">
                <i class="fas fa-shopping-cart"></i>
                <span class="cart-count" id="cart-count">0</span>
            </div>
            
            <div class="mobile-menu-btn" id="mobile-menu-btn">
                <i class="fas fa-bars"></i>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main>
        <!-- Home Page -->
        <section id="home-page" class="page active">
            <div class="container">
                <div class="hero">
                    <h1>Advanced Cybersecurity Solutions</h1>
                    <p>Protecting your business from evolving cyber threats with cutting-edge technology and expert support</p>
                    <div>
                        <a href="#contact" class="btn">Get in Touch</a>
                        <a href="#shop" class="btn btn-outline">Visit Shop</a>
                    </div>
                </div>
                
                <h2 class="section-title">Our Services</h2>
                
                <div class="services">
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-shield-alt"></i>
                        </div>
                        <h3>Endpoint Protection</h3>
                        <p>Comprehensive security for all endpoints in your network, ensuring devices are protected from threats.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-lock"></i>
                        </div>
                        <h3>Network Security</h3>
                        <p>Advanced solutions to secure your network infrastructure from unauthorized access and attacks.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-cloud"></i>
                        </div>
                        <h3>Cloud Security</h3>
                        <p>Protection for your cloud environments and data, ensuring compliance and security best practices.</p>
                    </div>
                </div>
                
                <div class="partners">
                    <div class="sophos-logo">SOPHOS</div>
                    <div class="trendmicro-logo">TREND MICRO</div>
                </div>
            </div>
        </section>

        <!-- About Page -->
        <section id="about-page" class="page">
            <div class="container">
                <h2 class="section-title">About Us</h2>
                
                <div class="about-content">
                    <div>
                        <p>Minh Tuan Cyber Security is a leading provider of cybersecurity solutions in Vietnam, specializing in enterprise-grade protection for businesses of all sizes.</p>
                        <p>Founded with a mission to make advanced cybersecurity accessible to Vietnamese businesses, we partner with global leaders like Sophos and Trend Micro to deliver world-class protection.</p>
                        <p>Our team of certified security experts provides round-the-clock monitoring, threat detection, and rapid response to keep your business secure in the evolving digital landscape.</p>
                        <p>With our headquarters in Hanoi, we serve clients across Vietnam and Southeast Asia, offering tailored solutions that address specific regional threats and compliance requirements.</p>
                    </div>
                    
                    <div>
                        <img src="https://images.unsplash.com/photo-1560264280-88b83d869d95?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80" alt="Sophos Security Team" class="team-photo">
                    </div>
                </div>
                
                <h3 class="section-title">Our Mission</h3>
                <p style="text-align: center; max-width: 800px; margin: 0 auto 40px;">To empower businesses with enterprise-grade cybersecurity solutions that are accessible, effective, and tailored to the unique challenges of the Vietnamese market. We believe that every organization deserves protection against cyber threats regardless of size or budget.</p>
            </div>
        </section>

        <!-- Services Page -->
        <section id="services-page" class="page">
            <div class="container">
                <h2 class="section-title">Our Services</h2>
                
                <div class="services">
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-shield-alt"></i>
                        </div>
                        <h3>Endpoint Protection</h3>
                        <p>Comprehensive security for all endpoints in your network, ensuring devices are protected from threats.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-lock"></i>
                        </div>
                        <h3>Network Security</h3>
                        <p>Advanced solutions to secure your network infrastructure from unauthorized access and attacks.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-cloud"></i>
                        </div>
                        <h3>Cloud Security</h3>
                        <p>Protection for your cloud environments and data, ensuring compliance and security best practices.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-database"></i>
                        </div>
                        <h3>Data Protection</h3>
                        <p>Encryption, backup, and recovery solutions to safeguard your critical business data.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-user-shield"></i>
                        </div>
                        <h3>Identity & Access Management</h3>
                        <p>Control and monitor access to your systems with multi-factor authentication and privilege management.</p>
                    </div>
                    
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-headset"></i>
                        </div>
                        <h3>24/7 Monitoring & Support</h3>
                        <p>Round-the-clock security monitoring and expert support to quickly respond to threats.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Shop Page -->
        <section id="shop-page" class="page">
            <div class="container">
                <h2 class="section-title">Our Products</h2>
                <p style="text-align: center; margin-bottom: 40px;">Explore our range of cybersecurity products and solutions</p>
                
                <div class="products">
                    <div class="product-card">
                        <img src="https://images.unsplash.com/photo-1563013544-824ae1b704d3?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80" alt="Endpoint Security Suite" class="product-image">
                        <div class="product-info">
                            <h3 class="product-title">Endpoint Security Suite</h3>
                            <div class="product-price">$89.99/year</div>
                            <p class="product-description">Complete protection for all your devices with advanced threat detection.</p>
                            <button class="add-to-cart" data-id="1" data-name="Endpoint Security Suite" data-price="89.99" data-image="https://images.unsplash.com/photo-1563013544-824ae1b704d3?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="product-card">
                        <img src="https://images.unsplash.com/photo-1550751827-4bd374c3f58b?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80" alt="Firewall Pro" class="product-image">
                        <div class="product-info">
                            <h3 class="product-title">Firewall Pro</h3>
                            <div class="product-price">$149.99/year</div>
                            <p class="product-description">Advanced network protection with intrusion prevention and monitoring.</p>
                            <button class="add-to-cart" data-id="2" data-name="Firewall Pro" data-price="149.99" data-image="https://images.unsplash.com/photo-1550751827-4bd374c3f58b?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="product-card">
                        <img src="https://images.unsplash.com/photo-1533750349088-cd871a92f312?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80" alt="Cloud Security" class="product-image">
                        <div class="product-info">
                            <h3 class="product-title">Cloud Security</h3>
                            <div class="product-price">$199.99/year</div>
                            <p class="product-description">Comprehensive protection for your cloud infrastructure and data.</p>
                            <button class="add-to-cart" data-id="3" data-name="Cloud Security" data-price="199.99" data-image="https://images.unsplash.com/photo-1533750349088-cd871a92f312?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="product-card">
                        <img src="https://images.unsplash.com/photo-1563207153-f403bf289096?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80" alt="Data Encryption" class="product-image">
                        <div class="product-info">
                            <h3 class="product-title">Data Encryption</h3>
                            <div class="product-price">$129.99/year</div>
                            <p class="product-description">Military-grade encryption for your sensitive business data.</p>
                            <button class="add-to-cart" data-id="4" data-name="Data Encryption" data-price="129.99" data-image="https://images.unsplash.com/photo-1563207153-f403bf289096?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80">Add to Cart</button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Cart Page -->
        <section id="cart-page" class="page">
            <div class="container">
                <h2 class="section-title">Your Shopping Cart</h2>
                
                <div class="cart-container">
                    <div id="cart-items">
                        <!-- Cart items will be dynamically inserted here -->
                        <div class="empty-cart-message" style="text-align: center; padding: 40px;">
                            <i class="fas fa-shopping-cart" style="font-size: 3rem; color: #ccc; margin-bottom: 20px;"></i>
                            <h3>Your cart is empty</h3>
                            <p>Browse our products and add items to your cart</p>
                            <a href="#shop" class="btn" style="margin-top: 20px;">Continue Shopping</a>
                        </div>
                    </div>
                    
                    <div class="cart-summary">
                        <div class="cart-total">Total: $<span id="cart-total-amount">0.00</span></div>
                        <button id="checkout-btn" class="btn" disabled>Proceed to Checkout</button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Checkout Page -->
        <section id="checkout-page" class="page">
            <div class="container">
                <h2 class="section-title">Checkout</h2>
                
                <div class="checkout-container">
                    <div class="checkout-form">
                        <h3>Customer Information</h3>
                        
                        <div class="form-group">
                            <label class="form-label">Full Name</label>
                            <input type="text" class="form-input" placeholder="Enter your full name">
                        </div>
                        
                        <div class="form-group">
                            <label class="form-label">Email Address</label>
                            <input type="email" class="form-input" placeholder="Enter your email">
                        </div>
                        
                        <div class="form-group">
                            <label class="form-label">Phone Number</label>
                            <input type="tel" class="form-input" placeholder="Enter your phone number">
                        </div>
                        
                        <h3 style="margin-top: 30px;">Shipping Address</h3>
                        
                        <div class="form-group">
                            <label class="form-label">Address</label>
                            <input type="text" class="form-input" placeholder="Enter your address">
                        </div>
                        
                        <div class="form-group">
                            <label class="form-label">City</label>
                            <input type="text" class="form-input" placeholder="Enter your city">
                        </div>
                        
                        <div class="form-group">
                            <label class="form-label">Postal Code</label>
                            <input type="text" class="form-input" placeholder="Enter postal code">
                        </div>
                        
                        <h3 style="margin-top: 30px;">Payment Method</h3>
                        
                        <div class="payment-methods">
                            <div class="payment-method active" data-method="visa">
                                <div class="payment-icon">
                                    <i class="fab fa-cc-visa"></i>
                                </div>
                                <div>Visa</div>
                            </div>
                            
                            <div class="payment-method" data-method="mastercard">
                                <div class="payment-icon">
                                    <i class="fab fa-cc-mastercard"></i>
                                </div>
                                <div>MasterCard</div>
                            </div>
                        </div>
                        
                        <div class="form-group">
                            <label class="form-label">Card Number</label>
                            <input type="text" class="form-input" placeholder="Enter card number">
                        </div>
                        
                        <div class="form-group" style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px;">
                            <div>
                                <label class="form-label">Expiry Date</label>
                                <input type="text" class="form-input" placeholder="MM/YY">
                            </div>
                            <div>
                                <label class="form-label">CVV</label>
                                <input type="text" class="form-input" placeholder="CVV">
                            </div>
                        </div>
                        
                        <button class="btn" style="width: 100%; margin-top: 20px;">Complete Purchase</button>
                    </div>
                    
                    <div class="checkout-summary">
                        <h3>Order Summary</h3>
                        
                        <div id="checkout-items">
                            <!-- Checkout items will be dynamically inserted here -->
                        </div>
                        
                        <div class="summary-total">
                            <span>Total:</span>
                            <span>$<span id="checkout-total">0.00</span></span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Partners Page -->
        <section id="partners-page" class="page">
            <div class="container">
                <h2 class="section-title">Our Partners</h2>
                
                <div class="about-content">
                    <div>
                        <h3>SOPHOS</h3>
                        <p>As a certified Sophos partner, we offer their industry-leading cybersecurity solutions to our clients. Sophos provides next-generation endpoint protection, firewall, and encryption technologies that form the foundation of our security offerings.</p>
                        <p>Our technical team is Sophos-certified, ensuring expert implementation and support of all Sophos products we deploy.</p>
                    </div>
                    
                    <div>
                        <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80" alt="Sophos Partnership" class="team-photo">
                    </div>
                </div>
                
                <div class="about-content">
                    <div>
                        <img src="https://images.unsplash.com/photo-1552664685-eaef9c17eabc?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&h=400&q=80" alt="Trend Micro Partnership" class="team-photo">
                    </div>
                    
                    <div>
                        <h3>TREND MICRO</h3>
                        <p>Our partnership with Trend Micro allows us to provide enterprise-grade cloud security and threat defense solutions. Trend Micro's expertise in hybrid cloud security and network defense complements our service portfolio perfectly.</p>
                        <p>We are proud to be a recognized Trend Micro partner, bringing their global security expertise to the Vietnamese market.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Page -->
        <section id="contact-page" class="page">
            <div class="container">
                <h2 class="section-title">Contact Us</h2>
                
                <div class="contact-info">
                    <div class="contact-card">
                        <div class="contact-icon">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <h3>Address</h3>
                        <p>Lane 23, Tran Khat Chan Street<br>Hai Ba Trung District<br>Ha Noi, Viet Nam</p>
                    </div>
                    
                    <div class="contact-card">
                        <div class="contact-icon">
                            <i class="fas fa-phone"></i>
                        </div>
                        <h3>Phone</h3>
                        <p>+84 0793007736</p>
                    </div>
                    
                    <div class="contact-card">
                        <div class="contact-icon">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <h3>Email</h3>
                        <p>sale@minhtuancybersecurity.com<br>minhtuan2020197@yahoo.com</p>
                    </div>
                </div>
                
                <div class="map">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3724.095374430021!2d105.8505563149329!3d21.030137193151447!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3135abde9aadce5d%3A0xeaacd0c7d0fb5e5b!2zVHLhuqduIEto4bqldCBDaMOibiwgSG_DoG4gS2nhur9tLCBIYWkgQmEgVHLGsG5nLCBIw6AgTuG7mWk!5e0!3m2!1svi!2s!4v1658745030824!5m2!1svi!2s" allowfullscreen="" loading="lazy"></iframe>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-about">
                    <div class="footer-logo">Minh Tuan Cyber Security</div>
                    <p>Advanced cybersecurity solutions for modern businesses. Partnered with industry leaders to bring you the best protection.</p>
                </div>
                
                <div class="footer-links">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#about">About Us</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#shop">Shop</a></li>
                        <li><a href="#partners">Partners</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                
                <div class="footer-links">
                    <h3>Contact Info</h3>
                    <ul>
                        <li><i class="fas fa-map-marker-alt"></i> Lane 23, Tran Khat Chan Street, Hanoi</li>
                        <li><i class="fas fa-phone"></i> +84 0793007736</li>
                        <li><i class="fas fa-envelope"></i> sale@minhtuancybersecurity.com</li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 Minh Tuan Cyber Security. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Navigation functionality
        document.addEventListener('DOMContentLoaded', function() {
            const navLinks = document.querySelectorAll('nav a');
            const mobileMenuBtn = document.getElementById('mobile-menu-btn');
            const nav = document.getElementById('nav');
            const cartIcon = document.getElementById('cart-icon');
            const cartCount = document.getElementById('cart-count');
            const checkoutBtn = document.getElementById('checkout-btn');
            
            // Initialize cart
            let cart = JSON.parse(localStorage.getItem('cart')) || [];
            updateCartCount();
            
            // Handle navigation clicks
            navLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    
                    // Get target page ID
                    const targetId = this.getAttribute('href').substring(1);
                    
                    // Update active navigation link
                    navLinks.forEach(navLink => {
                        navLink.parentElement.classList.remove('active');
                    });
                    this.parentElement.classList.add('active');
                    
                    // Show target page
                    const pages = document.querySelectorAll('.page');
                    pages.forEach(page => {
                        page.classList.remove('active');
                    });
                    document.getElementById(targetId + '-page').classList.add('active');
                    
                    // Close mobile menu if open
                    nav.classList.remove('active');
                    document.body.style.overflow = 'auto';
                });
            });
            
            // Mobile menu toggle
            mobileMenuBtn.addEventListener('click', function() {
                nav.classList.toggle('active');
                
                if (nav.classList.contains('active')) {
                    document.body.style.overflow = 'hidden';
                } else {
                    document.body.style.overflow = 'auto';
                }
            });
            
            // Close mobile menu when clicking outside
            document.addEventListener('click', function(e) {
                if (!nav.contains(e.target) && !mobileMenuBtn.contains(e.target) && nav.classList.contains('active')) {
                    nav.classList.remove('active');
                    document.body.style.overflow = 'auto';
                }
            });
            
            // Cart icon click
            cartIcon.addEventListener('click', function() {
                // Update active navigation link
                navLinks.forEach(navLink => {
                    navLink.parentElement.classList.remove('active');
                });
                
                // Show cart page
                const pages = document.querySelectorAll('.page');
                pages.forEach(page => {
                    page.classList.remove('active');
                });
                document.getElementById('cart-page').classList.add('active');
                
                // Render cart items
                renderCartItems();
            });
            
            // Add to cart buttons
            const addToCartButtons = document.querySelectorAll('.add-to-cart');
            addToCartButtons.forEach(button => {
                button.addEventListener('click', function() {
                    const id = this.getAttribute('data-id');
                    const name = this.getAttribute('data-name');
                    const price = parseFloat(this.getAttribute('data-price'));
                    const image = this.getAttribute('data-image');
                    
                    // Check if product already in cart
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
                    
                    // Save to local storage
                    localStorage.setItem('cart', JSON.stringify(cart));
                    
                    // Update cart count
                    updateCartCount();
                    
                    // Show confirmation
                    alert(`${name} has been added to your cart!`);
                });
            });
            
            // Checkout button
            checkoutBtn.addEventListener('click', function() {
                if (cart.length > 0) {
                    // Update active navigation link
                    navLinks.forEach(navLink => {
                        navLink.parentElement.classList.remove('active');
                    });
                    
                    // Show checkout page
                    const pages = document.querySelectorAll('.page');
                    pages.forEach(page => {
                        page.classList.remove('active');
                    });
                    document.getElementById('checkout-page').classList.add('active');
                    
                    // Render checkout items
                    renderCheckoutItems();
                }
            });
            
            // Payment method selection
            const paymentMethods = document.querySelectorAll('.payment-method');
            paymentMethods.forEach(method => {
                method.addEventListener('click', function() {
                    paymentMethods.forEach(m => m.classList.remove('active'));
                    this.classList.add('active');
                });
            });
            
            // Update cart count
            function updateCartCount() {
                const count = cart.reduce((total, item) => total + item.quantity, 0);
                cartCount.textContent = count;
                
                // Enable/disable checkout button
                checkoutBtn.disabled = count === 0;
            }
            
            // Render cart items
            function renderCartItems() {
                const cartItemsContainer = document.getElementById('cart-items');
                const cartTotalAmount = document.getElementById('cart-total-amount');
                
                if (cart.length === 0) {
                    cartItemsContainer.innerHTML = `
                        <div class="empty-cart-message" style="text-align: center; padding: 40px;">
                            <i class="fas fa-shopping-cart" style="font-size: 3rem; color: #ccc; margin-bottom: 20px;"></i>
                            <h3>Your cart is empty</h3>
                            <p>Browse our products and add items to your cart</p>
                            <a href="#shop" class="btn" style="margin-top: 20px;">Continue Shopping</a>
                        </div>
                    `;
                    cartTotalAmount.textContent = '0.00';
                    return;
                }
                
                let itemsHTML = '';
                let total = 0;
                
                cart.forEach(item => {
                    const itemTotal = item.price * item.quantity;
                    total += itemTotal;
                    
                    itemsHTML += `
                        <div class="cart-item" data-id="${item.id}">
                            <img src="${item.image}" alt="${item.name}" class="cart-item-image">
                            <div class="cart-item-name">${item.name}</div>
                            <div class="cart-item-price">$${item.price.toFixed(2)}</div>
                            <div class="cart-item-quantity">
                                <button class="quantity-btn minus">-</button>
                                <span>${item.quantity}</span>
                                <button class="quantity-btn plus">+</button>
                            </div>
                            <div class="cart-item-total">$${itemTotal.toFixed(2)}</div>
                            <div class="remove-item"><i class="fas fa-trash"></i></div>
                        </div>
                    `;
                });
                
                cartItemsContainer.innerHTML = itemsHTML;
                cartTotalAmount.textContent = total.toFixed(2);
                
                // Add event listeners to quantity buttons and remove buttons
                const minusButtons = document.querySelectorAll('.quantity-btn.minus');
                const plusButtons = document.querySelectorAll('.quantity-btn.plus');
                const removeButtons = document.querySelectorAll('.remove-item');
                
                minusButtons.forEach(button => {
                    button.addEventListener('click', function() {
                        const cartItem = this.closest('.cart-item');
                        const id = cartItem.getAttribute('data-id');
                        const item = cart.find(item => item.id === id);
                        
                        if (item.quantity > 1) {
                            item.quantity -= 1;
                        } else {
                            cart = cart.filter(item => item.id !== id);
                        }
                        
                        localStorage.setItem('cart', JSON.stringify(cart));
                        updateCartCount();
                        renderCartItems();
                    });
                });
                
                plusButtons.forEach(button => {
                    button.addEventListener('click', function() {
                        const cartItem = this.closest('.cart-item');
                        const id = cartItem.getAttribute('data-id');
                        const item = cart.find(item => item.id === id);
                        
                        item.quantity += 1;
                        localStorage.setItem('cart', JSON.stringify(cart));
                        updateCartCount();
                        renderCartItems();
                    });
                });
                
                removeButtons.forEach(button => {
                    button.addEventListener('click', function() {
                        const cartItem = this.closest('.cart-item');
                        const id = cartItem.getAttribute('data-id');
                        
                        cart = cart.filter(item => item.id !== id);
                        localStorage.setItem('cart', JSON.stringify(cart));
                        updateCartCount();
                        renderCartItems();
                    });
                });
            }
            
            // Render checkout items
            function renderCheckoutItems() {
                const checkoutItemsContainer = document.getElementById('checkout-items');
                const checkoutTotal = document.getElementById('checkout-total');
                
                let itemsHTML = '';
                let total = 0;
                
                cart.forEach(item => {
                    const itemTotal = item.price * item.quantity;
                    total += itemTotal;
                    
                    itemsHTML += `
                        <div class="summary-item">
                            <span>${item.name} x ${item.quantity}</span>
                            <span>$${itemTotal.toFixed(2)}</span>
                        </div>
                    `;
                });
                
                checkoutItemsContainer.innerHTML = itemsHTML;
                checkoutTotal.textContent = total.toFixed(2);
            }
        });
    </script>
</body>
</html>
