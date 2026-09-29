<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Excel Electricals | Motor Winding & Repair Workshop</title>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@500;600;700;800&family=Space+Grotesk:wght@700;800&display=swap" rel="stylesheet">
    
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <!-- Analytics Tag -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=AW-16970635311"></script>
    <script>
        window.dataLayer = window.dataLayer || [];
        function gtag(){dataLayer.push(arguments);}
        gtag('js', new Date());
        gtag('config', 'AW-16970635311');
    </script>

    <style>
        :root {
            --gold-primary: #d97706;
            --gold-accent: #f59e0b;
            --gold-bright: #fbbf24;
            --card-bg: rgba(15, 23, 42, 0.92);
            --card-border: rgba(245, 158, 11, 0.4);
            --text-main: #ffffff;
            --text-sub: #cbd5e1;
        }

        /* FULL SCREEN RESPONSIVE BACKGROUND IMAGE */
        html, body {
            width: 100%;
            min-height: 100vh;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: #000000;
            background-image: 
                linear-gradient(rgba(0, 0, 0, 0.45), rgba(0, 0, 0, 0.45)),
                url('motor%20wind..webp');
            background-repeat: no-repeat;
            background-position: center center;
            background-size: cover;
            background-attachment: fixed;
            color: #ffffff;
            scroll-behavior: smooth;
        }

        h1, h2, h3, h4, .brand-text {
            font-family: 'Space Grotesk', sans-serif;
            color: #ffffff;
            text-shadow: 0 3px 12px rgba(0,0,0,0.9);
        }

        * {
            box-sizing: border-box;
        }

        /* HEADER & NAVIGATION */
        header {
            width: 100%;
            background: rgba(10, 15, 29, 0.95);
            backdrop-filter: blur(12px);
            padding: 16px 5%;
            position: fixed;
            top: 0;
            left: 0;
            z-index: 1000;
            border-bottom: 2px solid var(--gold-primary);
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 25px rgba(0,0,0,0.8);
        }

        .brand-logo {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.4rem;
            font-weight: 800;
            color: #ffffff;
            text-decoration: none;
            letter-spacing: 0.5px;
        }

        .brand-icon {
            width: 44px;
            height: 44px;
            background: linear-gradient(135deg, var(--gold-bright), var(--gold-primary));
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #000;
            font-size: 1.3rem;
            box-shadow: 0 0 15px rgba(245, 158, 11, 0.6);
        }

        nav {
            display: flex;
            align-items: center;
            gap: 24px;
        }

        nav a {
            text-decoration: none;
            color: #ffffff;
            font-weight: 700;
            font-size: 0.98rem;
            transition: all 0.25s ease;
            text-shadow: 0 2px 4px rgba(0,0,0,0.8);
        }

        nav a:hover {
            color: var(--gold-bright);
        }

        .nav-btn {
            background: linear-gradient(135deg, var(--gold-bright), var(--gold-primary));
            color: #000000 !important;
            padding: 10px 22px;
            border-radius: 50px;
            font-weight: 800 !important;
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.5);
            text-shadow: none !important;
        }

        /* MOBILE MENU TOGGLE BUTTON */
        .mobile-toggle {
            display: none;
            background: linear-gradient(135deg, var(--gold-bright), var(--gold-primary));
            color: #000000;
            border: none;
            padding: 10px 14px;
            border-radius: 8px;
            font-size: 1.2rem;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.4);
        }

        /* HERO SECTION */
        .hero {
            position: relative;
            z-index: 1;
            width: 100%;
            min-height: 85vh;
            padding: 140px 5% 60px 5%;
            display: grid;
            grid-template-columns: 1.2fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .hero-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(0, 0, 0, 0.85);
            border: 1.5px solid var(--gold-bright);
            color: var(--gold-bright);
            padding: 8px 18px;
            border-radius: 50px;
            font-size: 0.9rem;
            font-weight: 800;
            margin-bottom: 22px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }

        .hero h1 {
            font-size: clamp(2.2rem, 5vw, 3.6rem);
            line-height: 1.15;
            margin-bottom: 20px;
            font-weight: 800;
            letter-spacing: -1px;
            text-shadow: 0 4px 20px rgba(0,0,0,1);
        }

        .hero h1 span {
            color: var(--gold-bright);
            text-shadow: 0 0 15px rgba(245, 158, 11, 0.5);
        }

        .hero p {
            font-size: clamp(1rem, 2vw, 1.2rem);
            color: #f8fafc;
            margin-bottom: 35px;
            max-width: 600px;
            line-height: 1.65;
            font-weight: 600;
            text-shadow: 0 2px 10px rgba(0,0,0,1);
        }

        .hero-buttons {
            display: flex;
            gap: 16px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 15px 32px;
            border-radius: 14px;
            font-weight: 800;
            font-size: 1rem;
            text-decoration: none;
            transition: all 0.3s ease;
            cursor: pointer;
            border: none;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--gold-bright), var(--gold-primary));
            color: #000000;
            box-shadow: 0 6px 20px rgba(245, 158, 11, 0.5);
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(245, 158, 11, 0.7);
        }

        .btn-outline {
            background: rgba(15, 23, 42, 0.9);
            color: #ffffff;
            border: 2px solid var(--gold-bright);
            box-shadow: 0 4px 15px rgba(0,0,0,0.6);
        }

        .btn-outline:hover {
            background: var(--gold-bright);
            color: #000000;
            transform: translateY(-3px);
        }

        .hero-img {
            width: 100%;
            height: 380px;
            object-fit: cover;
            border-radius: 24px;
            border: 3px solid var(--card-border);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.9);
        }

        /* SECTIONS */
        section {
            position: relative;
            z-index: 1;
            width: 100%;
            padding: 60px 5%;
            scroll-margin-top: 70px;
        }

        .section-header {
            text-align: center;
            max-width: 650px;
            margin: 0 auto 40px auto;
        }

        .section-header small {
            color: var(--gold-bright);
            font-weight: 800;
            letter-spacing: 2px;
            text-transform: uppercase;
            font-size: 0.9rem;
            display: block;
            margin-bottom: 8px;
            text-shadow: 0 2px 8px rgba(0,0,0,1);
        }

        .section-header h2 {
            font-size: clamp(1.8rem, 4vw, 2.6rem);
            letter-spacing: -0.8px;
            margin: 0;
            text-shadow: 0 4px 15px rgba(0,0,0,1);
        }

        /* GRID CARDS WITH MATCHING HEIGHT & NO BLANK GAPS */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 24px;
            width: 100%;
        }

        .card {
            background: var(--card-bg);
            border: 1.5px solid var(--card-border);
            border-radius: 20px;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            transition: all 0.35s ease;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(10px);
        }

        .card:hover {
            transform: translateY(-6px);
            border-color: var(--gold-bright);
            box-shadow: 0 15px 35px rgba(245, 158, 11, 0.35);
        }

        .card-img-wrapper {
            width: 100%;
            height: 180px;
            overflow: hidden;
            border-bottom: 2px solid var(--card-border);
        }

        .card-img-wrapper img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.4s ease;
        }

        .card:hover .card-img-wrapper img {
            transform: scale(1.05);
        }

        .card-body {
            padding: 22px;
            display: flex;
            flex-direction: column;
            flex-grow: 1;
        }

        .card-body h3 {
            font-size: 1.25rem;
            margin: 0 0 10px 0;
            color: #ffffff;
        }

        .card-body p {
            color: var(--text-sub);
            font-size: 0.95rem;
            line-height: 1.6;
            font-weight: 500;
            margin: 0;
        }

        .service-icon-box {
            display: flex;
            align-items: center;
            gap: 12px;
            margin-bottom: 12px;
        }

        .service-icon {
            width: 46px;
            height: 46px;
            min-width: 46px;
            background: linear-gradient(135deg, var(--gold-bright), var(--gold-primary));
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #000000;
            font-size: 1.3rem;
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.4);
        }

        /* ABOUT SECTION */
        .about-card {
            background: var(--card-bg);
            border: 1.5px solid var(--card-border);
            border-radius: 24px;
            padding: 35px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 35px;
            align-items: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(10px);
        }

        .about-features {
            list-style: none;
            margin-top: 20px;
            padding: 0;
        }

        .about-features li {
            margin-bottom: 12px;
            display: flex;
            align-items: center;
            gap: 12px;
            color: var(--text-sub);
            font-weight: 700;
            font-size: 1rem;
        }

        .about-features i {
            color: var(--gold-bright);
            font-size: 1.2rem;
        }

        /* CONTACTS & FORM */
        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            width: 100%;
        }

        .form-card {
            background: var(--card-bg);
            border: 1.5px solid var(--card-border);
            border-radius: 24px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(10px);
        }

        .form-group {
            margin-bottom: 18px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-size: 0.95rem;
            color: #ffffff;
            font-weight: 700;
        }

        .form-control {
            width: 100%;
            padding: 14px 16px;
            background: #ffffff;
            border: 2px solid #cbd5e1;
            border-radius: 12px;
            color: #000000;
            font-family: inherit;
            font-size: 1rem;
            font-weight: 600;
            transition: all 0.25s ease;
        }

        .form-control:focus {
            outline: none;
            border-color: var(--gold-bright);
            box-shadow: 0 0 0 4px rgba(245, 158, 11, 0.4);
        }

        .map-card {
            border-radius: 24px;
            overflow: hidden;
            border: 2px solid var(--card-border);
            min-height: 380px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.8);
        }

        /* FLOATING QUICK BAR */
        .floating-bar {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(10, 15, 29, 0.95);
            backdrop-filter: blur(16px);
            border: 2px solid var(--gold-bright);
            padding: 12px 28px;
            border-radius: 50px;
            display: flex;
            align-items: center;
            gap: 20px;
            z-index: 999;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.9);
            width: max-content;
            max-width: 90%;
            justify-content: center;
        }

        .float-link {
            display: flex;
            align-items: center;
            gap: 8px;
            color: #ffffff;
            text-decoration: none;
            font-size: 0.95rem;
            font-weight: 800;
        }

        .float-gold {
            color: var(--gold-bright);
        }

        /* FOOTER */
        footer {
            position: relative;
            z-index: 1;
            width: 100%;
            border-top: 2px solid var(--gold-primary);
            padding: 35px 5% 90px 5%;
            text-align: center;
            background: rgba(10, 15, 29, 0.95);
        }

        .rating-badge {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: rgba(0, 0, 0, 0.6);
            border: 1px solid var(--gold-bright);
            padding: 8px 20px;
            border-radius: 50px;
            margin-bottom: 18px;
            font-size: 0.95rem;
        }

        .stars {
            color: var(--gold-bright);
        }

        /* AUTOMATIC SCREEN SIZE RESPONSIVE RULES */
        @media (max-width: 992px) {
            .mobile-toggle {
                display: block;
            }

            nav {
                display: none;
                flex-direction: column;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background: rgba(10, 15, 29, 0.98);
                padding: 20px 5%;
                border-bottom: 2px solid var(--gold-primary);
                box-shadow: 0 10px 25px rgba(0,0,0,0.9);
                gap: 18px;
            }

            nav.active {
                display: flex;
            }

            nav a {
                font-size: 1.1rem;
                padding: 10px 0;
                text-align: center;
                border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            }

            .nav-btn {
                margin-top: 10px;
            }

            .hero {
                grid-template-columns: 1fr;
                text-align: center;
                padding-top: 110px;
                gap: 30px;
            }

            .hero p {
                margin: 0 auto 30px auto;
            }

            .hero-buttons {
                justify-content: center;
            }

            .about-card, .contact-grid {
                grid-template-columns: 1fr;
                padding: 24px;
            }

            section {
                padding: 50px 4%;
            }
        }
    </style>
</head>
<body>

    <!-- HEADER NAVIGATION -->
    <header>
        <a href="#home" class="brand-logo">
            <div class="brand-icon"><i class="fa-solid fa-bolt"></i></div>
            <span class="brand-text">EXCEL ELECTRICALS</span>
        </a>

        <!-- Hamburger Toggle Button for Mobile -->
        <button class="mobile-toggle" id="menuToggle" aria-label="Toggle Navigation">
            <i class="fa-solid fa-bars"></i>
        </button>

        <nav id="navMenu">
            <a href="#home">Home</a>
            <a href="#gallery">Gallery</a>
            <a href="#services">Services</a>
            <a href="#about">About</a>
            <a href="#contacts">Contacts</a>
            <a href="#request" class="nav-btn">Service Request</a>
        </nav>
    </header>

    <!-- HOME HERO SECTION -->
    <section class="hero" id="home">
        <div>
            <div class="hero-badge">
                <i class="fa-solid fa-shield-halved"></i> Certified Motor Workshop • Choondy, Aluva
            </div>
            <h1>EXPERT ELECTRIC <span>MOTOR WINDING</span> & REPAIR</h1>
            <p>Reliable stator rewinding, coil replacement, dynamic rotor testing, and complete motor repairs with guaranteed copper quality.</p>
            <div class="hero-buttons">
                <a href="tel:+918590259451" class="btn btn-primary"><i class="fa-solid fa-phone"></i> Call Workshop</a>
                <a href="https://wa.me/918590259451" class="btn btn-outline" target="_blank"><i class="fa-brands fa-whatsapp" style="color: #22c55e;"></i> WhatsApp Chat</a>
            </div>
        </div>
        <div>
            <img src="75 Hp.webp" alt="75 HP Motor Repair" class="hero-img">
        </div>
    </section>

    <!-- GALLERY SECTION -->
    <section id="gallery">
        <div class="section-header">
            <small>Workmanship</small>
            <h2>Motor Repair Gallery</h2>
        </div>
        <div class="cards-grid">
            <div class="card">
                <div class="card-img-wrapper">
                    <img src="Inducton motor.webp" alt="Induction Motor Repair">
                </div>
                <div class="card-body">
                    <h3>Induction Motor Repair</h3>
                    <p>Heavy duty single & 3-phase induction motor diagnostic, testing, and complete overhaul.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img-wrapper">
                    <img src="Motor.webp" alt="Mechanical Overhaul">
                </div>
                <div class="card-body">
                    <h3>Mechanical Overhaul</h3>
                    <p>Bearing replacement, shaft polish, dynamic rotor balancing, and housing alignment.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img-wrapper">
                    <img src="Field Winding.webp" alt="Stator Copper Winding">
                </div>
                <div class="card-body">
                    <h3>Stator Copper Winding</h3>
                    <p>High-grade dual coated copper wire coil insertion, slot insulation paper, and varnish dipping.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img-wrapper">
                    <img src="repair motor.webp" alt="Component Servicing">
                </div>
                <div class="card-body">
                    <h3>Component Servicing</h3>
                    <p>Capacitor replacement, cooling fan fitments, terminal board setups, and relay checks.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SERVICES SECTION -->
    <section id="services">
        <div class="section-header">
            <small>High Quality</small>
            <h2>Our Workshop Services</h2>
        </div>
        <div class="cards-grid">
            <div class="card">
                <div class="card-img-wrapper">
                    <img src="Field Winding.webp" alt="Stator Copper Rewinding">
                </div>
                <div class="card-body">
                    <div class="service-icon-box">
                        <div class="service-icon"><i class="fa-solid fa-bolt"></i></div>
                        <h3 style="margin: 0;">Stator Rewinding</h3>
                    </div>
                    <p>Complete single-phase and 3-phase electric motor coil rewinding with 100% super-enameled copper wire.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img-wrapper">
                    <img src="75 Hp.webp" alt="Electrical Testing & Fault Diagnosis">
                </div>
                <div class="card-body">
                    <div class="service-icon-box">
                        <div class="service-icon"><i class="fa-solid fa-screwdriver-wrench"></i></div>
                        <h3 style="margin: 0;">Fault Diagnosis</h3>
                    </div>
                    <p>Megger insulation resistance testing, short-circuit detection, and full voltage load inspection.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img-wrapper">
                    <img src="Motor.webp" alt="Bearing & Shaft Overhaul">
                </div>
                <div class="card-body">
                    <div class="service-icon-box">
                        <div class="service-icon"><i class="fa-solid fa-gear"></i></div>
                        <h3 style="margin: 0;">Bearing Overhaul</h3>
                    </div>
                    <p>Precision SKF/NBC bearing replacement, shaft re-centering, and dynamic mechanical noise reduction.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-img-wrapper">
                    <img src="repair motor.webp" alt="Spare Parts & Accessories">
                </div>
                <div class="card-body">
                    <div class="service-icon-box">
                        <div class="service-icon"><i class="fa-solid fa-car-battery"></i></div>
                        <h3 style="margin: 0;">Parts & Accessories</h3>
                    </div>
                    <p>Installation of high-grade capacitors, cooling fan impellers, terminal boxes, and overload protectors.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- ABOUT SECTION -->
    <section id="about">
        <div class="section-header">
            <small>Who We Are</small>
            <h2>About Excel Electricals</h2>
        </div>
        <div class="about-card">
            <div>
                <h3 style="font-size: 1.8rem; margin-bottom: 15px;">Dedicated Motor Winding Specialist</h3>
                <p style="color: var(--text-sub); line-height: 1.7; font-size: 1.05rem;">Excel Electricals provides fast, trusted, and durable motor winding solutions for industrial machines, domestic pumps, and commercial equipment in Choondy, Aluva.</p>
                <ul class="about-features">
                    <li><i class="fa-solid fa-circle-check"></i> 100% Super Enameled Copper Wire</li>
                    <li><i class="fa-solid fa-circle-check"></i> Fast Turnaround & Emergency Support</li>
                    <li><i class="fa-solid fa-circle-check"></i> Certified & Tested Before Delivery</li>
                </ul>
            </div>
            <div>
                <img src="motor wind..webp" alt="Workshop Repair" style="width: 100%; height: 260px; object-fit: cover; border-radius: 18px; border: 2px solid var(--card-border);">
            </div>
        </div>
    </section>

    <!-- CONTACTS SECTION -->
    <section id="contacts">
        <div class="section-header">
            <small>Reach Us</small>
            <h2>Contact & Location</h2>
        </div>
        <div class="contact-grid">
            <div class="form-card" style="display: flex; flex-direction: column; justify-content: center; gap: 20px;">
                <div style="display: flex; align-items: center; gap: 16px;">
                    <div class="service-icon" style="margin: 0;"><i class="fa-solid fa-location-dot"></i></div>
                    <div>
                        <h4 style="margin: 0 0 4px 0; font-size: 1.1rem;">Workshop Location</h4>
                        <p style="color: var(--text-sub); font-size: 0.95rem; font-weight: 500; margin: 0;">Choondy, Edathala, Aluva, Ernakulam, Kerala</p>
                    </div>
                </div>
                <div style="display: flex; align-items: center; gap: 16px;">
                    <div class="service-icon" style="margin: 0;"><i class="fa-solid fa-phone"></i></div>
                    <div>
                        <h4 style="margin: 0 0 4px 0; font-size: 1.1rem;">Phone & WhatsApp</h4>
                        <p style="color: var(--text-sub); font-size: 0.95rem; font-weight: 500; margin: 0;">+91 85902 59451</p>
                    </div>
                </div>
                <div style="display: flex; align-items: center; gap: 16px;">
                    <div class="service-icon" style="margin: 0;"><i class="fa-solid fa-envelope"></i></div>
                    <div>
                        <h4 style="margin: 0 0 4px 0; font-size: 1.1rem;">Email Address</h4>
                        <p style="color: var(--text-sub); font-size: 0.95rem; font-weight: 500; margin: 0;">excelelectricalswork@gmail.com</p>
                    </div>
                </div>
                <div style="display: flex; align-items: center; gap: 16px;">
                    <div class="service-icon" style="margin: 0;"><i class="fa-solid fa-id-card"></i></div>
                    <div>
                        <h4 style="margin: 0 0 4px 0; font-size: 1.1rem;">GST Registration</h4>
                        <p style="color: var(--text-sub); font-size: 0.95rem; font-weight: 500; margin: 0;">GSTIN: 32AAGPX3837Q1ZZ</p>
                    </div>
                </div>
            </div>
            <div class="map-card">
                <iframe src="https://maps.google.com/maps?q=Excel%20Electricals,%20Choondy,%20Aluva&t=&z=15&ie=UTF8&iwloc=&output=embed" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </div>
        </div>
    </section>

    <!-- SERVICE REQUEST FORM SECTION -->
    <section id="request">
        <div class="section-header">
            <small>Online Booking</small>
            <h2>Submit a Service Request</h2>
        </div>
        <div style="max-width: 650px; margin: 0 auto;">
            <div class="form-card">
                <form id="directMsgForm">
                    <input type="hidden" name="access_key" value="YOUR_WEB3FORMS_ACCESS_KEY">
                    <div class="form-group">
                        <label>Your Name</label>
                        <input type="text" name="name" class="form-control" placeholder="Enter full name" required>
                    </div>
                    <div class="form-group">
                        <label>Phone Number</label>
                        <input type="tel" name="phone" class="form-control" placeholder="Enter 10-digit mobile number" required>
                    </div>
                    <div class="form-group">
                        <label>Motor Issue / Equipment Details</label>
                        <textarea name="message" rows="4" class="form-control" placeholder="Describe HP, motor brand, or motor fault..." required></textarea>
                    </div>
                    <button type="submit" id="submitBtn" class="btn btn-primary" style="width: 100%; justify-content: center;">
                        <i class="fa-solid fa-paper-plane"></i> Send Request
                    </button>
                    <div id="formStatus" style="display: none; margin-top: 15px; text-align: center; font-weight: 700; font-size: 1.05rem;"></div>
                </form>
            </div>
        </div>
    </section>

    <!-- FLOATING QUICK BAR -->
    <div class="floating-bar">
        <a href="tel:+918590259451" class="float-link float-gold"><i class="fa-solid fa-phone"></i> Call Workshop</a>
        <span style="color: rgba(255,255,255,0.4);">|</span>
        <a href="https://wa.me/918590259451" class="float-link" target="_blank"><i class="fa-brands fa-whatsapp" style="color: #22c55e;"></i> WhatsApp</a>
    </div>

    <!-- FOOTER -->
    <footer>
        <div class="rating-badge">
            <span style="font-weight: 800; color: #ffffff;">4.9 Rating</span>
            <span class="stars">★★★★★</span>
            <span style="color: var(--text-sub); font-size: 0.9rem;">Google Verified</span>
        </div>
        <p style="color: var(--text-sub); font-size: 0.95rem; font-weight: 600;">&copy; 2026 EXCEL ELECTRICALS | Choondy, Aluva, Ernakulam, Kerala | GSTIN: 32AAGPX3837Q1ZZ</p>
    </footer>

    <!-- JavaScript -->
    <script>
        // Mobile Navigation Toggle
        const menuToggle = document.getElementById('menuToggle');
        const navMenu = document.getElementById('navMenu');

        menuToggle.addEventListener('click', () => {
            navMenu.classList.toggle('active');
            const icon = menuToggle.querySelector('i');
            if (navMenu.classList.contains('active')) {
                icon.className = 'fa-solid fa-xmark';
            } else {
                icon.className = 'fa-solid fa-bars';
            }
        });

        // Close menu automatically on link click
        document.querySelectorAll('nav a').forEach(link => {
            link.addEventListener('click', () => {
                navMenu.classList.remove('active');
                const icon = menuToggle.querySelector('i');
                if (icon) icon.className = 'fa-solid fa-bars';
            });
        });

        // Form Handling
        const form = document.getElementById('directMsgForm');
        const statusDiv = document.getElementById('formStatus');
        const submitBtn = document.getElementById('submitBtn');

        form.addEventListener('submit', async function(e) {
            e.preventDefault();
            submitBtn.innerHTML = '<i class="fa-solid fa-spinner fa-spin"></i> Submitting...';
            submitBtn.disabled = true;

            const formData = new FormData(form);
            const object = Object.fromEntries(formData);
            const json = JSON.stringify(object);

            try {
                const response = await fetch('https://api.web3forms.com/submit', {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json', 'Accept': 'application/json' },
                    body: json
                });

                const result = await response.json();
                if (response.status === 200) {
                    statusDiv.style.display = "block";
                    statusDiv.style.color = "#4ade80";
                    statusDiv.innerText = "✔️ Request sent! We will call you back shortly.";
                    form.reset();
                } else {
                    statusDiv.style.display = "block";
                    statusDiv.style.color = "#f87171";
                    statusDiv.innerText = "✖️ " + (result.message || "Failed to submit.");
                }
            } catch (error) {
                statusDiv.style.display = "block";
                statusDiv.style.color = "#f87171";
                statusDiv.innerText = "✖️ Error submitting. Please call directly.";
            } finally {
                submitBtn.innerHTML = '<i class="fa-solid fa-paper-plane"></i> Send Request';
                submitBtn.disabled = false;
            }
        });
    </script>
</body>
</html>
