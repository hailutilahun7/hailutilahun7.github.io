<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hailu Tilahun Kebede | Agricultural Scientist & Sustainable Development Specialist</title>
    <!-- Google Fonts & Font Awesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Outfit:wght@500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            /* Color System */
            --bg-main: #EDF7F1;           /* Light Mint Surface */
            --bg-card: #FFFFFF;           /* Pure White Card */
            --green-bold: #16A34A;       /* Vibrant Green */
            --green-header: #2D6A4F;      /* Rich Medium Green Header */
            --green-dark: #065F46;        /* Deep Bold Forest Green */
            --green-subtle: #D1FAE5;      /* Soft Green Tint */
            --green-border: #86EFAC;      /* Crisp Light-Green Border */
            --accent-gold: #D97706;       /* Warm Earth Gold Accent */
            --accent-gold-light: #FEF3C7; /* Warm Gold Tint */
            
            /* Footer & Contact Section High-Visibility Colors */
            --footer-bg: #0B2B1A;         /* Ultra Deep High-Contrast Green */
            --footer-text: #FFFFFF;       /* Crisp White Header/Body Text */
            --footer-accent: #86EFAC;     /* Bright Mint Highlight */
            
            --text-dark: #0F172A;         /* Dark Body Text */
            --text-muted: #334155;        /* Bolder Muted Text */
            
            --font-display: 'Outfit', sans-serif;
            --font-body: 'Plus Jakarta Sans', sans-serif;
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
            color: var(--text-dark);
            background-color: var(--bg-main);
            line-height: 1.65;
        }

        /* Typography */
        h1, h2, h3, h4, h5 {
            font-family: var(--font-display);
            color: var(--green-dark);
            line-height: 1.25;
            font-weight: 700;
        }

        p {
            color: var(--text-muted);
            margin-bottom: 1.2rem;
            font-size: 1.02rem;
        }

        a {
            text-decoration: none;
            transition: all 0.3s ease;
        }

        /* COLORED HEADER NAVIGATION */
        header {
            position: sticky;
            top: 0;
            background-color: var(--green-header);
            border-bottom: 3px solid var(--green-bold);
            z-index: 1000;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.15);
        }

        .nav-container {
            max-width: 1280px;
            margin: 0 auto;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 1.1rem 2rem;
        }

        .nav-links {
            display: flex;
            gap: 1.2rem;
            list-style: none;
            flex-wrap: wrap;
            justify-content: center;
        }

        .nav-links a {
            font-size: 0.92rem;
            font-weight: 700;
            color: #FFFFFF;
            padding: 0.4rem 0.8rem;
            border-radius: 6px;
        }

        .nav-links a:hover {
            color: var(--green-header);
            background: #FFFFFF;
        }

        .btn-gold {
            background-color: var(--accent-gold);
            color: #FFFFFF !important;
            padding: 0.75rem 1.6rem;
            border-radius: 50px;
            font-weight: 700;
            box-shadow: 0 4px 15px rgba(217, 119, 6, 0.3);
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }

        .btn-gold:hover {
            background-color: #B45309;
            transform: translateY(-2px);
        }

        .btn-outline-green {
            border: 2px solid var(--green-bold);
            color: var(--green-bold) !important;
            padding: 0.75rem 1.6rem;
            border-radius: 50px;
            font-weight: 700;
            background: #FFFFFF;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }

        .btn-outline-green:hover {
            background-color: var(--green-bold);
            color: #FFFFFF !important;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--green-subtle) 0%, #DCFCE7 50%, #BBF7D0 100%);
            color: var(--green-dark);
            padding: 6rem 2rem 5rem 2rem;
            position: relative;
            text-align: center;
            border-bottom: 2px solid var(--green-border);
        }

        .hero-container {
            max-width: 1100px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
        }

        .hero-badge {
            background: #FFFFFF;
            border: 1.5px solid var(--green-bold);
            color: var(--green-bold);
            padding: 0.45rem 1.3rem;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 1px;
            display: inline-block;
            margin-bottom: 1.5rem;
            box-shadow: 0 2px 8px rgba(0,0,0,0.06);
        }

        .hero h1 {
            color: var(--green-dark);
            font-size: 3.1rem;
            margin-bottom: 1.2rem;
            font-weight: 800;
        }

        .hero h1 span {
            color: var(--green-bold);
        }

        .hero p.lead {
            color: var(--text-muted);
            font-size: 1.18rem;
            max-width: 900px;
            margin: 0 auto 2.2rem auto;
            font-weight: 500;
        }

        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 1.2rem;
            flex-wrap: wrap;
        }

        /* Profile Image Styles */
        .profile-img-container {
            text-align: center;
            margin-bottom: 2rem;
        }

        .profile-img {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid var(--green-bold);
            box-shadow: 0 10px 25px rgba(22, 163, 74, 0.25);
        }

        /* Layout Structure */
        section {
            padding: 5rem 2rem;
        }

        .container {
            max-width: 1240px;
            margin: 0 auto;
        }

        .bg-white {
            background-color: #FFFFFF;
        }

        .section-title {
            text-align: center;
            max-width: 800px;
            margin: 0 auto 3.5rem auto;
        }

        .section-title h2 {
            font-size: 2.4rem;
            margin-bottom: 0.8rem;
            position: relative;
            font-weight: 800;
        }

        .section-title h2::after {
            content: '';
            display: block;
            width: 70px;
            height: 4px;
            background: var(--green-bold);
            margin: 0.8rem auto 0 auto;
            border-radius: 2px;
        }

        /* Grids & Cards */
        .grid-2 { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 2.5rem; }
        .grid-3 { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; }
        .grid-4 { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 1.5rem; }

        .card {
            background: var(--bg-card);
            border-radius: 14px;
            padding: 2.2rem;
            border: 1.5px solid var(--green-border);
            box-shadow: 0 4px 15px rgba(6, 95, 70, 0.04);
            transition: all 0.3s ease;
            position: relative;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 25px rgba(22, 163, 74, 0.15);
            border-color: var(--green-bold);
        }

        .card-icon {
            width: 52px;
            height: 52px;
            background: var(--green-subtle);
            color: var(--green-bold);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            margin-bottom: 1.2rem;
            border: 1px solid var(--green-border);
        }

        /* At A Glance Strip */
        .glance-card {
            background: var(--bg-card);
            border: 1.5px solid var(--green-border);
            border-radius: 12px;
            padding: 1.6rem;
            text-align: center;
            transition: all 0.3s ease;
        }

        .glance-card:hover {
            border-color: var(--green-bold);
            background: #FAFFFC;
        }

        .glance-card i {
            font-size: 2.3rem;
            color: var(--green-bold);
            margin-bottom: 0.8rem;
        }

        /* Pills & Badges */
        .pill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 1rem;
        }

        .pill {
            background: var(--green-subtle);
            color: var(--green-dark);
            padding: 0.4rem 0.9rem;
            border-radius: 50px;
            font-size: 0.83rem;
            font-weight: 700;
            border: 1px solid var(--green-border);
        }

        .green-bullets {
            list-style: none;
        }

        .green-bullets li {
            position: relative;
            padding-left: 1.8rem;
            margin-bottom: 0.6rem;
            color: var(--text-muted);
            font-weight: 500;
        }

        .green-bullets li::before {
            content: "\f00c";
            font-family: "Font Awesome 6 Free";
            font-weight: 900;
            position: absolute;
            left: 0;
            top: 2px;
            color: var(--green-bold);
            font-size: 0.85rem;
        }

        /* Process Bar */
        .process-flow {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: var(--green-dark);
            padding: 1.8rem;
            border-radius: 14px;
            color: #FFFFFF;
            flex-wrap: wrap;
            gap: 1rem;
            margin-top: 2.5rem;
        }

        .process-step {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-weight: 700;
            color: var(--green-subtle);
        }

        .process-step i {
            color: #86EFAC;
        }

        /* Styled Table */
        .table-responsive {
            overflow-x: auto;
            border-radius: 12px;
            border: 1.5px solid var(--green-border);
            box-shadow: 0 4px 15px rgba(0,0,0,0.03);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: var(--bg-card);
            text-align: left;
        }

        th {
            background-color: var(--green-bold);
            color: #FFFFFF;
            padding: 1.2rem;
            font-weight: 700;
        }

        td {
            padding: 1.1rem 1.2rem;
            border-bottom: 1px solid var(--green-subtle);
            color: var(--text-muted);
            font-weight: 500;
        }

        tr:nth-child(even) {
            background-color: var(--green-subtle);
        }

        /* HIGH-VISIBILITY CONTACT BOX */
        .contact-card {
            background: var(--footer-bg);
            border-radius: 20px;
            padding: 3.5rem 2rem;
            color: var(--footer-text);
            text-align: center;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3);
            border: 2px solid var(--green-bold);
        }

        .contact-card h2 { 
            color: #FFFFFF; 
            margin-bottom: 1rem; 
            font-size: 2.3rem; 
        }

        .contact-card p { 
            color: #E2E8F0; 
            max-width: 650px; 
            margin: 0 auto 2.5rem auto; 
            font-size: 1.1rem; 
            font-weight: 500; 
        }

        .contact-grid {
            display: flex;
            justify-content: center;
            gap: 2rem;
            flex-wrap: wrap;
            margin-bottom: 2.5rem;
        }

        .contact-method {
            display: flex;
            align-items: center;
            gap: 1rem;
            font-size: 1.15rem;
            background: rgba(255, 255, 255, 0.08);
            padding: 1rem 1.8rem;
            border-radius: 50px;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .contact-method i {
            width: 45px;
            height: 45px;
            background: var(--green-bold);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #FFFFFF;
            font-size: 1.2rem;
        }

        .contact-method a { 
            color: #FFFFFF !important; 
            font-weight: 700; 
        }

        .contact-method a:hover {
            color: var(--footer-accent) !important;
        }

        .social-bar {
            display: flex;
            justify-content: center;
            gap: 1.2rem;
            margin-top: 1.5rem;
        }

        .social-bar a {
            width: 46px;
            height: 46px;
            background: rgba(255,255,255,0.12);
            color: #FFFFFF;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.3s ease;
        }

        .social-bar a:hover {
            background: var(--footer-accent);
            color: var(--footer-bg);
            transform: translateY(-3px);
        }

        /* HIGH-VISIBILITY FOOTER */
        footer {
            background: #051A0F;
            color: #E2E8F0;
            padding: 2.5rem 2rem;
            text-align: center;
            font-size: 1rem;
            font-weight: 600;
            border-top: 3px solid var(--green-bold);
        }

        @media (max-width: 992px) {
            .hero h1 { font-size: 2.2rem; }
            .process-flow { flex-direction: column; align-items: flex-start; }
            .nav-links { gap: 0.6rem; }
            .nav-links a { font-size: 0.82rem; padding: 0.3rem 0.5rem; }
        }
    </style>
</head>
<body>

    <!-- Header Navigation -->
    <header>
        <div class="nav-container">
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#glance">At a Glance</a></li>
                <li><a href="#expertise">Expertise</a></li>
                <li><a href="#impact">Impact</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#publications">Publications</a></li>
                <li><a href="#partnerships">Partnerships</a></li>
                <li><a href="#research">Research</a></li>
                <li><a href="#consulting">Consulting</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-container">
            <span class="hero-badge"><i class="fa-solid fa-seedling"></i> Agricultural Scientist | Researcher | Climate & Sustainable Development Specialist</span>
            <h1>Connecting <span>Science, Nature, Finance & Markets</span> for Sustainable Development</h1>
            <p class="lead">I work at the intersection of Agricultural Science, Sustainable Agriculture, Climate Action, Biodiversity Conservation, Carbon Finance, Sustainable Development, and International Markets.</p>
            <div class="hero-btns">
                <a href="HAILU_RESUME_2026.pdf" download class="btn-gold"><i class="fa-solid fa-file-arrow-down"></i> Download CV (PDF)</a>
                <a href="#projects" class="btn-outline-green"><i class="fa-solid fa-folder-open"></i> Explore Projects</a>
            </div>
        </div>
    </section>

    <!-- About Section with Image -->
    <section id="about" class="bg-white">
        <div class="container">
            <div class="grid-2" style="align-items: center;">
                <div>
                    <!-- Integrated Profile Image -->
                    <div class="profile-img-container">
                        <img src="photo_2025-11-24_14-14-04.jpg" alt="Hailu Tilahun Kebede" class="profile-img">
                    </div>

                    <div style="text-align: left;" class="section-title">
                        <h2>From Science to Sustainable Impact</h2>
                    </div>
                    <p><strong>Hailu Tilahun Kebede</strong> is an Agricultural Scientist and Researcher with an MSc in Animal Breeding and Genetics and over eight years of experience in research, academic instruction, and community-based development[cite: 2]. His professional work has expanded from agricultural science and research into an integrated development approach connecting: <strong>Science | Agriculture | Climate | Nature | Finance | Markets | Communities</strong>[cite: 2].</p>
                    <p>This multidisciplinary perspective supports the development of solutions addressing interconnected challenges including climate change, food security, biodiversity loss, agricultural productivity, sustainable livelihoods, rural development, and access to international markets[cite: 2].</p>
                    <p>The focus is not only on developing ideas, but on connecting knowledge, resources, partnerships, and implementation to create practical and scalable impact[cite: 2]. I have also participated in youth leadership and climate action on COP programs and UNFCCC processes, serving as an Official Delegate at the UNECA Regional Forum on Sustainable Development and African Union Delegate to the G20 Social Summit[cite: 2].</p>
                    <p>I seek to build long-term partnerships with international investors, foundations, donors, grant-making organizations, NGOs, development agencies, research institutions, governments, and private-sector partners committed to measurable and sustainable impact[cite: 2].</p>
                </div>
                <div>
                    <div class="card" style="border-left: 5px solid var(--green-bold); margin-bottom: 1.5rem;">
                        <div class="card-icon"><i class="fa-solid fa-bullseye"></i></div>
                        <h3>Mission</h3>
                        <p>To connect science, innovation, finance, partnerships, and communities to develop sustainable solutions that improve livelihoods, strengthen climate resilience, protect nature, and create long-term economic and social value[cite: 2].</p>
                    </div>
                    <div class="card" style="border-left: 5px solid var(--accent-gold);">
                        <div class="card-icon" style="color: var(--accent-gold); background: var(--accent-gold-light);"><i class="fa-solid fa-eye"></i></div>
                        <h3>Vision</h3>
                        <p>A future where science, sustainable finance, responsible investment, nature, agriculture, and international partnerships work together to create resilient communities and inclusive prosperity[cite: 2].</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- At A Glance Section -->
    <section id="glance">
        <div class="container">
            <div class="section-title">
                <h2>At a Glance</h2>
                <p>Connecting Local Potential With Global Opportunity</p>
            </div>
            <div class="grid-3">
                <div class="glance-card">
                    <i class="fa-solid fa-dna"></i>
                    <h4>Science & Genetics</h4>
                    <p>Animal breeding, livestock genetics, genomics, GWAS, genetic resource conservation, and sustainable livestock systems[cite: 2].</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-cloud-sun-rain"></i>
                    <h4>Climate & Carbon</h4>
                    <p>Carbon-credit development, climate finance, climate mitigation and adaptation, climate-smart agriculture, and climate resilience[cite: 2].</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-tree"></i>
                    <h4>Nature & Biodiversity</h4>
                    <p>Biodiversity conservation, agroforestry, ecosystem restoration, regenerative agriculture, nature-based solutions, organic farming, aquaculture, and apiculture[cite: 2].</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-wheat-awn"></i>
                    <h4>Agriculture & Food Systems</h4>
                    <p>Sustainable agriculture, agroecology, food security, resilient food systems, agricultural value chains, community-based production, humanitarian food resilience, entrepreneurship, self-sufficiency, and sustainable livelihoods[cite: 2].</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-mug-hot"></i>
                    <h4>Coffee & Global Markets</h4>
                    <p>Sustainable coffee production, value-chain development, export, international market linkage, and agricultural investment.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-people-hold"></i>
                    <h4>Inclusive Development</h4>
                    <p>Youth empowerment, women's economic participation, community development, capacity building, and sustainable livelihoods[cite: 2].</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Why Partner Section -->
    <section class="bg-white">
        <div class="container">
            <div class="section-title">
                <h2>Why Partner With Me?</h2>
                <p>Connecting Local Potential With Global Opportunity</p>
            </div>
            <p style="text-align: center; max-width: 850px; margin: 0 auto 3rem auto;">Many high-impact development opportunities require more than funding[cite: 2]. They require technical knowledge, local understanding, trusted relationships, project development capacity, implementation partnerships, and access to wider networks[cite: 2].</p>
            
            <div class="grid-3">
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-microscope"></i></div>
                    <h3>Scientific & Technical Expertise</h3>
                    <p>A foundation in animal science, breeding, genetics, genomics (GWAS), biometry, SAS/R data analytics, and sustainable production systems[cite: 2].</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-temperature-arrow-up"></i></div>
                    <h3>Climate & Sustainability Knowledge</h3>
                    <p>Experience across climate mitigation, adaptation, climate-smart agriculture, biodiversity, agroforestry, ecosystem restoration, carbon markets, and climate finance[cite: 2].</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-users"></i></div>
                    <h3>Community Perspective</h3>
                    <p>A strong focus on smallholder farmers, communities, youth, women, gender inclusiveness, sustainable livelihoods, and inclusive development[cite: 2].</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-diagram-project"></i></div>
                    <h3>Project Development</h3>
                    <p>Proven track record translating ideas into structured projects, partnerships, MER frameworks, investment opportunities, and scalable initiatives[cite: 2].</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-globe"></i></div>
                    <h3>International Partnership Orientation</h3>
                    <p>Commitment to building relationships with international foundations, donors, NGOs, investors, research institutions, companies, and development agencies[cite: 2].</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-chart-line"></i></div>
                    <h3>Measurable Impact</h3>
                    <p>My approach integrates rigorous scientific research, investment, field implementation, and verified impact reporting[cite: 2].</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Expertise Section -->
    <section id="expertise">
        <div class="container">
            <div class="section-title">
                <h2>Areas of Expertise</h2>
                <p>Multidisciplinary capability built over 8+ years of scientific research, academic instruction, and community development[cite: 2].</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <h4 style="color: var(--accent-gold); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">01</h4>
                    <h3>Livestock Science & Practical Farming</h3>
                    <div class="pill-list">
                        <span class="pill">Livestock Farm Management</span>
                        <span class="pill">Dairy, Beef, Sheep, Goat & Poultry Farming</span>
                        <span class="pill">Animal Nutrition & Feed Production</span>
                        <span class="pill">Pasture & Forage Development</span>
                        <span class="pill">Breeding & Herd Improvement</span>
                        <span class="pill">Climate-Smart & Sustainable Farming</span>
                        <span class="pill">Livestock Health & Farm Hygiene</span>
                        <span class="pill">Integrated Crop–Livestock Farming</span>
                        <span class="pill">Agribusiness & Farm Entrepreneurship</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--accent-gold); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">02</h4>
                    <h3>Climate, Carbon & Sustainable Finance</h3>
                    <div class="pill-list">
                        <span class="pill">Carbon Credit Development</span>
                        <span class="pill">Climate Finance</span>
                        <span class="pill">Climate Mitigation & Adaptation</span>
                        <span class="pill">Climate-Smart Agriculture</span>
                        <span class="pill">Climate-Resilient Development</span>
                        <span class="pill">Sustainable Investment</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--accent-gold); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">03</h4>
                    <h3>Biodiversity, Nature & Restoration</h3>
                    <div class="pill-list">
                        <span class="pill">Biodiversity Conservation</span>
                        <span class="pill">Agroforestry</span>
                        <span class="pill">Ecosystem Restoration</span>
                        <span class="pill">Sustainable Land Management</span>
                        <span class="pill">Regenerative Agriculture</span>
                        <span class="pill">Nature-Based Solutions</span>
                        <span class="pill">Aquaculture & Apiculture</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--accent-gold); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">04</h4>
                    <h3>Agriculture & Food Systems</h3>
                    <div class="pill-list">
                        <span class="pill">Sustainable Agriculture</span>
                        <span class="pill">Agroecology</span>
                        <span class="pill">Climate-Smart Production</span>
                        <span class="pill">Sustainable Food Systems</span>
                        <span class="pill">Community-Based Agriculture</span>
                        <span class="pill">Agricultural Value Chains</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--accent-gold); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">05</h4>
                    <h3>Coffee & International Trade</h3>
                    <div class="pill-list">
                        <span class="pill">Sustainable Coffee Production</span>
                        <span class="pill">Coffee Export</span>
                        <span class="pill">International Market Linkage</span>
                        <span class="pill">Agricultural Investment</span>
                        <span class="pill">International Trade Partnerships</span>
                    </div>
                </div>

                <div class="card">
                    <h4 style="color: var(--accent-gold); font-size: 0.9rem; font-family: var(--font-display); font-weight: 700;">06</h4>
                    <h3>Community & Inclusive Development</h3>
                    <div class="pill-list">
                        <span class="pill">Youth Empowerment</span>
                        <span class="pill">Women's Economic Participation</span>
                        <span class="pill">Community Capacity Building</span>
                        <span class="pill">Green Livelihoods</span>
                        <span class="pill">Gender Inclusiveness</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Impact Areas -->
    <section id="impact" class="bg-white">
        <div class="container">
            <div class="section-title">
                <h2>Areas of Impact</h2>
                <p>Turning Knowledge into Action</p>
            </div>
            <div class="grid-2">
                <div class="card">
                    <h3>Climate Action & Resilience</h3>
                    <p>Developing approaches that connect climate action, adaptation, resilience, and sustainable finance to support communities and productive systems facing climate-related challenges[cite: 2].</p>
                </div>
                <div class="card">
                    <h3>Carbon Markets & Climate Finance</h3>
                    <p>Exploring opportunities to connect verified environmental outcomes with responsible climate finance and carbon-market mechanisms, while ensuring community and ecosystem benefits[cite: 2].</p>
                </div>
                <div class="card">
                    <h3>Biodiversity & Nature</h3>
                    <p>Supporting biodiversity conservation, agroforestry, ecosystem restoration, sustainable land management, and nature-based solutions[cite: 2].</p>
                </div>
                <div class="card">
                    <h3>Sustainable Agriculture</h3>
                    <p>Advancing agricultural systems that improve productivity, climate resilience, food security, environmental sustainability, and livelihoods[cite: 2].</p>
                </div>
                <div class="card">
                    <h3>Livestock & Genetic Resources</h3>
                    <p>Applying science and innovation to strengthen livestock productivity, dairy farming, honeybee production, poultry farming, genetic resources, sustainable production, and resilience[cite: 2].</p>
                </div>
                <div class="card">
                    <h3>Coffee & International Markets</h3>
                    <p>Connecting Ethiopia's agricultural potential with international buyers, investors, markets, value-chain development, and sustainable trade opportunities.</p>
                </div>
                <div class="card">
                    <h3>Youth & Women's Economic Empowerment</h3>
                    <p>Supporting approaches that create meaningful opportunities for youth and women through skills, enterprise, agriculture, innovation, employment, and sustainable livelihoods[cite: 2].</p>
                </div>
                <div class="card">
                    <h3>Community-Led Development</h3>
                    <p>Promoting development approaches that place communities at the center of planning, implementation, ownership, and long-term sustainability[cite: 2].</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Peer-Reviewed Scientific Publications Section -->
    <section id="publications">
        <div class="container">
            <div class="section-title">
                <h2>Peer-Reviewed Publications</h2>
                <p>Evidence-Based Academic Research Contributions</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-book"></i></div>
                    <h4>Journal of Applied Animal Research (2023)</h4>
                    <p><strong>"Assessment on rearing and husbandry practices of indigenous goats in North Shewa Zone, Amhara Region, Ethiopia"</strong></p>
                    <p style="font-size: 0.88rem; color: var(--green-dark);">Publisher: Taylor & Francis Group | DOI: 10.1080/09712119.2023.2185625[cite: 2]</p>
                </div>

                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-book"></i></div>
                    <h4>Journal of Applied Animal Research (2023)</h4>
                    <p><strong>"Phenotypic characterization of indigenous sheep breeds in the Jimma Zone, Oromia, Ethiopia"</strong></p>
                    <p style="font-size: 0.88rem; color: var(--green-dark);">Authors: Yaregal Derbie & Hailu Tilahun | Publisher: Taylor & Francis Group[cite: 2]</p>
                </div>

                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-book"></i></div>
                    <h4>IJRSAS (2019)</h4>
                    <p><strong>"Phenotypic Characterization of Indigenous Goats in North Shewa Zone, Amhara Region, Ethiopia"</strong></p>
                    <p style="font-size: 0.88rem; color: var(--green-dark);">Hailu Tilahun, Aynalem Haile, Ahmed Seid | Vol 5, Issue 7, pp. 44-55[cite: 2]</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Strategic Projects -->
    <section id="projects" class="bg-white">
        <div class="container">
            <div class="section-title">
                <h2>Strategic Projects & Field Implementation</h2>
                <p>From Research Concepts to Investable, Fundable, and Field-Tested Initiatives[cite: 2]</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <h3>01 — Climate & Carbon</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Carbon Credit Development & Climate Finance[cite: 2]</li>
                        <li>Climate Mitigation & Adaptation Strategies[cite: 2]</li>
                        <li>GTICDO Climate-Resilient Livelihoods[cite: 2]</li>
                        <li>Climate-Smart Agriculture & Nature-Based Solutions[cite: 2]</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>02 — Biodiversity & Ecosystem Restoration</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Biodiversity Conservation & Forest Protection[cite: 2]</li>
                        <li>Agroforestry & Ecosystem Restoration[cite: 2]</li>
                        <li>Organic Farming, Aquaculture & Apiculture[cite: 2]</li>
                        <li>Community Conservation & Safeguarding[cite: 2]</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>03 — Sustainable Agriculture & Livestock</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Salale University Honeybee Farm Establishment[cite: 2]</li>
                        <li>North Shewa Model Cattle Crush Infrastructure[cite: 2]</li>
                        <li>Dairy Feed Resource Evaluation & Synchronization[cite: 2]</li>
                        <li>Animal Breeding & Smallholder Development[cite: 2]</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>04 — Coffee & International Trade</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Sustainable Coffee Production</li>
                        <li>Coffee Value-Chain Development</li>
                        <li>Quality Improvement & Export Linkage</li>
                        <li>Agricultural Investment & Trade</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>05 — Youth & Women's Empowerment</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Youth Entrepreneurship & Green Jobs[cite: 2]</li>
                        <li>Women's Economic Participation[cite: 2]</li>
                        <li>Skills Development & Capacity Building[cite: 2]</li>
                        <li>Sustainable Community Enterprise[cite: 2]</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>06 — Research & Innovation</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Livestock Genomics & GWAS Applications[cite: 2]</li>
                        <li>ANOVA, Regression & R Analytics (Holeta HARC)[cite: 2]</li>
                        <li>Beekeeping Practice & Hive Tech Assessments[cite: 2]</li>
                        <li>Evidence-Based Development Partnerships[cite: 2]</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Partnerships Section -->
    <section id="partnerships">
        <div class="container">
            <div class="section-title">
                <h2>Partnership Opportunities</h2>
                <p>Building International Partnerships based on Trust, Transparency, Evidence, Inclusion, Innovation, Accountability, and Long-Term Impact[cite: 2].</p>
            </div>

            <!-- Target Partners Grid -->
            <div class="grid-4" style="margin-bottom: 3rem;">
                <div class="glance-card">
                    <i class="fa-solid fa-building-columns"></i>
                    <h4>International Foundations</h4>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-hand-holding-dollar"></i>
                    <h4>Donors & Grant Makers</h4>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-globe"></i>
                    <h4>NGOs & Civil Society</h4>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-landmark"></i>
                    <h4>Development Agencies</h4>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-chart-pie"></i>
                    <h4>Impact Investors</h4>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-graduation-cap"></i>
                    <h4>Research Institutions</h4>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-briefcase"></i>
                    <h4>Private-Sector Partners</h4>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-seedling"></i>
                    <h4>Agricultural & Environmental Orgs</h4>
                </div>
            </div>

            <!-- Table -->
            <h3 style="margin-bottom: 1.5rem;">Opportunity Focus & Partnership Types</h3>
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
                            <td>Carbon, resilience, climate finance[cite: 2]</td>
                            <td>Investment / Grant</td>
                        </tr>
                        <tr>
                            <td><strong>Biodiversity</strong></td>
                            <td>Conservation, restoration, nature[cite: 2]</td>
                            <td>Grant / Climate Finance</td>
                        </tr>
                        <tr>
                            <td><strong>Sustainable Agriculture</strong></td>
                            <td>Farmers, livestock, food systems[cite: 2]</td>
                            <td>Grant / Investment</td>
                        </tr>
                        <tr>
                            <td><strong>Coffee</strong></td>
                            <td>Production, value chain, export</td>
                            <td>Investment / Trade</td>
                        </tr>
                        <tr>
                            <td><strong>Youth & Women</strong></td>
                            <td>Enterprise, skills, livelihoods[cite: 2]</td>
                            <td>Grant / NGO Partnership</td>
                        </tr>
                        <tr>
                            <td><strong>Research</strong></td>
                            <td>Genetics, agriculture, climate[cite: 2]</td>
                            <td>Research Grant / University Partnership</td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <!-- Partnership Models & Packages -->
            <h3>Partnership Packages & Collaboration Models</h3>
            <div class="grid-3" style="margin-top: 1.5rem;">
                <div class="card">
                    <h4>1. Research Partnership</h4>
                    <p>Joint research, field studies, publications, data collection, and knowledge exchange[cite: 2].</p>
                </div>
                <div class="card">
                    <h4>2. Project Development Partnership</h4>
                    <p>Concept development, proposal writing, budgeting, technical design, and funding preparation[cite: 2].</p>
                </div>
                <div class="card">
                    <h4>3. Implementation Partnership</h4>
                    <p>Local coordination, community engagement, training, field implementation, and reporting[cite: 2].</p>
                </div>
                <div class="card">
                    <h4>4. Investment Partnership</h4>
                    <p>Agriculture, livestock, coffee, climate, carbon, biodiversity, and sustainable enterprise opportunities[cite: 2].</p>
                </div>
                <div class="card">
                    <h4>5. Technical Partnership</h4>
                    <p>Scientific expertise, agricultural technology, climate solutions, monitoring, and capacity building[cite: 2].</p>
                </div>
                <div class="card">
                    <h4>6. Market Partnership</h4>
                    <p>Connecting Ethiopian agricultural products and sustainable enterprises with international buyers, investors, and markets.</p>
                </div>
            </div>

            <!-- Process Flow -->
            <div class="process-flow">
                <div class="process-step"><i class="fa-solid fa-lightbulb"></i> Concept</div>
                <i class="fa-solid fa-chevron-right" style="color: #86EFAC;"></i>
                <div class="process-step"><i class="fa-solid fa-pen-ruler"></i> Project Design</div>
                <i class="fa-solid fa-chevron-right" style="color: #86EFAC;"></i>
                <div class="process-step"><i class="fa-solid fa-handshake"></i> Partnership</div>
                <i class="fa-solid fa-chevron-right" style="color: #86EFAC;"></i>
                <div class="process-step"><i class="fa-solid fa-coins"></i> Financing</div>
                <i class="fa-solid fa-chevron-right" style="color: #86EFAC;"></i>
                <div class="process-step"><i class="fa-solid fa-gears"></i> Implementation</div>
                <i class="fa-solid fa-chevron-right" style="color: #86EFAC;"></i>
                <div class="process-step"><i class="fa-solid fa-chart-line"></i> Monitoring & Impact</div>
            </div>
        </div>
    </section>

    <!-- Research Section -->
    <section id="research" class="bg-white">
        <div class="container">
            <div class="section-title">
                <h2>Research for Resilient Food Systems</h2>
                <p>Translating Evidence and Innovation into Field Solutions[cite: 2]</p>
            </div>
            <div class="grid-2">
                <div class="card">
                    <h3>Core Research Intersection</h3>
                    <p>My research interests focus on the relationship between: <strong>Animal Science | Genetics | Agriculture | Climate Resilience | Biodiversity | Sustainable Land Use | Community Development</strong>[cite: 2].</p>
                    <p>The objective is to translate research, evidence, and innovation into practical solutions that can benefit farmers, communities, institutions, businesses, and development partners[cite: 2].</p>
                </div>
                <div class="card">
                    <h3>Specific Research Interests</h3>
                    <ul class="green-bullets">
                        <li>Animal Breeding & Genetics (MSc Jimma University)[cite: 2]</li>
                        <li>Livestock Genomics & GWAS Applications[cite: 2]</li>
                        <li>Agricultural Innovation & Technology Transfer[cite: 2]</li>
                        <li>Climate-Smart Agriculture & Agroecology[cite: 2]</li>
                        <li>Sustainable Livestock Systems & Feed Resource Evaluation[cite: 2]</li>
                        <li>Biodiversity & Genetic Resources Conservation[cite: 2]</li>
                        <li>Climate Resilience & Humanitarian Development[cite: 2]</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Consulting Services -->
    <section id="consulting">
        <div class="container">
            <div class="section-title">
                <h2>Consultations for Organizations</h2>
                <p>We provide professional organizational and project development consulting services to support organizations, NGOs, CSOs, businesses, and community initiatives in turning ideas into practical, fundable, and sustainable programs[cite: 2].</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <h3>Documentation & Proposals</h3>
                    <ul class="green-bullets">
                        <li>Project Proposal Development[cite: 2]</li>
                        <li>Concept Notes and Project Summaries[cite: 2]</li>
                        <li>Grant and Donor Application Support[cite: 2]</li>
                        <li>Partnership and Funding Proposals[cite: 2]</li>
                        <li>Research and Technical Documentation[cite: 2]</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Planning & Strategy</h3>
                    <ul class="green-bullets">
                        <li>Business Plans and Feasibility Studies[cite: 2]</li>
                        <li>Strategic and Organizational Planning[cite: 2]</li>
                        <li>Project Budgets and Financial Plans[cite: 2]</li>
                        <li>Sustainability and Resource Mobilization Strategies[cite: 2]</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Design, Data & Reports</h3>
                    <ul class="green-bullets">
                        <li>Data Collection & Statistical Analysis (SAS/R)[cite: 2]</li>
                        <li>Program and Project Design[cite: 2]</li>
                        <li>Monitoring, Evaluation, and Reporting (MER) Frameworks[cite: 2]</li>
                        <li>Project Reports and Documentation[cite: 2]</li>
                        <li>Organizational Profiles and Capability Statements[cite: 2]</li>
                    </ul>
                </div>
            </div>

            <!-- Transparency Box -->
            <div class="card" style="margin-top: 2.5rem; background: var(--green-subtle); border-color: var(--green-border);">
                <h3>Transparency & Accountability Commitment</h3>
                <p>I am committed to professional standards of transparency, accountability, ethical conduct, responsible resource management, evidence-based decision-making, and measurable results[cite: 2]. For funded projects and partnerships, appropriate documentation may include[cite: 2]:</p>
                <div class="pill-list">
                    <span class="pill">Project Proposals</span>
                    <span class="pill">Logical Frameworks</span>
                    <span class="pill">Budgets</span>
                    <span class="pill">Work Plans</span>
                    <span class="pill">Monitoring & Evaluation Frameworks</span>
                    <span class="pill">Progress Reports</span>
                    <span class="pill">Financial Reports</span>
                    <span class="pill">Impact Reports</span>
                    <span class="pill">Partnership Agreements</span>
                    <span class="pill">Safeguarding & Risk Management Procedures</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Geographic Focus -->
    <section class="bg-white" style="padding: 3rem 2rem;">
        <div class="container" style="text-align: center;">
            <h3>Geographic Focus</h3>
            <p style="font-size: 1.15rem; color: var(--green-dark); font-weight: 700; margin-top: 0.5rem;">Ethiopia | East Africa | Africa | International[cite: 2]</p>
            <p style="max-width: 780px; margin: 0.5rem auto 0 auto;">With Ethiopia as a primary base, I work with local and international partners to develop initiatives that can be implemented, tested, and scaled across communities and wider regional contexts[cite: 2].</p>
        </div>
    </section>

    <!-- High-Visibility Contact Section -->
    <section id="contact">
        <div class="container">
            <div class="contact-card">
                <h2>Let's Build Sustainable Solutions Together</h2>
                <p>If you are a donor, foundation, grant maker, NGO, investor, development organization, researcher, government institution, or private-sector partner, I welcome the opportunity to explore collaboration[cite: 2].</p>
                
                <div class="contact-grid">
                    <div class="contact-method">
                        <i class="fa-solid fa-envelope"></i>
                        <div>
                            <div style="font-size: 0.82rem; color: var(--footer-accent); text-align: left;">Direct Email</div>
                            <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a>[cite: 2]
                        </div>
                    </div>
                    <div class="contact-method">
                        <i class="fa-brands fa-whatsapp"></i>
                        <div>
                            <div style="font-size: 0.82rem; color: var(--footer-accent); text-align: left;">WhatsApp / Mobile</div>
                            <a href="https://wa.me/251910204390">+251 910 204 390</a>[cite: 2]
                        </div>
                    </div>
                </div>

                <div class="social-bar">
                    <a href="https://wa.me/251910204390" title="WhatsApp"><i class="fa-brands fa-whatsapp"></i></a>
                    <a href="mailto:hailshtilahun@gmail.com" title="Email"><i class="fa-solid fa-envelope"></i></a>
                </div>
            </div>
        </div>
    </section>

    <!-- High-Visibility Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2026 Hailu Tilahun Kebede. All Rights Reserved. | Addis Ababa, Ethiopia[cite: 2]</p>
        </div>
    </footer>

</body>
</html>
