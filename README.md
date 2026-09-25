<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Agricultural Scientist & Sustainable Development Specialist</title>
    <!-- Google Fonts & Font Awesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Lora:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            /* Full Green Palette */
            --green-darkest: #0B2B1A;   /* Deep Forest Green */
            --green-dark: #134027;      /* Rich Emerald */
            --green-primary: #1E5E3A;   /* Primary Green */
            --green-medium: #2D8A53;    /* Vibrant Green */
            --green-light: #52B788;     /* Sage Green */
            --green-accent: #74C69D;    /* Mint Accent */
            --green-tint: #D8F3DC;      /* Soft Light Green Tint */
            --green-bg: #F4F9F5;        /* Ultra Soft Mint BG */
            
            --text-dark: #0F1E15;
            --text-muted: #3D5A4B;
            --white: #FFFFFF;
            
            --font-heading: 'Lora', serif;
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
            background-color: var(--white);
            line-height: 1.65;
        }

        /* Typography */
        h1, h2, h3, h4, h5 {
            font-family: var(--font-heading);
            color: var(--green-darkest);
            line-height: 1.25;
        }

        p {
            color: var(--text-muted);
            margin-bottom: 1.2rem;
            font-size: 1rem;
        }

        a {
            text-decoration: none;
            transition: all 0.3s ease;
        }

        /* Header Navigation */
        header {
            position: sticky;
            top: 0;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-bottom: 2px solid var(--green-tint);
            z-index: 1000;
        }

        .nav-container {
            max-width: 1280px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.2rem 2rem;
        }

        .logo {
            font-family: var(--font-heading);
            font-size: 1.25rem;
            font-weight: 700;
            color: var(--green-darkest);
            letter-spacing: -0.5px;
        }

        .logo span {
            color: var(--green-medium);
        }

        .nav-links {
            display: flex;
            gap: 1.2rem;
            list-style: none;
        }

        .nav-links a {
            font-size: 0.88rem;
            font-weight: 600;
            color: var(--text-dark);
            padding: 0.4rem 0.6rem;
            border-radius: 4px;
        }

        .nav-links a:hover {
            color: var(--green-medium);
            background: var(--green-tint);
        }

        .btn-green {
            background-color: var(--green-primary);
            color: var(--white) !important;
            padding: 0.65rem 1.4rem;
            border-radius: 6px;
            font-weight: 600;
            font-size: 0.9rem;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            box-shadow: 0 4px 12px rgba(30, 94, 58, 0.2);
        }

        .btn-green:hover {
            background-color: var(--green-dark);
            transform: translateY(-2px);
        }

        .btn-outline-green {
            border: 2px solid var(--green-accent);
            color: var(--white) !important;
            padding: 0.65rem 1.4rem;
            border-radius: 6px;
            font-weight: 600;
            font-size: 0.9rem;
        }

        .btn-outline-green:hover {
            background-color: var(--green-accent);
            color: var(--green-darkest) !important;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--green-darkest) 0%, var(--green-dark) 60%, var(--green-primary) 100%);
            color: var(--white);
            padding: 6rem 2rem;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0; right: 0; bottom: 0; left: 0;
            background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%2052b788' fill-opacity='0.08'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
        }

        .hero-container {
            max-width: 1100px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
            text-align: center;
        }

        .hero-badge {
            background: rgba(116, 198, 157, 0.15);
            border: 1px solid var(--green-accent);
            color: var(--green-accent);
            padding: 0.4rem 1.2rem;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1px;
            display: inline-block;
            margin-bottom: 1.5rem;
        }

        .hero h1 {
            color: var(--white);
            font-size: 2.8rem;
            margin-bottom: 1.2rem;
        }

        .hero p.lead {
            color: var(--green-tint);
            font-size: 1.15rem;
            max-width: 900px;
            margin: 0 auto 2rem auto;
        }

        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 1rem;
            flex-wrap: wrap;
        }

        /* Layout Structure */
        section {
            padding: 5rem 2rem;
        }

        .container {
            max-width: 1240px;
            margin: 0 auto;
        }

        .bg-green-soft {
            background-color: var(--green-bg);
        }

        .bg-green-dark {
            background-color: var(--green-darkest);
            color: var(--white);
        }

        .bg-green-dark h2, .bg-green-dark h3, .bg-green-dark h4 {
            color: var(--white);
        }

        .bg-green-dark p {
            color: var(--green-tint);
        }

        .section-title {
            text-align: center;
            max-width: 750px;
            margin: 0 auto 3.5rem auto;
        }

        .section-title h2 {
            font-size: 2.2rem;
            margin-bottom: 0.8rem;
            position: relative;
        }

        .section-title h2::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background: var(--green-medium);
            margin: 0.8rem auto 0 auto;
            border-radius: 2px;
        }

        .section-title p {
            font-size: 1.05rem;
        }

        /* Grids & Cards */
        .grid-2 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
        }

        .grid-3 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .grid-4 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 1.5rem;
        }

        .card {
            background: var(--white);
            border-radius: 12px;
            padding: 2rem;
            border: 1px solid var(--green-tint);
            box-shadow: 0 4px 20px rgba(19, 64, 39, 0.05);
            transition: all 0.3s ease;
            position: relative;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(19, 64, 39, 0.12);
            border-color: var(--green-light);
        }

        .card-icon {
            width: 50px;
            height: 50px;
            background: var(--green-tint);
            color: var(--green-primary);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.4rem;
            margin-bottom: 1.2rem;
        }

        /* At A Glance Strip */
        .glance-card {
            background: var(--white);
            border: 1px solid var(--green-tint);
            border-radius: 10px;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.03);
        }

        .glance-card i {
            font-size: 2rem;
            color: var(--green-medium);
            margin-bottom: 0.8rem;
        }

        .glance-card h4 {
            font-size: 1.1rem;
            margin-bottom: 0.4rem;
        }

        /* Tags & Pills */
        .pill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 1rem;
        }

        .pill {
            background: var(--green-tint);
            color: var(--green-darkest);
            padding: 0.35rem 0.85rem;
            border-radius: 50px;
            font-size: 0.82rem;
            font-weight: 600;
        }

        /* Bullet Styling */
        .green-bullets {
            list-style: none;
        }

        .green-bullets li {
            position: relative;
            padding-left: 1.8rem;
            margin-bottom: 0.6rem;
            color: var(--text-muted);
        }

        .green-bullets li::before {
            content: "\f00c";
            font-family: "Font Awesome 6 Free";
            font-weight: 900;
            position: absolute;
            left: 0;
            top: 2px;
            color: var(--green-medium);
            font-size: 0.85rem;
        }

        /* Process Flow Bar */
        .process-flow {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: var(--green-darkest);
            padding: 1.5rem;
            border-radius: 12px;
            color: var(--white);
            flex-wrap: wrap;
            gap: 1rem;
            margin-top: 2rem;
        }

        .process-step {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-weight: 600;
            color: var(--green-tint);
        }

        .process-step i {
            color: var(--green-accent);
        }

        /* Table Design */
        .table-responsive {
            overflow-x: auto;
            border-radius: 12px;
            border: 1px solid var(--green-tint);
            box-shadow: 0 4px 15px rgba(0,0,0,0.03);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: var(--white);
            text-align: left;
        }

        th {
            background-color: var(--green-primary);
            color: var(--white);
            padding: 1.2rem;
            font-weight: 600;
        }

        td {
            padding: 1.1rem 1.2rem;
            border-bottom: 1px solid var(--green-tint);
            color: var(--text-muted);
        }

        tr:nth-child(even) {
            background-color: var(--green-bg);
        }

        /* Contact Section Box */
        .contact-card {
            background: linear-gradient(135deg, var(--green-darkest), var(--green-primary));
            border-radius: 16px;
            padding: 3.5rem 2rem;
            color: var(--white);
            text-align: center;
            box-shadow: 0 10px 30px rgba(11, 43, 26, 0.2);
        }

        .contact-card h2 {
            color: var(--white);
            margin-bottom: 1rem;
        }

        .contact-card p {
            color: var(--green-tint);
            max-width: 650px;
            margin: 0 auto 2rem auto;
            font-size: 1.1rem;
        }

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
            gap: 0.8rem;
            font-size: 1.1rem;
        }

        .contact-method i {
            width: 45px;
            height: 45px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--green-accent);
        }

        .contact-method a {
            color: var(--white);
            font-weight: 600;
        }

        .social-bar {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 1.5rem;
        }

        .social-bar a {
            width: 40px;
            height: 40px;
            background: rgba(255,255,255,0.1);
            color: var(--white);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }

        .social-bar a:hover {
            background: var(--green-accent);
            color: var(--green-darkest);
        }

        /* Footer */
        footer {
            background: var(--green-darkest);
            color: var(--green-tint);
            padding: 2rem;
            text-align: center;
            font-size: 0.9rem;
            border-top: 1px solid rgba(255,255,255,0.1);
        }

        /* Mobile Adjustments */
        @media (max-width: 992px) {
            .nav-links { display: none; }
            .hero h1 { font-size: 2.1rem; }
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
            <a href="#contact" class="btn-green"><i class="fa-solid fa-paper-plane"></i> Get in Touch</a>
        </div>
    </header>

    <!-- Hero / Home -->
    <section class="hero" id="home">
        <div class="hero-container">
            <span class="hero-badge"><i class="fa-solid fa-leaf"></i> Agricultural Scientist & Sustainable Development Specialist</span>
            <h1>Connecting Science, Nature, Finance & Markets for Sustainable Development</h1>
            <p class="lead">Working at the intersection of Agricultural Science, Sustainable Agriculture, Climate Action, Biodiversity Conservation, Carbon Finance, Sustainable Development, and International Markets across Ethiopia and Africa.</p>
            <div class="hero-btns">
                <a href="#contact" class="btn-green"><i class="fa-solid fa-handshake"></i> Partner With Me</a>
                <a href="#projects" class="btn-outline-green"><i class="fa-solid fa-folder-open"></i> Explore Projects</a>
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
                    <p>His professional work has expanded from agricultural science and research into an integrated development approach connecting: <strong>Science | Agriculture | Climate | Nature | Finance | Markets | Communities</strong>.</p>
                    <p>This multidisciplinary perspective supports the development of solutions addressing interconnected challenges including climate change, food security, biodiversity loss, agricultural productivity, sustainable livelihoods, rural development, and access to international markets.</p>
                    <p>The focus is not only on developing ideas, but on connecting knowledge, resources, partnerships, and implementation to create practical and scalable impact. I have also participated in youth leadership and climate action on COP programs and UNFCCC processes.</p>
                </div>
                <div>
                    <div class="card" style="border-left: 5px solid var(--green-medium); margin-bottom: 1.5rem;">
                        <div class="card-icon"><i class="fa-solid fa-bullseye"></i></div>
                        <h3>Mission</h3>
                        <p>To connect science, innovation, finance, partnerships, and communities to develop sustainable solutions that improve livelihoods, strengthen climate resilience, protect nature, and create long-term economic and social value.</p>
                    </div>
                    <div class="card" style="border-left: 5px solid var(--green-light);">
                        <div class="card-icon"><i class="fa-solid fa-eye"></i></div>
                        <h3>Vision</h3>
                        <p>A future where science, sustainable finance, responsible investment, nature, agriculture, and international partnerships work together to create resilient communities and inclusive prosperity.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- At A Glance Section -->
    <section id="glance" class="bg-green-soft">
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
                    <i class="fa-solid fa-cloud-sun"></i>
                    <h4>Climate & Carbon</h4>
                    <p>Carbon-credit development, climate finance, climate mitigation and adaptation, climate-smart agriculture, and climate resilience.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-tree"></i>
                    <h4>Nature & Biodiversity</h4>
                    <p>Biodiversity conservation, agroforestry, ecosystem restoration, regenerative agriculture, and nature-based solutions.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-wheat-awn"></i>
                    <h4>Agriculture & Food Systems</h4>
                    <p>Sustainable agriculture, agroecology, food security, resilient food systems, agricultural value chains, community-based production, humanitarian food resilience, entrepreneurship, self-sufficiency, and sustainable livelihoods.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-mug-hot"></i>
                    <h4>Coffee & Global Markets</h4>
                    <p>Sustainable coffee production, value-chain development, export, international market linkage, and agricultural investment.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-people-hold"></i>
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
            <p style="text-align: center; max-width: 800px; margin: 0 auto 3rem auto;">Many high-impact development opportunities require more than funding. They require technical knowledge, local understanding, trusted relationships, project development capacity, implementation partnerships, and access to wider networks. I help organizations transform ambitious ideas into practical, scalable initiatives.</p>
            
            <div class="grid-3">
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-microscope"></i></div>
                    <h3>Scientific & Technical Expertise</h3>
                    <p>A foundation in animal science, breeding, genetics, genomics, agricultural research, and sustainable production systems.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-temperature-arrow-up"></i></div>
                    <h3>Climate & Sustainability</h3>
                    <p>Experience across climate mitigation, adaptation, climate-smart agriculture, biodiversity, agroforestry, ecosystem restoration, carbon markets, and climate finance.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-users"></i></div>
                    <h3>Community Perspective</h3>
                    <p>A strong focus on smallholder farmers, communities, youth, women, sustainable livelihoods, and inclusive development.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-diagram-project"></i></div>
                    <h3>Project Development</h3>
                    <p>An interest in translating ideas into structured projects, partnerships, investment opportunities, and scalable initiatives.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-globe"></i></div>
                    <h3>International Orientation</h3>
                    <p>A commitment to building relationships with international foundations, donors, NGOs, investors, research institutions, and development organizations.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-chart-line"></i></div>
                    <h3>Measurable Impact</h3>
                    <p>Integrating science, investment, implementation, and rigorous monitoring to deliver long-term value.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Expertise Section -->
    <section id="expertise" class="bg-green-soft">
        <div class="container">
            <div class="section-title">
                <h2>Areas of Expertise</h2>
                <p>Specialized multidisciplinary skills built across 8+ years of scientific research and field implementation.</p>
            </div>
            
            <div class="grid-3">
                
                <!-- 01 -->
                <div class="card">
                    <h4 style="color: var(--green-medium); font-size: 0.9rem; font-family: var(--font-body); font-weight: 700;">01</h4>
                    <h3>Livestock Science & Farming</h3>
                    <div class="pill-list">
                        <span class="pill">Livestock Farm Management</span>
                        <span class="pill">Dairy, Beef, Sheep, Goat & Poultry</span>
                        <span class="pill">Animal Nutrition & Feed Production</span>
                        <span class="pill">Pasture & Forage Development</span>
                        <span class="pill">Breeding & Herd Improvement</span>
                        <span class="pill">Climate-Smart Farming</span>
                        <span class="pill">Livestock Health & Farm Hygiene</span>
                        <span class="pill">Integrated Crop–Livestock Farming</span>
                        <span class="pill">Agribusiness & Entrepreneurship</span>
                    </div>
                </div>

                <!-- 02 -->
                <div class="card">
                    <h4 style="color: var(--green-medium); font-size: 0.9rem; font-family: var(--font-body); font-weight: 700;">02</h4>
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

                <!-- 03 -->
                <div class="card">
                    <h4 style="color: var(--green-medium); font-size: 0.9rem; font-family: var(--font-body); font-weight: 700;">03</h4>
                    <h3>Biodiversity, Nature & Restoration</h3>
                    <div class="pill-list">
                        <span class="pill">Biodiversity Conservation</span>
                        <span class="pill">Agroforestry</span>
                        <span class="pill">Ecosystem Restoration</span>
                        <span class="pill">Sustainable Land Management</span>
                        <span class="pill">Regenerative Agriculture</span>
                        <span class="pill">Nature-Based Solutions</span>
                    </div>
                </div>

                <!-- 04 -->
                <div class="card">
                    <h4 style="color: var(--green-medium); font-size: 0.9rem; font-family: var(--font-body); font-weight: 700;">04</h4>
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

                <!-- 05 -->
                <div class="card">
                    <h4 style="color: var(--green-medium); font-size: 0.9rem; font-family: var(--font-body); font-weight: 700;">05</h4>
                    <h3>Coffee & International Trade</h3>
                    <div class="pill-list">
                        <span class="pill">Sustainable Coffee Production</span>
                        <span class="pill">Coffee Export</span>
                        <span class="pill">International Market Linkage</span>
                        <span class="pill">Agricultural Investment</span>
                        <span class="pill">International Trade Partnerships</span>
                    </div>
                </div>

                <!-- 06 -->
                <div class="card">
                    <h4 style="color: var(--green-medium); font-size: 0.9rem; font-family: var(--font-body); font-weight: 700;">06</h4>
                    <h3>Community & Inclusive Development</h3>
                    <div class="pill-list">
                        <span class="pill">Youth Empowerment</span>
                        <span class="pill">Women's Economic Participation</span>
                        <span class="pill">Community Capacity Building</span>
                        <span class="pill">Green Livelihoods</span>
                        <span class="pill">Inclusive Value Chains</span>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Impact Areas -->
    <section id="impact">
        <div class="container">
            <div class="section-title">
                <h2>Areas of Impact</h2>
                <p>Turning Knowledge into Action</p>
            </div>
            <div class="grid-2">
                <div class="card">
                    <h3>Climate Action & Resilience</h3>
                    <p>Developing approaches that connect climate action, adaptation, resilience, and sustainable finance to support communities and productive systems facing climate-related challenges.</p>
                </div>
                <div class="card">
                    <h3>Carbon Markets & Climate Finance</h3>
                    <p>Exploring opportunities to connect verified environmental outcomes with responsible climate finance and carbon-market mechanisms, while ensuring community and ecosystem benefits.</p>
                </div>
                <div class="card">
                    <h3>Biodiversity & Nature</h3>
                    <p>Supporting biodiversity conservation, agroforestry, ecosystem restoration, sustainable land management, and nature-based solutions.</p>
                </div>
                <div class="card">
                    <h3>Sustainable Agriculture</h3>
                    <p>Advancing agricultural systems that improve productivity, climate resilience, food security, environmental sustainability, and livelihoods.</p>
                </div>
                <div class="card">
                    <h3>Livestock & Genetic Resources</h3>
                    <p>Applying science and innovation to strengthen livestock productivity, dairy farming, honeybee production, poultry farming, genetic resources, sustainable production, and resilience.</p>
                </div>
                <div class="card">
                    <h3>Coffee & International Markets</h3>
                    <p>Connecting Ethiopia's agricultural potential with international buyers, investors, markets, value-chain development, and sustainable trade opportunities.</p>
                </div>
                <div class="card">
                    <h3>Youth & Women's Economic Empowerment</h3>
                    <p>Supporting approaches that create meaningful opportunities for youth and women through skills, enterprise, agriculture, innovation, employment, and sustainable livelihoods.</p>
                </div>
                <div class="card">
                    <h3>Community-Led Development</h3>
                    <p>Promoting development approaches that place communities at the center of planning, implementation, ownership, and long-term sustainability.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Strategic Projects -->
    <section id="projects" class="bg-green-soft">
        <div class="container">
            <div class="section-title">
                <h2>Strategic Projects</h2>
                <p>From Ideas to Investable and Fundable Initiatives</p>
            </div>
            
            <div class="grid-3">
                
                <div class="card">
                    <h3>01 — Climate & Carbon</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Carbon Credit Development</li>
                        <li>Climate Mitigation & Adaptation</li>
                        <li>Climate-Resilient Livelihoods</li>
                        <li>Climate-Smart Agriculture</li>
                        <li>Nature-Based Climate Solutions</li>
                        <li>Climate Finance</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>02 — Biodiversity & Restoration</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Biodiversity Conservation</li>
                        <li>Agroforestry & Forest Restoration</li>
                        <li>Ecosystem Rehabilitation</li>
                        <li>Sustainable Land Management</li>
                        <li>Nature-Based Solutions</li>
                        <li>Community Conservation</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>03 — Sustainable Livestock</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Sustainable Livestock Production</li>
                        <li>Animal Breeding & Genetic Improvement</li>
                        <li>Climate-Smart Agriculture</li>
                        <li>Agricultural Innovation</li>
                        <li>Food-System Resilience</li>
                        <li>Smallholder Farmer Development</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>04 — Coffee & Trade</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Sustainable Coffee Production</li>
                        <li>Coffee Value-Chain Development</li>
                        <li>Quality Improvement & Export</li>
                        <li>International Market Linkage</li>
                        <li>Agricultural Investment</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>05 — Inclusive Empowerment</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Youth Entrepreneurship & Green Jobs</li>
                        <li>Women's Economic Participation</li>
                        <li>Skills Development & Innovation</li>
                        <li>Sustainable Livelihoods</li>
                        <li>Community Enterprise</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>06 — Research & Innovation</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Agricultural & Climate Research</li>
                        <li>Animal Genetics & Genomics</li>
                        <li>Sustainable Production Systems</li>
                        <li>Technology Transfer</li>
                        <li>Evidence-Based Development</li>
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
                <p>Building International Partnerships for Practical Impact based on Trust, Transparency, Evidence, Inclusion, Innovation, Accountability & Long-Term Impact.</p>
            </div>

            <!-- Target Partners -->
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
                    <i class="fa-solid fa-globe-africa"></i>
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
                    <h4>Agri & Climate Orgs</h4>
                </div>
            </div>

            <!-- Table of Matrix -->
            <h3 style="margin-bottom: 1.5rem;">Opportunity Focus & Models</h3>
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
                            <td>Carbon, resilience, climate finance</td>
                            <td>Investment / Grant</td>
                        </tr>
                        <tr>
                            <td><strong>Biodiversity</strong></td>
                            <td>Conservation, restoration, nature-based solutions</td>
                            <td>Grant / Climate Finance</td>
                        </tr>
                        <tr>
                            <td><strong>Sustainable Agriculture</strong></td>
                            <td>Smallholders, livestock, food systems</td>
                            <td>Grant / Investment</td>
                        </tr>
                        <tr>
                            <td><strong>Coffee</strong></td>
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
                    <p>Joint research, field studies, publications, data collection, and knowledge exchange with universities and scientists.</p>
                </div>
                <div class="card">
                    <h4>2. Project Development</h4>
                    <p>Concept development, proposal writing, budgeting, technical design, and funding preparation.</p>
                </div>
                <div class="card">
                    <h4>3. Implementation</h4>
                    <p>Local coordination, community engagement, training, field operations, and reporting.</p>
                </div>
                <div class="card">
                    <h4>4. Investment Partnership</h4>
                    <p>Agriculture, livestock, coffee, climate, carbon, biodiversity, and sustainable enterprise opportunities.</p>
                </div>
                <div class="card">
                    <h4>5. Technical Partnership</h4>
                    <p>Scientific expertise, agricultural technology, climate solutions, monitoring, and capacity building.</p>
                </div>
                <div class="card">
                    <h4>6. Market Partnership</h4>
                    <p>Connecting Ethiopian agricultural products and sustainable enterprises with international buyers and investors.</p>
                </div>
            </div>

            <!-- Process Flow -->
            <div class="process-flow">
                <div class="process-step"><i class="fa-solid fa-lightbulb"></i> Concept</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--green-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-pen-ruler"></i> Project Design</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--green-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-handshake"></i> Partnership</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--green-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-coins"></i> Financing</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--green-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-gears"></i> Implementation</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--green-accent);"></i>
                <div class="process-step"><i class="fa-solid fa-chart-line"></i> Monitoring & Impact</div>
            </div>
        </div>
    </section>

    <!-- Research Section -->
    <section id="research" class="bg-green-soft">
        <div class="container">
            <div class="section-title">
                <h2>Research & Innovation</h2>
                <p>Research for Resilient Food Systems and Communities</p>
            </div>
            <div class="grid-2">
                <div class="card">
                    <h3>Core Research Objective</h3>
                    <p>My research interests focus on the relationship between: <strong>Animal Science | Genetics | Agriculture | Climate Resilience | Biodiversity | Sustainable Land Use | Community Development</strong>.</p>
                    <p>The objective is to translate research, evidence, and innovation into practical solutions that can benefit farmers, communities, institutions, businesses, and development partners.</p>
                </div>
                <div class="card">
                    <h3>Specific Research Interests</h3>
                    <ul class="green-bullets">
                        <li>Animal Breeding & Genetics</li>
                        <li>Livestock Genomics & GWAS Applications</li>
                        <li>Agricultural Innovation & Technology Transfer</li>
                        <li>Climate-Smart Agriculture & Agroecology</li>
                        <li>Sustainable Livestock Systems & Feed Production</li>
                        <li>Biodiversity & Genetic Resources Conservation</li>
                        <li>Climate Resilience & Humanitarian Development</li>
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
                <p>Professional organizational and project development consulting services to support CSOs, NGOs, businesses, and community initiatives in turning ideas into practical, fundable, and sustainable programs.</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <h3>Documentation & Proposals</h3>
                    <ul class="green-bullets">
                        <li>Project Proposal Development</li>
                        <li>Concept Notes & Project Summaries</li>
                        <li>Grant & Donor Support Applications</li>
                        <li>Partnership & Funding Proposals</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Planning & Strategy</h3>
                    <p style="margin-bottom: 0.5rem; color: var(--text-dark); font-weight: 600;">Strategic Services:</p>
                    <ul class="green-bullets">
                        <li>Business Plans & Feasibility Studies</li>
                        <li>Strategic & Organizational Planning</li>
                        <li>Project Budgets & Financial Plans</li>
                        <li>Sustainability & Resource Strategies</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Research & Monitoring</h3>
                    <ul class="green-bullets">
                        <li>Data Collection & Analysis</li>
                        <li>Program & Project Design</li>
                        <li>MEL Frameworks (Monitoring, Learning)</li>
                        <li>Organizational Profiles & Reports</li>
                    </ul>
                </div>
            </div>

            <!-- Transparency Box -->
            <div class="card" style="margin-top: 2.5rem; background: var(--green-bg); border-color: var(--green-accent);">
                <h3>Transparency & Accountability Commitment</h3>
                <p>I am committed to professional standards of transparency, accountability, ethical conduct, responsible resource management, evidence-based decision-making, and measurable results. For funded projects and partnerships, standard documentation includes:</p>
                <div class="pill-list">
                    <span class="pill">Project Proposals</span>
                    <span class="pill">Logical Frameworks</span>
                    <span class="pill">Budgets</span>
                    <span class="pill">Work Plans</span>
                    <span class="pill">MEL Frameworks</span>
                    <span class="pill">Progress Reports</span>
                    <span class="pill">Financial Reports</span>
                    <span class="pill">Impact Reports</span>
                    <span class="pill">Partnership Agreements</span>
                    <span class="pill">Safeguarding & Risk Procedures</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Geographic Focus -->
    <section class="bg-green-soft" style="padding: 3rem 2rem;">
        <div class="container" style="text-align: center;">
            <h3>Geographic Focus</h3>
            <p style="font-size: 1.1rem; color: var(--green-darkest); font-weight: 600; margin-top: 0.5rem;">Ethiopia | East Africa | Africa | International</p>
            <p style="max-width: 750px; margin: 0.5rem auto 0 auto;">With Ethiopia as a primary base, I work with local and international partners to develop initiatives that can be implemented, tested, and scaled across communities and wider regional contexts.</p>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <div class="contact-card">
                <h2>Let's Build Sustainable Solutions Together</h2>
                <p>If you are a donor, foundation, grant maker, NGO, investor, development organization, researcher, government institution, or private-sector partner, I welcome the opportunity to explore collaboration.</p>
                
                <div class="contact-grid">
                    <div class="contact-method">
                        <i class="fa-solid fa-envelope"></i>
                        <div>
                            <div style="font-size: 0.8rem; color: var(--green-tint);">Email Directly</div>
                            <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a>
                        </div>
                    </div>
                    <div class="contact-method">
                        <i class="fa-brands fa-whatsapp"></i>
                        <div>
                            <div style="font-size: 0.8rem; color: var(--green-tint);">WhatsApp / Direct Line</div>
                            <a href="https://wa.me/251910204390">+251 910 204 390</a>
                        </div>
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
