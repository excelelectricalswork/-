<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Excel Electricals | Motor Winding & Repair Workshop</title>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700;800&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    
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
        /* RESET & BASE STYLES */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: #0b0f19;
            color: #e2e8f0;
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        h1, h2, h3, h4 {
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        section {
            padding: 80px 7%;
            scroll-margin-top: 70px;
        }

        /* HEADER & NAVIGATION */
        header {
            background-color: rgba(15, 23, 42, 0.95);
            backdrop-filter: blur(10px);
            padding: 15px 7%;
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(255, 184, 0, 0.2);
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            color: #ffb800;
            font-size: 1.4rem;
            font-weight: 800;
            letter-spacing: 0.5px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        nav {
            display: flex;
            align-items: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        nav a {
            color: #cbd5e1;
            font-weight: 500;
            font-size: 0.95rem;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #ffb800;
        }

        .nav-btn {
            background: #ffb800;
            color: #0b0f19 !important;
            padding: 8px 18px;
            border-radius: 6px;
            font-weight: 700 !important;
            transition: transform 0.2s, background 0.2s !important;
        }

        .nav-btn:hover {
            background: #e0a200;
            transform: translateY(-2px);
        }

        /* HERO SECTION */
        .hero {
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 40px;
            background: radial-gradient(circle at top right, #1e293b, #0b0f19);
            min-height: 80vh;
        }

        .hero-content {
            flex: 1 1 500px;
        }

        .hero-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(255, 184, 0, 0.1);
            border: 1px solid rgba(255, 184, 0, 0.3);
            color: #ffb800;
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-bottom: 20px;
        }

        .hero h1 {
            font-size: 2.8rem;
            line-height: 1.2;
            color: #ffffff;
            margin-bottom: 15px;
        }

        .hero h1 span {
            color: #ffb800;
        }

        .hero p {
            font-size: 1.1rem;
            color: #94a3b8;
            margin-bottom: 30px;
        }

        .hero-buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 12px 24px;
            border-radius: 8px;
            font-weight: 600;
            font-size: 0.95rem;
            transition: all 0.3s ease;
            cursor: pointer;
            border: none;
        }

        .btn-primary {
            background-color: #ffb800;
            color: #0b0f19;
        }

        .btn-primary:hover {
            background-color: #e0a200;
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(255, 184, 0, 0.2);
        }

        .btn-secondary {
            background-color: #1e293b;
            color: #e2e8f0;
            border: 1px solid #334155;
        }

        .btn-secondary:hover {
            background-color: #334155;
            transform: translateY(-2px);
        }

        .hero-image {
            flex: 1 1 400px;
            max-width: 480px;
            border-radius: 16px;
            overflow: hidden;
            border: 1px solid #334155;
            box-shadow: 0 20px 40px rgba(0,0,0,0.5);
        }

        .hero-image img {
            width: 100%;
            height: 380px;
            object-fit: cover;
        }

        /* SECTION HEADINGS */
        .section-header {
            text-align: center;
            max-width: 650px;
            margin: 0 auto 50px auto;
        }

        .section-header small {
            color: #ffb800;
            font-weight: 700;
            letter-spacing: 1.5px;
            text-transform: uppercase;
            font-size: 0.8rem;
        }

        .section-header h2 {
            font-size: 2.2rem;
            color: #ffffff;
            margin: 8px 0;
        }

        .section-header p {
            color: #94a3b8;
            font-size: 0.95rem;
        }

        /* GRID CARDS */
        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .card {
            background: #161e2e;
            border: 1px solid #232d3f;
            border-radius: 12px;
            overflow: hidden;
            transition: transform 0.3s ease, border-color 0.3s ease;
        }

        .card:hover {
            transform: translateY(-6px);
            border-color: rgba(255, 184, 0, 0.4);
        }

        .card img {
            width: 100%;
            height: 220px;
            object-fit: cover;
        }

        .card-body {
            padding: 20px;
        }

        .card-body h3 {
            color: #ffb800;
            font-size: 1.2rem;
            margin-bottom: 8px;
        }

        .card-body p {
            color: #94a3b8;
            font-size: 0.9rem;
        }

        /* SERVICES SECTION */
        .services-bg {
            background-color: #0f172a;
            border-top: 1px solid #1e293b;
            border-bottom: 1px solid #1e293b;
        }

        .service-card {
            background: #161e2e;
            padding: 25px;
            border-radius: 12px;
            border: 1px solid #232d3f;
            transition: all 0.3s ease;
        }

        .service-card:hover {
            border-color: #ffb800;
            transform: translateY(-4px);
        }

        .service-icon {
            width: 50px;
            height: 50px;
            background: rgba(255, 184, 0, 0.1);
            color: #ffb800;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.3rem;
            margin-bottom: 15px;
        }

        .service-card h3 {
            color: #ffffff;
            font-size: 1.15rem;
            margin-bottom: 10px;
        }

        .service-card p {
            color: #94a3b8;
            font-size: 0.9rem;
        }

        /* MAP & CONTACT */
        .contact-wrapper {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 40px;
            align-items: start;
        }

        .map-frame {
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid #334155;
            height: 380px;
        }

        /* FORM STYLES */
        .form-container {
            background: #161e2e;
            padding: 30px;
            border-radius: 12px;
            border: 1px solid #232d3f;
        }

        .form-group {
            margin-bottom: 18px;
        }

        .form-group label {
            display: block;
            margin-bottom: 6px;
            color: #cbd5e1;
            font-size: 0.9rem;
            font-weight: 500;
        }

        .form-control {
            width: 100%;
            padding: 12px;
            background: #0b0f19;
            border: 1px solid #334155;
            border-radius: 6px;
            color: #ffffff;
            font-family: inherit;
            font-size: 0.95rem;
            transition: border-color 0.3s;
        }

        .form-control:focus {
            outline: none;
            border-color: #ffb800;
        }

        /* TERMS & REVIEWS */
        .terms-box {
            background: #161e2e;
            padding: 30px;
            border-radius: 12px;
            border: 1px solid #232d3f;
        }

        .terms-box ul {
            list-style: none;
        }

        .terms-box li {
            position: relative;
            padding-left: 25px;
            margin-bottom: 15px;
            color: #94a3b8;
        }

        .terms-box li::before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #ffb800;
            font-weight: bold;
        }

        .terms-box strong {
            color: #ffffff;
        }

        /* FOOTER */
        footer {
            background: #070a10;
            padding: 40px 7% 20px 7%;
            border-top: 1px solid #1e293b;
            text-align: center;
        }

        .review-badge {
            background: #161e2e;
            display: inline-flex;
            align-items: center;
            gap: 12px;
            padding: 12px 24px;
            border-radius: 30px;
            border: 1px solid #232d3f;
            margin-bottom: 25px;
        }

        .rating-stars {
            color: #ffb800;
        }

        .footer-copy {
            color: #64748b;
            font-size: 0.85rem;
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                gap: 15px;
            }
            .hero {
                flex-direction: column;
                text-align: center;
            }
            .hero-buttons {
                justify-content: center;
            }
            .hero-badge {
                margin: 0 auto 20px auto;
            }
        }
    </style>
</head>
<body>

    <!-- HEADER -->
    <header>
        <div class="logo">
            <i class="fa-solid fa-bolt"></i> EXCEL ELECTRICALS
        </div>
        <nav>
            <a href="#home">Home</a>
            <a href="#motors">Motors</a>
            <a href="#winding">Winding</a>
            <a href="#services">Services</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
            <a href="#request" class="nav-btn">Service Request</a>
        </nav>
    </header>

    <!-- HERO SECTION -->
    <section class="hero" id="home">
        <div class="hero-content">
            <div class="hero-badge">
                <i class="fa-solid fa-certificate"></i> Verified Electrical Workshop
            </div>
            <h1>ELECTRIC MOTOR <span>WINDING & REPAIR</span></h1>
            <p>Professional motor winding, stator rewinding, rotor servicing, and electrical component replacement in Choondy, Aluva.</p>
            <div class="hero-buttons">
                <a href="tel:+919876543210" class="btn btn-primary"><i class="fa-solid fa-phone"></i> Call Now</a>
                <a href="https://wa.me/919876543210" class="btn btn-secondary"><i class="fa-brands fa-whatsapp"></i> WhatsApp</a>
                <a href="mailto:info@excelelectricals.co.in" class="btn btn-secondary"><i class="fa-solid fa-envelope"></i> Email</a>
            </div>
        </div>
        <div class="hero-image">
            <img src="25 Hp.jpg" alt="Motor Winding Workshop">
        </div>
    </section>

    <!-- GALLERY SECTION -->
    <section id="motors">
        <div class="section-header">
            <small>Electric Motor Repairs</small>
            <h2>Motor Work Gallery</h2>
            <p>Electric motors, stators, rotors, and components serviced at our workshop.</p>
        </div>
        <div class="grid-container">
            <div class="card">
                <img src="Inducton motor.webp" alt="Induction Motor Repair">
                <div class="card-body">
                    <h3>Induction Motor</h3>
                    <p>Complete motor repair and electrical maintenance.</p>
                </div>
            </div>
            <div class="card">
                <img src="Motor.webp" alt="Electric Motor Service">
                <div class="card-body">
                    <h3>Motor Overhaul</h3>
                    <p>Dismantling, inspection, testing, and mechanical overhaul.</p>
                </div>
            </div>
            <div class="card">
                <img src="Field Winding.webp" alt="Field Winding Stator">
                <div class="card-body">
                    <h3>Field Winding</h3>
                    <p>Stator coil rewinding with high-quality insulation materials.</p>
                </div>
            </div>
            <div class="card">
                <img src="repair motor.webp" alt="Motor Components Repair">
                <div class="card-body">
                    <h3>Component Fitting</h3>
                    <p>Rotor balancing, bearing replacements, and housing repairs.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- WINDING SECTION -->
    <section id="winding" style="background-color: #0f172a;">
        <div class="section-header">
            <small>Winding & Rewinding</small>
            <h2>Specialized Winding Services</h2>
            <p>High-grade copper wire rewinding for single-phase and three-phase motors.</p>
        </div>
        <div class="grid-container">
            <div class="card">
                <img src="Field Winding.webp" alt="Stator Winding Work">
                <div class="card-body">
                    <h3>Stator Rewinding</h3>
                    <p>Precision coil insertion, varnishing, and heating treatment.</p>
                </div>
            </div>
            <div class="card">
                <img src="Ex Rotor winding.webp" alt="Rotor Rewinding Work">
                <div class="card-body">
                    <h3>Rotor Winding</h3>
                    <p>Expert slip ring and armature rotor rewinding and electrical testing.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SERVICES SECTION -->
    <section class="services-bg" id="services">
        <div class="section-header">
            <small>Our Capabilities</small>
            <h2>Workshop Services</h2>
            <p>Comprehensive electrical and mechanical repair solutions under one roof.</p>
        </div>
        <div class="grid-container">
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-bolt"></i></div>
                <h3>Motor Winding</h3>
                <p>Complete coil rewinding for long-lasting high efficiency and heat resistance.</p>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-screwdriver-wrench"></i></div>
                <h3>Motor Repair</h3>
                <p>Full troubleshooting, electrical fault finding, and overhaul repairs.</p>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-compact-disc"></i></div>
                <h3>Bearing Replacement</h3>
                <p>Precision bearing extraction and fitting for quiet motor operation.</p>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-car-battery"></i></div>
                <h3>Capacitor Testing</h3>
                <p>Run and start capacitor testing and replacement with genuine parts.</p>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-fan"></i></div>
                <h3>Stator & Core Cleaning</h3>
                <p>Core re-varnishing, chemical washing, and insulation dipping.</p>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-gear"></i></div>
                <h3>Spare Parts Fitting</h3>
                <p>Cooling fan blades, terminal blocks, end covers, and shaft repairs.</p>
            </div>
        </div>
    </section>

    <!-- ABOUT & LOCATION SECTION -->
    <section id="about">
        <div class="contact-wrapper">
            <div>
                <div class="section-header" style="text-align: left; margin-bottom: 20px;">
                    <small>About Workshop</small>
                    <h2>Excel Electricals</h2>
                </div>
                <p style="color: #94a3b8; margin-bottom: 20px;">Located in Choondy, Aluva, Excel Electricals is a trusted workshop specializing in high-quality electric motor repair, stator rewinding, rotor servicing, and electrical component repairs.</p>
                <p style="color: #94a3b8; margin-bottom: 20px;"><i class="fa-solid fa-location-dot" style="color: #ffb800;"></i> Choondy, Aluva, Ernakulam, Kerala</p>
            </div>
            <div class="map-frame">
                <iframe src="https://maps.google.com/maps?q=Excel%20Electricals,%20Choondy,%20Aluva&t=&z=15&ie=UTF8&iwloc=&output=embed" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </div>
        </div>
    </section>

    <!-- SERVICE REQUEST FORM -->
    <section id="request" style="background-color: #0f172a;">
        <div class="section-header">
            <small>Direct Contact</small>
            <h2>Request A Service</h2>
            <p>Send your motor issue details directly to our team.</p>
        </div>
        <div class="form-container" style="max-width: 600px; margin: 0 auto;">
            <form id="directMsgForm">
                <input type="hidden" name="access_key" value="YOUR_WEB3FORMS_ACCESS_KEY">
                
                <div class="form-group">
                    <label>Your Name</label>
                    <input type="text" name="name" class="form-control" placeholder="Enter full name" required>
                </div>
                <div class="form-group">
                    <label>Phone Number</label>
                    <input type="tel" name="phone" class="form-control" placeholder="Enter mobile number" required>
                </div>
                <div class="form-group">
                    <label>Motor / Repair Details</label>
                    <textarea name="message" rows="4" class="form-control" placeholder="Describe motor type (e.g., 3HP Induction, Single Phase, Pump)" required></textarea>
                </div>
                <button type="submit" id="submitBtn" class="btn btn-primary" style="width: 100%; justify-content: center;">
                    <i class="fa-solid fa-paper-plane"></i> Send Request
                </button>
                <div id="formStatus" style="display: none; margin-top: 15px; text-align: center; font-weight: 600;"></div>
            </form>
        </div>
    </section>

    <!-- TERMS & CONDITIONS -->
    <section id="terms">
        <div class="section-header">
            <small>Policies</small>
            <h2>Terms & Conditions</h2>
        </div>
        <div class="terms-box" style="max-width: 800px; margin: 0 auto;">
            <ul>
                <li><strong>Inspection & Estimates:</strong> Initial diagnosis is provided upon receipt at our workshop. Final service charges depend on wire gauge, copper weight, and replacement parts.</li>
                <li><strong>Warranty:</strong> Rewinding carries a limited service warranty on manufacturing defects in copper/insulation work. Damage from phase loss, voltage fluctuation, dry running, or water entry is excluded.</li>
                <li><strong>Collection:</strong> Repaired motors should be collected within 30 days of completion notification.</li>
            </ul>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <div class="review-badge">
            <span style="font-weight: 700; color: #fff;">4.9</span>
            <span class="rating-stars">★★★★★</span>
            <span style="color: #94a3b8; font-size: 0.85rem;">Google Verified Reviews</span>
        </div>
        <div class="footer-copy">
            <p>&copy; 2026 EXCEL ELECTRICALS | GSTIN: 32AAGPX3837Q1ZZ</p>
        </div>
    </footer>

    <!-- Form Handler Script -->
    <script>
        const form = document.getElementById('directMsgForm');
        const statusDiv = document.getElementById('formStatus');
        const submitBtn = document.getElementById('submitBtn');

        form.addEventListener('submit', async function(e) {
            e.preventDefault();
            submitBtn.innerHTML = '<i class="fa-solid fa-spinner fa-spin"></i> Sending...';
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
                    statusDiv.innerText = "✔️ Service request submitted successfully!";
                    form.reset();
                } else {
                    statusDiv.style.display = "block";
                    statusDiv.style.color = "#ef4444";
                    statusDiv.innerText = "✖️ " + (result.message || "Submission failed.");
                }
            } catch (error) {
                statusDiv.style.display = "block";
                statusDiv.style.color = "#ef4444";
                statusDiv.innerText = "✖️ Error sending message. Please try calling directly.";
            } finally {
                submitBtn.innerHTML = '<i class="fa-solid fa-paper-plane"></i> Send Request';
                submitBtn.disabled = false;
            }
        });
    </script>
</body>
</html>
