# Ex02 Commercial Website
## Date:12/02/2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
```
index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechNova - Premium Electronics Store</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar">
        <div class="logo">TechNova</div>
        <ul class="nav-links">
            <li><a href="index.html">Home</a></li>
            <li><a href="products.html">Products</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="account.html">Account</a></li>
        </ul>
    </nav>

    <!-- Hero -->
    <section class="hero">
        <div class="hero-content">
            <h1>Premium Gadgets Await</h1>
            <p>Discover cutting-edge electronics with unbeatable prices and fast delivery</p>
            <a href="products.html" class="cta-primary">Shop Collection</a>
            <a href="products.html" class="cta-secondary">Latest Arrivals</a>
        </div>
    </section>

    <!-- Featured Products -->
    <section class="section container">
        <h2>Featured Products</h2>
        <div class="featured-grid">
            <div class="featured-card">
                <img src="images/istockphoto-2243244875-1024x1024.jpg" alt="iPhone 16 Pro">
                <div class="card-content">
                    <h3>iPhone 16 Pro</h3>
                    <div class="price">₹99,999</div>
                    <a href="products.html" class="btn">Quick View</a>
                </div>
            </div>
            <div class="featured-card">
                <img src="https://images.unsplash.com/photo-1541807084-5c52b6b3adef?w=400&h=300&fit=crop" alt="MacBook Pro">
                <div class="card-content">
                    <h3>MacBook Pro M3</h3>
                    <div class="price">₹1,79,999</div>
                    <a href="products.html" class="btn">Quick View</a>
                </div>
            </div>
            <div class="featured-card">
                <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=400&h=300&fit=crop" alt="Apple Watch">
                <div class="card-content">
                    <h3>Apple Watch Ultra</h3>
                    <div class="price">₹79,999</div>
                    <a href="products.html" class="btn">Quick View</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-content container">
            <p>© 2026 TechNova Store. Maleni M</p>
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-linkedin"></i></a>
            </div>
        </div>
    </footer>
</body>
</html>

products.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Products - TechNova Store</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Quick fixes for consistent cards */
        .product-card { position: relative; }
        .product-image { position: relative; overflow: hidden; }
        .product-image img { width: 100%; height: 240px; object-fit: cover; display: block; }
    </style>
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar">
        <div class="logo">TechNova</div>
        <ul class="nav-links">
            <li><a href="index.html">Home</a></li>
            <li><a href="products.html">Products</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="account.html">Account</a></li>
        </ul>
    </nav>

    <!-- Products Hero -->
    <section class="hero" style="height: 60vh; background: linear-gradient(135deg, #f8fafc, #e2e8f0); color: #1e293b;">
        <div class="hero-content container">
            <h1 style="color: #1e293b;">Our Product Collection</h1>
            <p style="color: #64748b;">Premium electronics with best prices guaranteed</p>
        </div>
    </section>

    <!-- Filters + Products -->
    <section class="section container">
        <!-- Filters -->
        <div class="filters" style="display: flex; gap: 1rem; margin-bottom: 3rem; flex-wrap: wrap; align-items: center;">
            <select style="padding: 12px 20px; border: 2px solid #e2e8f0; border-radius: 12px; font-family: inherit;">
                <option>All Categories</option>
                <option>Smartphones</option>
                <option>Laptops</option>
                <option>Watches</option>
                <option>Accessories</option>
            </select>
            <select style="padding: 12px 20px; border: 2px solid #e2e8f0; border-radius: 12px; font-family: inherit;">
                <option>Sort: Featured</option>
                <option>Price: Low to High</option>
                <option>Price: High to Low</option>
                <option>Newest</option>
            </select>
            <div style="margin-left: auto; display: flex; gap: 1rem;">
                <button class="btn" style="background: #f1f5f9; color: #475569; padding: 12px 24px;"><i class="fas fa-th-large"></i></button>
                <button class="btn" style="background: #2563eb; color: white; padding: 12px 24px;"><i class="fas fa-list"></i></button>
            </div>
        </div>

        <!-- Products Grid -->
        <div class="products-grid">
            <!-- Product 1 - iPhone -->
            <div class="product-card">
                <div class="product-image">
                    <img src="images/istockphoto-2243244875-1024x1024.jpg" alt="iPhone 16 Pro">
                    <div class="badge" style="position: absolute; top: 1rem; left: 1rem; background: #10b981; color: white; padding: 0.3rem 0.8rem; border-radius: 20px; font-size: 0.8rem; font-weight: 600;">-15%</div>
                    <button class="wishlist" style="position: absolute; top: 1rem; right: 1rem; background: rgba(255,255,255,0.9); border: none; width: 44px; height: 44px; border-radius: 50%; cursor: pointer;"><i class="far fa-heart"></i></button>
                </div>
                <div class="card-content" style="padding: 1.5rem;">
                    <h3>iPhone 16 Pro Max</h3>
                    <div class="rating" style="color: #fbbf24; margin-bottom: 0.5rem;">
                        <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i> (127)
                    </div>
                    <div class="price-flex" style="display: flex; align-items: center; gap: 1rem; margin-bottom: 1rem;">
                        <span class="new-price" style="font-size: 1.6rem; font-weight: 700; color: #10b981;">₹84,999</span>
                        <span class="old-price" style="text-decoration: line-through; color: #94a3b8; font-size: 1.1rem;">₹99,999</span>
                    </div>
                    <div class="product-actions" style="display: flex; gap: 1rem;">
                        <button class="btn" style="flex: 1; background: #2563eb; color: white; padding: 12px;">Add to Cart</button>
                        <button style="width: 44px; height: 44px; border: 2px solid #e2e8f0; background: white; border-radius: 12px; cursor: pointer;"><i class="fas fa-eye"></i></button>
                    </div>
                </div>
            </div>

            <!-- Product 2 - MacBook -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1541807084-5c52b6b3adef?w=400&h=280&fit=crop" alt="MacBook Pro">
                    <div class="badge" style="position: absolute; top: 1rem; left: 1rem; background: #10b981; color: white; padding: 0.3rem 0.8rem; border-radius: 20px; font-size: 0.8rem; font-weight: 600;">-10%</div>
                    <button class="wishlist" style="position: absolute; top: 1rem; right: 1rem; background: rgba(255,255,255,0.9); border: none; width: 44px; height: 44px; border-radius: 50%; cursor: pointer;"><i class="far fa-heart"></i></button>
                </div>
                <div class="card-content" style="padding: 1.5rem;">
                    <h3>MacBook Pro M3</h3>
                    <div class="rating" style="color: #fbbf24; margin-bottom: 0.5rem;">
                        <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="far fa-star"></i> (89)
                    </div>
                    <div class="price-flex" style="display: flex; align-items: center; gap: 1rem; margin-bottom: 1rem;">
                        <span style="font-size: 1.6rem; font-weight: 700; color: #10b981;">₹1,79,999</span>
                    </div>
                    <div class="product-actions" style="display: flex; gap: 1rem;">
                        <button class="btn" style="flex: 1; background: #2563eb; color: white; padding: 12px;">Add to Cart</button>
                        <button style="width: 44px; height: 44px; border: 2px solid #e2e8f0; background: white; border-radius: 12px; cursor: pointer;"><i class="fas fa-eye"></i></button>
                    </div>
                </div>
            </div>

            <!-- Product 3 - Apple Watch -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=400&h=280&fit=crop" alt="Apple Watch">
                    <div class="badge" style="position: absolute; top: 1rem; left: 1rem; background: #ef4444; color: white; padding: 0.3rem 0.8rem; border-radius: 20px; font-size: 0.8rem; font-weight: 600;">New</div>
                    <button class="wishlist" style="position: absolute; top: 1rem; right: 1rem; background: rgba(255,255,255,0.9); border: none; width: 44px; height: 44px; border-radius: 50%; cursor: pointer;"><i class="far fa-heart"></i></button>
                </div>
                <div class="card-content" style="padding: 1.5rem;">
                    <h3>Apple Watch Ultra 2</h3>
                    <div class="rating" style="color: #fbbf24; margin-bottom: 0.5rem;">
                        <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i> (203)
                    </div>
                    <div class="price-flex" style="display: flex; align-items: center; gap: 1rem; margin-bottom: 1rem;">
                        <span style="font-size: 1.6rem; font-weight: 700; color: #10b981;">₹79,999</span>
                    </div>
                    <div class="product-actions" style="display: flex; gap: 1rem;">
                        <button class="btn" style="flex: 1; background: #2563eb; color: white; padding: 12px;">Add to Cart</button>
                        <button style="width: 44px; height: 44px; border: 2px solid #e2e8f0; background: white; border-radius: 12px; cursor: pointer;"><i class="fas fa-eye"></i></button>
                    </div>
                </div>
            </div>

            <!-- Product 4 - Sony Headphones -->
            <div class="product-card">
                <div class="product-image">
                    <img src="images/Screenshot 2026-02-12 200943.png" alt="Sony Headphones">
                    <div class="badge" style="position: absolute; top: 1rem; left: 1rem; background: #f59e0b; color: white; padding: 0.3rem 0.8rem; border-radius: 20px; font-size: 0.8rem; font-weight: 600;">Top Rated</div>
                    <button class="wishlist" style="position: absolute; top: 1rem; right: 1rem; background: rgba(255,255,255,0.9); border: none; width: 44px; height: 44px; border-radius: 50%; cursor: pointer;"><i class="far fa-heart"></i></button>
                </div>
                <div class="card-content" style="padding: 1.5rem;">
                    <h3>Sony WH-1000XM5</h3>
                    <div class="rating" style="color: #fbbf24; margin-bottom: 0.5rem;">
                        <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="far fa-star"></i> (156)
                    </div>
                    <div class="price-flex" style="display: flex; align-items: center; gap: 1rem; margin-bottom: 1rem;">
                        <span style="font-size: 1.6rem; font-weight: 700; color: #10b981;">₹29,999</span>
                    </div>
                    <div class="product-actions" style="display: flex; gap: 1rem;">
                        <button class="btn" style="flex: 1; background: #2563eb; color: white; padding: 12px;">Add to Cart</button>
                        <button style="width: 44px; height: 44px; border: 2px solid #e2e8f0; background: white; border-radius: 12px; cursor: pointer;"><i class="fas fa-eye"></i></button>
                    </div>
                </div>
            </div>

            

           
            

            
        </div>
    </section>

    <!-- Pagination -->
    <div style="text-align: center; padding: 2rem 0;">
        <div style="display: flex; justify-content: center; gap: 0.5rem; flex-wrap: wrap;">
            <button style="padding: 12px 20px; border: 2px solid #e2e8f0; background: white; border-radius: 8px; cursor: pointer;">Previous</button>
            <button style="padding: 12px 20px; border: 2px solid #2563eb; background: #2563eb; color: white; border-radius: 8px; cursor: pointer;">1</button>
            <button style="padding: 12px 20px; border: 2px solid #e2e8f0; background: white; border-radius: 8px; cursor: pointer;">2</button>
            <button style="padding: 12px 20px; border: 2px solid #e2e8f0; background: white; border-radius: 8px; cursor: pointer;">3</button>
            <button style="padding: 12px 20px; border: 2px solid #e2e8f0; background: white; border-radius: 8px; cursor: pointer;">Next</button>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="footer-content container">
            <p>© 2026 TechNova Store. Maleni M</p>
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-linkedin"></i></a>
            </div>
        </div>
    </footer>
</body>
</html>

about.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About - TechNova Store</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar">
        <div class="logo">TechNova</div>
        <ul class="nav-links">
            <li><a href="index.html">Home</a></li>
            <li><a href="products.html">Products</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="account.html">Account</a></li>
        </ul>
    </nav>

    <!-- About Hero -->
    <section class="hero" style="height: 70vh; background: linear-gradient(135deg, #f8fafc, #e2e8f0); color: #1e293b;">
        <div class="hero-content container">
            <h1 style="color: #1e293b;">About TechNova</h1>
            <p style="color: #64748b; font-size: 1.3rem;">Premium electronics delivered with passion since 2020</p>
        </div>
    </section>

    <!-- Story Section -->
    <section class="section container">
        <div class="story-flex" style="display: flex; gap: 4rem; align-items: center; flex-wrap: wrap;">
            <div style="flex: 1; min-width: 300px;">
                <h2 style="font-size: 2.5rem; margin-bottom: 1.5rem; color: #2563eb;">Our Story</h2>
                <p style="font-size: 1.2rem; color: #64748b; line-height: 1.8; margin-bottom: 1.5rem;">
                    Founded in 2020, TechNova revolutionized electronics retail in India. We source directly 
                    from manufacturers to offer premium gadgets at unbeatable prices with lightning-fast delivery.
                </p>
                <div style="display: flex; gap: 2rem; flex-wrap: wrap;">
                    <div style="text-align: center;">
                        <div style="font-size: 3rem; font-weight: 700; color: #10b981;">50K+</div>
                        <p style="color: #64748b;">Happy Customers</p>
                    </div>
                    <div style="text-align: center;">
                        <div style="font-size: 3rem; font-weight: 700; color: #2563eb;">24</div>
                        <p style="color: #64748b;">Cities Served</p>
                    </div>
                    <div style="text-align: center;">
                        <div style="font-size: 3rem; font-weight: 700; color: #f59e0b;">99%</div>
                        <p style="color: #64748b;">On-Time Delivery</p>
                    </div>
                </div>
            </div>
            <div style="flex: 1; min-width: 300px; text-align: center;">
                
<img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?w=600&h=400&fit=crop" alt="TechNova Team"></div>
        </div>
    </section>

    <!-- Mission Section -->
    <section class="section" style="background: linear-gradient(135deg, #f8fafc, #f1f5f9);">
        <div class="container">
            <h2 style="text-align: center; margin-bottom: 4rem;">Our Mission</h2>
            <div style="display: flex; gap: 2rem; flex-wrap: wrap; justify-content: center;">
                <div style="flex: 1 1 300px; background: white; padding: 2.5rem; border-radius: 20px; text-align: center; box-shadow: 0 10px 40px rgba(0,0,0,0.08);">
                    <div style="width: 80px; height: 80px; background: linear-gradient(135deg, #2563eb, #1d4ed8); border-radius: 20px; display: flex; align-items: center; justify-content: center; margin: 0 auto 1.5rem;">
                        <i class="fas fa-truck" style="font-size: 2rem; color: white;"></i>
                    </div>
                    <h3 style="font-size: 1.5rem; margin-bottom: 1rem; color: #1e293b;">Fast Delivery</h3>
                    <p style="color: #64748b;">Lightning-fast shipping across India within 24-48 hours</p>
                </div>
                <div style="flex: 1 1 300px; background: white; padding: 2.5rem; border-radius: 20px; text-align: center; box-shadow: 0 10px 40px rgba(0,0,0,0.08);">
                    <div style="width: 80px; height: 80px; background: linear-gradient(135deg, #10b981, #059669); border-radius: 20px; display: flex; align-items: center; justify-content: center; margin: 0 auto 1.5rem;">
                        <i class="fas fa-shield-alt" style="font-size: 2rem; color: white;"></i>
                    </div>
                    <h3 style="font-size: 1.5rem; margin-bottom: 1rem; color: #1e293b;">Secure Shopping</h3>
                    <p style="color: #64748b;">SSL encrypted + 100% safe transactions guaranteed</p>
                </div>
                <div style="flex: 1 1 300px; background: white; padding: 2.5rem; border-radius: 20px; text-align: center; box-shadow: 0 10px 40px rgba(0,0,0,0.08);">
                    <div style="width: 80px; height: 80px; background: linear-gradient(135deg, #f59e0b, #d97706); border-radius: 20px; display: flex; align-items: center; justify-content: center; margin: 0 auto 1.5rem;">
                        <i class="fas fa-headset" style="font-size: 2rem; color: white;"></i>
                    </div>
                    <h3 style="font-size: 1.5rem; margin-bottom: 1rem; color: #1e293b;">24/7 Support</h3>
                    <p style="color: #64748b;">Round-the-clock customer service assistance</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-content container">
            <p>© 2026 TechNova Store. Maleni M </p>
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-linkedin"></i></a>
            </div>
        </div>
    </footer>
</body>
</html>

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact - TechNova Store</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar">
        <div class="logo">TechNova</div>
        <ul class="nav-links">
            <li><a href="index.html">Home</a></li>
            <li><a href="products.html">Products</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="account.html">Account</a></li>
        </ul>
    </nav>

    <!-- Contact Hero -->
    <section class="hero" style="height: 50vh; background: linear-gradient(135deg, #f8fafc, #e2e8f0); color: #1e293b;">
        <div class="hero-content container">
            <h1 style="color: #1e293b;">Get In Touch</h1>
            <p style="color: #64748b;">We're here to help. Contact us anytime!</p>
        </div>
    </section>

    <!-- Contact Main -->
    <section class="section container">
        <div class="contact-flex" style="display: flex; gap: 4rem; flex-wrap: wrap;">
            <!-- Contact Info -->
            <div style="flex: 1; min-width: 300px;">
                <h2 style="font-size: 2rem; margin-bottom: 2rem; color: #1e293b;">Contact Information</h2>
                <div style="display: flex; flex-direction: column; gap: 2rem;">
                    <div style="display: flex; align-items: center; gap: 1rem;">
                        <div style="width: 50px; height: 50px; background: linear-gradient(135deg, #2563eb, #1d4ed8); border-radius: 12px; display: flex; align-items: center; justify-content: center;">
                            <i class="fas fa-phone" style="color: white; font-size: 1.2rem;"></i>
                        </div>
                        <div>
                            <h4 style="font-size: 1.1rem; margin-bottom: 0.5rem;">Phone</h4>
                            <a href="tel:+919876543210" style="color: #2563eb; font-weight: 500;">+91 98765 43210</a>
                        </div>
                    </div>
                    <div style="display: flex; align-items: center; gap: 1rem;">
                        <div style="width: 50px; height: 50px; background: linear-gradient(135deg, #10b981, #059669); border-radius: 12px; display: flex; align-items: center; justify-content: center;">
                            <i class="fas fa-envelope" style="color: white; font-size: 1.2rem;"></i>
                        </div>
                        <div>
                            <h4 style="font-size: 1.1rem; margin-bottom: 0.5rem;">Email</h4>
                            <a href="mailto:support@technova.in" style="color: #2563eb; font-weight: 500;">support@technova.in</a>
                        </div>
                    </div>
                    <div style="display: flex; align-items: center; gap: 1rem;">
                        <div style="width: 50px; height: 50px; background: linear-gradient(135deg, #f59e0b, #d97706); border-radius: 12px; display: flex; align-items: center; justify-content: center;">
                            <i class="fas fa-map-marker-alt" style="color: white; font-size: 1.2rem;"></i>
                        </div>
                        <div>
                            <h4 style="font-size: 1.1rem; margin-bottom: 0.5rem;">Address</h4>
                            <p style="color: #64748b; margin: 0;">#123 Tech Street<br>Chennai, Tamil Nadu 600001</p>
                        </div>
                    </div>
                </div>
                <div style="margin-top: 2rem; padding: 1.5rem; background: #f8fafc; border-radius: 16px; text-align: center;">
                    <h4 style="color: #1e293b;">Business Hours</h4>
                    <p style="color: #64748b; margin: 0.5rem 0;">Mon-Sat: 9AM - 9PM<br>Sunday: 10AM - 6PM</p>
                </div>
            </div>

            <!-- Contact Form -->
            <div class="contact-form" style="flex: 1; min-width: 300px; background: white; padding: 3rem; border-radius: 24px; box-shadow: 0 20px 60px rgba(0,0,0,0.08);">
                <h2 style="font-size: 2rem; margin-bottom: 2rem; color: #1e293b;">Send Message</h2>
                <form>
                    <div class="form-row" style="display: flex; gap: 1rem; margin-bottom: 1.5rem;">
                        <div class="form-group" style="flex: 1;">
                            <input type="text" placeholder="Your Name" required style="width: 100%; padding: 1.2rem; border: 2px solid #e2e8f0; border-radius: 12px; font-family: inherit;">
                        </div>
                        <div class="form-group" style="flex: 1;">
                            <input type="email" placeholder="your@email.com" required style="width: 100%; padding: 1.2rem; border: 2px solid #e2e8f0; border-radius: 12px; font-family: inherit;">
                        </div>
                    </div>
                    <div class="form-group" style="margin-bottom: 1.5rem;">
                        <input type="text" placeholder="Subject" required style="width: 100%; padding: 1.2rem; border: 2px solid #e2e8f0; border-radius: 12px; font-family: inherit;">
                    </div>
                    <div class="form-group" style="margin-bottom: 2rem;">
                        <textarea rows="5" placeholder="Your message..." required style="width: 100%; padding: 1.2rem; border: 2px solid #e2e8f0; border-radius: 12px; font-family: inherit; resize: vertical;"></textarea>
                    </div>
                    <button type="submit" class="btn" style="width: 100%; padding: 1.2rem; background: linear-gradient(135deg, #2563eb, #1d4ed8); border: none; font-size: 1.1rem; font-weight: 600;">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-content container">
            <p>© 2026 TechNova Store. Maleni M</p>
            <div

account.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Account - TechNova Store</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar">
        <div class="logo">TechNova</div>
        <ul class="nav-links">
            <li><a href="index.html">Home</a></li>
            <li><a href="products.html">Products</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
            <li><a href="account.html" style="background: #2563eb; color: white;">Account</a></li>
        </ul>
    </nav>

    <!-- Account Hero -->
    <section class="hero" style="height: 50vh; background: linear-gradient(135deg, #f8fafc, #e2e8f0); color: #1e293b;">
        <div class="hero-content container">
            <h1 style="color: #1e293b;">My Account</h1>
            <p style="color: #64748b;">Manage your profile, orders, and preferences</p>
        </div>
    </section>

    <!-- Dashboard Main -->
    <div class="dashboard-container" style="max-width: 1200px; margin: 0 auto; padding: 3rem 20px; display: flex; gap: 3rem; flex-wrap: wrap;">
        
        <!-- Sidebar - FIXED -->
        <div class="account-sidebar" style="flex: 0 0 280px; min-width: 250px;">
            <div style="background: white; border-radius: 20px; padding: 2rem; box-shadow: 0 20px 60px rgba(0,0,0,0.08);">
                <div style="text-align: center; margin-bottom: 2rem;">
                    <img src="images/Screenshot 2026-02-12 201042.png" alt="Maleni Murugan" style="width: 80px; height: 80px; border-radius: 50%; border: 4px solid #e2e8f0; object-fit: cover;">
                    <h3 style="font-size: 1.3rem; color: #1e293b; margin: 0.5rem 0 0.25rem;">Maleni Murugan</h3>
                    <p style="color: #64748b; margin: 0; font-size: 0.95rem;">malenimurugan@email.com</p>
                </div>
                <ul style="list-style: none; padding: 0; margin: 0;">
                    <li style="margin-bottom: 0.5rem;"><a href="#profile" style="display: flex; align-items: center; gap: 1rem; padding: 1rem; color: #4b5563; text-decoration: none; border-radius: 12px; transition: all 0.3s; font-weight: 500;"><i class="fas fa-user"></i> Profile</a></li>
                    <li style="margin-bottom: 0.5rem;"><a href="#orders" style="display: flex; align-items: center; gap: 1rem; padding: 1rem; background: #f0f9ff; color: #2563eb; text-decoration: none; border-radius: 12px; font-weight: 600;"><i class="fas fa-shopping-bag"></i> Orders</a></li>
                    <li style="margin-bottom: 0.5rem;"><a href="#wishlist" style="display: flex; align-items: center; gap: 1rem; padding: 1rem; color: #4b5563; text-decoration: none; border-radius: 12px; font-weight: 500;"><i class="fas fa-heart"></i> Wishlist</a></li>
                    <li style="margin-bottom: 0.5rem;"><a href="#address" style="display: flex; align-items: center; gap: 1rem; padding: 1rem; color: #4b5563; text-decoration: none; border-radius: 12px; font-weight: 500;"><i class="fas fa-map-marker-alt"></i> Addresses</a></li>
                    <li style="margin-bottom: 2rem;"><a href="#payment" style="display: flex; align-items: center; gap: 1rem; padding: 1rem; color: #4b5563; text-decoration: none; border-radius: 12px; font-weight: 500;"><i class="fas fa-credit-card"></i> Payment Methods</a></li>
                    <li><a href="#" style="display: flex; align-items: center; gap: 1rem; padding: 1rem; background: linear-gradient(135deg, #ef4444, #dc2626); color: white; text-decoration: none; border-radius: 12px; font-weight: 500; box-shadow: 0 4px 12px rgba(239,68,68,0.3);"><i class="fas fa-sign-out-alt"></i> Logout</a></li>
                </ul>
            </div>
        </div>

        <!-- Main Content - FIXED -->
        <div class="account-main" style="flex: 1; min-width: 600px;">
            
            <!-- Orders Section -->
            <div id="orders" style="background: white; border-radius: 24px; padding: 3rem; box-shadow: 0 20px 60px rgba(0,0,0,0.08); margin-bottom: 2rem;">
                <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 2.5rem;">
                    <h2 style="font-size: 2.2rem; color: #1e293b; margin: 0;">Recent Orders</h2>
                    <a href="#" style="padding: 14px 28px; background: linear-gradient(135deg, #10b981, #059669); color: white; text-decoration: none; border-radius: 12px; font-weight: 600; box-shadow: 0 4px 12px rgba(16,185,129,0.3);">View All Orders</a>
                </div>
                
                <!-- Order 1 - FIXED -->
                <div style="display: flex; gap: 2rem; padding: 2rem; background: linear-gradient(135deg, #f8fafc, #f1f5f9); border-radius: 20px; align-items: center; margin-bottom: 1.5rem;">
                    <div style="flex: 0 0 90px; text-align: center;">
                        <img src="images/istockphoto-2243244875-1024x1024.jpg" alt="iPhone" style="width: 80px; height: 80px; border-radius: 16px; object-fit: cover; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
                    </div>
                    <div style="flex: 1;">
                        <h4 style="color: #1e293b; margin: 0 0 0.5rem; font-size: 1.2rem;">iPhone 16 Pro Max 256GB</h4>
                        <p style="color: #64748b; margin: 0 0 0.25rem; font-size: 0.95rem;">Order #12345 | Placed 2 days ago</p>
                    </div>
                    <div style="text-align: center; min-width: 120px;">
                        <div style="font-size: 1.6rem; font-weight: 700; color: #10b981; margin-bottom: 0.5rem;">₹84,999</div>
                        <span style="background: #dcfce7; color: #166534; padding: 0.4rem 1rem; border-radius: 25px; font-size: 0.85rem; font-weight: 500;">Delivered</span>
                    </div>
                    <a href="#" style="padding: 12px 24px; background: linear-gradient(135deg, #2563eb, #1d4ed8); color: white; text-decoration: none; border-radius: 12px; font-weight: 500; white-space: nowrap;">Reorder</a>
                </div>

                <!-- Order 2 - FIXED -->
                <div style="display: flex; gap: 2rem; padding: 2rem; background: linear-gradient(135deg, #f8fafc, #f1f5f9); border-radius: 20px; align-items: center;">
                    <div style="flex: 0 0 90px; text-align: center;">
                        <img src="https://images.unsplash.com/photo-1541807084-5c52b6b3adef?w=80&h=80&fit=crop" alt="MacBook" style="width: 80px; height: 80px; border-radius: 16px; object-fit: cover; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
                    </div>
                    <div style="flex: 1;">
                        <h4 style="color: #1e293b; margin: 0 0 0.5rem; font-size: 1.2rem;">MacBook Pro M3 512GB</h4>
                        <p style="color: #64748b; margin: 0 0 0.25rem; font-size: 0.95rem;">Order #12344 | Placed 1 week ago</p>
                    </div>
                    <div style="text-align: center; min-width: 120px;">
                        <div style="font-size: 1.6rem; font-weight: 700; color: #10b981; margin-bottom: 0.5rem;">₹1,79,999</div>
                        <span style="background: #fef3c7; color: #92400e; padding: 0.4rem 1rem; border-radius: 25px; font-size: 0.85rem; font-weight: 500;">Pending</span>
                    </div>
                    <a href="#" style="padding: 12px 24px; background: linear-gradient(135deg, #f59e0b, #d97706); color: white; text-decoration: none; border-radius: 12px; font-weight: 500; white-space: nowrap;">Track Order</a>
                </div>
            </div>

            <!-- Stats Cards - FIXED -->
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1.5rem; padding: 1rem;">
  <div style="background: linear-gradient(135deg, #3b82f6, #1d4ed8); color: white; padding: 2rem 1.5rem; border-radius: 24px; text-align: center; box-shadow: 0 20px 40px rgba(59,130,246,0.2);">
    <h3 style="font-size: clamp(2rem, 8vw, 2.5rem); font-weight: 700; margin: 0 0 0.25rem; line-height: 1; text-shadow: 0 2px 4px rgba(0,0,0,0.1);">3</h3>
    <p style="margin: 0; font-size: 1rem; opacity: 0.95; font-weight: 500;">Total Orders</p>
  </div>
  <div style="background: linear-gradient(135deg, #10b981, #059669); color: white; padding: 2rem 1.5rem; border-radius: 24px; text-align: center; box-shadow: 0 20px 40px rgba(16,185,129,0.2);">
    <h3 style="font-size: clamp(2rem, 8vw, 2.5rem); font-weight: 700; margin: 0 0 0.25rem; line-height: 1; text-shadow: 0 2px 4px rgba(0,0,0,0.1);">₹2,64,998</h3>
    <p style="margin: 0; font-size: 1rem; opacity: 0.95; font-weight: 500;">Total Spent</p>
  </div>
  <div style="background: linear-gradient(135deg, #f59e0b, #d97706); color: white; padding: 2rem 1.5rem; border-radius: 24px; text-align: center; box-shadow: 0 20px 40px rgba(245,158,11,0.2);">
    <h3 style="font-size: clamp(2rem, 8vw, 2.5rem); font-weight: 700; margin: 0 0 0.25rem; line-height: 1; text-shadow: 0 2px 4px rgba(0,0,0,0.1);">100%</h3>
    <p style="margin: 0; font-size: 1rem; opacity: 0.95; font-weight: 500;">On-Time Delivery</p>
  </div>
</div>

        </div>
    </div>

    <!-- Footer -->
    <footer style="margin-top: 4rem;">
        <div class="footer-content container">
            <p>© 2026 TechNova Store. Maleni M</p>
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-linkedin"></i></a>
            </div>
        </div>
    </footer>
</body>
</html>

style.css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');

* { margin: 0; padding: 0; box-sizing: border-box; }
body { 
    font-family: 'Inter', sans-serif; 
    line-height: 1.6; 
    color: #2d3748; 
    overflow-x: hidden;
}

.container { max-width: 1280px; margin: 0 auto; padding: 0 20px; }

/* === NAVBAR === */
.navbar {
    display: flex; 
    justify-content: space-between; 
    align-items: center; 
    padding: 1rem 5%; 
    background: rgba(255,255,255,0.95); 
    backdrop-filter: blur(20px);
    position: sticky; top: 0; z-index: 1000;
    box-shadow: 0 4px 20px rgba(0,0,0,0.08);
}
.logo { 
    font-size: 1.8rem; 
    font-weight: 700; 
    background: linear-gradient(135deg, #667eea, #764ba2); 
    -webkit-background-clip: text; 
    -webkit-text-fill-color: transparent; 
}
.nav-links { 
    display: flex; 
    list-style: none; 
    gap: 2.5rem; 
}
.nav-links a { 
    text-decoration: none; 
    color: #4a5568; 
    font-weight: 500; 
    padding: 0.5rem 1rem; 
    border-radius: 25px; 
    transition: all 0.3s ease; 
}
.nav-links a:hover { 
    background: linear-gradient(135deg, #667eea, #764ba2); 
    color: white; 
    transform: translateY(-2px);
}

/* === HERO === */
.hero { 
    height: 100vh; 
    background: linear-gradient(135deg, rgba(102,126,234,0.9), rgba(118,75,162,0.9)), 
                url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000"><defs><radialGradient id="a" cx="50%" cy="50%"><stop offset="0%" stop-color="%23ffffff" stop-opacity="0.1"/><stop offset="100%" stop-color="%23ffffff" stop-opacity="0"/></radialGradient></defs><rect width="100%" height="100%" fill="url(%23a)"/></svg>'); 
    display: flex; 
    align-items: center; 
    justify-content: center; 
    text-align: center; 
    color: white; 
}
.hero-content h1 { 
    font-size: clamp(3rem, 8vw, 6rem); 
    font-weight: 700; 
    margin-bottom: 1.5rem; 
    letter-spacing: -2px; 
}
.hero-content p { 
    font-size: 1.4rem; 
    max-width: 600px; 
    margin: 0 auto 3rem; 
    opacity: 0.95; 
}
.cta-primary, .cta-secondary {
    display: inline-block; 
    padding: 16px 40px; 
    border-radius: 50px; 
    font-weight: 600; 
    text-decoration: none; 
    transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1); 
    margin: 0 1rem; 
}
.cta-primary { 
    background: rgba(255,255,255,0.95); 
    color: #2d3748; 
    box-shadow: 0 10px 30px rgba(255,255,255,0.3); 
}
.cta-secondary { 
    background: transparent; 
    color: white; 
    border: 2px solid rgba(255,255,255,0.4); 
}
.cta-primary:hover, .cta-secondary:hover { 
    transform: translateY(-4px); 
    box-shadow: 0 20px 40px rgba(0,0,0,0.2); 
}

/* === SECTION === */
.section { padding: 8rem 0; }
.section h2 { 
    font-size: 3rem; 
    text-align: center; 
    margin-bottom: 4rem; 
    background: linear-gradient(135deg, #667eea, #764ba2); 
    -webkit-background-clip: text; 
    -webkit-text-fill-color: transparent; 
}

/* === FEATURED PRODUCTS === */
.featured-grid {
    display: flex; 
    gap: 2rem; 
    flex-wrap: wrap; 
    justify-content: center; 
}
.featured-card {
    flex: 1 1 350px; 
    background: white; 
    border-radius: 24px; 
    overflow: hidden; 
    box-shadow: 0 20px 60px rgba(0,0,0,0.1); 
    transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
    position: relative;
}
.featured-card::before {
    content: ''; 
    position: absolute; 
    top: 0; 
    left: 0; 
    right: 0; 
    height: 4px; 
    background: linear-gradient(90deg, #667eea, #764ba2, #f093fb); 
}
.featured-card:hover { 
    transform: translateY(-16px); 
    box-shadow: 0 40px 80px rgba(0,0,0,0.2); 
}
.featured-card img { 
    width: 100%; 
    height: 280px; 
    object-fit: cover; 
    transition: transform 0.4s ease; 
}
.featured-card:hover img { transform: scale(1.05); }
.card-content { 
    padding: 2rem; 
    text-align: center; 
}
.card-content h3 { 
    font-size: 1.5rem; 
    color: #2d3748; 
    margin-bottom: 0.5rem; 
}
.price { 
    font-size: 1.8rem; 
    font-weight: 700; 
    color: #10b981; 
    margin-bottom: 1rem; 
}

/* === PRODUCTS GRID (products.html) === */
.products-grid {
    display: flex; 
    flex-wrap: wrap; 
    gap: 2rem; 
    margin-top: 3rem; 
}
.product-card { 
    flex: 1 1 280px; 
    background: white; 
    border-radius: 20px; 
    overflow: hidden; 
    box-shadow: 0 10px 40px rgba(0,0,0,0.08); 
    transition: all 0.3s ease; 
}
.product-card:hover { 
    transform: translateY(-8px); 
    box-shadow: 0 20px 60px rgba(0,0,0,0.15); 
}

/* === CONTACT FORM === */
.contact-form {
    display: flex; 
    gap: 4rem; 
    max-width: 1000px; 
    margin: 0 auto; 
}
.form-group { 
    flex: 1; 
}
.form-group input, .form-group textarea { 
    width: 100%; 
    padding: 1.2rem; 
    border: 2px solid #e2e8f0; 
    border-radius: 12px; 
    font-family: inherit; 
    transition: all 0.3s; 
    font-size: 1rem; 
}
.form-group input:focus, .form-group textarea:focus { 
    outline: none; 
    border-color: #667eea; 
    box-shadow: 0 0 0 4px rgba(102,126,234,0.1); 
}

/* === FOOTER === */
footer { 
    background: linear-gradient(135deg, #1e293b, #334155); 
    color: white; 
    padding: 4rem 0 1rem; 
}
.footer-content {
    display: flex; 
    justify-content: space-between; 
    align-items: center; 
    flex-wrap: wrap; 
    gap: 2rem; 
    margin-bottom: 2rem; 
}
.social-links {
    display: flex; 
    gap: 1.5rem; 
}
.social-links a { 
    width: 48px; 
    height: 48px; 
    background: rgba(255,255,255,0.1); 
    border-radius: 50%; 
    display: flex; 
    align-items: center; 
    justify-content: center; 
    color: white; 
    text-decoration: none; 
    transition: all 0.3s; 
}
.social-links a:hover { 
    background: #667eea; 
    transform: translateY(-4px); 
}

/* === RESPONSIVE === */
@media (max-width: 768px) {
    .nav-links { gap: 1rem; flex-wrap: wrap; justify-content: center; }
    .hero-content h1 { font-size: 2.5rem; }
    .cta-primary, .cta-secondary { 
        padding: 14px 28px; 
        margin: 0.5rem; 
    }
    .contact-form { flex-direction: column; }
    .footer-content { flex-direction: column; text-align: center; }
}


```


## OUTPUT
![alt text](<Screenshot 2026-02-12 204715.png>)
![alt text](<Screenshot 2026-02-12 205552.png>)
![alt text](<Screenshot 2026-02-12 205624.png>)
![alt text](<Screenshot 2026-02-12 205636.png>)
![alt text](<Screenshot 2026-02-12 205657.png>)
![alt text](<Screenshot 2026-02-12 205820.png>)
![alt text](<Screenshot 2026-02-12 205710.png>)
![alt text](<Screenshot 2026-02-12 204906.png>)


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
