<title>Fabric Haven - Premium Fabrics & Textiles</title> <style> * { margin: 0; padding: 0; box-sizing: border-box; }
    :root {
        --primary-color: #8B4513;
        --secondary-color: #D2691E;
        --accent-color: #F4A460;
        --text-dark: #2C1810;
        --text-light: #6D4C41;
        --bg-light: #FFF8F3;
        --white: #FFFFFF;
        --glass-bg: rgba(255, 255, 255, 0.85);
        --glass-border: rgba(255, 255, 255, 0.3);
        --glass-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
    }

    body {
        font-family: 'Georgia', serif;
        line-height: 1.6;
        color: var(--text-dark);
        background-color: var(--bg-light);
    }

    /* Header Styles */
    header {
        background: var(--glass-bg);
        backdrop-filter: blur(10px);
        box-shadow: var(--glass-shadow);
        border-bottom: 1px solid var(--glass-border);
        position: fixed;
        width: 100%;
        top: 0;
        z-index: 1000;
    }

    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1rem 5%;
        max-width: 1200px;
        margin: 0 auto;
    }

    .logo {
        font-size: 2rem;
        font-weight: bold;
        color: var(--primary-color);
        text-decoration: none;
    }

    .nav-links {
        display: flex;
        list-style: none;
        gap: 2rem;
    }

    .nav-links a {
        text-decoration: none;
        color: var(--text-dark);
        font-weight: 500;
        transition: color 0.3s;
    }

    .nav-links a:hover {
        color: var(--secondary-color);
    }

    .cart-icon {
        position: relative;
        cursor: pointer;
    }

    .cart-count {
        position: absolute;
        top: -8px;
        right: -8px;
        background: var(--secondary-color);
        color: var(--white);
        border-radius: 50%;
        width: 20px;
        height: 20px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 0.8rem;
    }

    /* Hero Section */
    .hero {
        margin-top: 80px;
        background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
        color: var(--white);
        padding: 4rem 5%;
        text-align: center;
        position: relative;
        overflow: hidden;
    }

    .hero::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><path d="M0,0 Q50,20 100,0 L100,100 Q50,80 0,100 Z" fill="rgba(255,255,255,0.1)"/></svg>');
        background-size: cover;
        opacity: 0.3;
    }

    .hero h1 {
        font-size: 3rem;
        margin-bottom: 1rem;
    }

    .hero p {
        font-size: 1.2rem;
        margin-bottom: 2rem;
    }

    .cta-button {
        display: inline-block;
        background: var(--accent-color);
        color: var(--text-dark);
        padding: 1rem 2rem;
        text-decoration: none;
        border-radius: 5px;
        font-weight: bold;
        transition: all 0.3s ease;
        position: relative;
        overflow: hidden;
        z-index: 1;
    }

    .cta-button::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 0;
        height: 100%;
        background: var(--white);
        transition: width 0.5s ease;
        z-index: -1;
    }

    .cta-button:hover::before {
        width: 100%;
    }

    .cta-button:hover {
        transform: translateY(-3px);
        box-shadow: 0 10px 20px rgba(0,0,0,0.1);
    }

    /* Categories Section */
    .categories {
        padding: 4rem 5%;
        max-width: 1200px;
        margin: 0 auto;
    }

    .section-title {
        text-align: center;
        font-size: 2.5rem;
        color: var(--text-dark);
        margin-bottom: 3rem;
    }

    .category-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 2rem;
    }

    .category-card {
        background: var(--glass-bg);
        backdrop-filter: blur(10px);
        border-radius: 16px;
        overflow: hidden;
        border: 1px solid var(--glass-border);
        box-shadow: var(--glass-shadow);
        transition: all 0.3s ease;
        cursor: pointer;
    }

    .category-card:hover {
        transform: translateY(-8px);
        box-shadow: 0 15px 30px rgba(0,0,0,0.15);
    }

    .category-image {
        width: 100%;
        height: 200px;
        object-fit: cover;
        transition: transform 0.5s ease;
    }

    .category-card:hover .category-image {
        transform: scale(1.05);
    }

    .category-info {
        padding: 1.5rem;
    }

    .category-info h3 {
        color: var(--primary-color);
        margin-bottom: 0.5rem;
    }

    /* Products Section */
    .products {
        padding: 4rem 5%;
        max-width: 1200px;
        margin: 0 auto;
    }

    .product-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
        gap: 2rem;
    }

    .product-card {
        background: var(--glass-bg);
        backdrop-filter: blur(10px);
        border-radius: 16px;
        overflow: hidden;
        border: 1px solid var(--glass-border);
        box-shadow: var(--glass-shadow);
        transition: all 0.3s ease;
    }

    .product-card:hover {
        transform: translateY(-8px);
        box-shadow: 0 15px 30px rgba(0,0,0,0.15);
    }

    .product-image {
        width: 100%;
        height: 300px;
        object-fit: cover;
        transition: transform 0.5s ease;
    }

    .product-card:hover .product-image {
        transform: scale(1.05);
    }

    .product-info {
        padding: 1.5rem;
    }

    .product-name {
        font-size: 1.2rem;
        color: var(--text-dark);
        margin-bottom: 0.5rem;
    }

    .product-price {
        font-size: 1.5rem;
        color: var(--secondary-color);
        font-weight: bold;
        margin-bottom: 1rem;
    }

    .add-to-cart {
        width: 100%;
        background: var(--primary-color);
        color: var(--white);
        border: none;
        padding: 0.8rem;
        border-radius: 8px;
        cursor: pointer;
        font-size: 1rem;
        transition: all 0.3s ease;
        position: relative;
        overflow: hidden;
        z-index: 1;
    }

    .add-to-cart::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 0;
        height: 100%;
        background: var(--secondary-color);
        transition: width 0.5s ease;
        z-index: -1;
    }

    .add-to-cart:hover::before {
        width: 100%;
    }

    .add-to-cart:hover {
        transform: translateY(-2px);
        box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }

    /* Features Section */
    .features {
        background: linear-gradient(135deg, var(--bg-light) 0%, #F5E6D3 100%);
        padding: 4rem 5%;
        position: relative;
        overflow: hidden;
    }

    .features::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><path d="M0,0 Q50,20 100,0 L100,100 Q50,80 0,100 Z" fill="rgba(255,255,255,0.2)"/></svg>');
        background-size: cover;
        opacity: 0.3;
    }

    .features-container {
        max-width: 1200px;
        margin: 0 auto;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 2rem;
    }

    .feature {
        text-align: center;
        padding: 2rem;
    }

    .feature-icon {
        font-size: 3rem;
        color: var(--secondary-color);
        margin-bottom: 1rem;
    }

    .feature h3 {
        color: var(--text-dark);
        margin-bottom: 0.5rem;
    }

    /* Footer */
    footer {
        background: linear-gradient(135deg, var(--text-dark) 0%, #1A0F0A 100%);
        color: var(--white);
        padding: 3rem 5%;
        text-align: center;
        position: relative;
        overflow: hidden;
    }

    footer::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><path d="M0,0 Q50,20 100,0 L100,100 Q50,80 0,100 Z" fill="rgba(255,255,255,0.05)"/></svg>');
        background-size: cover;
        opacity: 0.3;
    }

    .footer-content {
        max-width: 1200px;
        margin: 0 auto;
    }

    .social-links {
        margin-top: 1rem;
    }

    .social-links a {
        color: var(--white);
        font-size: 1.5rem;
        margin: 0 1rem;
        text-decoration: none;
    }

    /* Responsive */
    @media (max-width: 768px) {
        .nav-links {
            display: none;
        }
        
        .hero h1 {
            font-size: 2rem;
        }
        
        .section-title {
            font-size: 2rem;
        }
    }
</style>
Fabric Haven
Home
Categories
Products
About
Contact
🛒 0
<!-- Hero Section -->
<section class="hero" id="home">
    <h1>Welcome to Fabric Haven</h1>
    <p>Discover the finest quality fabrics for all your creative projects</p>
    <a href="#products" class="cta-button">Shop Now</a>
</section>

<!-- Categories Section -->
<section class="categories" id="categories">
    <h2 class="section-title">Browse by Category</h2>
    <div class="category-grid">
        <div class="category-card">
            <img src="https://images.unsplash.com/photo-1558618666-fcd25c85cd64?w=400" alt="Cotton Fabric" class="category-image">
            <div class="category-info">
                <h3>Cotton Fabrics</h3>
                <p>Soft, breathable, and versatile cotton fabrics</p>
            </div>
        </div>
        <div class="category-card">
            <img src="https://images.unsplash.com/photo-1620799140408-edc6dcb6d633?w=400" alt="Silk Fabric" class="category-image">
            <div class="category-info">
                <h3>Silk Fabrics</h3>
                <p>Luxurious silk for special occasions</p>
            </div>
        </div>
        <div class="category-card">
            <img src="https://images.unsplash.com/photo-1608222352225-523c944a9616?w=400" alt="Linen Fabric" class="category-image">
            <div class="category-info">
                <h3>Linen Fabrics</h3>
                <p>Natural linen perfect for summer wear</p>
            </div>
        </div>
        <div class="category-card">
            <img src="https://images.unsplash.com/photo-1594633312681-425c7b97ccd1?w=400" alt="Wool Fabric" class="category-image">
            <div class="category-info">
                <h3>Wool Fabrics</h3>
                <p>Warm and cozy wool for winter projects</p>
            </div>
        </div>
    </div>
</section>

<!-- Products Section -->
<section class="products" id="products">
    <h2 class="section-title">Featured Products</h2>
    <div class="product-grid">
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1528795259021-d8c86e14355d?w=400" alt="Premium Cotton" class="product-image">
            <div class="product-info">
                <h3 class="product-name">Premium Cotton - Floral Print</h3>
                <p class="product-price">$12.99/yard</p>
                <button class="add-to-cart" onclick="addToCart()">Add to Cart</button>
            </div>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1568254183919-78a4f43a5c11?w=400" alt="Silk Satin" class="product-image">
            <div class="product-info">
                <h3 class="product-name">Silk Satin - Emerald Green</h3>
                <p class="product-price">$45.99/yard</p>
                <button class="add-to-cart" onclick="addToCart()">Add to Cart</button>
            </div>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1571115764595-644a1f56a55c?w=400" alt="Linen Blend" class="product-image">
            <div class="product-info">
                <h3 class="product-name">Linen Blend - Natural Beige</h3>
                <p class="product-price">$18.99/yard</p>
                <button class="add-to-cart" onclick="addToCart()">Add to Cart</button>
            </div>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1584917865442-de89df76afd3?w=400" alt="Wool Tweed" class="product-image">
            <div class="product-info">
                <h3 class="product-name">Wool Tweed - Classic Gray</h3>
                <p class="product-price">$35.99/yard</p>
                <button class="add-to-cart" onclick="addToCart()">Add to Cart</button>
            </div>
        </div>
    </div>
</section>

<!-- Features Section -->
<section class="features">
    <div class="features-container">
        <div class="feature">
            <div class="feature-icon">🚚</div>
            <h3>Free Shipping</h3>
            <p>On orders over $50</p>
        </div>
        <div class="feature">
            <div class="feature-icon">🎨</div>
            <h3>Wide Selection</h3>
            <p>Over 1000+ fabric choices</p>
        </div>
        <div class="feature">
            <div class="feature-icon">💎</div>
            <h3>Premium Quality</h3>
            <p>Hand-selected fabrics</p>
        </div>
        <div class="feature">
            <div class="feature-icon">📞</div>
            <h3>Expert Support</h3>
            <p>Help with fabric selection</p>
        </div>
    </div>
</section>

<!-- Footer -->
<footer>
    <div class="footer-content">
        <p>&copy; 2024 Fabric Haven. All rights reserved.</p>
        <div class="social-links">
            <a href="#">📘</a>
            <a href="#">📷</a>
            <a href="#">🐦</a>
            <a href="#">📧</a>
        </div>
    </div>
</footer>

<script>
    let cartCount = 0;

    function addToCart() {
        cartCount++;
        document.querySelector('.cart-count').textContent = cartCount;
        
        // Create a temporary notification
        const notification = document.createElement('div');
        notification.style.cssText = `
            position: fixed;
            top: 100px;
            right: 20px;
            background: var(--secondary-color);
            color: white;
            padding: 1rem 2rem;
            border-radius: 5px;
            animation: slideIn 0.3s ease;
            z-index: 2000;
        `;
        notification.textContent = 'Added to cart!';
        document.body.appendChild(notification);
        
        setTimeout(() => {
            notification.remove();
        }, 2000);
    }

    // Smooth scrolling for navigation links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            document.querySelector(this.getAttribute('href')).scrollIntoView({
                behavior: 'smooth'
            });
        });
    });

    // Add animation styles
    const style = document.createElement('style');
    style.textContent = `
        @keyframes slideIn {
            from {
                transform: translateX(100%);
                opacity: 0;
            }
            to {
                transform: translateX(0);
                opacity: 1;
            }
        }
    `;
    document.head.appendChild(style);
</script>
