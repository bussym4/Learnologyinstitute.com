<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Learnology Institute | Industrial OJT & Chemical Analysis Training</title>
  <meta name="description" content="Professional On-the-Job Training (OJT) in Chemical Analysis for B.Sc & M.Sc students. Coal, Water, Lubricant Oil, and Agricultural Soil Testing.">
  
  <!-- Google Fonts & FontAwesome Icons -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

  <style>
    :root {
      --primary: #137A8B;
      --primary-dark: #0d5a67;
      --accent: #E8604A;
      --accent-hover: #d34f3a;
      --dark: #1E293B;
      --gray-light: #F8FAFC;
      --gray-border: #E2E8F0;
      --text-muted: #64748B;
      --white: #ffffff;
      --shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.08), 0 8px 10px -6px rgba(0, 0, 0, 0.04);
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Plus Jakarta Sans', sans-serif;
    }

    body {
      background-color: var(--gray-light);
      color: var(--dark);
      line-height: 1.6;
    }

    /* --- Navigation Bar --- */
    .navbar {
      background: var(--white);
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.05);
      border-bottom: 3px solid var(--primary);
    }

    .nav-container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 1rem 1.5rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .brand-logo {
      display: flex;
      align-items: center;
      gap: 12px;
      text-decoration: none;
    }

    .logo-icon-svg {
      width: 48px;
      height: 48px;
    }

    .brand-text h1 {
      font-size: 1.35rem;
      font-weight: 800;
      color: var(--primary);
      line-height: 1.1;
      letter-spacing: 0.5px;
    }

    .brand-text span {
      font-size: 0.75rem;
      color: var(--text-muted);
      letter-spacing: 1.5px;
      text-transform: uppercase;
      font-weight: 600;
      display: block;
    }

    .nav-links {
      display: flex;
      gap: 1.8rem;
      list-style: none;
      align-items: center;
    }

    .nav-links a {
      text-decoration: none;
      color: var(--dark);
      font-weight: 600;
      font-size: 0.95rem;
      transition: color 0.2s;
    }

    .nav-links a:hover {
      color: var(--accent);
    }

    .nav-cta {
      background: var(--accent);
      color: var(--white) !important;
      padding: 0.6rem 1.2rem;
      border-radius: 6px;
      transition: background 0.2s;
    }

    .nav-cta:hover {
      background: var(--accent-hover) !important;
    }

    /* --- Hero Section --- */
    .hero {
      background: linear-gradient(135deg, rgba(19, 122, 139, 0.08) 0%, rgba(232, 96, 74, 0.05) 100%);
      padding: 5rem 1.5rem 4rem;
      border-bottom: 1px solid var(--gray-border);
    }

    .hero-container {
      max-width: 1200px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 3rem;
      align-items: center;
    }

    .badge {
      display: inline-block;
      background: rgba(19, 122, 139, 0.12);
      color: var(--primary);
      padding: 0.35rem 0.85rem;
      border-radius: 20px;
      font-size: 0.82rem;
      font-weight: 700;
      text-transform: uppercase;
      margin-bottom: 1rem;
    }

    .hero h2 {
      font-size: 2.75rem;
      font-weight: 800;
      color: var(--dark);
      line-height: 1.2;
      margin-bottom: 1.2rem;
    }

    .hero h2 span {
      color: var(--primary);
    }

    .hero p {
      font-size: 1.1rem;
      color: var(--text-muted);
      margin-bottom: 2rem;
    }

    .hero-actions {
      display: flex;
      gap: 1rem;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 0.85rem 1.6rem;
      border-radius: 6px;
      text-decoration: none;
      font-weight: 700;
      font-size: 0.95rem;
      transition: all 0.2s;
    }

    .btn-primary {
      background: var(--accent);
      color: var(--white);
    }

    .btn-primary:hover {
      background: var(--accent-hover);
      box-shadow: 0 4px 12px rgba(232, 96, 74, 0.3);
    }

    .btn-secondary {
      background: var(--white);
      color: var(--primary);
      border: 2px solid var(--primary);
    }

    .btn-secondary:hover {
      background: var(--primary);
      color: var(--white);
    }

    .hero-visual {
      background: var(--white);
      padding: 2.5rem;
      border-radius: 12px;
      box-shadow: var(--shadow);
      border: 1px solid var(--gray-border);
      position: relative;
    }

    .hero-visual ul {
      list-style: none;
      margin-top: 1rem;
    }

    .hero-visual li {
      padding: 0.75rem 0;
      display: flex;
      align-items: center;
      gap: 12px;
      border-bottom: 1px solid var(--gray-border);
      font-size: 0.95rem;
      font-weight: 600;
    }

    .hero-visual li:last-child {
      border-bottom: none;
    }

    .hero-visual i {
      color: var(--accent);
    }

    /* --- Training Modules Grid --- */
    .section {
      padding: 5rem 1.5rem;
      max-width: 1200px;
      margin: 0 auto;
    }

    .section-title {
      text-align: center;
      margin-bottom: 3.5rem;
    }

    .section-title h3 {
      font-size: 2rem;
      font-weight: 800;
      color: var(--dark);
    }

    .section-title p {
      color: var(--text-muted);
      font-size: 1rem;
      margin-top: 0.5rem;
    }

    .modules-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 1.8rem;
    }

    .module-card {
      background: var(--white);
      border-radius: 10px;
      padding: 2rem;
      border: 1px solid var(--gray-border);
      box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05);
      transition: transform 0.2s, box-shadow 0.2s, border-color 0.2s;
      position: relative;
      display: flex;
      flex-direction: column;
    }

    .module-card:hover {
      transform: translateY(-5px);
      box-shadow: var(--shadow);
      border-color: var(--primary);
    }

    .icon-box {
      width: 55px;
      height: 55px;
      border-radius: 8px;
      background: rgba(19, 122, 139, 0.1);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
      color: var(--primary);
      margin-bottom: 1.2rem;
    }

    .module-card h4 {
      font-size: 1.2rem;
      margin-bottom: 0.8rem;
      color: var(--dark);
    }

    .module-card p {
      font-size: 0.9rem;
      color: var(--text-muted);
      margin-bottom: 1.2rem;
      flex-grow: 1;
    }

    .card-tags {
      font-size: 0.8rem;
      font-weight: 700;
      color: var(--accent);
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    /* --- Training Highlights / OJT Section --- */
    .highlights-section {
      background: var(--white);
      border-top: 1px solid var(--gray-border);
      border-bottom: 1px solid var(--gray-border);
    }

    .highlights-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 2rem;
      margin-top: 2rem;
    }

    .highlight-item {
      text-align: center;
      padding: 1.5rem;
    }

    .highlight-item i {
      font-size: 2.2rem;
      color: var(--accent);
      margin-bottom: 1rem;
    }

    .highlight-item h5 {
      font-size: 1.1rem;
      margin-bottom: 0.5rem;
    }

    .highlight-item p {
      font-size: 0.9rem;
      color: var(--text-muted);
    }

    /* --- Contact & Application Form --- */
    .contact-container {
      background: var(--white);
      border-radius: 12px;
      border: 1px solid var(--gray-border);
      box-shadow: var(--shadow);
      display: grid;
      grid-template-columns: 1fr 1.2fr;
      overflow: hidden;
    }

    .contact-info {
      background: linear-gradient(145deg, var(--primary) 0%, var(--primary-dark) 100%);
      color: var(--white);
      padding: 3rem 2.5rem;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .contact-info h3 {
      font-size: 1.8rem;
      margin-bottom: 1rem;
    }

    .contact-item {
      display: flex;
      align-items: center;
      gap: 15px;
      margin-top: 1.5rem;
      font-size: 0.95rem;
    }

    .contact-item i {
      font-size: 1.2rem;
      color: var(--accent);
      background: rgba(255,255,255,0.1);
      padding: 10px;
      border-radius: 50%;
    }

    .contact-form-area {
      padding: 3rem 2.5rem;
    }

    .contact-form-area h4 {
      font-size: 1.4rem;
      margin-bottom: 1.5rem;
      color: var(--dark);
    }

    .form-group {
      margin-bottom: 1.2rem;
    }

    .form-group label {
      display: block;
      font-size: 0.85rem;
      font-weight: 700;
      color: var(--dark);
      margin-bottom: 0.4rem;
    }

    .form-group input, 
    .form-group select, 
    .form-group textarea {
      width: 100%;
      padding: 0.75rem 0.9rem;
      border: 1px solid var(--gray-border);
      border-radius: 6px;
      font-size: 0.9rem;
      color: var(--dark);
      outline: none;
      transition: border-color 0.2s;
    }

    .form-group input:focus, 
    .form-group select:focus, 
    .form-group textarea:focus {
      border-color: var(--primary);
    }

    .submit-btn {
      width: 100%;
      background: var(--accent);
      color: var(--white);
      border: none;
      padding: 0.85rem;
      font-size: 1rem;
      font-weight: 700;
      border-radius: 6px;
      cursor: pointer;
      transition: background 0.2s;
    }

    .submit-btn:hover {
      background: var(--accent-hover);
    }

    /* --- Footer --- */
    footer {
      background: var(--dark);
      color: #94A3B8;
      padding: 2.5rem 1.5rem;
      text-align: center;
      font-size: 0.9rem;
    }

    footer a {
      color: var(--accent);
      text-decoration: none;
    }

    /* --- Responsive --- */
    @media (max-width: 900px) {
      .hero-container, .contact-container {
        grid-template-columns: 1fr;
      }
      .nav-links {
        display: none;
      }
      .hero h2 {
        font-size: 2.1rem;
      }
    }/* --- Detailed Testing Modules & Tables --- */
    .module-card-detailed {
      background: var(--white);
      border-radius: 12px;
      border: 1px solid var(--gray-border);
      box-shadow: var(--shadow);
      margin-bottom: 2.5rem;
      overflow: hidden;
      border-left: 6px solid var(--primary);
    }

    .card-top {
      padding: 1.5rem 2rem;
      background: #fafcfe;
      border-bottom: 1px solid var(--gray-border);
      display: flex;
      align-items: center;
      gap: 1.2rem;
    }

    .card-icon {
      width: 52px;
      height: 52px;
      border-radius: 10px;
      background: rgba(19, 122, 139, 0.1);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
      color: var(--primary);
      flex-shrink: 0;
    }

    .card-title-group h4 {
      font-size: 1.35rem;
      font-weight: 800;
      color: var(--dark);
    }

    .card-title-group span {
      font-size: 0.8rem;
      font-weight: 700;
      color: var(--accent);
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    .card-body {
      padding: 1.8rem 2rem;
    }

    .importance-box {
      background: #FFFBF7;
      border: 1px solid #FFE6D8;
      border-left: 4px solid var(--accent);
      border-radius: 6px;
      padding: 0.9rem 1.1rem;
      margin-bottom: 1.5rem;
    }

    .importance-box h5 {
      font-size: 0.95rem;
      font-weight: 700;
      color: #9C3826;
      margin-bottom: 0.3rem;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .importance-box p {
      font-size: 0.9rem;
      color: #475569;
      margin: 0;
    }

    .table-responsive {
      width: 100%;
      overflow-x: auto;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      text-align: left;
      font-size: 0.9rem;
    }

    th {
      background: #F1F5F9;
      color: var(--dark);
      padding: 0.8rem 1rem;
      font-weight: 700;
      border-bottom: 2px solid var(--gray-border);
      text-transform: uppercase;
      font-size: 0.78rem;
      letter-spacing: 0.5px;
    }

    td {
      padding: 0.9rem 1rem;
      border-bottom: 1px solid var(--gray-border);
      vertical-align: top;
    }

    tr:last-child td {
      border-bottom: none;
    }

    tr:hover td {
      background-color: #f8fafc;
    }

    .param-name {
      font-weight: 700;
      color: var(--dark);
      display: block;
    }

    .param-sub {
      font-size: 0.8rem;
      color: var(--text-muted);
    }

    .method-tag {
      display: inline-block;
      background: #E2E8F0;
      color: #334155;
      padding: 0.2rem 0.5rem;
      border-radius: 4px;
      font-size: 0.75rem;
      font-weight: 600;
      margin-top: 3px;
    }

    .instrument-name {
      color: var(--primary);
      font-weight: 600;
    }
  </style>
</head>
<body>

  <!-- Top Navigation -->
  <nav class="navbar">
    <div class="nav-container">
      <a href="#" class="brand-logo">
        <!-- Exact Vector Recreation of your Learnology Logo -->
        <svg class="logo-icon-svg" viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
          <!-- Open Book Base -->
          <path d="M50 78C42 75 25 73 15 76V57C25 54 42 56 50 60C58 56 75 54 85 57V76C75 73 58 75 50 78Z" fill="#137A8B" fill-opacity="0.15"/>
          <path d="M50 78V60M15 76C25 73 42 75 50 78C58 75 75 73 85 76M15 67C25 64 42 66 50 70C58 66 75 64 85 67M15 57C25 54 42 56 50 60C58 56 75 54 85 57" stroke="#137A8B" stroke-width="2.5" stroke-linecap="round"/>
          
          <!-- Atom Orbit / Orbital Ring -->
          <ellipse cx="50" cy="45" rx="20" ry="18" stroke="#E8604A" stroke-width="2" stroke-dasharray="2 1" />
          
          <!-- Conical Flask -->
          <path d="M47 30H53V38L62 53C63 54.5 62 56.5 60 56.5H40C38 56.5 37 54.5 38 53L47 38V30Z" stroke="#137A8B" stroke-width="2.5" stroke-linejoin="round"/>
          <path d="M45 28H55" stroke="#137A8B" stroke-width="2.5" stroke-linecap="round"/>
          
          <!-- Liquid Drop & Chemistry Nodes -->
          <circle cx="50" cy="48" r="2" fill="#137A8B"/>
          <circle cx="50" cy="24" r="3" fill="#E8604A"/>
          <circle cx="33" cy="42" r="3" fill="#137A8B"/>
          <circle cx="67" cy="42" r="3" fill="#E8604A"/>
          <circle cx="50" cy="56" r="2.5" fill="#E8604A"/>
        </svg>

        <div class="brand-text">
          <h1>LEARNOLOGY</h1>
          <span>INSTITUTE</span>
        </div>
      </a>

      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#modules">Training Modules</a></li>
        <li><a href="#ojt">OJT Program</a></li>
        <li><a href="#apply" class="nav-cta">Apply for Training</a></li>
      </ul>
    </div>
  </nav>

  <!-- Hero Section -->
  <header class="hero" id="about">
    <div class="hero-container">
      <div>
        <span class="badge"><i class="fa-solid fa-flask-vial"></i> Bridging Academics & Industrial Labs</span>
        <h2>Master Hands-On <span>Chemical Analysis</span> & Industrial OJT</h2>
        <p>Specialized industrial training tailored for <strong>B.Sc., M.Sc. students, and fresh graduates</strong>. Get trained on actual equipment, standard testing protocols (IS/ASTM/APHA), and practical wet-lab analysis.</p>
        <div class="hero-actions">
          <a href="#apply" class="btn btn-primary"><i class="fa-solid fa-user-graduate"></i> Register for Batch</a>
          <a href="#modules" class="btn btn-secondary">Explore Modules</a>
        </div>
      </div>

      <div class="hero-visual">
        <h4 style="color: var(--primary); font-weight: 800; font-size: 1.15rem; margin-bottom: 0.5rem;">
          <i class="fa-solid fa-award" style="color: var(--accent);"></i> Industry-Grade Skillset
        </h4>
        <p style="font-size: 0.85rem; color: var(--text-muted);">Trained strictly according to commercial QA/QC laboratory routines.</p>
        <ul>
          <li><i class="fa-solid fa-check-circle"></i> Coal Proximate & Calorific Value Analysis</li>
          <li><i class="fa-solid fa-check-circle"></i> Potable & Effluent Water Testing (BOD/COD/Hardness)</li>
          <li><i class="fa-solid fa-check-circle"></i> Lubricant Oil Viscosity, Flash Point & Acidity</li>
          <li><i class="fa-solid fa-check-circle"></i> Agricultural Soil Fertility & Micronutrient Profiling</li>
        </ul>
      </div>
    </div>
  </header>

  <!-- Modules Section -->
 <!-- Detailed Modules Section -->
  <section class="section" id="modules">
    <div class="section-title">
      <span class="badge">Curriculum & Methodology</span>
      <h3>Core Laboratory Training Modules</h3>
      <p>Hands-on testing procedures, industrial significance, standard protocols, and instrumentation.</p>
    </div>

    <!-- 1. WATER & WASTEWATER -->
    <div class="module-card-detailed">
      <div class="card-top">
        <div class="card-icon"><i class="fa-solid fa-droplet"></i></div>
        <div class="card-title-group">
          <span>Module 01</span>
          <h4>Water & Wastewater Quality Analysis</h4>
        </div>
      </div>
      <div class="card-body">
        <div class="importance-box">
          <h5><i class="fa-solid fa-circle-exclamation"></i> Why Testing Is Important:</h5>
          <p>Determines drinking water safety, industrial boiler compatibility to prevent scaling/corrosion, and statutory compliance with environmental discharge regulations (CPCB/SPCB).</p>
        </div>
        <div class="table-responsive">
          <table>
            <thead>
              <tr>
                <th style="width: 25%;">Testing Parameter</th>
                <th style="width: 30%;">Standard Test Method</th>
                <th style="width: 25%;">Analytical Instrument Used</th>
                <th style="width: 20%;">Standard Code</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td><span class="param-name">pH & Conductivity / TDS</span><span class="param-sub">Acidity, alkalinity & dissolved ions</span></td>
                <td>Electrometric & Potentiometric measurement</td>
                <td><span class="instrument-name">Digital pH Meter & Conductivity Meter</span></td>
                <td><span class="method-tag">IS 3025 (P: 11 & 14)</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Total Hardness (Ca & Mg)</span><span class="param-sub">Scale-forming mineral evaluation</span></td>
                <td>EDTA Complexometric Titration (EBT indicator)</td>
                <td><span class="instrument-name">Volumetric Titration Station</span></td>
                <td><span class="method-tag">IS 3025 (Part 21)</span></td>
              </tr>
              <tr>
                <td><span class="param-name">BOD (5-Day @ 20°C)</span><span class="param-sub">Biochemical oxygen demand</span></td>
                <td>Winkler Azide Method / DO depletion test</td>
                <td><span class="instrument-name">B.O.D. Incubator & DO Meter</span></td>
                <td><span class="method-tag">IS 3025 (Part 44)</span></td>
              </tr>
              <tr>
                <td><span class="param-name">COD (Chemical Oxygen Demand)</span><span class="param-sub">Total chemically oxidizable load</span></td>
                <td>Closed/Open Reflux Digest with Potassium Dichromate</td>
                <td><span class="instrument-name">COD Digester Block & Titrator</span></td>
                <td><span class="method-tag">APHA 5220 / IS 3025</span></td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

    <!-- 2. AGRICULTURAL SOIL -->
    <div class="module-card-detailed">
      <div class="card-top">
        <div class="card-icon"><i class="fa-solid fa-seedling"></i></div>
        <div class="card-title-group">
          <span>Module 02</span>
          <h4>Agricultural Soil Testing & Fertility Profiling</h4>
        </div>
      </div>
      <div class="card-body">
        <div class="importance-box">
          <h5><i class="fa-solid fa-circle-exclamation"></i> Why Testing Is Important:</h5>
          <p>Provides critical diagnostic data on soil health, macronutrient levels, and salinity to optimize crop yield and formulate precise fertilizer dosage.</p>
        </div>
        <div class="table-responsive">
          <table>
            <thead>
              <tr>
                <th style="width: 25%;">Testing Parameter</th>
                <th style="width: 30%;">Standard Test Method</th>
                <th style="width: 25%;">Analytical Instrument Used</th>
                <th style="width: 20%;">Standard Code</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td><span class="param-name">pH & Electrical Conductivity</span><span class="param-sub">Salinity and nutrient availability</span></td>
                <td>1:2 soil-water suspension potentiometry</td>
                <td><span class="instrument-name">Soil pH & EC Analyzer</span></td>
                <td><span class="method-tag">IS 2720 (Part 26)</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Organic Carbon (OC)</span><span class="param-sub">Soil fertility & organic matter</span></td>
                <td>Walkley-Black Wet Dichromate Oxidation</td>
                <td><span class="instrument-name">Volumetric Titration Setup</span></td>
                <td><span class="method-tag">ICAR Manual</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Available Nitrogen (N)</span><span class="param-sub">Vegetative growth nutrient</span></td>
                <td>Alkaline Permanganate Distillation</td>
                <td><span class="instrument-name">Kjeldahl Distillation Unit</span></td>
                <td><span class="method-tag">Subbiah & Asija</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Available Phosphorus & Potassium</span><span class="param-sub">P & K macronutrients</span></td>
                <td>Olsen's extraction & Ammonium Acetate extraction</td>
                <td><span class="instrument-name">Spectrophotometer & Flame Photometer</span></td>
                <td><span class="method-tag">IS 10158 / Jackson</span></td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

    <!-- 3. COAL & SOLID FUELS -->
    <div class="module-card-detailed">
      <div class="card-top">
        <div class="card-icon"><i class="fa-solid fa-fire-flame-simple"></i></div>
        <div class="card-title-group">
          <span>Module 03</span>
          <h4>Coal, Coke & Solid Fuel Testing</h4>
        </div>
      </div>
      <div class="card-body">
        <div class="importance-box">
          <h5><i class="fa-solid fa-circle-exclamation"></i> Why Testing Is Important:</h5>
          <p>Thermal power plant efficiency, kiln operation, and commercial fuel pricing directly depend on calorific heating value and non-combustible ash content.</p>
        </div>
        <div class="table-responsive">
          <table>
            <thead>
              <tr>
                <th style="width: 25%;">Testing Parameter</th>
                <th style="width: 30%;">Standard Test Method</th>
                <th style="width: 25%;">Analytical Instrument Used</th>
                <th style="width: 20%;">Standard Code</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td><span class="param-name">Total & Inherent Moisture</span><span class="param-sub">Transport & combustion penalty</span></td>
                <td>Oven drying at 105°C–110°C under nitrogen/air</td>
                <td><span class="instrument-name">Hot Air Laboratory Oven & Balance</span></td>
                <td><span class="method-tag">IS 1350 (P:1) / ASTM D3173</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Ash Content</span><span class="param-sub">Inorganic residue percentage</span></td>
                <td>Controlled incineration in air at 815°C ± 10°C</td>
                <td><span class="instrument-name">High-Temp Muffle Furnace</span></td>
                <td><span class="method-tag">IS 1350 (P:1) / ASTM D3174</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Volatile Matter (VM)</span><span class="param-sub">Flame reactivity and ignition</span></td>
                <td>Pyrolysis without air contact at 900°C for 7 mins</td>
                <td><span class="instrument-name">VM Furnace & Cylindrical Crucible</span></td>
                <td><span class="method-tag">IS 1350 (P:1) / ASTM D3175</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Gross Calorific Value (GCV)</span><span class="param-sub">Direct energy/thermal output</span></td>
                <td>High-pressure oxygen bomb combustion</td>
                <td><span class="instrument-name">Oxygen Bomb Calorimeter</span></td>
                <td><span class="method-tag">IS 1350 (P:2) / ASTM D5865</span></td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

    <!-- 4. LUBRICATING OIL -->
    <div class="module-card-detailed">
      <div class="card-top">
        <div class="card-icon"><i class="fa-solid fa-oil-can"></i></div>
        <div class="card-title-group">
          <span>Module 04</span>
          <h4>Lubricating & Industrial Oil Testing</h4>
        </div>
      </div>
      <div class="card-body">
        <div class="importance-box">
          <h5><i class="fa-solid fa-circle-exclamation"></i> Why Testing Is Important:</h5>
          <p>Prevents severe equipment wear and failure by detecting oil degradation, viscosity shifts, acidity buildup, and water contamination.</p>
        </div>
        <div class="table-responsive">
          <table>
            <thead>
              <tr>
                <th style="width: 25%;">Testing Parameter</th>
                <th style="width: 30%;">Standard Test Method</th>
                <th style="width: 25%;">Analytical Instrument Used</th>
                <th style="width: 20%;">Standard Code</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td><span class="param-name">Kinematic Viscosity (40°C & 100°C)</span><span class="param-sub">Fluid friction & protective film</span></td>
                <td>Calibrated capillary flow under gravity</td>
                <td><span class="instrument-name">Kinematic Viscosity Bath / Redwood</span></td>
                <td><span class="method-tag">ASTM D445 / IS 1448</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Flash Point & Fire Point</span><span class="param-sub">Combustion and operational safety</span></td>
                <td>Closed/open cup exposure to test flame</td>
                <td><span class="instrument-name">Pensky-Martens / Cleveland Tester</span></td>
                <td><span class="method-tag">ASTM D93 / IS 1448 (P:21)</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Total Acid Number (TAN)</span><span class="param-sub">Corrosive oxidation degradation</span></td>
                <td>Potentiometric or Color-indicator titration with KOH</td>
                <td><span class="instrument-name">Digital/Manual Titration Setup</span></td>
                <td><span class="method-tag">ASTM D664 / IS 1448 (P:1)</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Moisture / Water Content</span><span class="param-sub">Emulsion and breakdown hazard</span></td>
                <td>Volumetric or Coulometric Karl Fischer reaction</td>
                <td><span class="instrument-name">Karl Fischer (KF) Titrator</span></td>
                <td><span class="method-tag">ASTM D6304</span></td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

    <!-- 5. MINERAL ORES -->
    <div class="module-card-detailed">
      <div class="card-top">
        <div class="card-icon"><i class="fa-solid fa-gem"></i></div>
        <div class="card-title-group">
          <span>Module 05</span>
          <h4>Mineral Ores (Iron Ore, Limestone & Bauxite)</h4>
        </div>
      </div>
      <div class="card-body">
        <div class="importance-box">
          <h5><i class="fa-solid fa-circle-exclamation"></i> Why Testing Is Important:</h5>
          <p>Vital for blast furnaces, metal smelters, and cement kilns to determine commercial ore grade, yield, and detrimental gangue elements.</p>
        </div>
        <div class="table-responsive">
          <table>
            <thead>
              <tr>
                <th style="width: 25%;">Testing Parameter</th>
                <th style="width: 30%;">Standard Test Method</th>
                <th style="width: 25%;">Analytical Instrument Used</th>
                <th style="width: 20%;">Standard Code</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td><span class="param-name">Total Iron (Fe) in Iron Ore</span><span class="param-sub">Primary commercial grade determinant</span></td>
                <td>Stannous chloride reduction & Potassium Dichromate titration</td>
                <td><span class="instrument-name">Volumetric Titration Setup</span></td>
                <td><span class="method-tag">IS 1493 (Part 1)</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Calcium & Magnesium (CaO/MgO)</span><span class="param-sub">Limestone & dolomite flux quality</span></td>
                <td>Acid decomposition followed by EDTA titration</td>
                <td><span class="instrument-name">Hot Plate & Chemical Titration Unit</span></td>
                <td><span class="method-tag">IS 1760 (Part 3)</span></td>
              </tr>
              <tr>
                <td><span class="param-name">Silica (SiO2) & Loss on Ignition (LOI)</span><span class="param-sub">Gangue impurities & structural loss</span></td>
                <td>Gravimetric dehydration & high temperature ignition</td>
                <td><span class="instrument-name">Muffle Furnace & Analytical Balance</span></td>
                <td><span class="method-tag">IS 1493 / IS 1760</span></td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </section>

  <!-- Application & Contact Section -->
  <section class="section" id="apply">
    <div class="contact-container">
      <div class="contact-info">
        <div>
          <span class="badge" style="background: rgba(255,255,255,0.2); color: #fff;">Get In Touch</span>
          <h3>Start Your Professional Laboratory Journey</h3>
          <p>Have questions regarding fees, batch dates, or syllabus? Email us directly or submit your details.</p>

          <div class="contact-item">
            <i class="fa-solid fa-envelope"></i>
            <div>
              <strong style="display:block;">Official Contact Email:</strong>
              <span>Learnologyinstitude@gmail.com</span>
            </div>
          </div>

          <div class="contact-item">
            <i class="fa-solid fa-graduation-cap"></i>
            <div>
              <strong style="display:block;">Eligible Profiles:</strong>
              <span>B.Sc. / M.Sc. Chemistry, Biochemistry, Environmental Science & Freshers</span>
            </div>
          </div>
        </div>

        <div style="font-size: 0.85rem; opacity: 0.85; margin-top: 2rem;">
          <p>© Learnology Institute. Dedicated to Laboratory Excellence.</p>
        </div>
      </div>

      <div class="contact-form-area">
        <h4>Register / Inquiry Form</h4>
        <form action="mailto:Learnologyinstitude@gmail.com" method="post" enctype="text/plain">
          <div class="form-group">
            <label for="name">Full Name</label>
            <input type="text" id="name" name="Name" placeholder="Enter your full name" required>
          </div>

          <div class="form-group">
            <label for="degree">Current Qualification</label>
            <select id="degree" name="Qualification" required>
              <option value="">Select Qualification</option>
              <option value="BSc Chemistry">B.Sc. Chemistry</option>
              <option value="MSc Chemistry">M.Sc. Chemistry / Analytical Chemistry</option>
              <option value="Environmental Science">B.Sc / M.Sc Environmental Science</option>
              <option value="Fresher Looking for Lab Job">Fresher (Completed Graduation)</option>
              <option value="Other">Other Life Science Field</option>
            </select>
          </div>

          <div class="form-group">
            <label for="interest">Module of Primary Interest</label>
            <select id="interest" name="Interested Module">
              <option value="All Integrated Chemical Analysis">Complete Integrated OJT Program (All Modules)</option>
              <option value="Water & Effluent Analysis">Water & Effluent Testing</option>
              <option value="Coal Analysis">Coal & Proximate Analysis</option>
              <option value="Lubricant Oil Testing">Lubricating Oil Analysis</option>
              <option value="Soil Testing">Soil Chemistry & Micronutrients</option>
            </select>
          </div>

          <div class="form-group">
            <label for="contact">Phone / WhatsApp Number</label>
            <input type="tel" id="contact" name="Phone" placeholder="Enter your contact number" required>
          </div>

          <button type="submit" class="submit-btn"><i class="fa-solid fa-paper-plane"></i> Submit Inquiry</button>
        </form>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div style="max-width: 1200px; margin: 0 auto; display: flex; flex-direction: column; gap: 8px;">
      <p><strong>Learnology Institute</strong> — Center for Practical Chemical Testing and Analytical Training.</p>
      <p>Official Admissions & Student Queries: <a href="mailto:Learnologyinstitude@gmail.com">Learnologyinstitude@gmail.com</a></p>
    </div>
  </footer>

</body>
</html>
