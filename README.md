<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>المحامية عمراوي خليدة | Cabinet d'Avocat Amraoui Khalida</title>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700;800&family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-gold: #D4AF37;
            --dark-gold: #B8941F;
            --navy: #0F172A;
            --light-navy: #1E293B;
            --cream: #FDFBF7;
            --text-dark: #1E293B;
            --text-light: #64748B;
            --white: #FFFFFF;
            --gradient-gold: linear-gradient(135deg, #D4AF37 0%, #F4D03F 50%, #D4AF37 100%);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Cairo', sans-serif;
            background-color: var(--cream);
            color: var(--text-dark);
            line-height: 1.8;
            overflow-x: hidden;
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(15, 23, 42, 0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            padding: 1rem 0;
            transition: all 0.3s ease;
            border-bottom: 2px solid var(--primary-gold);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary-gold);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            color: var(--white);
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            right: 0;
            width: 0;
            height: 2px;
            background: var(--primary-gold);
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .nav-links a:hover {
            color: var(--primary-gold);
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: var(--primary-gold);
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            margin-top: 80px;
            min-height: 90vh;
            background: linear-gradient(135deg, var(--navy) 0%, var(--light-navy) 100%);
            position: relative;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><text y=".9em" font-size="90" fill="rgba(212,175,55,0.03)">⚖</text></svg>');
            background-size: 200px;
            opacity: 0.5;
        }

        .hero-content {
            text-align: center;
            color: var(--white);
            position: relative;
            z-index: 2;
            padding: 2rem;
            max-width: 900px;
        }

        .scales-icon {
            font-size: 4rem;
            color: var(--primary-gold);
            margin-bottom: 1.5rem;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3.5rem;
            margin-bottom: 1rem;
            background: var(--gradient-gold);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero .subtitle {
            font-size: 1.5rem;
            color: var(--primary-gold);
            margin-bottom: 1rem;
            font-weight: 600;
        }

        .hero .description {
            font-size: 1.2rem;
            color: rgba(255,255,255,0.9);
            margin-bottom: 2rem;
            line-height: 1.8;
        }

        .credentials {
            display: flex;
            justify-content: center;
            gap: 2rem;
            flex-wrap: wrap;
            margin: 2rem 0;
        }

        .credential-item {
            background: rgba(212, 175, 55, 0.1);
            border: 1px solid var(--primary-gold);
            padding: 1rem 2rem;
            border-radius: 50px;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            color: var(--primary-gold);
            font-weight: 600;
        }

        .cta-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 2rem;
        }

        .btn {
            padding: 1rem 2.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }

        .btn-primary {
            background: var(--gradient-gold);
            color: var(--navy);
            box-shadow: 0 4px 15px rgba(212, 175, 55, 0.4);
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(212, 175, 55, 0.6);
        }

        .btn-secondary {
            background: transparent;
            color: var(--primary-gold);
            border: 2px solid var(--primary-gold);
        }

        .btn-secondary:hover {
            background: var(--primary-gold);
            color: var(--navy);
        }

        /* Section Styles */
        section {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
        }

        .section-title h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: var(--navy);
            margin-bottom: 1rem;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: var(--gradient-gold);
            margin: 0 auto;
            border-radius: 2px;
        }

        /* About Section */
        .about {
            background: var(--white);
            position: relative;
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        .about-text h3 {
            font-size: 2rem;
            color: var(--navy);
            margin-bottom: 1rem;
            font-family: 'Playfair Display', serif;
        }

        .about-text p {
            color: var(--text-light);
            margin-bottom: 1.5rem;
            font-size: 1.1rem;
        }

        .about-image {
            position: relative;
        }

        .about-image::before {
            content: '';
            position: absolute;
            top: -20px;
            right: -20px;
            width: 100%;
            height: 100%;
            border: 3px solid var(--primary-gold);
            border-radius: 10px;
            z-index: -1;
        }

        .about-image img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
            margin-top: 3rem;
        }

        .stat-item {
            text-align: center;
            padding: 2rem;
            background: var(--cream);
            border-radius: 10px;
            border-bottom: 3px solid var(--primary-gold);
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 800;
            color: var(--primary-gold);
            display: block;
        }

        .stat-label {
            color: var(--text-light);
            font-weight: 600;
        }

        /* Specialties Section */
        .specialties {
            background: var(--navy);
            color: var(--white);
            position: relative;
        }

        .specialties .section-title h2 {
            color: var(--white);
        }

        .specialties-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .specialty-card {
            background: rgba(255,255,255,0.05);
            border: 1px solid rgba(212, 175, 55, 0.3);
            padding: 2.5rem;
            border-radius: 15px;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .specialty-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--gradient-gold);
            opacity: 0;
            transition: opacity 0.3s ease;
            z-index: 0;
        }

        .specialty-card:hover::before {
            opacity: 0.1;
        }

        .specialty-card:hover {
            transform: translateY(-10px);
            border-color: var(--primary-gold);
            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.2);
        }

        .specialty-icon {
            font-size: 3rem;
            color: var(--primary-gold);
            margin-bottom: 1rem;
            position: relative;
            z-index: 1;
        }

        .specialty-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--primary-gold);
            position: relative;
            z-index: 1;
        }

        .specialty-card p {
            color: rgba(255,255,255,0.8);
            position: relative;
            z-index: 1;
        }

        /* Skills Section */
        .skills {
            background: var(--cream);
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .skill-item {
            background: var(--white);
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.05);
            text-align: center;
            transition: transform 0.3s ease;
            border-top: 4px solid var(--primary-gold);
        }

        .skill-item:hover {
            transform: translateY(-5px);
        }

        .skill-icon {
            width: 60px;
            height: 60px;
            background: var(--gradient-gold);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 1rem;
            color: var(--navy);
            font-size: 1.5rem;
        }

        .skill-item h3 {
            color: var(--navy);
            margin-bottom: 0.5rem;
        }

        .skill-item p {
            color: var(--text-light);
            font-size: 0.95rem;
        }

        /* Contact Section */
        .contact {
            background: linear-gradient(to bottom, var(--white), var(--cream));
        }

        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
        }

        .contact-info h3 {
            font-size: 2rem;
            color: var(--navy);
            margin-bottom: 2rem;
            font-family: 'Playfair Display', serif;
        }

        .contact-details {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        .contact-item {
            display: flex;
            align-items: flex-start;
            gap: 1rem;
            padding: 1.5rem;
            background: var(--white);
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: all 0.3s ease;
        }

        .contact-item:hover {
            transform: translateX(-10px);
            border-right: 4px solid var(--primary-gold);
        }

        .contact-icon {
            width: 50px;
            height: 50px;
            background: var(--gradient-gold);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--navy);
            font-size: 1.2rem;
            flex-shrink: 0;
        }

        .contact-text h4 {
            color: var(--navy);
            margin-bottom: 0.5rem;
        }

        .contact-text p, .contact-text a {
            color: var(--text-light);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .contact-text a:hover {
            color: var(--primary-gold);
        }

        .map-container {
            background: var(--navy);
            border-radius: 15px;
            padding: 2rem;
            position: relative;
            overflow: hidden;
        }

        .map-placeholder {
            width: 100%;
            height: 400px;
            background: linear-gradient(135deg, var(--light-navy) 0%, var(--navy) 100%);
            border-radius: 10px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: var(--primary-gold);
            border: 2px dashed var(--primary-gold);
        }

        .map-placeholder i {
            font-size: 4rem;
            margin-bottom: 1rem;
        }

        .address-text {
            margin-top: 1.5rem;
            color: var(--white);
            text-align: center;
            line-height: 1.8;
        }

        /* Footer */
        footer {
            background: var(--navy);
            color: var(--white);
            padding: 3rem 2rem 1rem;
            text-align: center;
            border-top: 3px solid var(--primary-gold);
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .footer-logo {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            color: var(--primary-gold);
            margin-bottom: 1rem;
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin: 2rem 0;
            flex-wrap: wrap;
        }

        .footer-links a {
            color: rgba(255,255,255,0.8);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-links a:hover {
            color: var(--primary-gold);
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin: 2rem 0;
        }

        .social-links a {
            width: 45px;
            height: 45px;
            background: rgba(212, 175, 55, 0.1);
            border: 1px solid var(--primary-gold);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--primary-gold);
            transition: all 0.3s ease;
        }

        .social-links a:hover {
            background: var(--primary-gold);
            color: var(--navy);
            transform: translateY(-3px);
        }

        .copyright {
            margin-top: 2rem;
            padding-top: 2rem;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: rgba(255,255,255,0.6);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                right: 0;
                background: var(--navy);
                flex-direction: column;
                padding: 2rem;
                gap: 1rem;
            }

            .nav-links.active {
                display: flex;
            }

            .mobile-menu-btn {
                display: block;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .about-content,
            .contact-container {
                grid-template-columns: 1fr;
            }

            .stats {
                grid-template-columns: 1fr;
            }

            .credentials {
                flex-direction: column;
                align-items: center;
            }
        }

        /* Scroll Animation */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Emergency Badge */
        .emergency-badge {
            position: fixed;
            bottom: 30px;
            left: 30px;
            background: #dc2626;
            color: white;
            padding: 1rem 1.5rem;
            border-radius: 50px;
            font-weight: 700;
            box-shadow: 0 4px 15px rgba(220, 38, 38, 0.4);
            z-index: 999;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            animation: pulse 2s infinite;
            cursor: pointer;
            text-decoration: none;
        }

        @keyframes pulse {
            0%, 100% { box-shadow: 0 0 0 0 rgba(220, 38, 38, 0.7); }
            70% { box-shadow: 0 0 0 15px rgba(220, 38, 38, 0); }
        }

        .emergency-badge:hover {
            background: #b91c1c;
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav id="navbar">
        <div class="nav-container">
            <a href="#" class="logo">
                <i class="fas fa-balance-scale"></i>
                <span>عمراوي خليدة</span>
            </a>
            <ul class="nav-links" id="navLinks">
                <li><a href="#accueil">الرئيسية</a></li>
                <li><a href="#apropos">من نحن</a></li>
                <li><a href="#specialites">التخصصات</a></li>
                <li><a href="#competences">المهارات</a></li>
                <li><a href="#contact">اتصل بنا</a></li>
            </ul>
            <button class="mobile-menu-btn" onclick="toggleMenu()">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="accueil">
        <div class="hero-content">
            <div class="scales-icon">
                <i class="fas fa-balance-scale"></i>
            </div>
            <h1>المحامية عمراوي خليدة</h1>
            <p class="subtitle">Cabinet d'Avocat Amraoui Khalida</p>
            <p class="description">
                محامية معتمدة لدى المحكمة العليا ومجلس الدولة<br>
                خبرة واسعة في القانون ا
