<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hailu Tilahun Kebede | Agricultural Scientist & Sustainable Development Specialist</title>
    <!-- Google Fonts & Font Awesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&family=Space+Grotesk:wght@500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            /* Dynamic Vibrant Color System */
            --bg-dark: #04130A;         /* Ultra Deep Obsidian Green */
            --bg-surface: #0A2315;      /* Rich Dark Emerald */
            --primary-green: #00E676;   /* Electric Neon Mint */
            --secondary-green: #10B981; /* Vibrant Emerald */
            --gold-accent: #F59E0B;     /* Warm Gold / Sun Accent */
            --gold-light: #FDE68A;      /* Light Gold Glow */
            --text-main: #0F172A;       /* Crisp Charcoal for Light BG */
            --text-muted: #475569;      /* Muted Slate */
            --light-bg: #F0FDF4;        /* Fresh Ice Green Tint */
            --white: #FFFFFF;
            
            --font-display: 'Space Grotesk', sans-serif;
            --font-body: 'Outfit', sans-serif;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: var(--font-body);
            color: var(--text-main);
            background-color: #FAFAFA;
            line-height: 1.6;
        }

        /* Typography */
        h1, h2, h3, h4, h5 {
            font-family: var(--font-display);
            color: var(--bg-dark);
            line-height: 1.2;
        }

        p {
            color: var(--text-muted);
            margin-bottom: 1.2rem;
            font-size: 1.05rem;
        }

        a {
            text-decoration: none;
            transition: all 0.3s ease;
        }

        /* Glassmorphism Header */
        header {
            position: sticky;
            top: 0;
            background: rgba(4, 19, 10, 0.9);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(0, 230, 118, 0.2);
            z-index: 1000;
        }

        .nav-container {
            max-width: 1280px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.1rem 2rem;
        }

        .logo {
            font-family: var(--font-display);
            font-size: 1.3rem;
            font-weight: 700;
            color: var(--white);
            letter-spacing: -0.5px;
        }

        .logo span {
            color: var(--primary-green);
        }

        .nav-links {
            display: flex;
            gap: 1.2rem;
            list-style: none;
        }

        .nav-links a {
            font-size: 0.9rem;
            font-weight: 500;
            color: #CBD5E1;
            padding: 0.4rem 0.6rem;
            border-radius: 6px;
        }

        .nav-links a:hover {
            color: var(--primary-green);
            background: rgba(255,255,255,0.05);
        }

        .btn-gradient {
            background: linear-gradient(135deg, var(--primary-green), var(--secondary-green));
            color: var(--bg-dark) !important;
            padding: 0.7rem 1.5rem;
            border-radius: 50px;
            font-weight: 700;
            font-size: 0.9rem;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            box-shadow: 0 4px 20px rgba(0, 230, 118, 0.35);
        }

        .btn-gradient:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 25px rgba(0, 230, 118, 0.5);
        }

        .btn-gold {
            background: linear-gradient(135deg, var(--gold-accent), #D97706);
            color: var(--white) !important;
            padding: 0.75rem 1.6rem;
            border-radius: 50px;
            font-weight: 700;
            box-shadow: 0 4px 15px rgba(245, 158, 11, 0.3);
        }

        .btn-gold:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(245, 158, 11, 0.4);
        }

        .btn-outline-light {
            border: 2px solid rgba(255,255,255,0.3);
            color: var(--white) !important;
            padding: 0.75rem 1.6rem;
            border-radius: 50px;
            font-weight: 600;
        }

        .btn-outline-light:hover {
            border-color: var(--primary-green);
            color: var(--primary-green) !important;
        }

        /* High Impact Hero */
        .hero {
            background: radial-gradient(circle at top right, #0A321C, var(--bg-dark));
            color: var(--white);
            padding: 7rem 2rem 6rem 2rem;
            position: relative;
            overflow: hidden;
        }

        .hero::after {
            content: '';
            position: absolute;
            bottom: 0; left: 0; right: 0;
            height: 80px;
            background: linear-gradient(to top, #FAFAFA, transparent);
        }

        .hero-container {
            max-width: 1100px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
            text-align: center;
        }

        .hero-badge {
            background: rgba(0, 230, 118, 0.1);
            border: 1px solid var(--primary-green);
            color: var(--primary-green);
            padding: 0.5rem 1.4rem;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            display: inline-block;
            margin-bottom: 1.8rem;
        }

        .hero h1 {
            color: var(--white);
            font-size: 3.2rem;
            margin-bottom: 1.2rem;
            letter-spacing: -1px;
        }

        .hero h1 span {
            background: linear-gradient(135deg, var(--primary-green), var(--gold-accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p.lead {
            color: #94A3B8;
            font-size: 1.2rem;
            max-width: 900px;
            margin: 0 auto 2.5rem auto;
        }

        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 1.2rem;
            flex-wrap: wrap;
        }

        /* Section Layouts */
        section {
            padding: 5.5rem 2rem;
        }

        .container {
            max-width: 1240px;
            margin: 0 auto;
        }

        .bg-mint-soft {
            background-color: var(--light-bg);
        }

        .bg-dark-emerald {
            background-color: var(--bg-surface);
            color: var(--white);
        }

        .bg-dark-emerald h2, .bg-dark-emerald h3, .bg-dark-emerald h4 {
            color: var(--white);
        }

        .section-title {
            text-align: center;
            max-width: 750px;
            margin: 0 auto 3.5rem auto;
        }

        .section-title h2 {
            font-size: 2.4rem;
            margin-bottom: 0.8rem;
            position: relative;
        }

        .section-title h2::after {
            content: '';
            display: block;
            width: 70px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary-green), var(--gold-accent));
            margin: 0.8rem auto 0 auto;
            border-radius: 2px;
        }

        /* Modern Card System */
        .grid-2 { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 2rem; }
        .grid-3 { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; }
        .grid-4 { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 1.5rem; }

        .card {
            background: var(--white);
            border-radius: 16px;
            padding: 2.2rem;
            border: 1px solid #E2E8F0;
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.05);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .card:hover {
            transform: translateY(-6px);
            box-shadow: 0 20px 35px -10px rgba(16, 185, 129, 0.15);
            border-color: var(--secondary-green);
        }

        .card-icon {
            width: 55px;
            height: 55px;
            background: var(--light-bg);
            color: var(--secondary-green);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            margin-bottom: 1.4rem;
        }

        /* Dark Card Variant */
        .card-dark {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 16px;
            padding: 2rem;
            color: var(--white);
        }

        .card-dark h3, .card-dark h4 { color: var(--white); }
        .card-dark p { color: #94A3B8; }

        /* At A Glance Grid */
        .glance-card {
            background: var(--white);
            border: 1px solid #E2E8F0;
            border-radius: 14px;
            padding: 1.8rem;
            text-align: center;
            transition: all 0.3s ease;
        }

        .glance-card:hover {
            border-color: var(--gold-accent);
            background: #FFFDF5;
        }

        .glance-card i {
            font-size: 2.2rem;
            background: linear-gradient(135deg, var(--secondary-green), var(--gold-accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 0.8rem;
        }

        /* Vibrant Pills */
        .pill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 1.2rem;
        }

        .pill {
            background: #E6F4EA;
            color: #065F46;
            padding: 0.4rem 0.9rem;
            border-radius: 50px;
            font-size: 0.82rem;
            font-weight: 600;
        }

        /* Process Bar */
        .process-flow {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: var(--bg-dark);
            padding: 2rem;
            border-radius: 16px;
            border: 1px solid rgba(0,230,118,0.2);
            color: var(--white);
            flex-wrap: wrap;
            gap: 1rem;
            margin-top: 2.5rem;
        }

        .process-step {
            display: flex;
            align-items: center;
            gap: 0.6rem;
            font-weight: 600;
            color: var(--white);
        }

        .process-step i {
            color: var(--primary-green);
        }

        /* Modern Styled Table */
        .table-responsive {
            overflow-x: auto;
            border-radius: 14px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
            border: 1px solid #E2E8F0;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: var(--white);
            text-align: left;
        }

        th {
            background: var(--bg-dark);
            color: var(--primary-green);
            padding: 1.2rem;
            font-family: var(--font-display);
            font-weight: 700;
        }

        td {
            padding: 1.1rem 1.2rem;
            border-bottom: 1px solid #E2E8F0;
            color: var(--text-muted);
        }

        tr:nth-child(even) {
            background-color: #F8FAFC;
        }

        /* Contact Box */
        .contact-card {
            background: linear-gradient(135deg, var(--bg-dark), var(--bg-surface));
            border-radius: 24px;
            padding: 4rem 2rem;
            color: var(--white);
            text-align: center;
            border: 1px solid rgba(0,230,118,0.3);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }

        .contact-card h2 { color: var(--white); margin-bottom: 1rem; }
        .contact-card p { color: #94A3B8; max-width: 650px; margin: 0 auto 2.5rem auto; }

        .contact-grid {
            display: flex;
            justify-content: center;
            gap: 2.5rem;
            flex-wrap: wrap;
            margin-bottom: 2rem;
        }

        .contact-method {
            display: flex;
            align-items: center;
            gap: 1rem;
            font-size: 1.1rem;
            background: rgba(255,255,255,0.05);
            padding: 0.8rem 1.5rem;
            border-radius: 50px;
            border: 1px solid rgba(255,255,255,0.1);
        }

        .contact-method i {
            color: var(--primary-green);
            font-size: 1.3rem;
        }

        .contact-method a { color: var(--white); font-weight: 600; }

        .social-bar {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
        }

        .social-bar a {
            width: 45px;
            height: 45px;
            background: rgba(255,255,255,0.08);
            color: var(--white);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }

        .social-bar a:hover {
            background: var(--primary-green);
            color: var(--bg-dark);
            transform: scale(1.1);
        }

        /* Footer */
        footer {
            background: var(--bg-dark);
            color: #64748B;
            padding: 2rem;
            text-align: center;
            font-size: 0.9rem;
            border-top: 1px solid rgba(255,255,255,0.05);
        }

        @media (max-width: 992px) {
            .nav-links { display: none; }
            .hero h1 { font-size: 2.2rem; }
            .process-flow { flex-direction: column; align-items: flex-start; }
        }
    </style>
</head>
<body>

    <!-- Header Navigation -->
    <header>
        <div class="nav-container">
            <a href="#home" class="logo">HAILU TILAHUN <span>KEBEDE</span></a>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#glance">At a Glance</a></li>
                <li><a href="#expertise">Expertise</a></li>
                <li><a href="#impact">Impact</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#partnerships">Partnerships</a></li>
                <li><a href="#research">Research</a></li>
                <li><a href="#consulting">Consulting</a></li>
            </ul>
            <a href="#contact" class="btn-gradient"><i class="fa-solid fa-paper-plane"></i> Let's Connect</a>
        </div>
    </header>

    <!-- Hero / Home -->
    <section class="hero" id="home">
        <div class="hero-container">
            <span class="hero-badge"><i class="fa-solid fa-bolt"></i> Agricultural Scientist & Sustainable Development Specialist</span>
            <h1>Connecting <span>Science, Nature, Finance & Markets</span> for Impact</h1>
            <p class="lead">Integrating Agricultural Science, Climate Action, Biodiversity Conservation, Carbon Credit Finance, and International Value Chains across Ethiopia and Africa.</p>
            <div class="hero-btns">
                <a href="#contact" class="btn-gold"><i class="fa-solid fa-handshake"></i> Partner With Me</a>
                <a href="#projects" class="btn-outline-light"><i class="fa-solid fa-compass"></i> Explore Projects</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <div class="container">
            <div class="grid-2" style="align-items: center;">
                <div>
                    <div style="text-align: left;" class="section-title">
                        <h2>From Science to Sustainable Impact</h2>
                    </div>
                    <p><strong>Hailu Tilahun Kebede</strong> is an Agricultural Scientist and Researcher with an MSc in Animal Breeding and Genetics and over eight years of experience in research, academic instruction, and community-based development.</p>
                    <p>His professional work has expanded into an integrated development approach connecting: <strong>Science | Agriculture | Climate | Nature | Finance | Markets | Communities</strong>.</p>
                    <p>This multidisciplinary perspective supports practical solutions addressing interconnected challenges including climate change, food security, biodiversity loss, livestock productivity, and access to international markets. He has also actively contributed to youth leadership and climate action through COP programs and UNFCCC processes.</p>
                </div>
                <div>
                    <div class="card" style="border-top: 5px solid var(--secondary-green); margin-bottom: 1.5rem;">
                        <div class="card-icon"><i class="fa-solid fa-bullseye"></i></div>
                        <h3>Mission</h3>
                        <p>To connect science, innovation, finance, partnerships, and communities to develop sustainable solutions that improve livelihoods, strengthen climate resilience, protect nature, and create long-term social value.</p>
                    </div>
                    <div class="card" style="border-top: 5px solid var(--gold-accent);">
                        <div class="card-icon" style="color: var(--gold-accent);"><i class="fa-solid fa-eye"></i></div>
                        <h3>Vision</h3>
                        <p>A future where science, sustainable finance, responsible investment, nature, agriculture, and international partnerships work together to build resilient communities and inclusive prosperity.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- At A Glance Section -->
    <section id="glance" class="bg-mint-soft">
        <div class="container">
            <div class="section-title">
                <h2>At a Glance</h2>
                <p>An integrated ecosystem connecting local potential with global opportunity.</p>
            </div>
            <div class="grid-3">
                <div class="glance-card">
                    <i class="fa-solid fa-dna"></i>
                    <h4>Science & Genetics</h4>
                    <p>Animal breeding, livestock genetics, genomics, GWAS, genetic resource conservation, and sustainable livestock systems.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-cloud-sun-rain"></i>
                    <h4>Climate & Carbon</h4>
                    <p>Carbon-credit development, climate finance, mitigation, adaptation, climate-smart agriculture, and climate resilience.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-tree"></i>
                    <h4>Nature & Biodiversity</h4>
                    <p>Biodiversity conservation, agroforestry, ecosystem restoration, regenerative agriculture, and nature-based solutions.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-wheat-awn"></i>
                    <h4>Agriculture & Food Systems</h4>
                    <p>Agroecology, food security, resilient food systems, value chains, community production, and sustainable livelihoods.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-mug-hot"></i>
                    <h4>Coffee & Global Markets</h4>
                    <p>Sustainable coffee production, value-chain development, export, international market linkage, and agricultural investment.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-users"></i>
                    <h4>Inclusive Development</h4>
                    <p>Youth empowerment, women's economic participation, community development, capacity building, and sustainable livelihoods.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Why Partner Section -->
    <section>
        <div class="container">
            <div class="section-title">
                <h2>Why Partner With Me?</h2>
                <p>Connecting Local Potential With Global Opportunity</p>
            </div>
            <div class="grid-3">
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-microscope"></i></div>
                    <h3>Scientific Expertise</h3>
                    <p>Foundation in animal science, breeding, genetics, genomics, agricultural research, and production systems.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-leaf"></i></div>
                    <h3>Climate & Sustainability</h3>
                    <p>Experience across climate mitigation, adaptation, climate-smart agriculture, biodiversity, carbon markets, and finance.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-people-group"></i></div>
                    <h3>Community Perspective</h3>
                    <p>Strong focus on smallholder farmers, youth, women, sustainable livelihoods, and inclusive development.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-diagram-project"></i></div>
                    <h3>Project Development</h3>
                    <p>Translating ambitious ideas into structured projects, partnerships, investment opportunities, and scalable initiatives.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-globe"></i></div>
                    <h3>International Orientation</h3>
                    <p>Dedicated to building relationships with international foundations, donors, NGOs, investors, and research institutions.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-chart-line"></i></div>
                    <h3>Measurable Impact</h3>
                    <p>Integrating science, investment, implementation, and rigorous monitoring to deliver verified long-term value.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Expertise Section -->
    <section id="expertise" class="bg-mint-soft">
        <div class="container">
            <div class="section-title">
                <h2>Areas of Expertise</h2>
                <p>Multidisciplinary capabilities built over 8+ years of scientific research and field leadership.</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <h4 style="color: var(--gold-accent); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">01</h4>
                    <h3>Livestock Science & Farming</h3>
                    <div class="pill-list">
                        <span class="pill">Livestock Management</span>
                        <span class="pill">Dairy, Beef, Sheep & Poultry</span>
                        <span class="pill">Animal Nutrition & Feed</span>
                        <span class="pill">Breeding & Herd Improvement</span>
                        <span class="pill">Pasture & Forage</span>
                        <span class="pill">Integrated Crop–Livestock</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--gold-accent); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">02</h4>
                    <h3>Climate, Carbon & Finance</h3>
                    <div class="pill-list">
                        <span class="pill">Carbon Credit Development</span>
                        <span class="pill">Climate Finance</span>
                        <span class="pill">Climate Mitigation & Adaptation</span>
                        <span class="pill">Climate-Smart Agriculture</span>
                        <span class="pill">Climate Resilience</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--gold-accent); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">03</h4>
                    <h3>Biodiversity & Restoration</h3>
                    <div class="pill-list">
                        <span class="pill">Biodiversity Conservation</span>
                        <span class="pill">Agroforestry</span>
                        <span class="pill">Ecosystem Restoration</span>
                        <span class="pill">Sustainable Land Management</span>
                        <span class="pill">Nature-Based Solutions</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--gold-accent); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">04</h4>
                    <h3>Agriculture & Food Systems</h3>
                    <div class="pill-list">
                        <span class="pill">Sustainable Agriculture</span>
                        <span class="pill">Agroecology</span>
                        <span class="pill">Climate-Smart Production</span>
                        <span class="pill">Food System Resilience</span>
                        <span class="pill">Agricultural Value Chains</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--gold-accent); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">05</h4>
                    <h3>Coffee & International Trade</h3>
                    <div class="pill-list">
                        <span class="pill">Sustainable Coffee Production</span>
                        <span class="pill">Coffee Export</span>
                        <span class="pill">International Market Linkage</span>
                        <span class="pill">Agricultural Investment</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--gold-accent); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">06</h4>
                    <h3>Community & Inclusive Growth</h3>
                    <div class="pill-list">
                        <span class="pill">Youth Empowerment</span>
                        <span class="pill">Women's Participation</span>
                        <span class="pill">Capacity Building</span>
                        <span class="pill">Green Livelihoods</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Strategic Projects -->
    <section id="projects">
        <div class="container">
            <div class="section-title">
                <h2>Strategic Projects</h2>
                <p>From Ideas to Investable and Fundable Initiatives</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <h3>01 — Climate & Carbon</h3>
                    <p>Carbon credit development, climate mitigation, adaptation, climate-smart agriculture, and nature-based climate finance solutions.</p>
                </div>
                <div class="card">
                    <h3>02 — Biodiversity & Restoration</h3>
                    <p>Forest and landscape restoration, ecosystem rehabilitation, agroforestry systems, and community-led conservation.</p>
                </div>
                <div class="card">
                    <h3>03 — Sustainable Livestock</h3>
                    <p>Animal breeding, genetic improvement, climate-resilient animal feed production, and smallholder livestock development.</p>
                </div>
                <div class="card">
                    <h3>04 — Coffee & Trade</h3>
                    <p>Quality improvement, value-chain development, sustainable export models, and direct international market linkage.</p>
                </div>
                <div class="card">
                    <h3>05 — Youth & Women</h3>
                    <p>Green jobs, skills development, youth entrepreneurship hubs, and women's economic participation in agriculture.</p>
                </div>
                <div class="card">
                    <h3>06 — Research & Innovation</h3>
                    <p>Joint agricultural research, animal genetics, climate adaptation studies, technology transfer, and evidence-based development.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Partnerships Section -->
    <section id="partnerships" class="bg-dark-emerald">
        <div class="container">
            <div class="section-title">
                <h2 style="color: var(--white);">Partnership Opportunities</h2>
                <p style="color: #94A3B8;">Building International Partnerships based on Trust, Evidence, Transparency, and Long-Term Impact.</p>
            </div>

            <!-- Target Partners Grid -->
            <div class="grid-4" style="margin-bottom: 3rem;">
                <div class="card-dark" style="text-align: center;">
                    <i class="fa-solid fa-building-columns" style="font-size: 2rem; color: var(--primary-green); margin-bottom: 0.8rem;"></i>
                    <h4>International Foundations</h4>
                </div>
                <div class="card-dark" style="text-align: center;">
                    <i class="fa-solid fa-hand-holding-dollar" style="font-size: 2rem; color: var(--primary-green); margin-bottom: 0.8rem;"></i>
                    <h4>Donors & Grant Makers</h4>
                </div>
                <div class="card-dark" style="text-align: center;">
                    <i class="fa-solid fa-globe" style="font-size: 2rem; color: var(--primary-green); margin-bottom: 0.8rem;"></i>
                    <h4>NGOs & Civil Society</h4>
                </div>
                <div class="card-dark" style="text-align: center;">
                    <i class="fa-solid fa-chart-pie" style="font-size: 2rem; color: var(--primary-green); margin-bottom: 0.8rem;"></i>
                    <h4>Impact Investors</h4>
                </div>
            </div>

            <!-- Table -->
            <div class="table-responsive" style="margin-bottom: 3rem;">
                <table>
                    <thead>
                        <tr>
                            <th>Opportunity Area</th>
                            <th>Focus Scope</th>
                            <th>Partnership Type</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td><strong>Climate & Carbon</strong></td>
                            <td>Carbon projects, adaptation, climate finance</td>
                            <td>Investment / Grant</td>
                        </tr>
                        <tr>
                            <td><strong>Biodiversity</strong></td>
                            <td>Conservation, ecosystem restoration, nature-based solutions</td>
                            <td>Grant / Climate Finance</td>
                        </tr>
                        <tr>
                            <td><strong>Sustainable Agriculture</strong></td>
                            <td>Smallholder farmers, livestock, food systems</td>
                            <td>Grant / Investment</td>
                        </tr>
                        <tr>
                            <td><strong>Coffee & Trade</strong></td>
                            <td>Production, value chain, export, market access</td>
                            <td>Investment / Trade</td>
                        </tr>
                        <tr>
                            <td><strong>Youth & Women</strong></td>
                            <td>Enterprise, green jobs, skills, livelihoods</td>
                            <td>Grant / NGO Partnership</td>
                        </tr>
                        <tr>
                            <td><strong>Research</strong></td>
                            <td>Genetics, agriculture, genomics, climate</td>
                            <td>Research Grant / University</td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <!-- Process Flow -->
            <div class="process-flow">
                <div class="process-step"><i class="fa-solid fa-lightbulb"></i> Concept</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--gold-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-pen-ruler"></i> Project Design</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--gold-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-handshake"></i> Partnership</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--gold-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-coins"></i> Financing</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--gold-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-gears"></i> Implementation</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--gold-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-chart-line"></i> Monitoring & Impact</div>
            </div>
        </div>
    </section>

    <!-- Research & Consulting -->
    <section id="research">
        <div class="container">
            <div class="section-title">
                <h2>Research & Consulting Services</h2>
                <p>Translating Scientific Research and Technical Writing into Practical Field Programs</p>
            </div>
            <div class="grid-2">
                <div class="card">
                    <h3>Research Focus</h3>
                    <p>Interdisciplinary studies across <strong>Animal Science, Genetics, Climate Resilience, Biodiversity, and Land Use</strong> to deliver evidence-based solutions for smallholder farmers and development partners.</p>
                    <div class="pill-list">
                        <span class="pill">Animal Breeding & GWAS</span>
                        <span class="pill">Livestock Genomics</span>
                        <span class="pill">Agroecology</span>
                        <span class="pill">Feed Production</span>
                    </div>
                </div>
                <div class="card" id="consulting">
                    <h3>Organizational Consulting</h3>
                    <p>Supporting NGOs, CSOs, and private enterprises in developing high-quality, fundable program documentation:</p>
                    <div class="pill-list">
                        <span class="pill">Grant Proposals</span>
                        <span class="pill">Concept Notes</span>
                        <span class="pill">Project Budgets</span>
                        <span class="pill">MEL Frameworks</span>
                        <span class="pill">Business Plans</span>
                        <span class="pill">Feasibility Studies</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <div class="contact-card">
                <h2>Let's Build Sustainable Solutions Together</h2>
                <p>If you are an international donor, foundation, impact investor, NGO, or research institution, I welcome the opportunity to explore partnership.</p>
                
                <div class="contact-grid">
                    <div class="contact-method">
                        <i class="fa-solid fa-envelope"></i>
                        <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a>
                    </div>
                    <div class="contact-method">
                        <i class="fa-brands fa-whatsapp"></i>
                        <a href="https://wa.me/251910204390">+251 910 204 390</a>
                    </div>
                </div>

                <div class="social-bar">
                    <a href="#" title="LinkedIn"><i class="fa-brands fa-linkedin-in"></i></a>
                    <a href="https://wa.me/251910204390" title="WhatsApp"><i class="fa-brands fa-whatsapp"></i></a>
                    <a href="#" title="Instagram"><i class="fa-brands fa-instagram"></i></a>
                    <a href="#" title="Telegram"><i class="fa-brands fa-telegram"></i></a>
                    <a href="#" title="Facebook"><i class="fa-brands fa-facebook-f"></i></a>
                    <a href="#" title="X"><i class="fa-brands fa-x-twitter"></i></a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2026 Hailu Tilahun Kebede. All Rights Reserved.</p>
        </div>
    </footer>

</body>
</html>
