<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Excel Electricals | Motor Winding & Repair Workshop</title>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Space+Grotesk:wght@600;700;800&display=swap" rel="stylesheet">
    
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
            --bg-deep: #030712;
            --bg-card: rgba(17, 24, 39, 0.75);
            --bg-card-hover: rgba(31, 41, 55, 0.9);
            --gold-bright: #fbbf24;
            --gold-glow: #f59e0b;
            --amber-accent: #ff8c00;
            --electric-cyan: #38bdf8;
            --text-main: #f9fafb;
            --text-sub: #9ca3af;
            --border-line: rgba(255, 255, 255, 0.12);
            --border-glow: rgba(251, 191, 36, 0.4);
        }

        /* 100% FULL-SCREEN PAGE SETUP */
        html, body {
            width: 100%;
            height: 100%;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-deep);
            color: var(--text-main);
            scroll-behavior: smooth;
        }

        h1, h2, h3, h4, .brand-text {
            font-family: 'Space Grotesk', sans-serif;
        }

        * {
            box-sizing: border-box;
        }

        /* DYNAMIC MOTIVATING BACKGROUND GLOWS */
        .glow-overlay-1 {
            position: fixed;
            top: -15%;
            right: -10%;
            width: 55vw;
            height: 55vw;
            background: radial-gradient(circle, rgba(251, 191, 36, 0.15) 0%, rgba(255, 140, 0, 0.05) 50%, rgba(0,0,0,0) 70%);
            pointer-events: none;
            z-index: 0;
        }

        .glow-overlay-2 {
            position: fixed;
            bottom: -20%;
            left: -10%;
            width: 60vw;
            height: 60vw;
            background: radial-gradient(circle, rgba(56, 189, 248, 0.1) 0%, rgba(0,0,0,0) 70%);
            pointer-events: none;
            z-index: 0;
        }

        /* FULL WIDTH HEADER & NAV */
        header {
            width: 100%;
            background: rgba(3, 7, 18, 0.85);
            backdrop-filter: blur(20px);
            padding: 18px 5%;
            position: fixed;
            top: 0;
            left: 0;
            z-index: 1000;
            border-bottom: 1px solid var(--border-line);
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .brand-logo {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.4rem;
            font-weight: 800;
            color: #fff;
            letter-spacing: -0.5px;
        }

        .brand-icon {
            width: 42px;
            height: 42px;
            background: linear-gradient(135deg, var(--gold-bright), var(--amber-accent));
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #000;
            font-size: 1.2rem;
            box-shadow: 0 0 20px rgba(251, 191, 36, 0.4);
        }

        nav {
            display: flex;
            align-items: center;
            gap: 28px;
        }

        nav a {
            text-decoration: none;
            color: var(--text-sub);
            font-weight: 600;
            font-size: 0.95rem;
            transition: all 0.3s ease;
        }

        nav a:hover {
            color: var(--gold-bright);
            text-shadow: 0 0 10px rgba(251, 191, 36, 0.5);
        }

        .nav-cta {
            background: linear-gradient(135deg, var(--gold-bright), var(--amber-accent));
            color: #000 !important;
            padding: 10px 24px;
            border-radius: 50px;
            font-weight: 700 !important;
            box-shadow: 0 4px 20px rgba(251, 191, 36, 0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease !important;
        }

        .nav-cta:hover {
            transform: translateY(-2px) scale(1.02);
            box-shadow: 0 8px 25px rgba(251, 191, 36, 0.5);
        }

        /* FULL-SCREEN HERO SECTION */
        .hero-section {
            position: relative;
            z-index: 1;
            width: 100%;
            min-height: 100vh;
            padding: 140px 5% 60px 5%;
            display: grid;
            grid-template-columns: 1.2fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .motivation-tag {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: rgba(251, 191, 36, 0.12);
            border: 1px solid rgba(251, 191, 36, 0.35);
            color: var(--gold-bright);
            padding: 8px 20px;
            border-radius: 50px;
            font-size: 0.88rem;
            font-weight: 700;
            letter-spacing: 0.5px;
            margin-bottom: 25px;
            box-shadow: 0 0 15px rgba(251, 191, 36, 0.15);
        }

        .hero-section h1 {
            font-size: 3.8rem;
            line-height: 1.1;
            margin-bottom: 24px;
            font-weight: 800;
            letter-spacing: -1.5px;
        }

        .hero-section h1 span {
            background: linear-gradient(135deg, #fbbf24 0%, #ff8c00 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 30px rgba(251, 191, 36, 0.2);
        }

        .hero-section p {
            font-size: 1.15rem;
            color: var(--text-sub);
            margin-bottom: 40px;
            max-width: 620px;
            line-height: 1.7;
        }

        .hero-buttons {
            display: flex;
            gap: 18px;
            flex-wrap: wrap;
        }

        .btn-action {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            padding: 16px 34px;
            border-radius: 14px;
            font-weight: 700;
            font-size: 1rem;
            text-decoration: none;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            cursor: pointer;
            border: none;
        }

        .btn-gold {
            background: linear-gradient(135deg, var(--gold-bright), var(--amber-accent));
            color: #000;
            box-shadow: 0 10px 30px rgba(251, 191, 36, 0.3);
        }

        .btn-gold:hover {
            transform: translateY(-4px) scale(1.02);
            box-shadow: 0 15px 35px rgba(251, 191, 36, 0.5);
        }

        .btn-glass {
            background: rgba(255, 255, 255, 0.06);
            color: #fff;
            border: 1px solid var(--border-line);
            backdrop-filter: blur(12px);
        }

        .btn-glass:hover {
            background: rgba(255, 255, 255, 0.12);
            border-color: rgba(255, 255, 255, 0.25);
            transform: translateY(-4px);
        }

        /* HERO DISPLAY CARDS & WIDGETS */
        .hero-visual {
            position: relative;
            width: 100%;
        }

        .main-hero-img {
            width: 100%;
            height: 480px;
            object-fit: cover;
            border-radius: 28px;
            border: 1px solid var(--border-glow);
            box-shadow: 0 30px 60px -12px rgba(0, 0, 0, 0.8), 0 0 30px rgba(251, 191, 36, 0.15);
        }

        .floating-widget {
            position: absolute;
            background: rgba(17, 24, 39, 0.85);
            backdrop-filter: blur(16px);
            border: 1px solid var(--border-glow);
            border-radius: 20px;
            padding: 20px 26px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.6);
            display: flex;
            align-items: center;
            gap: 18px;
            z-index: 2;
        }

        .widget-1 {
            bottom: -25px;
            left: -30px;
        }

        .widget-2 {
            top: -20px;
            right: -20px;
        }

        .widget-icon {
            width: 48px;
            height: 48px;
            background: rgba(251, 191, 36, 0.15);
            color: var(--gold-bright);
            border-radius: 14px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.4rem;
        }

        .widget-val {
            font-size: 1.5rem;
            font-weight: 800;
            color: #fff;
            line-height: 1;
        }

        .widget-lbl {
            font-size: 0.85rem;
            color: var(--text-sub);
            margin-top: 4px;
        }

        /* FULL SCREEN SECTIONS */
        section {
            position: relative;
            z-index: 1;
            width: 100%;
            padding: 100px 5%;
            scroll-margin-top: 80px;
        }

        .section-header {
            text-align: center;
            max-width: 700px;
            margin: 0 auto 60px auto;
        }

        .section-header small {
            color: var(--gold-bright);
            font-weight: 700;
            letter-spacing: 2.5px;
            text-transform: uppercase;
            font-size: 0.85rem;
            display: block;
            margin-bottom: 10px;
        }

        .section-header h2 {
            font-size: 2.6rem;
            letter-spacing: -1px;
            color: #fff;
        }

        /* GRID CARDS & WIDGETS */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            width: 100%;
        }

        .glass-card {
            background: var(--bg-card);
            border: 1px solid var(--border-line);
            border-radius: 24px;
            overflow: hidden;
            backdrop-filter: blur(16px);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .glass-card:hover {
            transform: translateY(-10px);
            border-color: var(--border-glow);
            background: var(--bg-card-hover);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.5), 0 0 20px rgba(251, 191, 36, 0.15);
        }

        .glass-card img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-bottom: 1px solid var(--border-line);
        }

        .card-body {
            padding: 28px;
        }

        .card-body h3 {
            font-size: 1.35rem;
            margin-bottom: 10px;
            color: #fff;
        }

        .card-body p {
            color: var(--text-sub);
            font-size: 0.95rem;
            line-height: 1.6;
        }

        /* SERVICES WIDGETS */
        .service-box {
            padding: 32px;
        }

        .service-icon {
            width: 58px;
            height: 58px;
            background: rgba(251, 191, 36, 0.12);
            border: 1px solid rgba(251, 191, 36, 0.25);
            border-radius: 16px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--gold-bright);
            font-size: 1.5rem;
            margin-bottom: 22px;
        }

        /* FORM & MAP CONTAINER */
        .contact-grid {
            display: grid;
            grid-template-columns: 1.1fr 1fr;
            gap: 40px;
            width: 100%;
        }

        .form-card {
            background: var(--bg-card);
            border: 1px solid var(--border-line);
            border-radius: 28px;
            padding: 40px;
            backdrop-filter: blur(16px);
        }

        .form-group {
            margin-bottom: 22px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-size: 0.9rem;
            color: var(--text-sub);
            font-weight: 600;
        }

        .form-control {
            width: 100%;
            padding: 16px 18px;
            background: rgba(3, 7, 18, 0.7);
            border: 1px solid var(--border-line);
            border-radius: 12px;
            color: #fff;
            font-family: inherit;
            font-size: 1rem;
            transition: all 0.3s ease;
        }

        .form-control:focus {
            outline: none;
            border-color: var(--gold-bright);
            box-shadow: 0 0 0 4px rgba(251, 191, 36, 0.15);
        }

        .map-card {
            border-radius: 28px;
            overflow: hidden;
            border: 1px solid var(--border-line);
            min-height: 450px;
        }

        /* FLOATING ACTION BAR */
        .floating-bar {
            position: fixed;
            bottom: 25px;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(17, 24, 39, 0.9);
            backdrop-filter: blur(20px);
            border: 1px solid var(--border-glow);
            padding: 12px 28px;
            border-radius: 60px;
            display: flex;
            align-items: center;
            gap: 20px;
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.7), 0 0 20px rgba(251, 191, 36, 0.2);
            z-index: 999;
        }

        .float-link {
            display: flex;
            align-items: center;
            gap: 10px;
            color: #fff;
            text-decoration: none;
            font-size: 0.95rem;
            font-weight: 700;
        }

        .float-gold {
            color: var(--gold-bright);
        }

        /* FOOTER */
        footer {
            position: relative;
            z-index: 1;
            width: 100%;
            border-top: 1px solid var(--border-line);
            padding: 50px 5% 35px 5%;
            text-align: center;
            background: #02040a;
        }

        .rating-badge {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            background: rgba(255, 255, 255, 0.04);
            border: 1px solid var(--border-line);
            padding: 10px 24px;
            border-radius: 50px;
            margin-bottom: 24px;
        }

        .stars {
            color: var(--gold-bright);
        }

        /* RESPONSIVE LAYOUT */
        @media (max-width: 992px) {
            .hero-section {
                grid-template-columns: 1fr;
                text-align: center;
                padding-top: 120px;
            }
            .hero-section p {
                margin: 0 auto 35px auto;
            }
            .hero-buttons {
                justify-content: center;
            }
            .motivation-tag {
                margin: 0 auto 25px auto;
            }
            .floating-widget {
                position: relative;
                bottom: auto;
                left: auto;
                top: auto;
                right: auto;
                margin-top: 15px;
            }
            .contact-grid {
                grid-template-columns: 1fr;
            }
            nav {
                display: none;
            }
        }
    </style>
</head>
<body>

    <div class="glow-overlay-1"></div>
    <div class="glow-overlay-2"></div>

    <!-- HEADER -->
    <header>
        <div class="brand-logo">
            <div class="brand-icon"><i class="fa-solid fa-bolt"></i></div>
            <span class="brand-text">EXCEL ELECTRICALS</span>
        </div>
        <nav>
            <a href="#home">Home</a>
            <a href="#motors">Motors</a>
            <a href="#winding">Winding</a>
            <a href="#services">Services</a>
            <a href="#about">About</a>
            <a href="#request" class="nav-cta">Service Request</a>
        </nav>
    </header>

    <!-- HERO SECTION -->
    <section class="hero-section" id="home">
        <div>
            <div class="motivation-tag">
                <i class="fa-solid fa-fire"></i> POWERING INDUSTRIAL PERFORMANCE • CHOONDY
            </div>
            <h1>EXPERT MOTOR <span>WINDING & REPAIR</span> WORKSHOP</h1>
            <p>Precision copper rewinding, stator insulation, rotor dynamic checks, and complete mechanical overhaul for high-torque industrial & domestic electric motors.</p>
            <div class="hero-buttons">
                <a href="tel:+919876543210" class="btn-action btn-gold"><i class="fa-solid fa-phone"></i> Call Workshop Now</a>
                <a href="https://wa.me/919876543210" class="btn-action btn-glass"><i class="fa-brands fa-whatsapp" style="color: #22c55e;"></i> WhatsApp Message</a>
            </div>
        </div>
        <div class="hero-visual">
            <img src="25 Hp.jpg" alt="Motor Winding Workshop" class="main-hero-img">
            <div class="floating-widget widget-1">
                <div class="widget-icon"><i class="fa-solid fa-award"></i></div>
                <div>
                    <div class="widget-val">100%</div>
                    <div class="widget-lbl">Copper Quality Assured</div>
                </div>
            </div>
        </div>
    </section>

    <!-- MOTOR GALLERY -->
    <section id="motors">
        <div class="section-header">
            <small>Precision Engineering</small>
            <h2>Motor Work Gallery</h2>
        </div>
        <div class="cards-grid">
            <div class="glass-card">
                <img src="Inducton motor.webp" alt="Induction Motors">
                <div class="card-body">
                    <h3>Induction Motors</h3>
                    <p>Heavy duty single-phase and 3-phase induction motor rewinding & overhaul.</p>
                </div>
            </div>
            <div class="glass-card">
                <img src="Motor.webp" alt="Mechanical Overhaul">
                <div class="card-body">
                    <h3>Mechanical Servicing</h3>
                    <p>Complete bearing replacements, rotor shaft checks, and cover fitting.</p>
                </div>
            </div>
            <div class="glass-card">
                <img src="Field Winding.webp" alt="Stator Coil Winding">
                <div class="card-body">
                    <h3>Stator Rewinding</h3>
                    <p>Dual-coated copper wire coil insertion with high-temp insulation varnish.</p>
                </div>
            </div>
            <div class="glass-card">
                <img src="repair motor.webp" alt="Component Repairs">
                <div class="card-body">
                    <h3>Motor Spare Parts</h3>
                    <p>Capacitor replacements, cooling fan fitments, and terminal block setups.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SERVICES WIDGET SECTION -->
    <section id="services" style="background: rgba(255,255,255,0.01);">
        <div class="section-header">
            <small>High Performance</small>
            <h2>Workshop Services</h2>
        </div>
        <div class="cards-grid">
            <div class="glass-card service-box">
                <div class="service-icon"><i class="fa-solid fa-bolt"></i></div>
                <h3>Stator Rewinding</h3>
                <p>High-grade copper coil rewinding with top quality insulation paper and dip varnishing.</p>
            </div>
            <div class="glass-card service-box">
                <div class="service-icon"><i class="fa-solid fa-screwdriver-wrench"></i></div>
                <h3>Motor Diagnostics</h3>
                <p>Megger testing, coil resistance verification, and winding fault troubleshooting.</p>
            </div>
            <div class="glass-card service-box">
                <div class="service-icon"><i class="fa-solid fa-gear"></i></div>
                <h3>Bearing Fitting</h3>
                <p>Precision bearing extraction and installation for vibration-free motor operation.</p>
            </div>
            <div class="glass-card service-box">
                <div class="service-icon"><i class="fa-solid fa-car-battery"></i></div>
                <h3>Capacitors & Switches</h3>
                <p>Testing and replacement of run/start capacitors, relays, and centrifugal switches.</p>
            </div>
        </div>
    </section>

    <!-- DIRECT SERVICE FORM & MAP -->
    <section id="request">
        <div class="section-header">
            <small>Direct Connect</small>
            <h2>Request Service & Location</h2>
        </div>
        <div class="contact-grid">
            <div class="form-card">
                <form id="directMsgForm">
                    <input type="hidden" name="access_key" value="YOUR_WEB3FORMS_ACCESS_KEY">
                    <div class="form-group">
                        <label>Your Name</label>
                        <input type="text" name="name" class="form-control" placeholder="Enter your full name" required>
                    </div>
                    <div class="form-group">
                        <label>Phone Number</label>
                        <input type="tel" name="phone" class="form-control" placeholder="Enter mobile number" required>
                    </div>
                    <div class="form-group">
                        <label>Motor Issue / Repair Details</label>
                        <textarea name="message" rows="4" class="form-control" placeholder="Specify HP, motor type, or issue..." required></textarea>
                    </div>
                    <button type="submit" id="submitBtn" class="btn-action btn-gold" style="width: 100%; justify-content: center;">
                        <i class="fa-solid fa-paper-plane"></i> Submit Request
                    </button>
                    <div id="formStatus" style="display: none; margin-top: 15px; text-align: center; font-weight: 600;"></div>
                </form>
            </div>
            <div class="map-card">
                <iframe src="https://maps.google.com/maps?q=Excel%20Electricals,%20Choondy,%20Aluva&t=&z=15&ie=UTF8&iwloc=&output=embed" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </div>
        </div>
    </section>

    <!-- FLOATING ACTION BAR -->
    <div class="floating-bar">
        <a href="tel:+919876543210" class="float-link float-gold"><i class="fa-solid fa-phone"></i> Call Workshop</a>
        <span style="color: var(--border-line);">|</span>
        <a href="https://wa.me/919876543210" class="float-link"><i class="fa-brands fa-whatsapp" style="color: #22c55e;"></i> WhatsApp</a>
    </div>

    <!-- FOOTER -->
    <footer>
        <div class="rating-badge">
            <span style="font-weight: 800; color: #fff;">4.9 Rating</span>
            <span class="stars">★★★★★</span>
            <span style="color: var(--text-sub); font-size: 0.85rem;">Google Verified</span>
        </div>
        <p style="color: var(--text-sub); font-size: 0.9rem;">&copy; 2026 EXCEL ELECTRICALS | Choondy, Aluva, Ernakulam, Kerala | GSTIN: 32AAGPX3837Q1ZZ</p>
    </footer>

    <!-- Form Handler Script -->
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
                    statusDiv.style.color = "#22c55e";
                    statusDiv.innerText = "✔️ Request submitted successfully! We will contact you shortly.";
                    form.reset();
                } else {
                    statusDiv.style.display = "block";
                    statusDiv.style.color = "#ef4444";
                    statusDiv.innerText = "✖️ " + (result.message || "Failed to submit.");
                }
            } catch (error) {
                statusDiv.style.display = "block";
                statusDiv.style.color = "#ef4444";
                statusDiv.innerText = "✖️ Submission error. Please call us directly.";
            } finally {
                submitBtn.innerHTML = '<i class="fa-solid fa-paper-plane"></i> Submit Request';
                submitBtn.disabled = false;
            }
        });
    </script>
</body>
</html>
