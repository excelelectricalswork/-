<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Excel Electricals | Premium Motor Winding & Repair Workshop</title>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Space+Grotesk:wght@500;700&display=swap" rel="stylesheet">
    
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
            --bg-main: #060913;
            --bg-card: rgba(18, 26, 43, 0.7);
            --bg-card-hover: rgba(28, 39, 64, 0.9);
            --accent-gold: #ffc107;
            --accent-glow: rgba(255, 193, 7, 0.25);
            --accent-blue: #38bdf8;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
            --border-line: rgba(255, 255, 255, 0.08);
            --border-glow: rgba(255, 193, 7, 0.4);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-main);
            color: var(--text-main);
            line-height: 1.6;
            scroll-behavior: smooth;
            overflow-x: hidden;
        }

        h1, h2, h3, .logo-text {
            font-family: 'Space Grotesk', sans-serif;
        }

        /* BACKGROUND GLOW EFFECTS */
        .glow-sphere-1 {
            position: fixed;
            top: -100px;
            right: -100px;
            width: 450px;
            height: 450px;
            background: radial-gradient(circle, rgba(255, 193, 7, 0.12) 0%, rgba(0,0,0,0) 70%);
            z-index: -1;
            pointer-events: none;
        }

        .glow-sphere-2 {
            position: fixed;
            bottom: -150px;
            left: -100px;
            width: 500px;
            height: 500px;
            background: radial-gradient(circle, rgba(56, 189, 248, 0.08) 0%, rgba(0,0,0,0) 70%);
            z-index: -1;
            pointer-events: none;
        }

        /* HEADER & NAVIGATION */
        header {
            background: rgba(6, 9, 19, 0.85);
            backdrop-filter: blur(16px);
            padding: 16px 8%;
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid var(--border-line);
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 1.35rem;
            font-weight: 700;
            color: #fff;
            letter-spacing: -0.5px;
        }

        .logo-icon {
            width: 38px;
            height: 38px;
            background: linear-gradient(135deg, var(--accent-gold), #d97706);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #000;
            font-size: 1.1rem;
            box-shadow: 0 0 15px var(--accent-glow);
        }

        nav {
            display: flex;
            align-items: center;
            gap: 24px;
        }

        nav a {
            text-decoration: none;
            color: var(--text-muted);
            font-weight: 500;
            font-size: 0.92rem;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--accent-gold);
        }

        .nav-btn {
            background: linear-gradient(135deg, var(--accent-gold), #eab308);
            color: #000 !important;
            padding: 10px 20px;
            border-radius: 30px;
            font-weight: 700 !important;
            box-shadow: 0 4px 15px var(--accent-glow);
            transition: all 0.3s ease !important;
        }

        .nav-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(255, 193, 7, 0.4);
        }

        /* HERO SECTION */
        .hero {
            padding: 90px 8% 60px 8%;
            display: grid;
            grid-template-columns: 1.2fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .hero-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(255, 193, 7, 0.1);
            border: 1px solid rgba(255, 193, 7, 0.3);
            color: var(--accent-gold);
            padding: 6px 16px;
            border-radius: 30px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-bottom: 24px;
        }

        .hero h1 {
            font-size: 3.4rem;
            line-height: 1.15;
            margin-bottom: 20px;
            letter-spacing: -1px;
        }

        .hero h1 span {
            background: linear-gradient(135deg, #ffc107, #f59e0b);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p {
            font-size: 1.1rem;
            color: var(--text-muted);
            margin-bottom: 35px;
            max-width: 540px;
        }

        .hero-cta {
            display: flex;
            gap: 16px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 14px 28px;
            border-radius: 12px;
            font-weight: 600;
            font-size: 0.95rem;
            text-decoration: none;
            transition: all 0.3s ease;
            cursor: pointer;
            border: none;
        }

        .btn-gold {
            background: linear-gradient(135deg, var(--accent-gold), #d97706);
            color: #000;
            box-shadow: 0 8px 25px var(--accent-glow);
        }

        .btn-gold:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 30px rgba(255, 193, 7, 0.4);
        }

        .btn-glass {
            background: rgba(255, 255, 255, 0.05);
            color: #fff;
            border: 1px solid var(--border-line);
            backdrop-filter: blur(10px);
        }

        .btn-glass:hover {
            background: rgba(255, 255, 255, 0.1);
            border-color: rgba(255, 255, 255, 0.2);
            transform: translateY(-3px);
        }

        .hero-img-wrapper {
            position: relative;
        }

        .hero-card-img {
            width: 100%;
            height: 420px;
            object-fit: cover;
            border-radius: 24px;
            border: 1px solid var(--border-line);
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.7);
        }

        .experience-badge {
            position: absolute;
            bottom: -20px;
            left: -20px;
            background: rgba(18, 26, 43, 0.9);
            backdrop-filter: blur(12px);
            border: 1px solid var(--border-glow);
            padding: 16px 24px;
            border-radius: 16px;
            display: flex;
            align-items: center;
            gap: 15px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.5);
        }

        .exp-num {
            font-size: 2rem;
            font-weight: 800;
            color: var(--accent-gold);
            line-height: 1;
        }

        .exp-text {
            font-size: 0.85rem;
            color: var(--text-muted);
            line-height: 1.3;
        }

        /* SECTION HEADINGS */
        section {
            padding: 80px 8%;
            scroll-margin-top: 70px;
        }

        .section-title {
            text-align: center;
            max-width: 650px;
            margin: 0 auto 55px auto;
        }

        .section-title small {
            color: var(--accent-gold);
            font-weight: 700;
            letter-spacing: 2px;
            text-transform: uppercase;
            font-size: 0.8rem;
            display: block;
            margin-bottom: 8px;
        }

        .section-title h2 {
            font-size: 2.3rem;
            letter-spacing: -0.5px;
        }

        /* GRID CARDS & GALLERY */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
            gap: 28px;
        }

        .glass-card {
            background: var(--bg-card);
            border: 1px solid var(--border-line);
            border-radius: 20px;
            overflow: hidden;
            backdrop-filter: blur(12px);
            transition: all 0.35s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .glass-card:hover {
            transform: translateY(-8px);
            border-color: var(--border-glow);
            background: var(--bg-card-hover);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
        }

        .glass-card img {
            width: 100%;
            height: 230px;
            object-fit: cover;
            border-bottom: 1px solid var(--border-line);
        }

        .card-content {
            padding: 24px;
        }

        .card-content h3 {
            font-size: 1.25rem;
            margin-bottom: 8px;
            color: #fff;
        }

        .card-content p {
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        /* SERVICES GRID */
        .service-icon-box {
            width: 52px;
            height: 52px;
            background: rgba(255, 193, 7, 0.1);
            border: 1px solid rgba(255, 193, 7, 0.2);
            border-radius: 14px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--accent-gold);
            font-size: 1.3rem;
            margin-bottom: 20px;
        }

        /* FORM & LOCATION SECTION */
        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: start;
        }

        .form-card {
            background: var(--bg-card);
            border: 1px solid var(--border-line);
            border-radius: 24px;
            padding: 35px;
            backdrop-filter: blur(12px);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-size: 0.88rem;
            color: var(--text-muted);
            font-weight: 500;
        }

        .form-input {
            width: 100%;
            padding: 14px 16px;
            background: rgba(6, 9, 19, 0.6);
            border: 1px solid var(--border-line);
            border-radius: 10px;
            color: #fff;
            font-family: inherit;
            font-size: 0.95rem;
            transition: all 0.3s;
        }

        .form-input:focus {
            outline: none;
            border-color: var(--accent-gold);
            box-shadow: 0 0 0 3px rgba(255, 193, 7, 0.15);
        }

        .map-box {
            border-radius: 24px;
            overflow: hidden;
            border: 1px solid var(--border-line);
            height: 100%;
            min-height: 420px;
        }

        /* FLOATING ACTION BAR FOR MOBILE */
        .floating-actions {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(18, 26, 43, 0.9);
            backdrop-filter: blur(16px);
            border: 1px solid var(--border-glow);
            padding: 10px 20px;
            border-radius: 40px;
            display: flex;
            align-items: center;
            gap: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.6);
            z-index: 999;
        }

        .float-btn {
            display: flex;
            align-items: center;
            gap: 8px;
            color: #fff;
            text-decoration: none;
            font-size: 0.88rem;
            font-weight: 600;
        }

        .float-btn-gold {
            color: var(--accent-gold);
        }

        /* FOOTER */
        footer {
            border-top: 1px solid var(--border-line);
            padding: 40px 8% 30px 8%;
            text-align: center;
            background: #04060d;
        }

        .rating-chip {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid var(--border-line);
            padding: 8px 20px;
            border-radius: 30px;
            margin-bottom: 20px;
            font-size: 0.9rem;
        }

        .stars {
            color: var(--accent-gold);
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 992px) {
            .hero {
                grid-template-columns: 1fr;
                text-align: center;
                padding-top: 50px;
            }
            .hero p {
                margin: 0 auto 30px auto;
            }
            .hero-cta {
                justify-content: center;
            }
            .experience-badge {
                left: 50%;
                transform: translateX(-50%);
            }
            .contact-container {
                grid-template-columns: 1fr;
            }
            nav {
                display: none; /* Mobile menu can be simplified */
            }
        }
    </style>
</head>
<body>

    <div class="glow-sphere-1"></div>
    <div class="glow-sphere-2"></div>

    <!-- HEADER -->
    <header>
        <div class="logo">
            <div class="logo-icon"><i class="fa-solid fa-bolt"></i></div>
            <span class="logo-text">EXCEL ELECTRICALS</span>
        </div>
        <nav>
            <a href="#home">Home</a>
            <a href="#motors">Motors</a>
            <a href="#winding">Winding</a>
            <a href="#services">Services</a>
            <a href="#about">About</a>
            <a href="#request" class="nav-btn">Service Request</a>
        </nav>
    </header>

    <!-- HERO SECTION -->
    <section class="hero" id="home">
        <div>
            <div class="hero-badge">
                <i class="fa-solid fa-shield-halved"></i> Certified Motor Workshop • Choondy
            </div>
            <h1>EXPERT ELECTRIC MOTOR <span>WINDING & REPAIR</span></h1>
            <p>High-precision stator rewinding, rotor balancing, coil modifications, and mechanical overhaul for single & three-phase motors.</p>
            <div class="hero-cta">
                <a href="tel:+919876543210" class="btn btn-gold"><i class="fa-solid fa-phone"></i> Call Workshop</a>
                <a href="https://wa.me/919876543210" class="btn btn-glass"><i class="fa-brands fa-whatsapp"></i> WhatsApp</a>
            </div>
        </div>
        <div class="hero-img-wrapper">
            <img src="25 Hp.jpg" alt="Industrial Motor Winding Workshop" class="hero-card-img">
            <div class="experience-badge">
                <div class="exp-num">100%</div>
                <div class="exp-text">Quality Copper Winding<br>& Testing Assured</div>
            </div>
        </div>
    </section>

    <!-- MOTOR GALLERY -->
    <section id="motors">
        <div class="section-title">
            <small>Precision Work</small>
            <h2>Motor Repair Gallery</h2>
        </div>
        <div class="cards-grid">
            <div class="glass-card">
                <img src="Inducton motor.webp" alt="Induction Motor">
                <div class="card-content">
                    <h3>Induction Motors</h3>
                    <p>Complete overhaul and insulation test for heavy induction motors.</p>
                </div>
            </div>
            <div class="glass-card">
                <img src="Motor.webp" alt="Motor Overhaul">
                <div class="card-content">
                    <h3>Mechanical Overhaul</h3>
                    <p>Bearing replacements, shaft polishing, and housing re-alignment.</p>
                </div>
            </div>
            <div class="glass-card">
                <img src="Field Winding.webp" alt="Field Stator Winding">
                <div class="card-content">
                    <h3>Stator Coil Winding</h3>
                    <p>High-grade dual-coated copper wire rewinding for maximum heat capacity.</p>
                </div>
            </div>
            <div class="glass-card">
                <img src="repair motor.webp" alt="Motor Repair Parts">
                <div class="card-content">
                    <h3>Rotor & Components</h3>
                    <p>Dynamic rotor check, terminal replacement, and capacitor upgrading.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SERVICES SECTION -->
    <section id="services" style="background: rgba(255,255,255,0.01);">
        <div class="section-title">
            <small>What We Do</small>
            <h2>Workshop Services</h2>
        </div>
        <div class="cards-grid">
            <div class="glass-card card-content">
                <div class="service-icon-box"><i class="fa-solid fa-bolt-lightning"></i></div>
                <h3>Copper Rewinding</h3>
                <p>Complete stator and armature rewinding using top-grade insulation paper and high-temp varnish.</p>
            </div>
            <div class="glass-card card-content">
                <div class="service-icon-box"><i class="fa-solid fa-wrench"></i></div>
                <h3>Complete Diagnostics</h3>
                <p>Electrical fault diagnosis, megger insulation test, and phase imbalance troubleshooting.</p>
            </div>
            <div class="glass-card card-content">
                <div class="service-icon-box"><i class="fa-solid fa-gear"></i></div>
                <h3>Bearing Replacement</h3>
                <p>Precision removal and installation of original SKF / NBC brand high-speed motor bearings.</p>
            </div>
            <div class="glass-card card-content">
                <div class="service-icon-box"><i class="fa-solid fa-car-battery"></i></div>
                <h3>Capacitor & Relay Service</h3>
                <p>Testing and replacement of start/run capacitors, centrifugal switches, and overload relays.</p>
            </div>
        </div>
    </section>

    <!-- SERVICE REQUEST FORM & LOCATION -->
    <section id="request">
        <div class="section-title">
            <small>Get In Touch</small>
            <h2>Service Request & Location</h2>
        </div>
        <div class="contact-container">
            <div class="form-card">
                <form id="directMsgForm">
                    <input type="hidden" name="access_key" value="YOUR_WEB3FORMS_ACCESS_KEY">
                    <div class="form-group">
                        <label>Full Name</label>
                        <input type="text" name="name" class="form-input" placeholder="e.g. Rahul Nair" required>
                    </div>
                    <div class="form-group">
                        <label>Phone Number</label>
                        <input type="tel" name="phone" class="form-input" placeholder="e.g. 9876543210" required>
                    </div>
                    <div class="form-group">
                        <label>Motor Issue / Equipment Details</label>
                        <textarea name="message" rows="4" class="form-input" placeholder="Describe the motor type (HP, Single/Three Phase) or problem..." required></textarea>
                    </div>
                    <button type="submit" id="submitBtn" class="btn btn-gold" style="width: 100%; justify-content: center;">
                        <i class="fa-solid fa-paper-plane"></i> Submit Request
                    </button>
                    <div id="formStatus" style="display: none; margin-top: 15px; text-align: center; font-size: 0.9rem;"></div>
                </form>
            </div>
            <div class="map-box">
                <iframe src="https://maps.google.com/maps?q=Excel%20Electricals,%20Choondy,%20Aluva&t=&z=15&ie=UTF8&iwloc=&output=embed" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </div>
        </div>
    </section>

    <!-- FLOATING QUICK ACTIONS BAR -->
    <div class="floating-actions">
        <a href="tel:+919876543210" class="float-btn float-btn-gold"><i class="fa-solid fa-phone"></i> Call Workshop</a>
        <span style="color: var(--border-line);">|</span>
        <a href="https://wa.me/919876543210" class="float-btn"><i class="fa-brands fa-whatsapp" style="color: #22c55e;"></i> WhatsApp</a>
    </div>

    <!-- FOOTER -->
    <footer>
        <div class="rating-chip">
            <span style="font-weight: 700; color: #fff;">4.9 Rating</span>
            <span class="stars">★★★★★</span>
            <span style="color: var(--text-muted); font-size: 0.85rem;">Google Verified</span>
        </div>
        <p style="color: var(--text-muted); font-size: 0.85rem;">&copy; 2026 EXCEL ELECTRICALS | Choondy, Aluva | GSTIN: 32AAGPX3837Q1ZZ</p>
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
                    statusDiv.innerText = "✔️ Your request has been sent! We will contact you back shortly.";
                    form.reset();
                } else {
                    statusDiv.style.display = "block";
                    statusDiv.style.color = "#ef4444";
                    statusDiv.innerText = "✖️ " + (result.message || "Failed to submit.");
                }
            } catch (error) {
                statusDiv.style.display = "block";
                statusDiv.style.color = "#ef4444";
                statusDiv.innerText = "✖️ Error submitting request. Please call directly.";
            } finally {
                submitBtn.innerHTML = '<i class="fa-solid fa-paper-plane"></i> Submit Request';
                submitBtn.disabled = false;
            }
        });
    </script>
</body>
</html>
