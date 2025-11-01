<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>M A Q - Professional Social Media Services</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;700;900&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-color: #000000;
            --accent-color: #ffffff;
            --glow-color: rgba(255, 255, 255, 0.8);
            --text-color: #f0f0f0;
            --card-bg: rgba(30, 30, 30, 0.8);
            --transition: all 0.3s ease;
        }

        body {
            background-color: var(--primary-color);
            color: var(--text-color);
            line-height: 1.6;
            overflow-x: hidden;
            font-family: 'Orbitron', sans-serif;
        }

        /* Header Styles */
        header {
            background-color: rgba(0, 0, 0, 0.9);
            padding: 1.5rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 2.5rem;
            font-weight: 900;
            letter-spacing: 5px;
            color: var(--accent-color);
            text-shadow: 0 0 10px var(--glow-color);
            text-decoration: none;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            color: var(--text-color);
            text-decoration: none;
            font-weight: 500;
            font-size: 1.1rem;
            transition: var(--transition);
            padding: 0.5rem 1rem;
            border-radius: 4px;
        }

        nav ul li a:hover {
            color: var(--accent-color);
            text-shadow: 0 0 8px var(--glow-color);
            background: rgba(255, 255, 255, 0.1);
        }

        /* Enhanced Styles for Links and Lists */
        .service-card ul {
            list-style: none;
            padding-left: 1rem;
            margin-top: 1rem;
        }

        .service-card ul li {
            margin-bottom: 0.5rem;
            position: relative;
            padding-left: 1.5rem;
            color: #ccc;
        }

        .service-card ul li:before {
            content: "•";
            position: absolute;
            left: 0;
            color: var(--accent-color);
        }

        .contact-text p {
            white-space: pre-line;
        }

        a {
            color: var(--accent-color);
            text-decoration: none;
            transition: var(--transition);
        }

        a:hover {
            text-shadow: 0 0 8px var(--glow-color);
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 8rem 0 5rem;
            background: radial-gradient(circle at center, rgba(40, 40, 40, 0.8) 0%, rgba(0, 0, 0, 1) 70%);
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            color: var(--accent-color);
            text-shadow: 0 0 15px var(--glow-color);
            letter-spacing: 3px;
        }

        .hero p {
            font-size: 1.3rem;
            max-width: 800px;
            margin: 0 auto 2.5rem;
            color: #ccc;
        }

        /* Service Cards */
        .services {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .service-card {
            background: var(--card-bg);
            border-radius: 10px;
            padding: 2.5rem 2rem;
            text-align: left;
            transition: var(--transition);
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(5px);
        }

        .service-card:hover {
            transform: translateY(-10px);
            border-color: var(--accent-color);
            box-shadow: 0 10px 20px rgba(255, 255, 255, 0.1);
        }

        .service-card i {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            color: var(--accent-color);
            text-shadow: 0 0 10px var(--glow-color);
        }

        .service-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--accent-color);
        }

        .service-card p {
            color: #ccc;
            margin-bottom: 1rem;
        }

        /* Contact Section */
        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            margin-top: 3rem;
        }

        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }

        .contact-item {
            background: var(--card-bg);
            border-radius: 10px;
            padding: 2rem;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .contact-item i {
            font-size: 2rem;
            color: var(--accent-color);
            margin-bottom: 1rem;
        }

        .contact-text h3 {
            color: var(--accent-color);
            margin-bottom: 0.5rem;
        }

        .contact-form {
            background: var(--card-bg);
            padding: 2.5rem;
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        /* Additional Styles */
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2.5rem;
            color: var(--accent-color);
            text-shadow: 0 0 10px var(--glow-color);
            letter-spacing: 2px;
        }

        .btn {
            display: inline-block;
            background: transparent;
            color: var(--accent-color);
            padding: 0.9rem 2rem;
            border: 2px solid var(--accent-color);
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: var(--transition);
            text-transform: uppercase;
            letter-spacing: 1px;
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.2);
        }

        .btn:hover {
            background: rgba(255, 255, 255, 0.1);
            box-shadow: 0 0 20px var(--glow-color);
            transform: translateY(-3px);
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .contact-content {
                grid-template-columns: 1fr;
            }
            
            .hero h1 {
                font-size: 3rem;
            }
        }

        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }

            nav ul {
                margin-top: 1.5rem;
                justify-content: center;
                flex-wrap: wrap;
            }

            nav ul li {
                margin: 0.5rem;
            }

            .hero {
                padding: 6rem 0 3rem;
            }

            .hero h1 {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <a href="#" class="logo">M A Q</a>
                <nav>
                    <ul>
                        <li><a href="#home" class="nav-link active">Home</a></li>
                        <li><a href="#services" class="nav-link">Services</a></li>
                        <li><a href="#about" class="nav-link">About</a></li>
                        <li><a href="#contact" class="nav-link">Contact</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <h1>PROFESSIONAL SOCIAL MEDIA SERVICES & ACCOUNT RECOVERY</h1>
            <p>Industry-leading expertise in social media account recovery, verification, and platform optimization. Trusted by influencers, businesses, and individual users worldwide.</p>
            <a href="#services" class="btn">Explore Our Solutions</a>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="container">
        <h2 class="section-title">Our Professional Services</h2>
        <div class="services">
            <div class="service-card">
                <i class="fas fa-shield-alt"></i>
                <h3>Meta Verification Services</h3>
                <p>Comprehensive Meta verification services for both personal and business accounts on Instagram and Facebook. Our process includes:</p>
                <ul>
                    <li>Documentation review and optimization</li>
                    <li>Profile enhancement for verification eligibility</li>
                    <li>Press coverage and digital presence development</li>
                    <li>Direct support throughout the verification process</li>
                    <li>Post-verification compliance guidance</li>
                </ul>
            </div>

            <div class="service-card">
                <i class="fas fa-user-shield"></i>
                <h3>Professional Account Recovery</h3>
                <p>Specialized in recovering compromised, banned, or restricted accounts across all major social media platforms:</p>
                <ul>
                    <li>Detailed account security audit</li>
                    <li>Custom appeal documentation preparation</li>
                    <li>Direct communication with platform support</li>
                    <li>Account reinstatement verification</li>
                    <li>Post-recovery security implementation</li>
                </ul>
            </div>

            <div class="service-card">
                <i class="fas fa-building"></i>
                <h3>Business Verification</h3>
                <p>Complete business verification services for enhanced credibility:</p>
                <ul>
                    <li>Business documentation preparation</li>
                    <li>Legal compliance verification</li>
                    <li>Business manager setup and optimization</li>
                    <li>Domain verification assistance</li>
                    <li>Business suite integration</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="container">
        <h2 class="section-title">Get In Touch</h2>
        <div class="contact-content">
            <div class="contact-info">
                <div class="contact-item">
                    <i class="fab fa-telegram"></i>
                    <div class="contact-text">
                        <h3>Secure Telegram Contact</h3>
                        <p>Official Channel: @MAQExpert_Official
                        Direct Support: @MAQExpert_Support
                        Response Time: Within 2 Hours</p>
                    </div>
                </div>
                
                <div class="contact-item">
                    <i class="fas fa-shield-check"></i>
                    <div class="contact-text">
                        <h3>Security Guarantee</h3>
                        <p>• End-to-end encrypted communication
                        • Secure payment processing
                        • Confidentiality agreement available
                        • Money-back guarantee</p>
                    </div>
                </div>

                <div class="contact-item">
                    <i class="fas fa-clock"></i>
                    <div class="contact-text">
                        <h3>Business Hours</h3>
                        <p>24/7 Support Available
                        Average Response Time: 2 Hours
                        Priority Support Available</p>
                    </div>
                </div>
            </div>

            <div class="contact-form">
                <form id="contactForm">
                    <div class="form-group">
                        <label for="name">Full Name</label>
                        <input type="text" id="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email Address</label>
                        <input type="email" id="email" required>
                    </div>
                    <div class="form-group">
                        <label for="service">Service Required</label>
                        <select id="service" required>
                            <option value="">Select a Service</option>
                            <option value="meta-verification">Meta Verification</option>
                            <option value="account-recovery">Account Recovery</option>
                            <option value="business-verification">Business Verification</option>
                            <option value="consultation">Professional Consultation</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="message">Your Message</label>
                        <textarea id="message" rows="5" required></textarea>
                    </div>
                    <button type="submit" class="btn">Send Secure Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2025 MAQ Professional Services. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Basic Navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Form Submission
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            // Add your form submission logic here
            alert('Thank you for your message. We will contact you shortly.');
        });
    </script>
</body>
</html>
