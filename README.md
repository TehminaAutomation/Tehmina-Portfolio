<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Tehmina Automation | AI • Python • Creative Digital Experiences</title>

    <meta
        name="description"
        content="Tehmina Automation — AI, Python, Automation, Birthday, Anniversary, Wedding, Invitation and Custom Digital Experiences."
    >

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link
        href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Space+Grotesk:wght@400;500;600;700&display=swap"
        rel="stylesheet"
    >

    <style>
        /* =========================================================
           RESET
        ========================================================= */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: "Inter", sans-serif;
            background:
                radial-gradient(circle at 10% 10%, rgba(126, 87, 255, 0.16), transparent 30%),
                radial-gradient(circle at 90% 20%, rgba(0, 229, 255, 0.10), transparent 28%),
                radial-gradient(circle at 50% 90%, rgba(255, 0, 153, 0.10), transparent 30%),
                #060711;
            color: #f7f7ff;
            overflow-x: hidden;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        button {
            font-family: inherit;
        }

        ::selection {
            background: #9d5cff;
            color: white;
        }

        /* =========================================================
           BACKGROUND
        ========================================================= */

        .background-glow {
            position: fixed;
            inset: 0;
            pointer-events: none;
            z-index: -2;
            overflow: hidden;
        }

        .orb {
            position: absolute;
            border-radius: 50%;
            filter: blur(90px);
            opacity: 0.22;
        }

        .orb.one {
            width: 300px;
            height: 300px;
            background: #713cff;
            top: 5%;
            left: -100px;
        }

        .orb.two {
            width: 250px;
            height: 250px;
            background: #00d9ff;
            top: 35%;
            right: -80px;
        }

        .orb.three {
            width: 280px;
            height: 280px;
            background: #ff28b8;
            bottom: 0;
            left: 40%;
        }

        .grid-background {
            position: fixed;
            inset: 0;
            z-index: -3;
            opacity: 0.18;
            background-image:
                linear-gradient(rgba(255,255,255,0.035) 1px, transparent 1px),
                linear-gradient(90deg, rgba(255,255,255,0.035) 1px, transparent 1px);
            background-size: 55px 55px;
            mask-image: linear-gradient(to bottom, black, transparent 90%);
        }

        /* =========================================================
           NAVBAR
        ========================================================= */

        nav {
            position: fixed;
            top: 18px;
            left: 50%;
            transform: translateX(-50%);
            width: min(1150px, calc(100% - 30px));
            padding: 14px 20px;

            display: flex;
            align-items: center;
            justify-content: space-between;

            background: rgba(10, 11, 25, 0.72);
            border: 1px solid rgba(255,255,255,0.10);
            backdrop-filter: blur(18px);
            -webkit-backdrop-filter: blur(18px);

            border-radius: 20px;
            z-index: 1000;

            box-shadow:
                0 15px 50px rgba(0,0,0,0.30),
                inset 0 1px rgba(255,255,255,0.05);
        }

        .logo {
            font-family: "Space Grotesk", sans-serif;
            font-size: 20px;
            font-weight: 700;
            letter-spacing: -0.5px;
        }

        .logo span {
            background: linear-gradient(90deg, #b779ff, #00e5ff, #ff59c7);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .nav-links {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        .nav-links a {
            color: #b9bacb;
            font-size: 14px;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: white;
        }

        .nav-button {
            padding: 10px 16px;
            border-radius: 12px;
            font-size: 13px;
            font-weight: 700;

            background: linear-gradient(135deg, #814cff, #bd4cff);
            box-shadow: 0 0 25px rgba(139, 76, 255, 0.30);
        }

        .menu-btn {
            display: none;
            background: transparent;
            border: 0;
            color: white;
            font-size: 25px;
            cursor: pointer;
        }

        /* =========================================================
           GENERAL
        ========================================================= */

        section {
            width: min(1150px, calc(100% - 30px));
            margin: auto;
            padding: 110px 0;
        }

        .section-label {
            color: #a879ff;
            font-size: 12px;
            font-weight: 800;
            letter-spacing: 3px;
            text-transform: uppercase;
            margin-bottom: 12px;
        }

        .section-title {
            font-family: "Space Grotesk", sans-serif;
            font-size: clamp(34px, 5vw, 58px);
            line-height: 1;
            letter-spacing: -2px;
            margin-bottom: 18px;
        }

        .section-description {
            max-width: 650px;
            color: #9fa0b2;
            line-height: 1.8;
            font-size: 15px;
        }

        /* =========================================================
           HERO
        ========================================================= */

        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding-top: 140px;
            position: relative;
        }

        .hero-content {
            max-width: 820px;
        }

        .status {
            display: inline-flex;
            align-items: center;
            gap: 9px;

            padding: 9px 14px;
            border-radius: 100px;

            background: rgba(255,255,255,0.045);
            border: 1px solid rgba(255,255,255,0.09);

            color: #c9cad8;
            font-size: 12px;
            margin-bottom: 28px;
        }

        .status-dot {
            width: 8px;
            height: 8px;
            background: #54f2a5;
            border-radius: 50%;
            box-shadow: 0 0 15px #54f2a5;
        }

        .hero h1 {
            font-family: "Space Grotesk", sans-serif;
            font-size: clamp(50px, 8vw, 100px);
            line-height: 0.92;
            letter-spacing: -5px;
            margin-bottom: 28px;
        }

        .gradient-text {
            background: linear-gradient(
                100deg,
                #ffffff 0%,
                #b87cff 35%,
                #00e5ff 68%,
                #ff5fc7 100%
            );
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero-subtitle {
            font-size: clamp(18px, 2vw, 23px);
            color: #d4d4df;
            max-width: 760px;
            line-height: 1.6;
            margin-bottom: 18px;
        }

        .hero-description {
            max-width: 690px;
            color: #9294a7;
            line-height: 1.8;
            font-size: 15px;
            margin-bottom: 32px;
        }

        .hero-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 13px;
        }

        .primary-btn,
        .secondary-btn {
            padding: 14px 21px;
            border-radius: 13px;
            font-size: 14px;
            font-weight: 700;
            transition: 0.3s;
        }

        .primary-btn {
            background: linear-gradient(135deg, #8654ff, #c84cff);
            box-shadow: 0 12px 35px rgba(135, 75, 255, 0.25);
        }

        .secondary-btn {
            border: 1px solid rgba(255,255,255,0.12);
            background: rgba(255,255,255,0.035);
            color: #d8d8e4;
        }

        .primary-btn:hover,
        .secondary-btn:hover {
            transform: translateY(-3px);
        }

        .hero-mini {
            display: flex;
            gap: 35px;
            margin-top: 55px;
            flex-wrap: wrap;
        }

        .mini-item strong {
            display: block;
            font-family: "Space Grotesk", sans-serif;
            font-size: 25px;
        }

        .mini-item span {
            color: #858799;
            font-size: 12px;
        }

        /* =========================================================
           ABOUT
        ========================================================= */

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1.3fr;
            gap: 45px;
            align-items: center;
        }

        .about-card {
            min-height: 330px;
            border-radius: 28px;
            padding: 30px;

            background:
                linear-gradient(
                    145deg,
                    rgba(135, 82, 255, 0.15),
                    rgba(0, 229, 255, 0.04)
                );

            border: 1px solid rgba(255,255,255,0.09);
            position: relative;
            overflow: hidden;
        }

        .about-card::before {
            content: "";
            position: absolute;
            width: 170px;
            height: 170px;
            border-radius: 50%;
            background: #a158ff;
            filter: blur(80px);
            top: -60px;
            right: -40px;
            opacity: 0.3;
        }

        .about-symbol {
            width: 70px;
            height: 70px;
            display: grid;
            place-items: center;
            border-radius: 20px;

            font-size: 30px;

            background: rgba(255,255,255,0.07);
            border: 1px solid rgba(255,255,255,0.09);

            margin-bottom: 50px;
        }

        .about-card h3 {
            font-family: "Space Grotesk", sans-serif;
            font-size: 25px;
            margin-bottom: 10px;
        }

        .about-card p {
            color: #9698aa;
            line-height: 1.7;
            font-size: 14px;
        }

        .about-text p {
            color: #9fa0b1;
            line-height: 1.9;
            margin-bottom: 18px;
            font-size: 15px;
        }

        /* =========================================================
           SERVICES
        ========================================================= */

        .services-grid {
            margin-top: 50px;
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 16px;
        }

        .service-card {
            padding: 25px;
            min-height: 200px;

            background: rgba(255,255,255,0.035);
            border: 1px solid rgba(255,255,255,0.08);
            border-radius: 22px;

            transition: 0.35s;
            position: relative;
            overflow: hidden;
        }

        .service-card:hover {
            transform: translateY(-7px);
            border-color: rgba(170,110,255,0.35);
            background: rgba(255,255,255,0.055);
        }

        .service-icon {
            font-size: 28px;
            margin-bottom: 30px;
        }

        .service-card h3 {
            font-family: "Space Grotesk", sans-serif;
            font-size: 18px;
            margin-bottom: 10px;
        }

        .service-card p {
            color: #898b9d;
            font-size: 13px;
            line-height: 1.65;
        }

        /* =========================================================
           SKILLS
        ========================================================= */

        .skills-container {
            margin-top: 45px;
            display: flex;
            flex-wrap: wrap;
            gap: 11px;
        }

        .skill {
            padding: 11px 16px;
            border-radius: 100px;
            background: rgba(255,255,255,0.045);
            border: 1px solid rgba(255,255,255,0.09);
            color: #c7c8d5;
            font-size: 13px;
            transition: 0.3s;
        }

        .skill:hover {
            border-color: #9a62ff;
            color: white;
            transform: translateY(-2px);
        }

        /* =========================================================
           PROJECTS
        ========================================================= */

        .projects-grid {
            margin-top: 50px;
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }

        .project-card {
            border-radius: 25px;
            overflow: hidden;

            background: rgba(255,255,255,0.035);
            border: 1px solid rgba(255,255,255,0.09);

            transition: 0.35s;
        }

        .project-card:hover {
            transform: translateY(-7px);
            border-color: rgba(165,100,255,0.4);
        }

        .project-visual {
            height: 220px;
            position: relative;
            overflow: hidden;

            display: flex;
            align-items: center;
            justify-content: center;

            background:
                radial-gradient(circle at 20% 30%, rgba(157,83,255,0.35), transparent 35%),
                radial-gradient(circle at 80% 70%, rgba(0,225,255,0.22), transparent 35%),
                #0c0e1d;
        }

        .project-visual::after {
            content: "";
            position: absolute;
            inset: 20px;
            border: 1px solid rgba(255,255,255,0.07);
            border-radius: 18px;
        }

        .project-big-icon {
            font-size: 70px;
            filter: drop-shadow(0 0 25px rgba(173,105,255,0.5));
        }

        .project-content {
            padding: 25px;
        }

        .project-tag {
            color: #a879ff;
            font-size: 11px;
            letter-spacing: 2px;
            text-transform: uppercase;
            font-weight: 800;
            margin-bottom: 10px;
        }

        .project-content h3 {
            font-family: "Space Grotesk", sans-serif;
            font-size: 23px;
            margin-bottom: 10px;
        }

        .project-content p {
            color: #9092a4;
            font-size: 13px;
            line-height: 1.7;
            margin-bottom: 18px;
        }

        .project-links {
            display: flex;
            gap: 10px;
        }

        .project-link {
            padding: 9px 13px;
            border-radius: 10px;
            background: rgba(255,255,255,0.06);
            border: 1px solid rgba(255,255,255,0.08);
            font-size: 12px;
            color: #c9cad6;
        }

        /* =========================================================
           CREATIVE EXPERIENCES
        ========================================================= */

        .creative-section {
            position: relative;
        }

        .creative-box {
            margin-top: 50px;
            padding: 45px;
            border-radius: 30px;

            background:
                linear-gradient(
                    120deg,
                    rgba(131,73,255,0.15),
                    rgba(0,215,255,0.08),
                    rgba(255,66,182,0.10)
                );

            border: 1px solid rgba(255,255,255,0.10);
            position: relative;
            overflow: hidden;
        }

        .creative-box::before {
            content: "";
            position: absolute;
            width: 300px;
            height: 300px;
            border-radius: 50%;
            background: #8248ff;
            filter: blur(100px);
            opacity: 0.12;
            top: -180px;
            left: 35%;
        }

        .creative-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 14px;
            position: relative;
        }

        .creative-item {
            padding: 25px;
            border-radius: 18px;
            background: rgba(5,6,15,0.40);
            border: 1px solid rgba(255,255,255,0.08);
        }

        .creative-item span {
            font-size: 30px;
            display: block;
            margin-bottom: 18px;
        }

        .creative-item h3 {
            font-family: "Space Grotesk", sans-serif;
            margin-bottom: 7px;
        }

        .creative-item p {
            color: #9193a4;
            font-size: 12px;
            line-height: 1.6;
        }

        /* =========================================================
           JOURNEY
        ========================================================= */

        .timeline {
            margin-top: 50px;
            border-left: 1px solid rgba(255,255,255,0.10);
            padding-left: 30px;
        }

        .timeline-item {
            position: relative;
            margin-bottom: 35px;
        }

        .timeline-item::before {
            content: "";
            position: absolute;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background: #9d5cff;
            box-shadow: 0 0 20px #9d5cff;
            left: -36px;
            top: 7px;
        }

        .timeline-date {
            color: #9d6dff;
            font-size: 11px;
            font-weight: 800;
            letter-spacing: 2px;
            margin-bottom: 7px;
        }

        .timeline-item h3 {
            font-family: "Space Grotesk", sans-serif;
            font-size: 20px;
            margin-bottom: 6px;
        }

        .timeline-item p {
            color: #8d8f9f;
            line-height: 1.7;
            font-size: 13px;
            max-width: 700px;
        }

        /* =========================================================
           CTA
        ========================================================= */

        .cta {
            text-align: center;
            padding: 100px 30px;
            border-radius: 35px;

            background:
                radial-gradient(circle at 50% 0%, rgba(142,77,255,0.22), transparent 45%),
                rgba(255,255,255,0.025);

            border: 1px solid rgba(255,255,255,0.09);
        }

        .cta h2 {
            font-family: "Space Grotesk", sans-serif;
            font-size: clamp(35px, 5vw, 60px);
            letter-spacing: -2px;
            margin-bottom: 18px;
        }

        .cta p {
            max-width: 600px;
            margin: 0 auto 30px;
            color: #9698aa;
            line-height: 1.8;
        }

        /* =========================================================
           FOOTER
        ========================================================= */

        footer {
            width: min(1150px, calc(100% - 30px));
            margin: auto;
            padding: 35px 0 45px;

            display: flex;
            align-items: center;
            justify-content: space-between;

            border-top: 1px solid rgba(255,255,255,0.07);
            color: #77798a;
            font-size: 12px;
        }

        .footer-brand {
            color: #bdbeca;
            font-weight: 700;
        }

        .footer-links {
            display: flex;
            gap: 20px;
        }

        .footer-links a:hover {
            color: white;
        }

        /* =========================================================
           RESPONSIVE
        ========================================================= */

        @media (max-width: 900px) {

            .nav-links {
                display: none;
                position: absolute;
                top: 70px;
                left: 0;
                width: 100%;

                flex-direction: column;
                gap: 0;

                background: rgba(10,11,25,0.95);
                border: 1px solid rgba(255,255,255,0.08);
                border-radius: 18px;
                padding: 10px;
            }

            .nav-links.active {
                display: flex;
            }

            .nav-links a {
                display: block;
                padding: 13px;
            }

            .nav-button {
                display: none;
            }

            .menu-btn {
                display: block;
            }

            .about-grid {
                grid-template-columns: 1fr;
            }

            .services-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .creative-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 650px) {

            section {
                padding: 80px 0;
            }

            .hero h1 {
                letter-spacing: -3px;
            }

            .projects-grid {
                grid-template-columns: 1fr;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }

            .creative-box {
                padding: 25px;
            }

            footer {
                flex-direction: column;
                gap: 18px;
                text-align: center;
            }

            .hero-mini {
                gap: 22px;
            }
        }
    </style>
</head>

<body>

    <!-- =========================================================
         BACKGROUND
    ========================================================== -->

    <div class="grid-background"></div>

    <div class="background-glow">
        <div class="orb one"></div>
        <div class="orb two"></div>
        <div class="orb three"></div>
    </div>


    <!-- =========================================================
         NAVIGATION
    ========================================================== -->

    <nav>

        <a href="#home" class="logo">
            Tehmina<span>Automation</span>
        </a>

        <ul class="nav-links" id="navLinks">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#services">What I Create</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#creative">Creative</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>

        <a
            href="https://github.com/TehminaAutomation"
            target="_blank"
            class="nav-button"
        >
            GitHub ↗
        </a>

        <button class="menu-btn" onclick="toggleMenu()" aria-label="Open menu">
            ☰
        </button>

    </nav>


    <!-- =========================================================
         HERO
    ========================================================== -->

    <main>

        <section class="hero" id="home">

            <div class="hero-content">

                <div class="status">
                    <span class="status-dot"></span>
                    Building ideas into digital experiences
                </div>

                <h1>
                    <span class="gradient-text">
                        Ideas.
                    </span>
                    <br>
                    Experiences.
                    <br>
                    <span class="gradient-text">
                        Created.
                    </span>
                </h1>

                <p class="hero-subtitle">
                    AI Developer • Python • Automation • Creative Digital Experiences
                </p>

                <p class="hero-description">
                    I create intelligent applications, useful automations,
                    interactive experiences and personalized digital projects —
                    from AI-powered solutions to beautiful birthday,
                    anniversary, wedding and wishes experiences.
                </p>

                <div class="hero-buttons">

                    <a href="#projects" class="primary-btn">
                        Explore My Work →
                    </a>

                    <a href="#contact" class="secondary-btn">
                        Create Something Custom
                    </a>

                </div>

                <div class="hero-mini">

                    <div class="mini-item">
                        <strong>AI</strong>
                        <span>Intelligent Apps</span>
                    </div>

                    <div class="mini-item">
                        <strong>Python</strong>
                        <span>Powerful Solutions</span>
                    </div>

                    <div class="mini-item">
                        <strong>∞</strong>
                        <span>Creative Possibilities</span>
                    </div>

                </div>

            </div>

        </section>


        <!-- =====================================================
             ABOUT
        ====================================================== -->

        <section id="about">

            <div class="about-grid">

                <div class="about-card">

                    <div class="about-symbol">
                        ✦
                    </div>

                    <h3>
                        More Than A Portfolio
                    </h3>

                    <p>
                        A creative space where technology,
                        automation and imagination come together.
                    </p>

                </div>

                <div class="about-text">

                    <div class="section-label">
                        01 — About
                    </div>

                    <h2 class="section-title">
                        I build things
                        <span class="gradient-text">people remember.</span>
                    </h2>

                    <p>
                        I'm Tehmina, focused on Python, AI and intelligent
                        digital solutions. I enjoy turning an idea into
                        something functional, useful and visually engaging.
                    </p>

                    <p>
                        My work isn't limited to one category. I create
                        AI/ML applications and automation tools, while also
                        building personalized digital experiences for
                        birthdays, anniversaries, weddings, invitations,
                        wishes and special occasions.
                    </p>

                    <p>
                        Every project starts with an idea — and the goal is
                        to turn that idea into something unique.
                    </p>

                </div>

            </div>

        </section>


        <!-- =====================================================
             SERVICES
        ====================================================== -->

        <section id="services">

            <div class="section-label">
                02 — What I Create
            </div>

            <h2 class="section-title">
                One idea.
                <span class="gradient-text">Many possibilities.</span>
            </h2>

            <p class="section-description">
                Custom digital solutions designed around the idea,
                purpose and experience you want to create.
            </p>


            <div class="services-grid">

                <div class="service-card">

                    <div class="service-icon">🤖</div>

                    <h3>AI Applications</h3>

                    <p>
                        AI/ML applications, intelligent tools,
                        NLP, computer vision and practical AI solutions.
                    </p>

                </div>


                <div class="service-card">

                    <div class="service-icon">🐍</div>

                    <h3>Python Projects</h3>

                    <p>
                        Custom Python applications, utilities,
                        dashboards and project solutions.
                    </p>

                </div>


                <div class="service-card">

                    <div class="service-icon">⚙️</div>

                    <h3>Automation</h3>

                    <p>
                        Automating repetitive tasks and building
                        useful digital workflows.
                    </p>

                </div>


                <div class="service-card">

                    <div class="service-icon">🎂</div>

                    <h3>Birthday Experiences</h3>

                    <p>
                        Interactive birthday surprises with wishes,
                        animations, music, memories and special effects.
                    </p>

                </div>


                <div class="service-card">

                    <div class="service-icon">💍</div>

                    <h3>Anniversary</h3>

                    <p>
                        Personalized anniversary experiences with
                        photos, memories, messages and animations.
                    </p>

                </div>


                <div class="service-card">

                    <div class="service-icon">💌</div>

                    <h3>Invitations</h3>

                    <p>
                        Digital wedding, engagement, birthday and
                        event invitation experiences.
                    </p>

                </div>


                <div class="service-card">

                    <div class="service-icon">✨</div>

                    <h3>Custom Wishes</h3>

                    <p>
                        Personalized greeting pages, wishes,
                        surprise messages and interactive moments.
                    </p>

                </div>


                <div class="service-card">

                    <div class="service-icon">🎨</div>

                    <h3>Creative Projects</h3>

                    <p>
                        Unique digital concepts created around
                        your imagination and requirements.
                    </p>

                </div>

            </div>

        </section>


        <!-- =====================================================
             SKILLS
        ====================================================== -->

        <section id="skills">

            <div class="section-label">
                03 — Toolkit
            </div>

            <h2 class="section-title">
                What I <span class="gradient-text">work with.</span>
            </h2>

            <p class="section-description">
                Technologies and areas I use to build practical
                AI-powered and custom digital solutions.
            </p>

            <div class="skills-container">

                <span class="skill">Python</span>
                <span class="skill">Artificial Intelligence</span>
                <span class="skill">Machine Learning</span>
                <span class="skill">Generative AI</span>
                <span class="skill">LLMs</span>
                <span class="skill">RAG</span>
                <span class="skill">NLP</span>
                <span class="skill">Computer Vision</span>
                <span class="skill">Streamlit</span>
                <span class="skill">FastAPI</span>
                <span class="skill">Automation</span>
                <span class="skill">Creative Applications</span>

            </div>

        </section>


        <!-- =====================================================
             PROJECTS
        ====================================================== -->

        <section id="projects">

            <div class="section-label">
                04 — Selected Work
            </div>

            <h2 class="section-title">
                Projects built with
                <span class="gradient-text">purpose.</span>
            </h2>

            <p class="section-description">
                A selection of AI, Python, automation and creative
                applications.
            </p>


            <div class="projects-grid">


                <!-- PROJECT 1 -->

                <article class="project-card">

                    <div class="project-visual">
                        <div class="project-big-icon">
                            🎙️
                        </div>
                    </div>

                    <div class="project-content">

                        <div class="project-tag">
                            AI / Machine Learning
                        </div>

                        <h3>
                            SpeechSense AI
                        </h3>

                        <p>
                            Speech Emotion Recognition application using
                            audio features and machine learning to identify
                            emotions from speech.
                        </p>

                        <div class="project-links">

                            <a
                                href="https://github.com/Tehmina124/Emotion-Recognition-from-Speech"
                                target="_blank"
                                class="project-link"
                            >
                                GitHub ↗
                            </a>

                        </div>

                    </div>

                </article>


                <!-- PROJECT 2 -->

                <article class="project-card">

                    <div class="project-visual">
                        <div class="project-big-icon">
                            📊
                        </div>
                    </div>

                    <div class="project-content">

                        <div class="project-tag">
                            AI / Analytics
                        </div>

                        <h3>
                            AI Business Analytics Assistant
                        </h3>

                        <p>
                            An interactive AI-powered analytics application
                            for exploring business data and generating
                            useful insights.
                        </p>

                        <div class="project-links">

                            <a
                                href="https://ai-business-analytics-assistant-2toqqp4ypuwiavq2v23gk5.streamlit.app/"
                                target="_blank"
                                class="project-link"
                            >
                                Live Demo ↗
                            </a>

                        </div>

                    </div>

                </article>


                <!-- PROJECT 3 -->

                <article class="project-card">

                    <div class="project-visual">
                        <div class="project-big-icon">
                            📚
                        </div>
                    </div>

                    <div class="project-content">

                        <div class="project-tag">
                            Generative AI / RAG
                        </div>

                        <h3>
                            Document Q&A with Citations
                        </h3>

                        <p>
                            A document question-answering system using
                            semantic search and retrieval techniques to
                            provide answers with supporting citations.
                        </p>

                        <div class="project-links">

                            <a
                                href="https://github.com/TehminaAutomation"
                                target="_blank"
                                class="project-link"
                            >
                                More Projects ↗
                            </a>

                        </div>

                    </div>

                </article>


                <!-- PROJECT 4 -->

                <article class="project-card">

                    <div class="project-visual">
                        <div class="project-big-icon">
                            👁️
                        </div>
                    </div>

                    <div class="project-content">

                        <div class="project-tag">
                            Computer Vision
                        </div>

                        <h3>
                            AI Object Detection & Tracking
                        </h3>

                        <p>
                            Computer vision application using object
                            detection and tracking techniques for
                            real-time visual analysis.
                        </p>

                        <div class="project-links">

                            <a
                                href="https://github.com/TehminaAutomation"
                                target="_blank"
                                class="project-link"
                            >
                                GitHub ↗
                            </a>

                        </div>

                    </div>

                </article>


                <!-- PROJECT 5 -->

                <article class="project-card">

                    <div class="project-visual">
                        <div class="project-big-icon">
                            🌐
                        </div>
                    </div>

                    <div class="project-content">

                        <div class="project-tag">
                            Python / Creative AI
                        </div>

                        <h3>
                            Language Translation Tool
                        </h3>

                        <p>
                            A multilingual translation application with
                            text translation and speech-related features.
                        </p>

                        <div class="project-links">

                            <a
                                href="https://codealphalanguagetranslationtool-kjfgtohte9xx9to5bj9gst.streamlit.app/"
                                target="_blank"
                                class="project-link"
                            >
                                Live Demo ↗
                            </a>

                        </div>

                    </div>

                </article>


                <!-- PROJECT 6 -->

                <article class="project-card">

                    <div class="project-visual">
                        <div class="project-big-icon">
                            ⚡
                        </div>
                    </div>

                    <div class="project-content">

                        <div class="project-tag">
                            Custom / Automation
                        </div>

                        <h3>
                            Personalized Digital Experiences
                        </h3>

                        <p>
                            Custom interactive experiences for birthdays,
                            anniversaries, wishes, invitations and special
                            moments.
                        </p>

                        <div class="project-links">

                            <a
                                href="#creative"
                                class="project-link"
                            >
                                Explore ↓
                            </a>

                        </div>

                    </div>

                </article>

            </div>

        </section>


        <!-- =====================================================
             CREATIVE EXPERIENCES
        ====================================================== -->

        <section id="creative" class="creative-section">

            <div class="section-label">
                05 — Creative Experiences
            </div>

            <h2 class="section-title">
                Special moments,
                <span class="gradient-text">digitally created.</span>
            </h2>

            <p class="section-description">
                Technology doesn't always have to feel technical.
                Sometimes it can be personal, emotional and fun.
            </p>


            <div class="creative-box">

                <div class="creative-grid">

                    <div class="creative-item">

                        <span>🎂</span>

                        <h3>Birthday Surprise</h3>

                        <p>
                            Animated birthday experiences with balloons,
                            cake, wishes, photos, music and surprise moments.
                        </p>

                    </div>


                    <div class="creative-item">

                        <span>💍</span>

                        <h3>Anniversary Story</h3>

                        <p>
                            Turn memories and messages into a beautiful
                            interactive anniversary experience.
                        </p>

                    </div>


                    <div class="creative-item">

                        <span>💌</span>

                        <h3>Digital Invitation</h3>

                        <p>
                            Personalized invitation experiences for
                            weddings, birthdays, engagements and events.
                        </p>

                    </div>


                    <div class="creative-item">

                        <span>💖</span>

                        <h3>Love & Wishes</h3>

                        <p>
                            Custom pages designed around personal messages,
                            memories and meaningful moments.
                        </p>

                    </div>


                    <div class="creative-item">

                        <span>🎁</span>

                        <h3>Digital Surprise</h3>

                        <p>
                            Interactive surprises created for someone
                            special, with animations and storytelling.
                        </p>

                    </div>


                    <div class="creative-item">

                        <span>✨</span>

                        <h3>Your Idea</h3>

                        <p>
                            Have a different idea? Let's turn your concept
                            into a custom digital experience.
                        </p>

                    </div>

                </div>

            </div>

        </section>


        <!-- =====================================================
             JOURNEY
        ====================================================== -->

        <section id="journey">

            <div class="section-label">
                06 — Journey
            </div>

            <h2 class="section-title">
                Learning,
                <span class="gradient-text">building & creating.</span>
            </h2>

            <div class="timeline">

                <div class="timeline-item">

                    <div class="timeline-date">
                        AI / ML
                    </div>

                    <h3>
                        Building Intelligent Applications
                    </h3>

                    <p>
                        Working with Python, machine learning,
                        NLP, computer vision and AI application development.
                    </p>

                </div>


                <div class="timeline-item">

                    <div class="timeline-date">
                        GENERATIVE AI
                    </div>

                    <h3>
                        Exploring LLMs & RAG
                    </h3>

                    <p>
                        Exploring modern AI application patterns including
                        LLMs, retrieval augmented generation and intelligent
                        document experiences.
                    </p>

                </div>


                <div class="timeline-item">

                    <div class="timeline-date">
                        AUTOMATION
                    </div>

                    <h3>
                        Turning Repetitive Work Into Workflows
                    </h3>

                    <p>
                        Creating practical Python-based automations and
                        utility applications.
                    </p>

                </div>


                <div class="timeline-item">

                    <div class="timeline-date">
                        CREATIVE DIGITAL WORK
                    </div>

                    <h3>
                        Making Technology Personal
                    </h3>

                    <p>
                        Creating interactive birthday, anniversary,
                        invitation, wishes and personalized experiences.
                    </p>

                </div>

            </div>

        </section>


        <!-- =====================================================
             CONTACT
        ====================================================== -->

        <section id="contact">

            <div class="cta">

                <div class="section-label">
                    07 — Let's Create
                </div>

                <h2>
                    Have an idea?
                    <br>
                    <span class="gradient-text">
                        Let's build it.
                    </span>
                </h2>

                <p>
                    Whether it's an AI application, Python project,
                    automation, birthday surprise, anniversary experience,
                    invitation or something completely different —
                    your idea can become a digital experience.
                </p>

                <div class="hero-buttons" style="justify-content:center;">

                    <a
                        href="https://github.com/TehminaAutomation"
                        target="_blank"
                        class="primary-btn"
                    >
                        Visit My GitHub ↗
                    </a>

                    <a
                        href="https://www.linkedin.com/in/tehmina-anwar-77b8a841/"
                        target="_blank"
                        class="secondary-btn"
                    >
                        LinkedIn ↗
                    </a>

                </div>

            </div>

        </section>

    </main>


    <!-- =========================================================
         FOOTER
    ========================================================== -->

    <footer>

        <div>
            © 2026
            <span class="footer-brand">
                Tehmina Automation
            </span>
            — Built with ideas & creativity.
        </div>

        <div class="footer-links">

            <a
                href="https://github.com/TehminaAutomation"
                target="_blank"
            >
                GitHub
            </a>

            <a
                href="https://www.linkedin.com/in/tehmina-anwar-77b8a841/"
                target="_blank"
            >
                LinkedIn
            </a>

        </div>

    </footer>


    <!-- =========================================================
         JAVASCRIPT
    ========================================================== -->

    <script>

        function toggleMenu() {
            const nav = document.getElementById("navLinks");
            nav.classList.toggle("active");
        }


        // Close mobile menu after clicking a link

        document.querySelectorAll(".nav-links a").forEach(link => {

            link.addEventListener("click", () => {

                document
                    .getElementById("navLinks")
                    .classList.remove("active");

            });

        });


        // Simple reveal animation

        const revealElements = document.querySelectorAll(
            ".service-card, .project-card, .creative-item, .timeline-item, .about-card"
        );

        const observer = new IntersectionObserver(

            entries => {

                entries.forEach(entry => {

                    if (entry.isIntersecting) {

                        entry.target.style.opacity = "1";
                        entry.target.style.transform = "translateY(0)";

                    }

                });

            },

            {
                threshold: 0.12
            }

        );


        revealElements.forEach(element => {

            element.style.opacity = "0";
            element.style.transform = "translateY(25px)";
            element.style.transition = "opacity 0.7s ease, transform 0.7s ease";

            observer.observe(element);

        });

    </script>

</body>
</html>
