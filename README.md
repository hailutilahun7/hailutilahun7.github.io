<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hailu Tilahun Kebede | Agricultural Scientist & Sustainable Development Specialist</title>
    <!-- Google Fonts & Font Awesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Merriweather:ital,wght@0,300;0,400;0,700;1,300&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --primary: #1B4332;       /* Deep Forest Green */
            --primary-light: #2D6A4F; /* Sage Green */
            --accent: #D4A373;        /* Warm Gold/Earth */
            --accent-light: #FAEDCD;  /* Light Gold Tint */
            --dark: #1F2421;          /* Charcoal */
            --light: #F8F9FA;         /* Soft White */
            --gray: #6C757D;          /* Neutral Gray */
            --border: #E9ECEF;        /* Light Border */
            --font-heading: 'Merriweather', serif;
            --font-body: 'Inter', sans-serif;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: var(--font-body);
            color: var(--dark);
            background-color: #FFFFFF;
            line-height: 1.6;
        }

        /* Typography */
        h1, h2, h3, h4 {
            font-family: var(--font-heading);
            color: var(--primary);
            margin-bottom: 1rem;
        }

        p {
            margin-bottom: 1rem;
            color: #4A5568;
        }

        a {
            text-decoration: none;
            color: var(--primary-light);
            transition: all 0.3s ease;
        }

        a:hover {
            color: var(--primary);
        }

        /* Header & Navigation */
        header {
            position: sticky;
            top: 0;
            background: #FFFFFF;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            z-index: 1000;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        .logo {
            font-family: var(--font-heading);
            font-size: 1.25rem;
            font-weight: 700;
            color: var(--primary);
        }

        .nav-links {
            display: flex;
            gap: 1.5rem;
            list-style: none;
        }

        .nav-links a {
            font-size: 0.9rem;
            font-weight: 500;
            color: var(--dark);
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        .btn-primary {
            background-color: var(--primary);
            color: #FFFFFF !important;
            padding: 0.6rem 1.2rem;
            border-radius: 4px;
            font-weight: 500;
            display: inline-block;
        }

        .btn-primary:hover {
            background-color: var(--primary-light);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, rgba(27,67,50,0.95) 0%, rgba(45,106,79,0.9) 100%), url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&w=1600&q=80') center/cover;
            color: #FFFFFF;
            padding: 6rem 2rem;
            text-align: center;
        }

        .hero-content {
            max-width: 900px;
            margin: 0 auto;
        }

        .hero h1 {
            color: #FFFFFF;
            font-size: 2.8rem;
            margin-bottom: 1rem;
            line-height: 1.2;
        }

        .hero-subtitle {
            font-size: 1.2rem;
            color: var(--accent-light);
            font-weight: 600;
            margin-bottom: 1.5rem;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .hero p {
            color: #E2E8F0;
            font-size: 1.1rem;
            margin-bottom: 2rem;
        }

        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 1rem;
            flex-wrap: wrap;
        }

        .btn-accent {
            background-color: var(--accent);
            color: var(--dark) !important;
            padding: 0.75rem 1.5rem;
            border-radius: 4px;
            font-weight: 600;
        }

        .btn-outline {
            border: 2px solid #FFFFFF;
            color: #FFFFFF !important;
            padding: 0.75rem 1.5rem;
            border-radius: 4px;
            font-weight: 500;
        }

        /* Layout Structure */
        section {
            padding: 5rem 2rem;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .bg-light {
            background-color: var(--light);
        }

        .section-header {
            text-align: center;
            max-width: 700px;
            margin: 0 auto 3rem auto;
        }

        .section-header h2 {
            font-size: 2.2rem;
            position: relative;
            display: inline-block;
            margin-bottom: 0.5rem;
        }

        .section-header h2::after {
            content: '';
            display: block;
            width: 50px;
            height: 3px;
            background: var(--accent);
            margin: 0.5rem auto 0 auto;
        }

        /* Grid Systems */
        .grid-2 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2.5rem;
        }

        .grid-3 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        /* Feature & Card Designs */
        .card {
            background: #FFFFFF;
            border-radius: 8px;
            padding: 2rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.04);
            border: 1px solid var(--border);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px rgba(0,0,0,0.08);
        }

        .card-icon {
            font-size: 2rem;
            color: var(--primary-light);
            margin-bottom: 1rem;
        }

        /* Expertise Accordion / List Styling */
        .expertise-num {
            font-size: 0.9rem;
            font-weight: 700;
            color: var(--accent);
            margin-bottom: 0.5rem;
        }

        .pill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 1rem;
        }

        .pill {
            background: var(--light);
            border: 1px solid var(--border);
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.85rem;
            color: var(--dark);
        }

        /* At A Glance Horizontal Strip */
        .glance-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 1.5rem;
            text-align: center;
        }

        .glance-item {
            padding: 1.5rem;
            background: #FFFFFF;
            border-radius: 6px;
            border: 1px solid var(--border);
        }

        /* Table Design */
        .table-wrapper {
            overflow-x: auto;
            background: #FFFFFF;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.04);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            text-align: left;
        }

        th, td {
            padding: 1rem 1.5rem;
            border-bottom: 1px solid var(--border);
        }

        th {
            background-color: var(--primary);
            color: #FFFFFF;
            font-weight: 600;
        }

        /* Contact Section */
        .contact-box {
            background: var(--primary);
            color: #FFFFFF;
            border-radius: 12px;
            padding: 3rem;
            text-align: center;
        }

        .contact-box h2, .contact-box p {
            color: #FFFFFF;
        }

        .contact-links {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 2rem;
            flex-wrap: wrap;
        }

        .contact-item {
            color: #FFFFFF;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 1.1rem;
        }

        .contact-item a {
            color: var(--accent-light);
        }

        /* Footer */
        footer {
            background: var(--dark);
            color: #A0AEC0;
            padding: 2rem;
            text-align: center;
            font-size: 0.9rem;
        }

        /* Mobile Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none; /* Can be expanded with a JS toggle */
            }
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Navigation Header -->
    <header>
        <div class="nav-container">
            <a href="#" class="logo">HAILU TILAHUN KEBEDE</a>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#expertise">Expertise</a></li>
                <li><a href="#impact">Impact</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#partnerships">Partnerships</a></li>
                <li><a href="#research">Research</a></li>
            </ul>
            <a href="#contact" class="btn-primary">Contact</a>
        </div>
    </header>

    <!-- Hero / Home Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <p class="hero-subtitle">Agricultural Scientist | Researcher | Climate & Sustainable Development Specialist</p>
            <h1>Connecting Science, Nature, Finance & Markets for Sustainable Development</h1>
            <p>Working at the intersection of Scientific Research, Community Development, Carbon Finance, Biodiversity Conservation, and International Partnerships to advance practical solutions across Ethiopia and Africa.</p>
            <div class="hero-btns">
                <a href="#partnerships" class="btn-accent">Partner With Me</a>
                <a href="#projects" class="btn-outline">Explore Projects</a>
            </div>
        </div>
    </section>

    <!-- At A Glance Ribbon -->
    <section class="bg-light" style="padding: 2.5rem 2rem;">
        <div class="container">
            <div class="glance-grid">
                <div class="glance-item">
                    <i class="fa-solid fa-dna card-icon"></i>
                    <h4>Science & Genetics</h4>
                </div>
                <div class="glance-item">
                    <i class="fa-solid fa-cloud-sun card-icon"></i>
                    <h4>Climate & Carbon</h4>
                </div>
                <div class="glance-item">
                    <i class="fa-solid fa-leaf card-icon"></i>
                    <h4>Nature & Biodiversity</h4>
                </div>
                <div class="glance-item">
                    <i class="fa-solid fa-seedling card-icon"></i>
                    <h4>Agriculture & Food</h4>
                </div>
                <div class="glance-item">
                    <i class="fa-solid fa-mug-hot card-icon"></i>
                    <h4>Coffee & Trade</h4>
                </div>
                <div class="glance-item">
                    <i class="fa-solid fa-users card-icon"></i>
                    <h4>Inclusive Growth</h4>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <div class="container">
            <div class="grid-2" style="align-items: center;">
                <div>
                    <div class="section-header" style="text-align: left; margin: 0 0 1.5rem 0;">
                        <h2>From Science to Sustainable Impact</h2>
                    </div>
                    <p><strong>Hailu Tilahun Kebede</strong> is an Agricultural Scientist and Researcher with an MSc in Animal Breeding and Genetics and over eight years of experience in research, academic instruction, and community-based development.</p>
                    <p>His professional work connects: <strong>Science | Agriculture | Climate | Nature | Finance | Markets | Communities</strong>.</p>
                    <p>This multidisciplinary perspective supports the development of solutions addressing interconnected challenges including climate change, food security, biodiversity loss, agricultural productivity, sustainable livelihoods, and access to international markets.</p>
                </div>
                <div style="display: grid; gap: 1.5rem;">
                    <div class="card" style="border-left: 4px solid var(--primary);">
                        <h3>Mission</h3>
                        <p>To connect science, innovation, finance, partnerships, and communities to develop sustainable solutions that improve livelihoods, strengthen climate resilience, protect nature, and create long-term economic and social value.</p>
                    </div>
                    <div class="card" style="border-left: 4px solid var(--accent);">
                        <h3>Vision</h3>
                        <p>A future where science, sustainable finance, responsible investment, nature, agriculture, and international partnerships work together to create resilient communities and inclusive prosperity.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Expertise Section -->
    <section id="expertise" class="bg-light">
        <div class="container">
            <div class="section-header">
                <h2>Core Expertise</h2>
                <p>Technical, scientific, and strategic capabilities built over 8+ years.</p>
            </div>
            <div class="grid-3">
                
                <div class="card">
                    <div class="expertise-num">01</div>
                    <h3>Livestock Science & Farming</h3>
                    <div class="pill-list">
                        <span class="pill">Livestock Management</span>
                        <span class="pill">Dairy, Beef, Sheep & Poultry</span>
                        <span class="pill">Animal Nutrition & Feed</span>
                        <span class="pill">Breeding & Herd Improvement</span>
                        <span class="pill">Pasture & Forage</span>
                        <span class="pill">Integrated Crop-Livestock</span>
                    </div>
                </div>

                <div class="card">
                    <div class="expertise-num">02</div>
                    <h3>Climate, Carbon & Finance</h3>
                    <div class="pill-list">
                        <span class="pill">Carbon Credit Development</span>
                        <span class="pill">Climate Finance</span>
                        <span class="pill">Mitigation & Adaptation</span>
                        <span class="pill">Climate-Smart Agriculture</span>
                        <span class="pill">Climate-Resilient Development</span>
                    </div>
                </div>

                <div class="card">
                    <div class="expertise-num">03</div>
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
                    <div class="expertise-num">04</div>
                    <h3>Agriculture & Food Systems</h3>
                    <div class="pill-list">
                        <span class="pill">Agroecology</span>
                        <span class="pill">Food System Resilience</span>
                        <span class="pill">Agricultural Value Chains</span>
                        <span class="pill">Community Production</span>
                        <span class="pill">Sustainable Livelihoods</span>
                    </div>
                </div>

                <div class="card">
                    <div class="expertise-num">05</div>
                    <h3>Coffee & International Trade</h3>
                    <div class="pill-list">
                        <span class="pill">Sustainable Coffee Production</span>
                        <span class="pill">Coffee Export</span>
                        <span class="pill">International Market Linkage</span>
                        <span class="pill">Agricultural Investment</span>
                    </div>
                </div>

                <div class="card">
                    <div class="expertise-num">06</div>
                    <h3>Consulting & Project Design</h3>
                    <div class="pill-list">
                        <span class="pill">Proposal & Grant Writing</span>
                        <span class="pill">Concept Notes & Budgets</span>
                        <span class="pill">MEL Frameworks</span>
                        <span class="pill">Feasibility Studies</span>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Impact Areas Section -->
    <section id="impact">
        <div class="container">
            <div class="section-header">
                <h2>Areas of Impact</h2>
                <p>Translating research, data, and policy into measurable field outcomes.</p>
            </div>
            <div class="grid-2">
                <div class="card">
                    <h4>Climate Action & Carbon Markets</h4>
                    <p>Connecting verified environmental outcomes with responsible climate finance and carbon-market mechanisms while ensuring local community benefits.</p>
                </div>
                <div class="card">
                    <h4>Biodiversity & Ecosystem Restoration</h4>
                    <p>Supporting landscape restoration, agroforestry systems, and nature-based solutions across vulnerable regional contexts.</p>
                </div>
                <div class="card">
                    <h4>Sustainable Agriculture & Livestock Genetics</h4>
                    <p>Applying science to strengthen livestock productivity, dairy farming, honeybee production, and genetic resource conservation.</p>
                </div>
                <div class="card">
                    <h4>Coffee & Global Market Access</h4>
                    <p>Connecting Ethiopia’s agricultural potential directly with international buyers, investors, and sustainable trade opportunities.</p>
                </div>
                <div class="card">
                    <h4>Youth & Women’s Empowerment</h4>
                    <p>Creating sustainable pathways for economic participation through skills, green enterprise, and agricultural innovation.</p>
                </div>
                <div class="card">
                    <h4>Community-Led Development</h4>
                    <p>Placing local communities at the core of project planning, implementation, ownership, and long-term sustainability.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Strategic Projects -->
    <section id="projects" class="bg-light">
        <div class="container">
            <div class="section-header">
                <h2>Strategic Projects</h2>
                <p>From Ideas to Investable and Fundable Initiatives</p>
            </div>
            <div class="grid-3">
                <div class="card">
                    <h3>01. Climate & Carbon</h3>
                    <p>Development of carbon credit initiatives, climate-smart agriculture programs, and nature-based climate adaptation systems.</p>
                </div>
                <div class="card">
                    <h3>02. Biodiversity & Nature</h3>
                    <p>Forest and landscape restoration, community conservation initiatives, and integrated agroforestry development.</p>
                </div>
                <div class="card">
                    <h3>03. Sustainable Livestock</h3>
                    <p>Smallholder genetic improvement, climate-resilient animal feed production, and sustainable food system models.</p>
                </div>
                <div class="card">
                    <h3>04. Coffee Value Chains</h3>
                    <p>Quality improvement, sustainable certification, international market linkage, and export pipeline development.</p>
                </div>
                <div class="card">
                    <h3>05. Inclusive Enterprise</h3>
                    <p>Youth entrepreneurship hubs, green job creation, and women's economic participation in agriculture.</p>
                </div>
                <div class="card">
                    <h3>06. Research Consortia</h3>
                    <p>Joint academic studies on animal breeding, genomics, GWAS, climate adaptation, and technology transfer.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Partnerships Matrix -->
    <section id="partnerships">
        <div class="container">
            <div class="section-header">
                <h2>Partnership Opportunities</h2>
                <p>Building trusted international collaborations across Ethiopia and East Africa.</p>
            </div>

            <div class="table-wrapper" style="margin-bottom: 3rem;">
                <table>
                    <thead>
                        <tr>
                            <th>Opportunity Focus</th>
                            <th>Key Objectives</th>
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
                            <td>Smallholder resilience, livestock improvement, food systems</td>
                            <td>Grant / Investment</td>
                        </tr>
                        <tr>
                            <td><strong>Coffee & Trade</strong></td>
                            <td>Sustainable production, value-chain development, export</td>
                            <td>Investment / Trade</td>
                        </tr>
                        <tr>
                            <td><strong>Youth & Women</strong></td>
                            <td>Enterprise, green jobs, skills, livelihoods</td>
                            <td>Grant / NGO Partnership</td>
                        </tr>
                        <tr>
                            <td><strong>Research & Innovation</strong></td>
                            <td>Genetics, genomics, climate impacts, field studies</td>
                            <td>Research Grant / University</td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <!-- Partnership Models Grid -->
            <h3 style="text-align: center; margin-bottom: 2rem;">Collaborative Models</h3>
            <div class="grid-3">
                <div class="card">
                    <h4>Research Partnership</h4>
                    <p>Joint studies, field trials, publications, and scientific data exchange.</p>
                </div>
                <div class="card">
                    <h4>Project Design & Grants</h4>
                    <p>Concept development, proposal writing, budgeting, and donor applications.</p>
                </div>
                <div class="card">
                    <h4>Implementation</h4>
                    <p>Local coordination, community engagement, training, and field operations.</p>
                </div>
                <div class="card">
                    <h4>Investment Partnership</h4>
                    <p>Responsible investment in scalable carbon, agriculture, and coffee projects.</p>
                </div>
                <div class="card">
                    <h4>Technical Support</h4>
                    <p>Scientific expertise, MEL frameworks, and technology transfer.</p>
                </div>
                <div class="card">
                    <h4>Market Access</h4>
                    <p>Connecting agricultural producers with international market networks.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Research Focus -->
    <section id="research" class="bg-light">
        <div class="container">
            <div class="section-header">
                <h2>Research & Evidence</h2>
                <p>Translating scientific research into practical solutions for resilient communities.</p>
            </div>
            <div class="grid-2">
                <div class="card">
                    <h3>Research Focus Areas</h3>
                    <ul style="padding-left: 1.2rem; color: #4A5568;">
                        <li style="margin-bottom: 0.5rem;">Animal Breeding & Livestock Genetics</li>
                        <li style="margin-bottom: 0.5rem;">Livestock Genomics & GWAS Applications</li>
                        <li style="margin-bottom: 0.5rem;">Climate-Smart Agriculture & Agroecology</li>
                        <li style="margin-bottom: 0.5rem;">Genetic Resource Conservation</li>
                        <li style="margin-bottom: 0.5rem;">Sustainable Livestock Production Systems</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>Organizational Consulting Services</h3>
                    <p>We assist civil society organizations, NGOs, and businesses in turning ideas into fundable, sustainable programs:</p>
                    <div class="pill-list">
                        <span class="pill">Project Proposals</span>
                        <span class="pill">Logical Frameworks</span>
                        <span class="pill">Financial Plans</span>
                        <span class="pill">MEL Frameworks</span>
                        <span class="pill">Feasibility Studies</span>
                        <span class="pill">Impact Reports</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <div class="contact-box">
                <h2>Let's Build Sustainable Solutions Together</h2>
                <p style="max-width: 600px; margin: 1rem auto;">Whether you are an international donor, foundation, impact investor, research institution, or development agency, I welcome the opportunity to explore partnership.</p>
                
                <div class="contact-links">
                    <div class="contact-item">
                        <i class="fa-solid fa-envelope"></i>
                        <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a>
                    </div>
                    <div class="contact-item">
                        <i class="fa-brands fa-whatsapp"></i>
                        <a href="https://wa.me/251910204390">+251 910 204 390</a>
                    </div>
                    <div class="contact-item">
                        <i class="fa-solid fa-location-dot"></i>
                        <span>Addis Ababa, Ethiopia</span>
                    </div>
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
