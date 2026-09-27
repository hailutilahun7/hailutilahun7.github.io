<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profile | Hailu Tilahun Kebede - Agricultural Scientist & Sustainable Development Specialist</title>
    <!-- Google Fonts & Font Awesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Outfit:wght@500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            /* Full Requested Color Palette */
            --deep-blue: #0A192F;        /* Deep Blue Background & Nav */
            --purple-main: #6D28D9;      /* Purple Headers & Badges */
            --purple-light: #F3E8FF;     
            --green-main: #10B981;       /* Emerald Green Highlights */
            --green-light: #ECFDF5;      
            --orange-main: #F97316;      /* Vibrant Orange Buttons */
            --orange-hover: #EA580C;     
            --yellow-main: #FBBF24;      /* Radiant Yellow Accents */
            --yellow-light: #FEF3C7;     
            
            --bg-body: #F8FAFC;           
            --bg-card: #FFFFFF;           
            --text-dark: #0F172A;         
            --text-muted: #475569;        
            
            --font-display: 'Outfit', sans-serif;
            --font-body: 'Plus Jakarta Sans', sans-serif;

            --shadow-card: 0 10px 25px -5px rgba(10, 25, 47, 0.08);
            --shadow-hover: 0 20px 35px -10px rgba(109, 40, 217, 0.25);
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
            background-color: var(--bg-body);
            line-height: 1.65;
            width: 100vw;
            overflow-x: hidden;
        }

        /* Typography */
        h1, h2, h3, h4, h5 {
            font-family: var(--font-display);
            color: var(--text-dark);
            line-height: 1.2;
            font-weight: 700;
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

        /* Full Screen Width Header */
        header {
            position: sticky;
            top: 0;
            background: rgba(10, 25, 47, 0.96);
            backdrop-filter: blur(12px);
            border-bottom: 3px solid var(--yellow-main);
            z-index: 1000;
            width: 100%;
            padding: 1.1rem 3rem;
        }

        .nav-container {
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .header-brand {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            color: #FFFFFF;
            font-family: var(--font-display);
            font-size: 1.25rem;
            font-weight: 800;
            letter-spacing: -0.3px;
        }

        .header-brand span.profile-tag {
            background: linear-gradient(135deg, var(--purple-main), var(--green-main));
            color: #FFFFFF;
            padding: 0.25rem 0.65rem;
            border-radius: 6px;
            font-size: 0.75rem;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .nav-links {
            display: flex;
            gap: 1.2rem;
            list-style: none;
            flex-wrap: wrap;
            justify-content: flex-end;
        }

        .nav-links a {
            font-size: 0.95rem;
            font-weight: 600;
            color: #E2E8F0;
            padding: 0.45rem 0.85rem;
            border-radius: 8px;
        }

        .nav-links a:hover {
            color: var(--yellow-main);
            background: rgba(255, 255, 255, 0.1);
        }

        /* Buttons */
        .btn-orange {
            background: linear-gradient(135deg, var(--orange-main) 0%, var(--orange-hover) 100%);
            color: #FFFFFF !important;
            padding: 0.9rem 2rem;
            border-radius: 50px;
            font-weight: 700;
            box-shadow: 0 10px 25px rgba(249, 115, 22, 0.35);
            display: inline-flex;
            align-items: center;
            gap: 0.6rem;
        }

        .btn-orange:hover {
            transform: translateY(-2px);
            box-shadow: 0 14px 30px rgba(249, 115, 22, 0.45);
        }

        .btn-outline-yellow {
            border: 2px solid var(--yellow-main);
            color: var(--yellow-main) !important;
            padding: 0.9rem 2rem;
            border-radius: 50px;
            font-weight: 700;
            background: transparent;
            display: inline-flex;
            align-items: center;
            gap: 0.6rem;
        }

        .btn-outline-yellow:hover {
            background-color: var(--yellow-main);
            color: var(--deep-blue) !important;
            transform: translateY(-2px);
        }

        /* Full Screen Hero Section */
        .hero {
            width: 100vw;
            background: linear-gradient(135deg, var(--deep-blue) 0%, #1E1B4B 60%, #0F172A 100%);
            color: #FFFFFF;
            padding: 7rem 4rem 6rem 4rem;
            text-align: center;
            position: relative;
        }

        .hero-container {
            width: 100%;
        }

        .hero-badge {
            background: rgba(109, 40, 217, 0.3);
            border: 1px solid var(--yellow-main);
            color: var(--yellow-main);
            padding: 0.55rem 1.6rem;
            border-radius: 50px;
            font-size: 0.9rem;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 1.2px;
            display: inline-block;
            margin-bottom: 1.8rem;
        }

        .hero h1 {
            color: #FFFFFF;
            font-size: 3.6rem;
            margin-bottom: 1.4rem;
            font-weight: 800;
            letter-spacing: -1px;
        }

        .hero h1 span {
            color: var(--green-main);
        }

        .hero p.lead {
            color: #CBD5E1;
            font-size: 1.3rem;
            max-width: 1000px;
            margin: 0 auto 2.8rem auto;
            font-weight: 400;
        }

        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 1.2rem;
            flex-wrap: wrap;
        }

        /* Profile Photo Container */
        .profile-img-container {
            text-align: center;
            margin-bottom: 2rem;
        }

        .profile-img {
            width: 270px;
            height: 270px;
            border-radius: 50%;
            object-fit: cover;
            border: 6px solid var(--yellow-main);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }

        /* Full Screen Sections */
        section {
            width: 100vw;
            padding: 6rem 4rem;
        }

        .container {
            width: 100%;
        }

        .bg-white {
            background-color: #FFFFFF;
        }

        .bg-purple-tint {
            background-color: var(--purple-light);
        }

        .bg-green-tint {
            background-color: var(--green-light);
        }

        .section-title {
            text-align: center;
            margin-bottom: 3.8rem;
        }

        .section-title h2 {
            font-size: 2.7rem;
            margin-bottom: 0.8rem;
            font-weight: 800;
            color: var(--purple-main);
        }

        .section-title h2::after {
            content: '';
            display: block;
            width: 80px;
            height: 5px;
            background: linear-gradient(90deg, var(--orange-main), var(--yellow-main));
            margin: 0.9rem auto 0 auto;
            border-radius: 4px;
        }

        /* Grids & Cards spanning full width */
        .grid-2 { display: grid; grid-template-columns: repeat(auto-fit, minmax(360px, 1fr)); gap: 2.5rem; width: 100%; }
        .grid-3 { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 2.2rem; width: 100%; }
        .grid-4 { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 1.8rem; width: 100%; }

        .card {
            background: var(--bg-card);
            border-radius: 20px;
            padding: 2.5rem;
            border: 2px solid #E2E8F0;
            box-shadow: var(--shadow-card);
            transition: all 0.3s ease;
            width: 100%;
        }

        .card:hover {
            transform: translateY(-6px);
            box-shadow: var(--shadow-hover);
            border-color: var(--purple-main);
        }

        .card-icon {
            width: 60px;
            height: 60px;
            background: var(--yellow-light);
            color: var(--orange-main);
            border-radius: 16px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.6rem;
            margin-bottom: 1.5rem;
        }

        /* At A Glance Strip */
        .glance-card {
            background: var(--bg-card);
            border: 2px solid #E2E8F0;
            border-radius: 20px;
            padding: 2.2rem 1.6rem;
            text-align: center;
            box-shadow: var(--shadow-card);
            transition: all 0.3s ease;
        }

        .glance-card:hover {
            border-color: var(--green-main);
            transform: translateY(-5px);
            box-shadow: var(--shadow-hover);
        }

        .glance-card i {
            font-size: 2.6rem;
            color: var(--green-main);
            margin-bottom: 1.1rem;
        }

        /* Pills & Tags */
        .pill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.6rem;
            margin-top: 1.3rem;
        }

        .pill {
            background: var(--purple-light);
            color: var(--purple-main);
            padding: 0.45rem 1rem;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 700;
            border: 1px solid #DDD6FE;
        }

        .green-bullets {
            list-style: none;
        }

        .green-bullets li {
            position: relative;
            padding-left: 1.8rem;
            margin-bottom: 0.75rem;
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
            color: var(--green-main);
            font-size: 0.9rem;
        }

        /* Process Flow Banner */
        .process-flow {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: linear-gradient(135deg, var(--deep-blue) 0%, var(--purple-main) 100%);
            padding: 2.5rem 3rem;
            border-radius: 22px;
            color: #FFFFFF;
            flex-wrap: wrap;
            gap: 1.2rem;
            margin-top: 3.5rem;
            width: 100%;
        }

        .process-step {
            display: flex;
            align-items: center;
            gap: 0.6rem;
            font-weight: 700;
            color: #E2E8F0;
        }

        .process-step i {
            color: var(--yellow-main);
            font-size: 1.25rem;
        }

        /* Table */
        .table-responsive {
            overflow-x: auto;
            border-radius: 18px;
            border: 2px solid #E2E8F0;
            box-shadow: var(--shadow-card);
            width: 100%;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            background: #FFFFFF;
            text-align: left;
        }

        th {
            background-color: var(--deep-blue);
            color: var(--yellow-main);
            padding: 1.3rem;
            font-weight: 700;
        }

        td {
            padding: 1.1rem 1.3rem;
            border-bottom: 1px solid #E2E8F0;
            color: var(--text-muted);
            font-weight: 500;
        }

        tr:nth-child(even) {
            background-color: var(--purple-light);
        }

        /* Full Screen Contact Section */
        .contact-card {
            background: linear-gradient(135deg, var(--deep-blue) 0%, #1E1B4B 100%);
            border-radius: 28px;
            padding: 5rem 3rem;
            color: #FFFFFF;
            text-align: center;
            width: 100%;
            border: 2px solid var(--yellow-main);
        }

        .contact-card h2 { 
            color: #FFFFFF; 
            margin-bottom: 1rem; 
            font-size: 2.8rem; 
        }

        .contact-card p { 
            color: #CBD5E1; 
            max-width: 800px; 
            margin: 0 auto 2.8rem auto; 
            font-size: 1.2rem; 
        }

        .contact-grid {
            display: flex;
            justify-content: center;
            gap: 2rem;
            flex-wrap: wrap;
            margin-bottom: 3.2rem;
        }

        .contact-method {
            display: flex;
            align-items: center;
            gap: 1rem;
            font-size: 1.15rem;
            background: rgba(255, 255, 255, 0.08);
            padding: 1.1rem 2.2rem;
            border-radius: 50px;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .contact-method i {
            width: 48px;
            height: 48px;
            background: var(--orange-main);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #FFFFFF;
            font-size: 1.25rem;
        }

        .contact-method a { 
            color: #FFFFFF !important; 
            font-weight: 700; 
        }

        .social-title {
            font-size: 1.1rem;
            color: var(--yellow-main);
            text-transform: uppercase;
            letter-spacing: 1.2px;
            font-weight: 700;
            margin-bottom: 1.5rem;
        }

        .social-bar {
            display: flex;
            justify-content: center;
            gap: 1.2rem;
            flex-wrap: wrap;
        }

        .social-bar a {
            width: 54px;
            height: 54px;
            background: rgba(255, 255, 255, 0.1);
            color: #FFFFFF;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.4rem;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.3s ease;
        }

        .social-bar a:hover {
            background: var(--orange-main);
            color: #FFFFFF;
            transform: translateY(-5px);
        }

        /* Footer */
        footer {
            background: #020617;
            color: #94A3B8;
            padding: 2.5rem 3rem;
            text-align: center;
            font-size: 1rem;
            font-weight: 600;
            width: 100vw;
        }

        @media (max-width: 992px) {
            header, section { padding-left: 1.5rem; padding-right: 1.5rem; }
            .nav-container { flex-direction: column; gap: 1rem; }
            .hero h1 { font-size: 2.5rem; }
            .process-flow { flex-direction: column; align-items: flex-start; }
            .nav-links { gap: 0.6rem; justify-content: center; }
            .nav-links a { font-size: 0.85rem; padding: 0.3rem 0.5rem; }
        }
    </style>
</head>
<body>

    <!-- Navigation Header -->
    <header>
        <div class="nav-container">
            <a href="#home" class="header-brand">
                <span class="profile-tag">Profile</span> HAILU TILAHUN KEBEDE
            </a>
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
            <p class="lead">Working across Agricultural Science, Sustainable Agriculture, Climate Action, Biodiversity Conservation, Carbon Finance, Sustainable Development, and International Markets.</p>
            <div class="hero-btns">
                <a href="HAILU_RESUME_2026.pdf" download class="btn-orange"><i class="fa-solid fa-file-arrow-down"></i> Download CV (PDF)</a>
                <a href="#projects" class="btn-outline-yellow"><i class="fa-solid fa-folder-open"></i> Explore Projects</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="bg-white">
        <div class="container">
            <div class="grid-2" style="align-items: center;">
                <div>
                    <div class="profile-img-container">
                        <img src="photo_2025-11-24_14-14-04.jpg" alt="Hailu Tilahun Kebede" class="profile-img">
                    </div>

                    <div style="text-align: left;" class="section-title">
                        <h2>From Science to Sustainable Impact</h2>
                    </div>
                    <p><strong>Hailu Tilahun Kebede</strong> is an Agricultural Scientist and Researcher with an MSc in Animal Breeding and Genetics and over eight years of experience in research, academic instruction, and community-based development. His professional work connects: <strong>Science | Agriculture | Climate | Nature | Finance | Markets | Communities</strong>.</p>
                    <p>This multidisciplinary perspective supports solutions addressing interconnected challenges including climate change, food security, biodiversity loss, agricultural productivity, sustainable livelihoods, rural development, and access to international markets.</p>
                    <p>The focus is not only on developing ideas, but on connecting knowledge, resources, partnerships, and implementation to create practical and scalable impact. I have participated in youth leadership and climate action on COP programs and UNFCCC processes, serving as an Official Delegate at the UNECA Regional Forum on Sustainable Development and African Union Delegate to the G20 Social Summit.</p>
                    <p>I seek long-term partnerships with international investors, foundations, donors, grant-making organizations, NGOs, development agencies, research institutions, governments, and private-sector partners committed to measurable and sustainable impact.</p>
                </div>
                <div>
                    <div class="card" style="border-left: 6px solid var(--purple-main); margin-bottom: 1.8rem;">
                        <div class="card-icon"><i class="fa-solid fa-bullseye"></i></div>
                        <h3>Mission</h3>
                        <p>To connect science, innovation, finance, partnerships, and communities to develop sustainable solutions that improve livelihoods, strengthen climate resilience, protect nature, and create long-term economic and social value.</p>
                    </div>
                    <div class="card" style="border-left: 6px solid var(--orange-main);">
                        <div class="card-icon" style="color: var(--orange-main); background: var(--yellow-light);"><i class="fa-solid fa-eye"></i></div>
                        <h3>Vision</h3>
                        <p>A future where science, sustainable finance, responsible investment, nature, agriculture, and international partnerships work together to create resilient communities and inclusive prosperity.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- At A Glance Section -->
    <section id="glance" class="bg-purple-tint">
        <div class="container">
            <div class="section-title">
                <h2>At a Glance</h2>
                <p>Connecting Local Potential With Global Opportunity</p>
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
                    <p>Carbon-credit development, climate finance, climate mitigation and adaptation, climate-smart agriculture, and climate resilience.</p>
                </div>
                <div class="glance-card">
                    <i class="fa-solid fa-tree"></i>
                    <h4>Nature & Biodiversity</h4>
                    <p>Biodiversity conservation, agroforestry, ecosystem restoration, regenerative agriculture, nature-based solutions, organic farming, aquaculture, and apiculture.</p>
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
    <section class="bg-white">
        <div class="container">
            <div class="section-title">
                <h2>Why Partner With Me?</h2>
                <p>Connecting Local Potential With Global Opportunity</p>
            </div>
            <p style="text-align: center; max-width: 900px; margin: 0 auto 3.2rem auto;">High-impact development opportunities require technical knowledge, local understanding, trusted relationships, project development capacity, implementation partnerships, and access to wider networks.</p>
            
            <div class="grid-3">
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-microscope"></i></div>
                    <h3>Scientific & Technical Expertise</h3>
                    <p>A foundation in animal science, breeding, genetics, genomics (GWAS), biometry, SAS/R data analytics, and sustainable production systems.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-temperature-arrow-up"></i></div>
                    <h3>Climate & Sustainability Knowledge</h3>
                    <p>Experience across climate mitigation, adaptation, climate-smart agriculture, biodiversity, agroforestry, ecosystem restoration, carbon markets, and climate finance.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-users"></i></div>
                    <h3>Community Perspective</h3>
                    <p>A strong focus on smallholder farmers, communities, youth, women, gender inclusiveness, sustainable livelihoods, and inclusive development.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-diagram-project"></i></div>
                    <h3>Project Development</h3>
                    <p>Proven track record translating ideas into structured projects, partnerships, MER frameworks, investment opportunities, and scalable initiatives.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-globe"></i></div>
                    <h3>International Partnership Orientation</h3>
                    <p>Commitment to building relationships with international foundations, donors, NGOs, investors, research institutions, companies, and development agencies.</p>
                </div>
                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-chart-line"></i></div>
                    <h3>Measurable Impact</h3>
                    <p>My approach integrates rigorous scientific research, investment, field implementation, and verified impact reporting.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Expertise Section -->
    <section id="expertise" class="bg-green-tint">
        <div class="container">
            <div class="section-title">
                <h2>Areas of Expertise</h2>
                <p>Multidisciplinary capability built over 8+ years of scientific research, academic instruction, and community development.</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <h4 style="color: var(--orange-main); font-size: 0.95rem; font-family: var(--font-display); font-weight: 700;">01</h4>
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
                    <h4 style="color: var(--orange-main); font-size: 0.95rem; font-family: var(--font-display); font-weight: 700;">02</h4>
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
                    <h4 style="color: var(--orange-main); font-size: 0.95rem; font-family: var(--font-display); font-weight: 700;">03</h4>
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
                    <h4 style="color: var(--orange-main); font-size: 0.95rem; font-family: var(--font-display); font-weight: 700;">04</h4>
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
                    <h4 style="color: var(--orange-main); font-size: 0.95rem; font-family: var(--font-display); font-weight: 700;">05</h4>
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
                    <h4 style="color: var(--orange-main); font-size: 0.95rem; font-family: var(--font-display); font-weight: 700;">06</h4>
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
                    <p>Developing approaches connecting climate action, adaptation, resilience, and sustainable finance to support communities facing climate-related challenges.</p>
                </div>
                <div class="card">
                    <h3>Carbon Markets & Climate Finance</h3>
                    <p>Connecting verified environmental outcomes with climate finance and carbon-market mechanisms while ensuring community benefits.</p>
                </div>
                <div class="card">
                    <h3>Biodiversity & Nature</h3>
                    <p>Supporting biodiversity conservation, agroforestry, ecosystem restoration, and nature-based solutions.</p>
                </div>
                <div class="card">
                    <h3>Sustainable Agriculture</h3>
                    <p>Advancing agricultural systems that improve productivity, climate resilience, food security, and environmental sustainability.</p>
                </div>
                <div class="card">
                    <h3>Livestock & Genetic Resources</h3>
                    <p>Applying science to strengthen livestock productivity, dairy farming, apiculture, genetic resources, and resilience.</p>
                </div>
                <div class="card">
                    <h3>Coffee & International Markets</h3>
                    <p>Connecting Ethiopia's agricultural potential with buyers, investors, markets, value-chain development, and trade opportunities.</p>
                </div>
                <div class="card">
                    <h3>Youth & Women's Economic Empowerment</h3>
                    <p>Creating meaningful opportunities for youth and women through skills, enterprise, agriculture, innovation, and sustainable livelihoods.</p>
                </div>
                <div class="card">
                    <h3>Community-Led Development</h3>
                    <p>Promoting development approaches placing communities at the center of planning, implementation, ownership, and sustainability.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Publications Section -->
    <section id="publications" class="bg-purple-tint">
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
                    <p style="font-size: 0.88rem; color: var(--purple-main);">Publisher: Taylor & Francis Group | DOI: 10.1080/09712119.2023.2185625</p>
                </div>

                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-book"></i></div>
                    <h4>Journal of Applied Animal Research (2023)</h4>
                    <p><strong>"Phenotypic characterization of indigenous sheep breeds in the Jimma Zone, Oromia, Ethiopia"</strong></p>
                    <p style="font-size: 0.88rem; color: var(--purple-main);">Authors: Yaregal Derbie & Hailu Tilahun | Publisher: Taylor & Francis Group</p>
                </div>

                <div class="card">
                    <div class="card-icon"><i class="fa-solid fa-book"></i></div>
                    <h4>IJRSAS (2019)</h4>
                    <p><strong>"Phenotypic Characterization of Indigenous Goats in North Shewa Zone, Amhara Region, Ethiopia"</strong></p>
                    <p style="font-size: 0.88rem; color: var(--purple-main);">Hailu Tilahun, Aynalem Haile, Ahmed Seid | Vol 5, Issue 7, pp. 44-55</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Strategic Projects -->
    <section id="projects" class="bg-white">
        <div class="container">
            <div class="section-title">
                <h2>Strategic Projects & Field Implementation</h2>
                <p>From Research Concepts to Field-Tested Initiatives</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <h3>01 — Climate & Carbon</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Carbon Credit Development & Climate Finance</li>
                        <li>Climate Mitigation & Adaptation Strategies</li>
                        <li>GTICDO Climate-Resilient Livelihoods</li>
                        <li>Climate-Smart Agriculture & Nature-Based Solutions</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>02 — Biodiversity & Ecosystem Restoration</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Biodiversity Conservation & Forest Protection</li>
                        <li>Agroforestry & Ecosystem Restoration</li>
                        <li>Organic Farming, Aquaculture & Apiculture</li>
                        <li>Community Conservation & Safeguarding</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>03 — Sustainable Agriculture & Livestock</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Salale University Honeybee Farm Establishment</li>
                        <li>North Shewa Model Cattle Crush Infrastructure</li>
                        <li>Dairy Feed Resource Evaluation & Synchronization</li>
                        <li>Animal Breeding & Smallholder Development</li>
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
                        <li>Youth Entrepreneurship & Green Jobs</li>
                        <li>Women's Economic Participation</li>
                        <li>Skills Development & Capacity Building</li>
                        <li>Sustainable Community Enterprise</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>06 — Research & Innovation</h3>
                    <p><strong>Projects focused on:</strong></p>
                    <ul class="green-bullets">
                        <li>Livestock Genomics & GWAS Applications</li>
                        <li>ANOVA, Regression & R Analytics (Holeta HARC)</li>
                        <li>Beekeeping Practice & Hive Tech Assessments</li>
                        <li>Evidence-Based Development Partnerships</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Partnerships Section -->
    <section id="partnerships" class="bg-green-tint">
        <div class="container">
            <div class="section-title">
                <h2>Partnership Opportunities</h2>
                <p>Building International Partnerships based on Trust, Transparency, Evidence, Inclusion, Innovation, Accountability, and Long-Term Impact.</p>
            </div>

            <div class="grid-4" style="margin-bottom: 3.2rem;">
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

            <h3 style="margin-bottom: 1.5rem; color: var(--purple-main);">Opportunity Focus & Partnership Types</h3>
            <div class="table-responsive" style="margin-bottom: 3.2rem;">
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
                            <td>Conservation, restoration, nature</td>
                            <td>Grant / Climate Finance</td>
                        </tr>
                        <tr>
                            <td><strong>Sustainable Agriculture</strong></td>
                            <td>Farmers, livestock, food systems</td>
                            <td>Grant / Investment</td>
                        </tr>
                        <tr>
                            <td><strong>Coffee</strong></td>
                            <td>Production, value chain, export</td>
                            <td>Investment / Trade</td>
                        </tr>
                        <tr>
                            <td><strong>Youth & Women</strong></td>
                            <td>Enterprise, skills, livelihoods</td>
                            <td>Grant / NGO Partnership</td>
                        </tr>
                        <tr>
                            <td><strong>Research</strong></td>
                            <td>Genetics, agriculture, climate</td>
                            <td>Research Grant / University Partnership</td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <h3 style="color: var(--purple-main);">Partnership Packages & Collaboration Models</h3>
            <div class="grid-3" style="margin-top: 1.5rem;">
                <div class="card">
                    <h4>1. Research Partnership</h4>
                    <p>Joint research, field studies, publications, data collection, and knowledge exchange.</p>
                </div>
                <div class="card">
                    <h4>2. Project Development Partnership</h4>
                    <p>Concept development, proposal writing, budgeting, technical design, and funding preparation.</p>
                </div>
                <div class="card">
                    <h4>3. Implementation Partnership</h4>
                    <p>Local coordination, community engagement, training, field implementation, and reporting.</p>
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
                    <p>Connecting Ethiopian agricultural products and sustainable enterprises with international buyers, investors, and markets.</p>
                </div>
            </div>

            <div class="process-flow">
                <div class="process-step"><i class="fa-solid fa-lightbulb"></i> Concept</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--yellow-main);"></i>
                <div class="process-step"><i class="fa-solid fa-pen-ruler"></i> Project Design</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--yellow-main);"></i>
                <div class="process-step"><i class="fa-solid fa-handshake"></i> Partnership</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--yellow-main);"></i>
                <div class="process-step"><i class="fa-solid fa-coins"></i> Financing</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--yellow-main);"></i>
                <div class="process-step"><i class="fa-solid fa-gears"></i> Implementation</div>
                <i class="fa-solid fa-chevron-right" style="color: var(--yellow-main);"></i>
                <div class="process-step"><i class="fa-solid fa-chart-line"></i> Monitoring & Impact</div>
            </div>
        </div>
    </section>

    <!-- Research Section -->
    <section id="research" class="bg-white">
        <div class="container">
            <div class="section-title">
                <h2>Research for Resilient Food Systems</h2>
                <p>Translating Evidence and Innovation into Field Solutions</p>
            </div>
            <div class="grid-2">
                <div class="card">
                    <h3>Core Research Intersection</h3>
                    <p>My research interests focus on the relationship between: <strong>Animal Science | Genetics | Agriculture | Climate Resilience | Biodiversity | Sustainable Land Use | Community Development</strong>.</p>
                    <p>The objective is to translate research, evidence, and innovation into practical solutions benefiting farmers, communities, institutions, businesses, and development partners.</p>
                </div>
                <div class="card">
                    <h3>Specific Research Interests</h3>
                    <ul class="green-bullets">
                        <li>Animal Breeding & Genetics (MSc Jimma University)</li>
                        <li>Livestock Genomics & GWAS Applications</li>
                        <li>Agricultural Innovation & Technology Transfer</li>
                        <li>Climate-Smart Agriculture & Agroecology</li>
                        <li>Sustainable Livestock Systems & Feed Resource Evaluation</li>
                        <li>Biodiversity & Genetic Resources Conservation</li>
                        <li>Climate Resilience & Humanitarian Development</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Consulting Services -->
    <section id="consulting" class="bg-purple-tint">
        <div class="container">
            <div class="section-title">
                <h2>Consultations for Organizations</h2>
                <p>We provide professional organizational and project development consulting services to support organizations, NGOs, CSOs, businesses, and community initiatives in turning ideas into practical, fundable, and sustainable programs.</p>
            </div>
            
            <div class="grid-3">
                <div class="card">
                    <h3>Documentation & Proposals</h3>
                    <ul class="green-bullets">
                        <li>Project Proposal Development</li>
                        <li>Concept Notes and Project Summaries</li>
                        <li>Grant and Donor Application Support</li>
                        <li>Partnership and Funding Proposals</li>
                        <li>Research and Technical Documentation</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Planning & Strategy</h3>
                    <ul class="green-bullets">
                        <li>Business Plans and Feasibility Studies</li>
                        <li>Strategic and Organizational Planning</li>
                        <li>Project Budgets and Financial Plans</li>
                        <li>Sustainability and Resource Mobilization Strategies</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Design, Data & Reports</h3>
                    <ul class="green-bullets">
                        <li>Data Collection & Statistical Analysis (SAS/R)</li>
                        <li>Program and Project Design</li>
                        <li>Monitoring, Evaluation, and Reporting (MER) Frameworks</li>
                        <li>Project Reports and Documentation</li>
                        <li>Organizational Profiles and Capability Statements</li>
                    </ul>
                </div>
            </div>

            <div class="card" style="margin-top: 2.8rem; background: var(--green-light); border-color: var(--green-main);">
                <h3>Transparency & Accountability Commitment</h3>
                <p>I am committed to professional standards of transparency, accountability, ethical conduct, responsible resource management, evidence-based decision-making, and measurable results. For funded projects and partnerships, appropriate documentation may include:</p>
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
    <section class="bg-white" style="padding: 4rem 3rem;">
        <div class="container" style="text-align: center;">
            <h3 style="color: var(--purple-main);">Geographic Focus</h3>
            <p style="font-size: 1.25rem; color: var(--green-main); font-weight: 700; margin-top: 0.5rem;">Ethiopia | East Africa | Africa | International</p>
            <p style="max-width: 900px; margin: 0.5rem auto 0 auto;">With Ethiopia as a primary base, I work with local and international partners to develop initiatives that can be implemented, tested, and scaled across communities and wider regional contexts.</p>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="bg-purple-tint">
        <div class="container">
            <div class="contact-card">
                <h2>Let's Build Sustainable Solutions Together</h2>
                <p>If you are a donor, foundation, grant maker, NGO, investor, development organization, researcher, government institution, or private-sector partner, I welcome the opportunity to explore collaboration.</p>
                
                <div class="contact-grid">
                    <div class="contact-method">
                        <i class="fa-solid fa-envelope"></i>
                        <div>
                            <div style="font-size: 0.85rem; color: var(--yellow-main); text-align: left;">Direct Email</div>
                            <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a>
                        </div>
                    </div>
                    <div class="contact-method">
                        <i class="fa-brands fa-whatsapp"></i>
                        <div>
                            <div style="font-size: 0.85rem; color: var(--yellow-main); text-align: left;">WhatsApp / Mobile</div>
                            <a href="https://wa.me/251910204390">+251 910 204 390</a>
                        </div>
                    </div>
                </div>

                <div class="social-title">Connect on Social Media</div>
                <div class="social-bar">
                    <a href="https://www.linkedin.com/in/hailu-kebede-292a07373" target="_blank" title="LinkedIn"><i class="fa-brands fa-linkedin-in"></i></a>
                    <a href="https://wa.me/251910204390" target="_blank" title="WhatsApp (hailu_tilahun.2026)"><i class="fa-brands fa-whatsapp"></i></a>
                    <a href="https://t.me/hailsh21" target="_blank" title="Telegram"><i class="fa-brands fa-telegram"></i></a>
                    <a href="https://accountscenter.facebook.com/profiles/100091523209816/" target="_blank" title="Facebook"><i class="fa-brands fa-facebook-f"></i></a>
                    <a href="https://x.com/Hailu_2025" target="_blank" title="X (Twitter)"><i class="fa-brands fa-x-twitter"></i></a>
                    <a href="https://www.instagram.com/hailsha21?stkn=dm9jMHYxa3poOGRt" target="_blank" title="Instagram"><i class="fa-brands fa-instagram"></i></a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2026 Hailu Tilahun Kebede. All Rights Reserved. | Addis Ababa, Ethiopia</p>
        </div>
    </footer>

</body>
</html>
