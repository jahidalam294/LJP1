<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lok Janta Party (LJP) - Official Website</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-orange: #FF671F;
            --primary-white: #FFFFFF;
            --primary-green: #046A38;
            --ashoka-blue: #06038D;
            --dark-blue: #062A62;
            --light-blue: #0B3C84;
            --bg-light: #F4F7FA;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--primary-white);
            color: #333;
        }

        /* --- Premium Header / Navigation --- */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 5%;
            background: linear-gradient(to right, #ffffff, #f9fbfe);
            box-shadow: 0 4px 20px rgba(6, 42, 98, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 3px solid var(--primary-orange);
        }

        .logo-area {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        /* Upgraded Premium Badge Logo */
        .logo-circle {
            width: 65px;
            height: 65px;
            border-radius: 50%;
            background: #ffffff;
            border: 4px solid transparent;
            background-image: linear-gradient(white, white), linear-gradient(135deg, var(--primary-orange), var(--ashoka-blue), var(--primary-green));
            background-origin: border-box;
            background-clip: content-box, border-box;
            display: flex;
            justify-content: center;
            align-items: center;
            font-weight: 900;
            font-size: 22px;
            color: var(--dark-blue);
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
            letter-spacing: 1px;
            position: relative;
        }
        
        .logo-circle::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            border-radius: 50%;
            border: 1px dashed var(--ashoka-blue);
            opacity: 0.5;
            animation: rotate 20s linear infinite;
        }

        @keyframes rotate { 100% { transform: rotate(360deg); } }

        .logo-text h1 {
            color: var(--dark-blue);
            font-size: 24px;
            letter-spacing: 1px;
            font-weight: 800;
        }

        .logo-text p {
            color: var(--primary-green);
            font-size: 13px;
            font-weight: 700;
            letter-spacing: 0.5px;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 22px;
            align-items: center;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--dark-blue);
            font-weight: 700;
            font-size: 13px;
            text-transform: uppercase;
            transition: 0.3s;
            padding: 8px 12px;
            border-radius: 4px;
        }

        nav ul li a:hover, nav ul li a.active {
            color: white;
            background: linear-gradient(135deg, var(--dark-blue), var(--light-blue));
            box-shadow: 0 4px 10px rgba(6, 42, 98, 0.2);
        }

        .lang-switch-btn {
            background: linear-gradient(135deg, var(--primary-orange), #ff8443);
            color: white;
            border: none;
            padding: 8px 16px;
            font-size: 13px;
            font-weight: bold;
            border-radius: 4px;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(255, 103, 31, 0.3);
            transition: 0.3s;
        }
        .lang-switch-btn:hover {
            transform: translateY(-1px);
            box-shadow: 0 6px 12px rgba(255, 103, 31, 0.4);
        }

        .join-btn {
            background: linear-gradient(135deg, var(--dark-blue), var(--light-blue));
            color: white;
            padding: 10px 24px;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            font-size: 13px;
            transition: 0.3s;
            box-shadow: 0 4px 10px rgba(6, 42, 98, 0.2);
        }

        .join-btn:hover {
            background: linear-gradient(135deg, var(--primary-green), #058245);
            box-shadow: 0 4px 10px rgba(4, 106, 56, 0.2);
        }

        /* --- Dynamic & High-Fidelity Banner Section --- */
        .hero {
            background: linear-gradient(180deg, rgba(255,255,255,0.8) 0%, rgba(244,247,250,0.95) 100%), url('https://images.unsplash.com/photo-1599930113854-d6d7fd521f10?q=80&w=1920&auto=format&fit=crop') no-repeat center center/cover;
            padding: 100px 5%;
            text-align: center;
            border-bottom: 5px solid var(--primary-green);
            position: relative;
            overflow: hidden;
        }

        /* Indian Flag Creative Overlay Shapes inside Banner */
        .hero::before {
            content: '';
            position: absolute;
            top: 0; left: 0; width: 15px; height: 100%;
            background: var(--primary-orange);
        }

        .hero-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 25px;
            position: relative;
            z-index: 2;
        }

        /* Mega Display Branding */
        .hero-logo-box {
            background: white;
            padding: 15px 35px;
            border-radius: 50px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            display: inline-flex;
            align-items: center;
            gap: 15px;
            border: 1px solid #eee;
            margin-bottom: 10px;
        }

        .hero-logo-box img {
            height: 40px;
        }

        .hero-main-title {
            font-size: 68px;
            font-weight: 900;
            letter-spacing: 2px;
            line-height: 1.1;
            text-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }

        .text-lok { color: var(--dark-blue); }
        .text-janta { color: var(--primary-orange); }
        .text-party { color: var(--primary-green); }

        .hero-slogan {
            font-size: 32px;
            font-weight: 800;
            color: var(--dark-blue);
            margin: 5px 0 20px 0;
            letter-spacing: 0.5px;
            background: linear-gradient(to right, var(--primary-orange), var(--dark-blue), var(--primary-green));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero-action-btn {
            background: linear-gradient(135deg, var(--dark-blue) 0%, var(--light-blue) 100%);
            color: white;
            padding: 16px 45px;
            font-size: 18px;
            font-weight: bold;
            text-decoration: none;
            text-transform: uppercase;
            border-radius: 50px;
            box-shadow: 0 6px 25px rgba(6, 42, 98, 0.3);
            transition: 0.3s;
        }

        .hero-action-btn:hover {
            background: linear-gradient(135deg, var(--primary-orange) 0%, #ff8443 100%);
            box-shadow: 0 6px 25px rgba(255, 103, 31, 0.4);
            transform: translateY(-2px);
        }

        /* --- Common Section Styles --- */
        .section-padding {
            padding: 80px 8%;
        }

        .center-title {
            text-align: center;
            font-size: 36px;
            color: var(--dark-blue);
            text-transform: uppercase;
            margin-bottom: 50px;
            font-weight: 800;
            letter-spacing: 1px;
        }

        /* --- About & Vision Section --- */
        .about-vision {
            background: linear-gradient(135deg, var(--dark-blue) 0%, #041b3f 100%);
            color: white;
            display: grid;
            grid-template-columns: 1fr 1fr;
            padding: 70px 8%;
            gap: 60px;
            border-bottom: 4px solid var(--primary-orange);
        }

        .info-box {
            display: flex;
            gap: 25px;
            align-items: flex-start;
        }

        .info-icon {
            font-size: 35px;
            background: rgba(255,255,255,0.08);
            padding: 15px;
            border-radius: 12px;
            min-width: 75px;
            height: 75px;
            display: flex;
            justify-content: center;
            align-items: center;
            border: 1px solid rgba(255,255,255,0.2);
            color: var(--primary-orange);
        }

        .info-content h2 {
            font-size: 26px;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .info-content p {
            font-size: 15px;
            line-height: 1.7;
            color: #e2e8f0;
        }

        .vision-box {
            border-left: 1px solid rgba(255,255,255,0.15);
            padding-left: 60px;
        }
        
        .vision-box .info-icon {
            color: #00ff87;
        }

        /* --- Founder Section --- */
        .founder-section {
            background-color: var(--bg-light);
            text-align: center;
        }

        .founder-card {
            background: white;
            max-width: 750px;
            margin: 0 auto;
            padding: 50px 40px;
            border-radius: 16px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.04);
            border-top: 5px solid var(--primary-orange);
            position: relative;
        }

        .founder-avatar {
            width: 130px;
            height: 130px;
            border-radius: 50%;
            background: linear-gradient(135deg, #f0f4f8, #e2e8f0);
            margin: 0 auto 25px auto;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 55px;
            color: var(--dark-blue);
            border: 4px solid var(--primary-green);
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        .founder-name {
            font-size: 26px;
            color: var(--dark-blue);
            font-weight: 800;
            margin-bottom: 5px;
        }

        .founder-title {
            font-size: 14px;
            color: var(--primary-orange);
            text-transform: uppercase;
            font-weight: bold;
            letter-spacing: 1.5px;
            margin-bottom: 25px;
        }

        .founder-quote {
            font-size: 16px;
            line-height: 1.8;
            color: #4a5568;
            font-style: italic;
        }

        /* --- Commitments Section --- */
        .commitments-section {
            background-color: var(--primary-white);
        }

        .commitments-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 25px;
            max-width: 1400px;
            margin: 0 auto;
        }

        .commitment-card {
            background: white;
            border: 1px solid #e2e8f0;
            border-radius: 12px;
            padding: 30px 20px;
            position: relative;
            box-shadow: 0 4px 6px rgba(0,0,0,0.01);
            transition: 0.3s;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

        .commitment-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 30px rgba(6, 42, 98, 0.1);
            border-color: #cbd5e0;
        }

        .badge-num {
            position: absolute;
            top: -15px;
            width: 32px;
            height: 32px;
            border-radius: 50%;
            color: white;
            font-weight: bold;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 13px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.15);
        }

        /* Badge Card Accent Colors */
        .card-1 .badge-num { background-color: #062A62; }
        .card-2 .badge-num { background-color: #046A38; }
        .card-3 .badge-num { background-color: #D9381E; }
        .card-4 .badge-num { background-color: #2B6CB0; }
        .card-5 .badge-num { background-color: #1A8243; }
        .card-6 .badge-num { background-color: #E65100; }
        .card-7 .badge-num { background-color: #0D47A1; }
        .card-8 .badge-num { background-color: #2E7D32; }
        .card-9 .badge-num { background-color: #C62828; }
        .card-10 .badge-num { background-color: #37474F; }

        .card-icon {
            font-size: 38px;
            color: var(--dark-blue);
            margin: 15px 0;
        }

        .commitment-card h3 {
            font-size: 15px;
            color: var(--dark-blue);
            text-transform: uppercase;
            font-weight: 800;
            margin-bottom: 12px;
            min-height: 36px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .commitment-card p {
            font-size: 13px;
            color: #4a5568;
            line-height: 1.6;
        }

        /* --- Team Section --- */
        .team-section {
            background-color: var(--bg-light);
        }

        .team-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
            max-width: 1100px;
            margin: 0 auto;
        }

        .team-member {
            background: white;
            padding: 40px 30px;
            border-radius: 12px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.02);
            border-bottom: 3px solid transparent;
            transition: 0.3s;
        }

        .team-member:hover {
            border-bottom-color: var(--primary-green);
            transform: translateY(-3px);
        }

        .member-icon {
            font-size: 45px;
            color: var(--primary-green);
            margin-bottom: 20px;
        }

        /* --- News Section --- */
        .news-section {
            background-color: var(--primary-white);
        }

        .news-container {
            max-width: 900px;
            margin: 0 auto;
        }

        .news-item {
            background: var(--bg-light);
            padding: 25px;
            border-radius: 8px;
            margin-bottom: 20px;
            border-left: 6px solid var(--light-blue);
            transition: 0.2s;
        }

        .news-item:hover {
            transform: translateX(5px);
            background: #edf2f7;
        }

        .news-date {
            font-size: 12px;
            color: var(--primary-orange);
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        /* --- Contact Section --- */
        .contact-section {
            background: linear-gradient(135deg, #111116 0%, #1a1a24 100%);
            color: white;
            border-top: 5px solid var(--primary-orange);
        }

        .contact-section .center-title {
            color: white;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 40px;
            max-width: 1100px;
            margin: 0 auto;
            text-align: center;
        }

        .contact-box {
            background: rgba(255,255,255,0.03);
            padding: 35px 25px;
            border-radius: 12px;
            border: 1px solid rgba(255,255,255,0.05);
        }

        .contact-box i {
            font-size: 35px;
            color: var(--primary-orange);
            margin-bottom: 20px;
        }

        /* --- Footer Bottom Bar --- */
        footer {
            background-color: var(--primary-green);
            color: white;
            padding: 30px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
        }

        .footer-left h2 {
            font-size: 22px;
            text-transform: uppercase;
            font-weight: 800;
            letter-spacing: 0.5px;
        }

        .footer-center {
            display: flex;
            gap: 15px;
        }

        .footer-btn {
            padding: 12px 28px;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            font-size: 14px;
            text-transform: uppercase;
            transition: 0.3s;
        }

        .footer-btn.blue { background-color: var(--dark-blue); color: white; box-shadow: 0 4px 10px rgba(0,0,0,0.15); }
        .footer-btn.outline { background-color: transparent; color: white; border: 2px solid white; }
        .footer-btn:hover { opacity: 0.9; transform: translateY(-1px); }

        .footer-right {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .social-icons a {
            color: white;
            background: rgba(255,255,255,0.1);
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: inline-flex;
            justify-content: center;
            align-items: center;
            text-decoration: none;
            transition: 0.3s;
            font-size: 18px;
        }

        .social-icons a:hover { background-color: var(--primary-orange); transform: scale(1.1); }

        /* --- Responsive Design (Mobile Friendly) --- */
        @media (max-width: 1200px) {
            .commitments-grid { grid-template-columns: repeat(3, 1fr); }
        }

        @media (max-width: 1024px) {
            .about-vision { grid-template-columns: 1fr; gap: 40px; }
            .vision-box { border-left: none; padding-left: 0; border-top: 1px solid rgba(255,255,255,0.15); padding-top: 40px; }
            .team-grid { grid-template-columns: repeat(2, 1fr); }
        }

        @media (max-width: 768px) {
            header { flex-direction: column; gap: 20px; text-align: center; padding: 20px 5%; }
            nav ul { flex-wrap: wrap; justify-content: center; gap: 10px; }
            .hero { padding: 70px 5%; }
            .hero-main-title { font-size: 42px; }
            .hero-slogan { font-size: 22px; }
            .commitments-grid { grid-template-columns: repeat(2, 1fr); }
            .team-grid, .contact-grid { grid-template-columns: 1fr; }
            footer { flex-direction: column; text-align: center; gap: 25px; }
        }

        @media (max-width: 480px) {
            .commitments-grid { grid-template-columns: 1fr; }
            .hero-main-title { font-size: 36px; }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo-area">
            <div class="logo-circle">LJP</div>
            <div class="logo-text">
                <h1>LOK JANTA PARTY</h1>
                <p id="nav-slogan">Power of People, Progress of Nation</p>
            </div>
        </div>
        <nav>
            <ul>
                <li><a href="#" class="active" id="nav-home">Home</a></li>
                <li><a href="#about" id="nav-about">About Us</a></li>
                <li><a href="#vision" id="nav-vision">Our Vision</a></li>
                <li><a href="#commitments" id="nav-commitments">Commitments</a></li>
                <li><a href="#team" id="nav-team">Team</a></li>
                <li><a href="#news" id="nav-news">News</a></li>
                <li><a href="#contact" id="nav-contact">Contact</a></li>
                <li><button class="lang-switch-btn" onclick="toggleLanguage()" id="lang-btn">हिंदी</button></li>
            </ul>
        </nav>
        <a href="#contact" class="join-btn" id="nav-join">Join Us</a>
    </header>

    <section class="hero">
        <div class="hero-container">
            <div class="hero-logo-box">
                <div class="logo-circle" style="width:40px; height:40px; font-size:14px; border-width:2px;">LJP</div>
                <span style="font-weight: 800; color: var(--dark-blue); letter-spacing: 1px;">LOK JANTA PARTY</span>
            </div>
            <h1 class="hero-main-title">
                <span class="text-lok">LOK</span> 
                <span class="text-janta">JANTA</span> 
                <span class="text-party">PARTY</span>
            </h1>
            <div class="hero-slogan" id="hero-slogan">Voice of People, Development of Nation</div>
            <a href="#contact" class="hero-action-btn" id="hero-btn">Join The Change</a>
        </div>
    </section>

    <section class="about-vision" id="about">
        <div class="info-box">
            <div class="info-icon"><i class="fas fa-users"></i></div>
            <div class="info-content">
                <h2 id="about-title">About LJP</h2>
                <p id="about-desc">Lok Janta Party (LJP) is a people-first political movement dedicated to building a strong, transparent and developed India. Our power is the people, our mission is a better tomorrow.</p>
            </div>
        </div>
        <div class="info-box vision-box" id="vision">
            <div class="info-icon"><i class="fas fa-bullseye"></i></div>
            <div class="info-content">
                <h2 id="vision-title">Our Vision</h2>
                <p id="vision-desc">A corruption-free India with equal opportunities, quality education, healthcare for all, and a strong economy driven by honesty, innovation and youth power.</p>
            </div>
        </div>
    </section>

    <section class="section-padding founder-section">
        <h2 class="center-title" id="founder-section-title">Our Founder</h2>
        <div class="founder-card">
            <div class="founder-avatar">
                <i class="fas fa-user-tie"></i>
            </div>
            <div class="founder-name">Mr. Jahid</div>
            <div class="founder-title" id="founder-post">Founder, Lok Janta Party</div>
            <p class="founder-quote" id="founder-quote">"My goal is to strengthen the voice of the common citizen of the country. Lok Janta Party is not just a party, but the hope of every Indian who wants change and development. Together we will build a new and golden India."</p>
        </div>
    </section>

    <section class="section-padding commitments-section" id="commitments">
        <h2 class="center-title" id="commitments-title">Our 10 Commitments</h2>
        
        <div class="commitments-grid">
            <div class="commitment-card card-1">
                <div class="badge-num">01</div>
                <div class="card-icon"><i class="fas fa-handshake"></i></div>
                <h3 id="c1-t">Zero Corruption</h3>
                <p id="c1-d">Complete zero tolerance towards corruption with strict laws.</p>
            </div>
            <div class="commitment-card card-2">
                <div class="badge-num">02</div>
                <div class="card-icon"><i class="fas fa-user-graduate"></i></div>
                <h3 id="c2-t">Quality Education</h3>
                <p id="c2-d">Free and high-quality education for every child.</p>
            </div>
            <div class="commitment-card card-3">
                <div class="badge-num">03</div>
                <div class="card-icon"><i class="fas fa-heartbeat"></i></div>
                <h3 id="c3-t">Healthcare For All</h3>
                <p id="c3-d">Affordable and premium healthcare services for every citizen.</p>
            </div>
            <div class="commitment-card card-4">
                <div class="badge-num">04</div>
                <div class="card-icon"><i class="fas fa-briefcase"></i></div>
                <h3 id="c4-t">Jobs For Youth</h3>
                <p id="c4-d">Skill development and guaranteed employment opportunities.</p>
            </div>
            <div class="commitment-card card-5">
                <div class="badge-num">05</div>
                <div class="card-icon"><i class="fas fa-tractor"></i></div>
                <h3 id="c5-t">Strong Farmers</h3>
                <p id="c5-d">Fair prices for crops and modern technical support for farmers.</p>
            </div>
            <div class="commitment-card card-6">
                <div class="badge-num">06</div>
                <div class="card-icon"><i class="fas fa-building"></i></div>
                <h3 id="c6-t">Infrastructure</h3>
                <p id="c6-d">World-class roads, electricity, and clean water in every village and city.</p>
            </div>
            <div class="commitment-card card-7">
                <div class="badge-num">07</div>
                <div class="card-icon"><i class="fas fa-shield-alt"></i></div>
                <h3 id="c7-t">Women Safety</h3>
                <p id="c7-d">Ensure absolute safety, respect, and equal opportunities for women.</p>
            </div>
            <div class="commitment-card card-8">
                <div class="badge-num">08</div>
                <div class="card-icon"><i class="fas fa-leaf"></i></div>
                <h3 id="c8-t">Green India</h3>
                <p id="c8-d">Clean air, pure water, and dedication to environmental protection.</p>
            </div>
            <div class="commitment-card card-9">
                <div class="badge-num">09</div>
                <div class="card-icon"><i class="fas fa-gavel"></i></div>
                <h3 id="c9-t">Transparent Govt</h3>
                <p id="c9-d">Transparent policies, citizen rights, and an accountable system.</p>
            </div>
            <div class="commitment-card card-10">
                <div class="badge-num">10</div>
                <div class="card-icon"><i class="fas fa-users-cog"></i></div>
                <h3 id="c10-t">People First Always</h3>
                <p id="c10-d">Every single decision will be for the welfare of the people.</p>
            </div>
        </div>
    </section>

    <section class="section-padding team-section" id="team">
        <h2 class="center-title" id="team-title">Our Executive Team</h2>
        <div class="team-grid">
            <div class="team-member">
                <div class="member-icon"><i class="fas fa-user-tie"></i></div>
                <h3>Mr. Jahid</h3>
                <p style="color:var(--primary-orange); font-weight:bold; margin-bottom:10px;" id="t1-p">National President & Founder</p>
                <p id="t1-d">Leading the nation towards a new era of development and honesty.</p>
            </div>
            <div class="team-member">
                <div class="member-icon"><i class="fas fa-users"></i></div>
                <h3 id="t2-t">Core Committee</h3>
                <p style="color:var(--primary-orange); font-weight:bold; margin-bottom:10px;" id="t2-p">Youth Leadership</p>
                <p id="t2-d">A team of energetic and young leaders from all across the nation.</p>
            </div>
            <div class="team-member">
                <div class="member-icon"><i class="fas fa-bullhorn"></i></div>
                <h3 id="t3-t">State Leaders</h3>
                <p style="color:var(--primary-orange); font-weight:bold; margin-bottom:10px;" id="t3-p">Regional Representatives</p>
                <p id="t3-d">Dedicated members raising public issues in every single state.</p>
            </div>
        </div>
    </section>

    <section class="section-padding news-section" id="news">
        <h2 class="center-title" id="news-title">Latest Updates & News</h2>
        <div class="news-container">
            <div class="news-item">
                <div class="news-date">May 20, 2026</div>
                <h3 style="margin: 5px 0; color: var(--dark-blue);" id="n1-t">LJP Core Committee Meeting Soon</h3>
                <p id="n1-d">A nation-wide membership drive campaign will be launched very soon.</p>
            </div>
            <div class="news-item">
                <div class="news-date">May 15, 2026</div>
                <h3 style="margin: 5px 0; color: var(--dark-blue);" id="n2-t">Founder Mr. Jahid's Message to Youth</h3>
                <p id="n2-d">Youth urged to join politics actively to take India to new heights.</p>
            </div>
        </div>
    </section>

    <section class="section-padding contact-section" id="contact">
        <h2 class="center-title" id="contact-title">Connect With Us</h2>
        <div class="contact-grid">
            <div class="contact-box">
                <i class="fas fa-map-marker-alt"></i>
                <h3 id="con-a">Office Address</h3>
                <p style="color: #aaa; margin-top:10px;">LJP Central Office, New Delhi, India</p>
            </div>
            <div class="contact-box">
                <i class="fas fa-envelope"></i>
                <h3 id="con-e">Email Us</h3>
                <p style="color: #aaa; margin-top:10px;">info@lokjantaparty.org</p>
            </div>
            <div class="contact-box">
                <i class="fas fa-phone-alt"></i>
                <h3 id="con-p">Call Support</h3>
                <p style="color: #aaa; margin-top:10px;">+91 98765 43210</p>
            </div>
        </div>
    </section>

    <footer>
        <div class="footer-left">
            <h2 id="foot-text">Together For A Stronger, Better India</h2>
        </div>
        <div class="footer-center">
            <a href="#contact" class="footer-btn blue" id="f-b1">Join LJP</a>
            <a href="#contact" class="footer-btn outline" id="f-b2">Donate Now</a>
        </div>
        <div class="footer-right">
            <span style="margin-right:10px; font-weight:bold;" id="foot-follow">Follow Us:</span>
            <div class="social-icons">
                <a href="#"><i class="fab fa-facebook-f"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
            </div>
        </div>
    </footer>

    <script>
        let currentLang = "EN";

        const langData = {
            EN: {
                navSlogan: "Power of People, Progress of Nation",
                home: "Home", about: "About Us", vision: "Our Vision", commitments: "Commitments", team: "Team", news: "News", contact: "Contact", join: "Join Us",
                heroSlogan: "Voice of People, Development of Nation", heroBtn: "Join The Change",
                aboutTitle: "About LJP", aboutDesc: "Lok Janta Party (LJP) is a people-first political movement dedicated to building a strong, transparent and developed India. Our power is the people, our mission is a better tomorrow.",
                visionTitle: "Our Vision", visionDesc: "A corruption-free India with equal opportunities, quality education, healthcare for all, and a strong economy driven by honesty, innovation and youth power.",
                founderSec: "Our Founder", founderPost: "Founder, Lok Janta Party", founderQuote: '"My goal is to strengthen the voice of the common citizen of the country. Lok Janta Party is not just a party, but the hope of every Indian who wants change and development. Together we will build a new and golden India."',
                commTitle: "Our 10 Commitments",
                c1t: "Zero Corruption", c1d: "Complete zero tolerance towards corruption with strict laws.",
                c2t: "Quality Education", c2d: "Free and high-quality education for every child.",
                c3t: "Healthcare For All", c3d: "Affordable and premium healthcare services for every citizen.",
                c4t: "Jobs For Youth", c4d: "Skill development and guaranteed employment opportunities.",
                c5t: "Strong Farmers", c5d: "Fair prices for crops and modern technical support for farmers.",
                c6t: "Infrastructure", c6d: "World-class roads, electricity, and clean water in every village and city.",
                c7t: "Women Safety", c7d: "Ensure absolute safety, respect, and equal opportunities for women.",
                c8t: "Green India", c8d: "Clean air, pure water, and dedication to environmental protection.",
                c9t: "Transparent Govt", c9d: "Transparent policies, citizen rights, and an accountable system.",
                c10t: "People First Always", c10d: "Every single decision will be for the welfare of the people.",
                teamTitle: "Our Executive Team", t1p: "National President & Founder", t1d: "Leading the nation towards a new era of development and honesty.",
                t2t: "Core Committee", t2p: "Youth Leadership", t2d: "A team of energetic and young leaders from all across the nation.",
                t3t: "State Leaders", t3p: "Regional Representatives", t3d: "Dedicated members raising public issues in every single state.",
                newsTitle: "Latest Updates & News", n1t: "LJP Core Committee Meeting Soon", n1d: "A nation-wide membership drive campaign will be launched very soon.",
                n2t: "Founder Mr. Jahid's Message to Youth", n2d: "Youth urged to join politics actively to take India to new heights.",
                conTitle: "Connect With Us", conA: "Office Address", conE: "Email Us", conP: "Call Support",
                footText: "Together For A Stronger, Better India", footFollow: "Follow Us:", btnText: "हिंदी"
            },
            HI: {
                navSlogan: "जनता की ताकत, देश की प्रगति",
                home: "होम", about: "हमारे बारे में", vision: "हमारा दृष्टिकोण", commitments: "प्रतिबद्धताएं", team: "टीम", news: "समाचार", contact: "संपर्क", join: "जुड़ें",
                heroSlogan: "जनता की आवाज, देश का विकास", heroBtn: "बदलाव से जुड़ें",
                aboutTitle: "एलजेपी के बारे में", aboutDesc: "लोक जनता पार्टी (LJP) एक जन-केंद्रित राजनीतिक आंदोलन है जो भारत को मजबूत, पारदर्शी और विकसित बनाने के लिए प्रतिबद्ध है। हमारी शक्ति जनता है, हमारा मिशन एक बेहतर कल है।",
                visionTitle: "हमारा दृष्टिकोण", visionDesc: "एक भ्रष्टाचार मुक्त भारत जहां सभी को समान अवसर मिले। हर बच्चे को गुणवत्तापूर्ण शिक्षा, हर नागरिक को बेहतर स्वास्थ्य सेवा और युवाओं को रोजगार देना हमारा संकल्प है।",
                founderSec: "हमारे संस्थापक", founderPost: "संस्थापक, लोक जनता पार्टी", founderQuote: '"मेरा मकसद देश के आम नागरिक की आवाज को मजबूत करना है। लोक जनता पार्टी सिर्फ एक दल नहीं, बल्कि हर उस हिंदुस्तानी की उम्मीद है जो बदलाव चाहता है। हम मिलकर एक स्वर्णिम भारत बनाएंगे।"',
                commTitle: "हमारी 10 प्रतिबद्धताएं",
                c1t: "शून्य भ्रष्टाचार", c1d: "कड़े कानूनों के साथ भ्रष्टाचार के खिलाफ पूर्ण रूप से जीरो टॉलरेंस।",
                c2t: "गुणवत्तापूर्ण शिक्षा", c2d: "हर बच्चे के लिए मुफ्त और उच्च स्तर की शिक्षा व्यवस्था।",
                c3t: "सभी के लिए स्वास्थ्य", c3d: "हर नागरिक के लिए सस्ती और बेहतर चिकित्सा सुविधाएं।",
                c4t: "युवाओं को रोजगार", c4d: "कौशल विकास और गारंटीकृत रोजगार के नए अवसर।",
                c5t: "मजबूत किसान", c5d: "किसानों को फसलों का सही दाम और आधुनिक तकनीकी सहायता।",
                c6t: "बुनियादी ढांचा", c6d: "हर गांव और शहर में विश्व स्तरीय सड़कें, बिजली और साफ पानी।",
                c7t: "महिला सुरक्षा", c7d: "महिलाओं की पूर्ण सुरक्षा, सम्मान और समान अधिकार सुनिश्चित करना।",
                c8t: "हरित भारत", c8d: "स्वच्छ हवा, शुद्ध पानी और पर्यावरण संरक्षण के प्रति प्रतिबद्धता।",
                c9t: "पारदर्शी सरकार", c9d: "पारदर्शी नीतियां, नागरिकों के अधिकार और जवाबदेह प्रणाली।",
                c10t: "जनता हमेशा सर्वोपरि", c10d: "हर एक फैसला पूरी तरह से जनता की भलाई और सहमति के लिए होगा।",
                teamTitle: "हमारी कार्यकारी टीम", t1p: "राष्ट्रीय अध्यक्ष एवं संस्थापक", t1d: "देश को विकास और ईमानदारी के एक नए युग की ओर ले जा रहे हैं।",
                t2t: "कोर कमेटी", t2p: "युवा नेतृत्व", t2d: "देश भर से जुड़े ऊर्जावान और युवा नेताओं की एक मजबूत टीम।",
                t3t: "राज्य के नेता", t3p: "क्षेत्रीय प्रतिनिधि", t3d: "हर राज्य में जनता की समस्याओं को प्रमुखता से उठाने वाले सदस्य।",
                newsTitle: "नवीनतम समाचार", n1t: "एलजेपी कोर कमेटी की बैठक जल्द", n1d: "देश भर में नए सदस्यों को जोड़ने के लिए जल्द ही एक बड़ा अभियान शुरू होगा।",
                n2t: "संस्थापक श्री जाहिद का युवाओं को संदेश", n2d: "भारत को नई ऊंचाइयों पर ले जाने के लिए युवाओं से राजनीति में आने का आह्वान।",
                conTitle: "हमसे जुड़ें", conA: "कार्यालय का पता", conE: "ईमेल करें", conP: "हेल्पलाइन नंबर",
                footText: "एक मजबूत और बेहतर भारत के लिए साथ आएं", footFollow: "फॉलो करें:", btnText: "English"
            }
        };

        function toggleLanguage() {
            currentLang = currentLang === "EN" ? "HI" : "EN";
            const data = langData[currentLang];

            // Update Navigation & Layout Text
            document.getElementById("nav-slogan").innerText = data.navSlogan;
            document.getElementById("nav-home").innerText = data.home;
            document.getElementById("nav-about").innerText = data.about;
            document.getElementById("nav-vision
