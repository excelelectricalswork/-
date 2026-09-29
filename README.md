<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Excel Electricals | Motor Winding & Repair Workshop</title>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Space+Grotesk:wght@600;700;800&display=swap" rel="stylesheet">
    
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
            --bg-light: #f8fafc;
            --bg-white: #ffffff;
            --primary-amber: #d97706;
            --primary-gold: #f59e0b;
            --accent-blue: #0284c7;
            --text-dark: #0f172a;
            --text-muted: #475569;
            --border-light: #e2e8f0;
            --shadow-soft: 0 10px 30px -5px rgba(0, 0, 0, 0.05), 0 4px 12px -2px rgba(0, 0, 0, 0.03);
            --shadow-card: 0 20px 25px -5px rgba(0, 0, 0, 0.08), 0 8px 10px -6px rgba(0, 0, 0, 0.02);
        }

        /* 100% FULL-SCREEN BRIGHT LAYOUT */
        html, body {
            width: 100%;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-light);
            color: var(--text-dark);
            scroll-behavior: smooth;
        }

        h1, h2, h3, h4, .brand-text {
            font-family: 'Space Grotesk', sans-serif;
        }

        * {
            box-sizing: border-box;
        }

        /* LIGHT & BRIGHT MOTIVATIONAL MESH GRADIENT BACKDROPS */
        .ambient-glow-1 {
            position: fixed;
            top: -10vw;
            right: -10vw;
            width: 50vw;
            height: 50vw;
            background: radial-gradient(circle, rgba(251, 191, 36, 0.18) 0%, rgba(245, 158, 11, 0.08) 50%, rgba(255,255,255,0) 70%);
            pointer-events: none;
            z-index: 0;
        }

        .ambient-glow-2 {
            position: fixed;
            bottom: -10vw;
            left: -10vw;
            width: 55vw;
            height: 55vw;
            background: radial-gradient(circle, rgba(56, 189, 248, 0.12) 0%, rgba(255,255,255,0) 70%);
            pointer-events: none;
            z-index: 0;
        }

        /* HEADER NAVIGATION */
        header {
            width: 100%;
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(16px);
            padding: 16px 5%;
            position: fixed;
            top: 0;
            left: 0;
            z-index: 1000;
            border-bottom: 1px solid var(--border-light);
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.03);
        }

        .brand-logo {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.35rem;
            font-weight: 800;
            color: var(--text-dark);
            text-decoration: none;
        }

        .brand-icon {
            width: 42px;
            height: 42px;
            background: linear-gradient(135deg, var(--primary-gold), var(--primary-amber));
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #fff;
            font-size: 1.2rem;
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.35);
        }

        nav {
            display: flex;
            align-items: center;
            gap: 24px;
        }

        nav a {
            text-decoration: none;
            color: var(--text-muted);
            font-weight: 600;
            font-size: 0.95rem;
            transition: all 0.25s ease;
        }

        nav a:hover {
            color: var(--primary-amber);
        }

        .nav-btn {
            background: linear-gradient(135deg, var(--primary-gold), var(--primary-amber));
            color: #fff !important;
            padding: 10px 22px;
            border-radius: 50px;
            font-weight: 700 !important;
            box-shadow: 0 4px 15px rgba(217, 119, 6, 0.3);
            transition: transform 0.25s ease, box-shadow 0.25s ease !important;
        }

        .nav-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(217, 119, 6, 0.45);
        }

        /* HERO SECTION */
        .hero {
            position: relative;
            z-index: 1;
            width: 100%;
            min-height: 90vh;
            padding: 130px 5% 60px 5%;
            display: grid;
            grid-template-columns: 1.2fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .hero-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(245, 158, 11, 0.12);
            border: 1px solid rgba(245, 158, 11, 0.3);
            color: var(--primary-amber);
            padding: 8px 18px;
            border-radius: 50px;
            font-size: 0.88rem;
            font-weight: 700;
            margin-bottom: 22px;
        }

        .hero h1 {
            font-size: 3.6rem;
            line-height: 1.15;
            margin-bottom: 20px;
            font-weight: 800;
            letter-spacing: -1.2px;
            color: var(--text-dark);
        }

        .hero h1 span {
            background: linear-gradient(135deg, var(--primary-amber), #b45309);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p {
            font-size: 1.15rem;
            color: var(--text-muted);
            margin-bottom: 35px;
            max-width: 600px;
            line-height: 1.65;
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
            padding: 15px 30px;
            border-radius: 14px;
            font-weight: 700;
            font-size: 0.98rem;
            text-decoration: none;
            transition: all 0.3s ease;
            cursor: pointer;
            border: none;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--primary-gold), var(--primary-amber));
            color: #fff;
            box-shadow: 0 6px 20px rgba(217, 119, 6, 0.3);
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(217, 119, 6, 0.45);
        }

        .btn-outline {
            background: var(--bg-white);
            color: var(--text-dark);
            border: 1px solid var(--border-light);
            box-shadow: var(--shadow-soft);
        }

        .btn-outline:hover {
            border-color: var(--primary-gold);
            color: var(--primary-amber);
            transform: translateY(-3px);
        }

        .hero-image-box {
            position: relative;
        }

        .hero-img {
            width: 100%;
            height: 450px;
            object-fit: cover;
            border-radius: 28px;
            border: 4px solid var(--bg-white);
            box-shadow: var(--shadow-card);
        }

        /* SECTION STYLING */
        section {
            position: relative;
            z-index: 1;
            width: 100%;
            padding: 90px 5%;
            scroll-margin-top: 70px;
        }

        .section-header {
            text-align: center;
            max-width: 650px;
            margin: 0 auto 50px auto;
        }

        .section-header small {
            color: var(--primary-amber);
            font-weight: 800;
            letter-spacing: 2px;
            text-transform: uppercase;
            font-size: 0.82rem;
            display: block;
            margin-bottom: 8px;
        }

        .section-header h2 {
            font-size: 2.4rem;
            letter-spacing: -0.8px;
            color: var(--text-dark);
        }

        /* GRID CARDS */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 28px;
            width: 100%;
        }

        .card {
            background: var(--bg-white);
            border: 1px solid var(--border-light);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: var(--shadow-soft);
            transition: all 0.35s ease;
        }

        .card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-card);
            border-color: var(--primary-gold);
        }

        .card img {
            width: 100%;
            height: 230px;
            object-fit: cover;
        }

        .card-body {
            padding: 24px;
        }

        .card-body h3 {
            font-size: 1.25rem;
            margin-bottom: 8px;
            color: var(--text-dark);
        }

        .card-body p {
            color: var(--text-muted);
            font-size: 0.92rem;
            line-height: 1.6;
        }

        /* SERVICES WIDGETS */
        .service-icon {
            width: 52px;
            height: 52px;
            background: rgba(245, 158, 11, 0.1);
            border-radius: 14px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--primary-amber);
            font-size: 1.4rem;
            margin-bottom: 18px;
        }

        /* ABOUT SECTION */
        .about-card {
            background: var(--bg-white);
            border: 1px solid var(--border-light);
            border-radius: 24px;
            padding: 40px;
            box-shadow: var(--shadow-soft);
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .about-features {
            list-style: none;
            margin-top: 20px;
        }

        .about-features li {
            margin-bottom: 12px;
            display: flex;
            align-items: center;
            gap: 10px;
            color: var(--text-muted);
            font-weight: 600;
        }

        .about-features i {
            color: var(--primary-amber);
        }

        /* CONTACTS & SERVICE REQUEST */
        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 35px;
            width: 100%;
        }

        .form-card {
            background: var(--bg-white);
            border: 1px solid var(--border-light);
            border-radius: 24px;
            padding: 35px;
            box-shadow: var(--shadow-soft);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-size: 0.88rem;
            color: var(--text-dark);
            font-weight: 600;
        }

        .form-control {
            width: 100%;
            padding: 14px 16px;
            background: var(--bg-light);
            border: 1px solid var(--border-light);
            border-radius: 10px;
            color: var(--text-dark);
            font-family: inherit;
            font-size: 0.95rem;
            transition: all 0.25s ease;
        }

        .form-control:focus {
            outline: none;
            background: #fff;
            border-color: var(--primary-amber);
            box-shadow: 0 0 0 3px rgba(245, 158, 11, 0.15);
        }

        .map-card {
            border-radius: 24px;
            overflow: hidden;
            border: 1px solid var(--border-light);
            min-height: 420px;
            box-shadow: var(--shadow-soft);
        }

        /* FLOATING ACTION BAR */
        .floating-bar {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(16px);
            border: 1px solid var(--border-light);
            padding: 10px 24px;
            border-radius: 50px;
            display: flex;
            align-items: center;
            gap: 18px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            z-index: 999;
        }

        .float-link {
            display: flex;
            align-items: center;
            gap: 8px;
            color: var(--text-dark);
            text-decoration: none;
            font-size: 0.9rem;
            font-weight: 700;
        }

        .float-gold {
            color: var(--primary-amber);
        }

        /* FOOTER */
        footer {
            position: relative;
            z-index: 1;
            width: 100%;
            border-top: 1px solid var(--border-light);
            padding: 40px 5% 30px 5%;
            text-align: center;
            background: var(--bg-white);
        }

        .rating-badge {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: var(--bg-light);
            border: 1px solid var(--border-light);
            padding: 8px 20px;
            border-radius: 50px;
            margin-bottom: 20px;
            font-size: 0.9rem;
        }

        .stars {
            color: var(--primary-gold);
        }

        /* RESPONSIVE */
        @media (max-width: 992px) {
            .hero {
                grid-template-columns: 1fr;
                text-align: center;
                padding-top: 110px;
            }
            .hero p {
                margin: 0 auto 30px auto;
            }
            .hero-buttons {
                justify-content: center;
            }
            .about-card, .contact-grid {
                grid-template-columns: 1fr;
            }
            nav {
                display: none;
            }
        }
    </style>
</head>
<body>

    <div class="ambient-glow-1"></div>
    <div class="ambient-glow-2"></div>

    <!-- HEADER NAVIGATION -->
    <header>
        <a href="#home" class="brand-logo">
            <div class="brand-icon"><i class="fa-solid fa-bolt"></i></div>
            <span class="brand-text">EXCEL ELECTRICALS</span>
        </a>
        <nav>
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
                <i class="fa-solid fa-shield-halved"></i> Certified Workshop • Choondy, Aluva
            </div>
            <h1>EXPERT ELECTRIC <span>MOTOR WINDING</span> & REPAIR</h1>
            <p>Reliable stator rewinding, coil replacement, dynamic rotor testing, and complete motor repairs with guaranteed copper quality.</p>
            <div class="hero-buttons">
                <a href="tel:+919876543210" class="btn btn-primary"><i class="fa-solid fa-phone"></i> Call Workshop</a>
                <a href="https://wa.me/919876543210" class="btn btn-outline"><i class="fa-brands fa-whatsapp" style="color: #22c55e;"></i> WhatsApp Chat</a>
            </div>
        </div>
        <div class="hero-image-box">
            <img src="25 Hp.jpg" alt="Motor Winding Workshop" class="hero-img">
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
                <img src="Inducton motor.webp" alt="Induction Motor">
                <div class="card-body">
                    <h3>Induction Motor Repair</h3>
                    <p>Heavy duty single & 3-phase induction motor diagnostic and overhaul.</p>
                </div>
            </div>
            <div class="card">
                <img src="Motor.webp" alt="Motor Servicing">
                <div class="card-body">
                    <h3>Mechanical Overhaul</h3>
                    <p>Bearing replacement, shaft polish, and dynamic housing alignment.</p>
                </div>
            </div>
            <div class="card">
                <img src="Field Winding.webp" alt="Stator Rewinding">
                <div class="card-body">
                    <h3>Stator Copper Winding</h3>
                    <p>High-grade dual coated copper wire coil insertion & varnish dipping.</p>
                </div>
            </div>
            <div class="card">
                <img src="repair motor.webp" alt="Motor Parts">
                <div class="card-body">
                    <h3>Component Servicing</h3>
                    <p>Capacitors, cooling fan blades, terminal boards, and relay repairs.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SERVICES SECTION -->
    <section id="services" style="background: rgba(255,255,255,0.6);">
        <div class="section-header">
            <small>High Quality</small>
            <h2>Our Workshop Services</h2>
        </div>
        <div class="cards-grid">
            <div class="card card-body">
                <div class="service-icon"><i class="fa-solid fa-bolt"></i></div>
                <h3>Copper Rewinding</h3>
                <p>Complete stator & coil rewinding using premium copper wire and thermal insulation paper.</p>
            </div>
            <div class="card card-body">
                <div class="service-icon"><i class="fa-solid fa-screwdriver-wrench"></i></div>
                <h3>Electrical Testing</h3>
                <p>Megger insulation test, fault troubleshooting, and coil balancing checks.</p>
            </div>
            <div class="card card-body">
                <div class="service-icon"><i class="fa-solid fa-gear"></i></div>
                <h3>Bearing Fitting</h3>
                <p>Precision removal and installation of high-speed SKF/NBC motor bearings.</p>
            </div>
            <div class="card card-body">
                <div class="service-icon"><i class="fa-solid fa-car-battery"></i></div>
                <h3>Capacitor & Relays</h3>
                <p>Testing and replacement of start/run capacitors and centrifugal switches.</p>
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
                <h3 style="font-size: 1.6rem; margin-bottom: 15px;">Dedicated Motor Winding Specialist</h3>
                <p style="color: var(--text-muted); line-height: 1.7;">Excel Electricals provides fast, trusted, and durable motor winding solutions for industrial machines, domestic pumps, and commercial equipment in Choondy, Aluva.</p>
                <ul class="about-features">
                    <li><i class="fa-solid fa-circle-check"></i> 100% Super Enameled Copper Wire</li>
                    <li><i class="fa-solid fa-circle-check"></i> Fast Turnaround & Emergency Support</li>
                    <li><i class="fa-solid fa-circle-check"></i> Certified & Tested Before Delivery</li>
                </ul>
            </div>
            <div>
                <img src="repair motor.webp" alt="Workshop Repair" style="width: 100%; height: 260px; object-fit: cover; border-radius: 16px;">
            </div>
        </div>
    </section>

    <!-- CONTACTS SECTION -->
    <section id="contacts" style="background: rgba(255,255,255,0.6);">
        <div class="section-header">
            <small>Reach Us</small>
            <h2>Contact & Location</h2>
        </div>
        <div class="contact-grid">
            <div class="form-card" style="display: flex; flex-direction: column; justify-content: center; gap: 20px;">
                <div style="display: flex; align-items: center; gap: 15px;">
                    <div class="service-icon" style="margin: 0;"><i class="fa-solid fa-location-dot"></i></div>
                    <div>
                        <h4 style="margin-bottom: 4px;">Workshop Location</h4>
                        <p style="color: var(--text-muted); font-size: 0.95rem;">Choondy, Edathala, Aluva, Ernakulam, Kerala</p>
                    </div>
                </div>
                <div style="display: flex; align-items: center; gap: 15px;">
                    <div class="service-icon" style="margin: 0;"><i class="fa-solid fa-phone"></i></div>
                    <div>
                        <h4 style="margin-bottom: 4px;">Phone Call</h4>
                        <p style="color: var(--text-muted); font-size: 0.95rem;">+91 98765 43210</p>
                    </div>
                </div>
                <div style="display: flex; align-items: center; gap: 15px;">
                    <div class="service-icon" style="margin: 0;"><i class="fa-solid fa-id-card"></i></div>
                    <div>
                        <h4 style="margin-bottom: 4px;">GST Registration</h4>
                        <p style="color: var(--text-muted); font-size: 0.95rem;">GSTIN: 32AAGPX3837Q1ZZ</p>
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
                    <div id="formStatus" style="display: none; margin-top: 15px; text-align: center; font-weight: 600;"></div>
                </form>
            </div>
        </div>
    </section>

    <!-- FLOATING QUICK BAR -->
    <div class="floating-bar">
        <a href="tel:+919876543210" class="float-link float-gold"><i class="fa-solid fa-phone"></i> Call Workshop</a>
        <span style="color: var(--border-light);">|</span>
        <a href="https://wa.me/919876543210" class="float-link"><i class="fa-brands fa-whatsapp" style="color: #22c55e;"></i> WhatsApp</a>
    </div>

    <!-- FOOTER -->
    <footer>
        <div class="rating-badge">
            <span style="font-weight: 800; color: var(--text-dark);">4.9 Rating</span>
            <span class="stars">★★★★★</span>
            <span style="color: var(--text-muted); font-size: 0.85rem;">Google Verified</span>
        </div>
        <p style="color: var(--text-muted); font-size: 0.9rem;">&copy; 2026 EXCEL ELECTRICALS | Choondy, Aluva, Ernakulam, Kerala | GSTIN: 32AAGPX3837Q1ZZ</p>
    </footer>

    <!-- Form Script -->
    <script>
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
                    statusDiv.style.color = "#16a34a";
                    statusDiv.innerText = "✔️ Request sent! We will call you back shortly.";
                    form.reset();
                } else {
                    statusDiv.style.display = "block";
                    statusDiv.style.color = "#dc2626";
                    statusDiv.innerText = "✖️ " + (result.message || "Failed to submit.");
                }
            } catch (error) {
                statusDiv.style.display = "block";
                statusDiv.style.color = "#dc2626";
                statusDiv.innerText = "✖️ Error submitting. Please call directly.";
            } finally {
                submitBtn.innerHTML = '<i class="fa-solid fa-paper-plane"></i> Send Request';
                submitBtn.disabled = false;
            }
        });
    </script>
</body>
</html>
