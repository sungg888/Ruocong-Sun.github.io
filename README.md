<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ruocong (Josh) Sun — Senior Data Analyst</title>
<meta name="description" content="Senior Data Analyst with 3+ years of experience in analytics, forecasting, and A/B testing. Python, SQL, Power BI.">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,500;0,9..144,700;0,9..144,800;1,9..144,300&family=Outfit:wght@300;400;500;600&family=JetBrains+Mono:wght@300;400&display=swap" rel="stylesheet">
<style>
  :root {
    --cream: #faf8f4;
    --warm-white: #f5f2ec;
    --sand: #e8e2d8;
    --stone: #c9c1b4;
    --charcoal: #2c2c2c;
    --ink: #1a1a1a;
    --clay: #6b6156;
    --terracotta: #c4704b;
    --deep-teal: #1a5c5a;
    --sage: #5a7a6a;
    --soft-blue: #4a7c9b;
    --gold: #b8933a;
    --serif: 'Fraunces', Georgia, serif;
    --sans: 'Outfit', sans-serif;
    --mono: 'JetBrains Mono', monospace;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }
  html { scroll-behavior: smooth; }

  body {
    background: var(--cream);
    color: var(--charcoal);
    font-family: var(--sans);
    font-size: 16px;
    line-height: 1.7;
    overflow-x: hidden;
    -webkit-font-smoothing: antialiased;
  }

  /* NAV */
  nav {
    position: fixed;
    top: 0; left: 0; right: 0;
    z-index: 100;
    padding: 1rem 4vw;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: rgba(250,248,244,0.88);
    backdrop-filter: blur(20px);
    border-bottom: 1px solid var(--sand);
  }

  .nav-name {
    font-family: var(--serif);
    font-weight: 700;
    font-size: 1.15rem;
    color: var(--ink);
    text-decoration: none;
    letter-spacing: -0.02em;
  }

  .nav-links { display: flex; gap: 2.2rem; align-items: center; }

  .nav-links a {
    font-family: var(--sans);
    font-size: 0.82rem;
    font-weight: 500;
    color: var(--clay);
    text-decoration: none;
    letter-spacing: 0.02em;
    transition: color 0.2s;
  }

  .nav-links a:hover { color: var(--ink); }

  .nav-contact {
    font-family: var(--mono) !important;
    font-size: 0.75rem !important;
    padding: 0.5rem 1.2rem;
    background: var(--ink);
    color: var(--cream) !important;
    border-radius: 100px;
    transition: background 0.2s, transform 0.2s !important;
  }

  .nav-contact:hover {
    background: var(--deep-teal);
    transform: translateY(-1px) !important;
  }

  /* HERO */
  .hero {
    min-height: 100vh;
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    padding: 8rem 4vw 4rem;
    max-width: 1300px;
    margin: 0 auto;
    gap: 4rem;
  }

  .hero-left {
    opacity: 0;
    animation: rise 0.7s ease forwards 0.15s;
  }

  .hero-label {
    font-family: var(--mono);
    font-size: 0.72rem;
    font-weight: 400;
    color: var(--deep-teal);
    letter-spacing: 0.14em;
    text-transform: uppercase;
    margin-bottom: 1.2rem;
    display: flex;
    align-items: center;
    gap: 0.6rem;
  }

  .hero-label::before {
    content: '';
    width: 28px;
    height: 1.5px;
    background: var(--deep-teal);
  }

  .hero-name {
    font-family: var(--serif);
    font-size: clamp(2.8rem, 5.5vw, 4.5rem);
    font-weight: 800;
    line-height: 1.05;
    letter-spacing: -0.03em;
    color: var(--ink);
    margin-bottom: 1.5rem;
  }

  .hero-name em {
    font-style: italic;
    font-weight: 300;
    color: var(--clay);
  }

  .hero-bio {
    font-size: 1.08rem;
    color: var(--clay);
    max-width: 480px;
    margin-bottom: 2.2rem;
    line-height: 1.75;
  }

  .hero-bio strong {
    color: var(--charcoal);
    font-weight: 500;
  }

  .hero-ctas {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
  }

  .btn {
    font-family: var(--sans);
    font-size: 0.85rem;
    font-weight: 500;
    padding: 0.85rem 1.8rem;
    border-radius: 8px;
    text-decoration: none;
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    transition: all 0.2s;
    cursor: pointer;
    border: none;
  }

  .btn-fill {
    background: var(--ink);
    color: var(--cream);
  }

  .btn-fill:hover {
    background: var(--deep-teal);
    transform: translateY(-2px);
    box-shadow: 0 8px 24px rgba(26,92,90,0.2);
  }

  .btn-outline {
    border: 1.5px solid var(--sand);
    color: var(--charcoal);
    background: transparent;
  }

  .btn-outline:hover {
    border-color: var(--charcoal);
    transform: translateY(-2px);
  }

  /* HERO RIGHT — IMPACT METRICS */
  .hero-right {
    opacity: 0;
    animation: rise 0.7s ease forwards 0.4s;
  }

  .metrics-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1.2rem;
  }

  .metric-card {
    background: var(--warm-white);
    border: 1px solid var(--sand);
    border-radius: 14px;
    padding: 1.6rem;
    transition: all 0.25s;
    position: relative;
    overflow: hidden;
  }

  .metric-card::after {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
    background: var(--deep-teal);
    opacity: 0;
    transition: opacity 0.25s;
  }

  .metric-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 12px 32px rgba(0,0,0,0.06);
  }

  .metric-card:hover::after { opacity: 1; }

  .metric-num {
    font-family: var(--serif);
    font-size: 2rem;
    font-weight: 700;
    color: var(--ink);
    line-height: 1.1;
    margin-bottom: 0.4rem;
  }

  .metric-label {
    font-size: 0.82rem;
    color: var(--clay);
    line-height: 1.4;
  }

  /* SECTIONS */
  .section {
    max-width: 1300px;
    margin: 0 auto;
    padding: 6rem 4vw;
  }

  .section-head {
    display: flex;
    align-items: baseline;
    gap: 1rem;
    margin-bottom: 3.5rem;
  }

  .section-number {
    font-family: var(--mono);
    font-size: 0.7rem;
    color: var(--stone);
    letter-spacing: 0.06em;
  }

  .section-title {
    font-family: var(--serif);
    font-size: 2rem;
    font-weight: 700;
    letter-spacing: -0.02em;
    color: var(--ink);
  }

  .section-rule {
    flex: 1;
    height: 1px;
    background: var(--sand);
    margin-left: 1rem;
  }

  .divider {
    max-width: 1300px;
    margin: 0 auto;
    padding: 0 4vw;
  }

  .divider hr {
    border: none;
    height: 1px;
    background: var(--sand);
  }

  /* EXPERIENCE */
  .exp-item {
    display: grid;
    grid-template-columns: 220px 1fr;
    gap: 2.5rem;
    padding: 2.5rem 0;
    border-bottom: 1px solid var(--sand);
    transition: all 0.3s;
  }

  .exp-item:last-child { border-bottom: none; }
  .exp-item:hover { padding-left: 0.5rem; }

  .exp-company-name {
    font-family: var(--serif);
    font-weight: 700;
    font-size: 1.05rem;
    color: var(--ink);
    margin-bottom: 0.25rem;
  }

  .exp-location {
    font-size: 0.82rem;
    color: var(--clay);
    margin-bottom: 0.6rem;
  }

  .exp-date {
    font-family: var(--mono);
    font-size: 0.72rem;
    color: var(--deep-teal);
    letter-spacing: 0.04em;
    padding: 0.3rem 0.7rem;
    background: rgba(26,92,90,0.06);
    border-radius: 4px;
    display: inline-block;
  }

  .exp-title {
    font-family: var(--sans);
    font-size: 1.15rem;
    font-weight: 600;
    color: var(--ink);
    margin-bottom: 1rem;
  }

  .exp-bullets {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 0.65rem;
  }

  .exp-bullets li {
    font-size: 0.92rem;
    color: var(--clay);
    padding-left: 1.4rem;
    position: relative;
    line-height: 1.65;
  }

  .exp-bullets li::before {
    content: '';
    position: absolute;
    left: 0;
    top: 0.65em;
    width: 5px;
    height: 5px;
    background: var(--deep-teal);
    border-radius: 50%;
  }

  .exp-highlight {
    color: var(--charcoal) !important;
    font-weight: 500;
  }

  /* PROJECTS */
  .projects-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.2rem;
  }

  .proj-card {
    background: var(--warm-white);
    border: 1px solid var(--sand);
    border-radius: 14px;
    padding: 1.8rem;
    display: flex;
    flex-direction: column;
    gap: 0.8rem;
    transition: all 0.25s;
    text-decoration: none;
    color: inherit;
  }

  .proj-card:hover {
    border-color: var(--stone);
    transform: translateY(-4px);
    box-shadow: 0 16px 40px rgba(0,0,0,0.06);
  }

  .proj-top {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
  }

  .proj-tag {
    font-family: var(--mono);
    font-size: 0.65rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    padding: 0.25rem 0.6rem;
    border-radius: 4px;
    background: rgba(26,92,90,0.07);
    color: var(--deep-teal);
  }

  .proj-tag.confidential {
    background: rgba(196,112,75,0.08);
    color: var(--terracotta);
  }

  .proj-links { display: flex; gap: 0.4rem; }

  .proj-link {
    font-family: var(--mono);
    font-size: 0.68rem;
    color: var(--clay);
    text-decoration: none;
    padding: 0.2rem 0.5rem;
    border: 1px solid var(--sand);
    border-radius: 4px;
    transition: all 0.2s;
  }

  .proj-link:hover {
    color: var(--deep-teal);
    border-color: var(--deep-teal);
  }

  .proj-name {
    font-family: var(--serif);
    font-size: 1rem;
    font-weight: 700;
    color: var(--ink);
    line-height: 1.3;
  }

  .proj-desc {
    font-size: 0.85rem;
    color: var(--clay);
    line-height: 1.6;
    flex: 1;
  }

  .proj-stack {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
    margin-top: 0.4rem;
  }

  .proj-tech {
    font-family: var(--mono);
    font-size: 0.65rem;
    color: var(--clay);
    padding: 0.18rem 0.5rem;
    background: rgba(0,0,0,0.03);
    border-radius: 3px;
    letter-spacing: 0.02em;
  }

  /* EDUCATION */
  .edu-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.2rem;
  }

  .edu-card {
    background: var(--warm-white);
    border: 1px solid var(--sand);
    border-radius: 14px;
    padding: 2rem;
    position: relative;
    overflow: hidden;
    transition: all 0.2s;
  }

  .edu-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 24px rgba(0,0,0,0.04);
  }

  .edu-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
  }

  .edu-card:nth-child(1)::before { background: var(--deep-teal); }
  .edu-card:nth-child(2)::before { background: var(--terracotta); }
  .edu-card:nth-child(3)::before { background: var(--gold); }

  .edu-year {
    font-family: var(--mono);
    font-size: 0.7rem;
    color: var(--stone);
    letter-spacing: 0.06em;
    margin-bottom: 0.8rem;
  }

  .edu-degree {
    font-family: var(--serif);
    font-size: 1.05rem;
    font-weight: 700;
    color: var(--ink);
    line-height: 1.3;
    margin-bottom: 0.4rem;
  }

  .edu-school {
    font-size: 0.88rem;
    color: var(--clay);
  }

  /* SKILLS */
  .skills-layout {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
  }

  .skill-cat-name {
    font-family: var(--mono);
    font-size: 0.7rem;
    color: var(--deep-teal);
    letter-spacing: 0.12em;
    text-transform: uppercase;
    margin-bottom: 1rem;
    padding-bottom: 0.6rem;
    border-bottom: 1px solid var(--sand);
  }

  .skill-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
  }

  .skill-tag {
    font-size: 0.85rem;
    color: var(--charcoal);
    background: var(--warm-white);
    border: 1px solid var(--sand);
    padding: 0.4rem 0.85rem;
    border-radius: 6px;
    transition: all 0.2s;
  }

  .skill-tag:hover {
    border-color: var(--deep-teal);
    color: var(--deep-teal);
    background: rgba(26,92,90,0.04);
  }

  /* CONTACT */
  .contact-section {
    background: var(--ink);
    color: var(--cream);
    margin-top: 4rem;
    padding: 6rem 4vw;
  }

  .contact-inner {
    max-width: 1300px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1.3fr 1fr;
    gap: 4rem;
    align-items: center;
  }

  .contact-headline {
    font-family: var(--serif);
    font-size: clamp(2rem, 4vw, 3.2rem);
    font-weight: 800;
    letter-spacing: -0.03em;
    line-height: 1.1;
    margin-bottom: 1rem;
  }

  .contact-headline em {
    font-style: italic;
    font-weight: 300;
    color: var(--stone);
  }

  .contact-sub {
    color: var(--stone);
    font-size: 1rem;
    max-width: 400px;
    line-height: 1.7;
  }

  .contact-details {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }

  .contact-row {
    display: flex;
    align-items: center;
    gap: 1rem;
    font-size: 0.95rem;
    color: var(--stone);
    text-decoration: none;
    transition: color 0.2s;
    padding: 0.8rem 1.2rem;
    border: 1px solid rgba(255,255,255,0.08);
    border-radius: 10px;
  }

  a.contact-row:hover {
    color: var(--cream);
    border-color: rgba(255,255,255,0.2);
    background: rgba(255,255,255,0.03);
  }

  .contact-row-label {
    font-family: var(--mono);
    font-size: 0.68rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--clay);
    min-width: 60px;
  }

  .contact-row-value {
    font-family: var(--sans);
    color: var(--cream);
  }

  footer {
    background: var(--ink);
    border-top: 1px solid rgba(255,255,255,0.06);
    padding: 1.5rem 4vw;
    text-align: center;
  }

  footer p {
    font-family: var(--mono);
    font-size: 0.7rem;
    color: var(--clay);
    letter-spacing: 0.04em;
  }

  /* ANIMATIONS */
  @keyframes rise {
    from { opacity: 0; transform: translateY(28px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .reveal {
    opacity: 0;
    transform: translateY(24px);
    transition: opacity 0.55s ease, transform 0.55s ease;
  }

  .reveal.visible {
    opacity: 1;
    transform: translateY(0);
  }

  /* RESPONSIVE */
  @media (max-width: 1024px) {
    .projects-grid { grid-template-columns: repeat(2, 1fr); }
  }

  @media (max-width: 768px) {
    nav { padding: 0.8rem 1.5rem; }
    .nav-links { gap: 1rem; }
    .nav-links a:not(.nav-contact) { display: none; }
    .hero {
      grid-template-columns: 1fr;
      padding: 7rem 1.5rem 3rem;
      gap: 3rem;
      min-height: auto;
    }
    .section { padding: 4rem 1.5rem; }
    .exp-item {
      grid-template-columns: 1fr;
      gap: 0.8rem;
    }
    .projects-grid { grid-template-columns: 1fr; }
    .edu-grid { grid-template-columns: 1fr; }
    .contact-inner {
      grid-template-columns: 1fr;
      gap: 2.5rem;
    }
    .contact-section { padding: 4rem 1.5rem; }
  }

  ::-webkit-scrollbar { width: 5px; }
  ::-webkit-scrollbar-track { background: var(--cream); }
  ::-webkit-scrollbar-thumb { background: var(--sand); border-radius: 3px; }
  ::-webkit-scrollbar-thumb:hover { background: var(--stone); }
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <a href="#" class="nav-name">Josh Sun</a>
  <div class="nav-links">
    <a href="#experience">Experience</a>
    <a href="#projects">Projects</a>
    <a href="#education">Education</a>
    <a href="#skills">Skills</a>
    <a href="mailto:sunjoshua64@gmail.com" class="nav-contact">Get in touch</a>
  </div>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-left">
    <div class="hero-label">Available for opportunities</div>
    <h1 class="hero-name">Ruocong<br><em>(Josh)</em> Sun</h1>
    <p class="hero-bio">
      <strong>Senior Data Analyst</strong> with 3+ years driving data-informed decisions through advanced analytics, experimentation, and forecasting. I build <strong>production-grade pipelines</strong>, executive dashboards, and A/B testing frameworks that connect data to business strategy.
    </p>
    <div class="hero-ctas">
      <a href="mailto:sunjoshua64@gmail.com" class="btn btn-fill">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
        Contact me
      </a>
      <a href="https://github.com/sungg888" target="_blank" class="btn btn-outline">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.3 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61-.546-1.385-1.335-1.755-1.335-1.755-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 21.795 24 17.295 24 12c0-6.63-5.37-12-12-12"/></svg>
        GitHub
      </a>
      <a href="https://linkedin.com/in/ruocongsun" target="_blank" class="btn btn-outline">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 0 1-2.063-2.065 2.064 2.064 0 1 1 2.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
        LinkedIn
      </a>
    </div>
  </div>

  <div class="hero-right">
    <div class="metrics-grid">
      <div class="metric-card">
        <div class="metric-num">3+</div>
        <div class="metric-label">Years of professional data analytics experience</div>
      </div>
      <div class="metric-card">
        <div class="metric-num">1,000+</div>
        <div class="metric-label">SKUs forecasted with production LSTM pipeline</div>
      </div>
      <div class="metric-card">
        <div class="metric-num">20%</div>
        <div class="metric-label">Reduction in stockouts via forecast-driven reorder system</div>
      </div>
      <div class="metric-card">
        <div class="metric-num">3</div>
        <div class="metric-label">Degrees across data science, analytics, and statistics</div>
      </div>
    </div>
  </div>
</section>

<div class="divider"><hr></div>

<!-- EXPERIENCE -->
<section class="section" id="experience">
  <div class="section-head reveal">
    <span class="section-number">01</span>
    <h2 class="section-title">Experience</h2>
    <div class="section-rule"></div>
  </div>

  <div class="exp-item reveal">
    <div>
      <div class="exp-company-name">Infinisia</div>
      <div class="exp-location">Vancouver, BC</div>
      <span class="exp-date">Aug 2024 – Present</span>
    </div>
    <div>
      <div class="exp-title">Senior Data Analyst</div>
      <ul class="exp-bullets">
        <li>Built an executive-level <span class="exp-highlight">Power BI financial performance dashboard</span> enabling month-over-month comparison of revenue, COGS, and expenses across US and CA regions, reducing ~10 hours of manual monthly reporting.</li>
        <li>Developed a <span class="exp-highlight">production-grade LSTM demand forecasting pipeline</span> in Python generating 12-month SKU-level forecasts for 1,000+ products, accurately capturing seasonality and trend dynamics.</li>
        <li>Implemented a <span class="exp-highlight">forecast-driven reorder algorithm</span> combining LSTM predictions with on-hand inventory, inbound shipments, and supplier lead times — resulting in a 20% reduction in out-of-stock incidents.</li>
        <li>Built an <span class="exp-highlight">automated Amazon pricing optimization system</span> using statistical A/B testing and profit-based decision logic, integrating BigQuery sales data and OMS APIs to drive daily price decisions. Performance monitored via a Flask-based executive dashboard.</li>
        <li>Developed a <span class="exp-highlight">shipping cost simulation tool</span> using MySQL historical order data to model zone-based carrier pricing, enabling accurate carrier selection and break-even decisions.</li>
      </ul>
    </div>
  </div>

  <div class="exp-item reveal">
    <div>
      <div class="exp-company-name">Autozen</div>
      <div class="exp-location">Vancouver, BC</div>
      <span class="exp-date">Apr – Jun 2024</span>
    </div>
    <div>
      <div class="exp-title">Data Scientist (Co-op)</div>
      <ul class="exp-bullets">
        <li>Designed a <span class="exp-highlight">log-normal regression pricing model</span> to predict vehicle values, achieving valuation accuracy within 10% of actual market prices and reducing reliance on external services.</li>
        <li>Developed an <span class="exp-highlight">API-driven AI explanation agent</span> combining model outputs with live market signals to support pricing negotiations and improve seller engagement.</li>
      </ul>
    </div>
  </div>

  <div class="exp-item reveal">
    <div>
      <div class="exp-company-name">Accenture</div>
      <div class="exp-location">Shanghai, China</div>
      <span class="exp-date">Sep 2021 – Dec 2022</span>
    </div>
    <div>
      <div class="exp-title">Business Analyst, Cybersecurity Department</div>
      <ul class="exp-bullets">
        <li>Led <span class="exp-highlight">data governance and compliance reporting</span> initiatives for Fortune 500 clients, partnering with 10+ departments to conduct enterprise risk and gap assessments.</li>
        <li>Built executive dashboards tracking findings and remediation progress, reducing client data risk exposure by <span class="exp-highlight">90%+</span>.</li>
      </ul>
    </div>
  </div>
</section>

<div class="divider"><hr></div>

<!-- PROJECTS -->
<section class="section" id="projects">
  <div class="section-head reveal">
    <span class="section-number">02</span>
    <h2 class="section-title">Projects</h2>
    <div class="section-rule"></div>
  </div>

  <div class="projects-grid">

    <div class="proj-card reveal">
      <div class="proj-top">
        <span class="proj-tag confidential">Production</span>
      </div>
      <div class="proj-name">Automated Pricing Optimization System</div>
      <p class="proj-desc">Statistical A/B testing framework with risk-scoring model integrating BigQuery and OMS APIs. Custom Flask dashboard for executive monitoring of daily price decisions across Amazon US & CA.</p>
      <div class="proj-stack">
        <span class="proj-tech">Python</span>
        <span class="proj-tech">BigQuery</span>
        <span class="proj-tech">Flask</span>
        <span class="proj-tech">z-test</span>
        <span class="proj-tech">APIs</span>
      </div>
    </div>

    <div class="proj-card reveal">
      <div class="proj-top">
        <span class="proj-tag confidential">Production</span>
      </div>
      <div class="proj-name">LSTM Demand Forecasting & Reorder Pipeline</div>
      <p class="proj-desc">Deep learning pipeline generating 12-month forecasts for 1,000+ SKUs. Paired with a reorder optimization algorithm that achieved a 20% reduction in stockouts.</p>
      <div class="proj-stack">
        <span class="proj-tech">Python</span>
        <span class="proj-tech">LSTM</span>
        <span class="proj-tech">SQL</span>
        <span class="proj-tech">MySQL</span>
      </div>
    </div>

    <div class="proj-card reveal">
      <div class="proj-top">
        <span class="proj-tag confidential">Co-op</span>
      </div>
      <div class="proj-name">Vehicle Pricing Model & AI Agent</div>
      <p class="proj-desc">Log-normal regression model predicting used car values within 10% accuracy. LLM-powered explanation agent combining model outputs with live market signals.</p>
      <div class="proj-stack">
        <span class="proj-tech">Python</span>
        <span class="proj-tech">Regression</span>
        <span class="proj-tech">LLM</span>
        <span class="proj-tech">Flask</span>
      </div>
    </div>

    <div class="proj-card reveal">
      <div class="proj-top">
        <span class="proj-tag">Academic</span>
        <div class="proj-links">
          <a href="https://github.com/UBC-MDS/DSCI-532_2024_15_dreamhouse" target="_blank" class="proj-link">GitHub</a>
          <a href="https://dsci-532-2024-15-dreamhouse.onrender.com/" target="_blank" class="proj-link">Live</a>
        </div>
      </div>
      <div class="proj-name">Dream House Dashboard</div>
      <p class="proj-desc">Interactive housing price visualization across top 50 US cities. Filterable by state, city, square footage, price range, bedrooms, and more.</p>
      <div class="proj-stack">
        <span class="proj-tech">Python</span>
        <span class="proj-tech">Dash</span>
        <span class="proj-tech">Plotly</span>
      </div>
    </div>

    <div class="proj-card reveal">
      <div class="proj-top">
        <span class="proj-tag">Academic</span>
        <div class="proj-links">
          <a href="https://github.com/UBC-MDS/Red-Wine-Quality-Prediction" target="_blank" class="proj-link">GitHub</a>
          <a href="https://ubc-mds.github.io/Red-Wine-Quality-Prediction/red_wine_quality_prediction.html" target="_blank" class="proj-link">Report</a>
        </div>
      </div>
      <div class="proj-name">Red Wine Quality Prediction</div>
      <p class="proj-desc">ML classification benchmarking logistic regression, decision tree, kNN, and SVM RBF to predict wine quality from physiochemical properties. Reproducible via Docker.</p>
      <div class="proj-stack">
        <span class="proj-tech">Python</span>
        <span class="proj-tech">scikit-learn</span>
        <span class="proj-tech">SVM</span>
        <span class="proj-tech">Docker</span>
      </div>
    </div>

    <div class="proj-card reveal">
      <div class="proj-top">
        <span class="proj-tag">Academic</span>
        <div class="proj-links">
          <a href="https://github.com/UBC-MDS/gic_calculator" target="_blank" class="proj-link">GitHub</a>
          <a href="https://gic-calculator.readthedocs.io/en/latest/" target="_blank" class="proj-link">Docs</a>
        </div>
      </div>
      <div class="proj-name">GIC Calculator Python Package</div>
      <p class="proj-desc">Published Python package for analyzing Guaranteed Investment Certificate returns. Calculates interest, compares terms, and generates visual plots.</p>
      <div class="proj-stack">
        <span class="proj-tech">Python</span>
        <span class="proj-tech">PyPI</span>
        <span class="proj-tech">Finance</span>
      </div>
    </div>

  </div>
</section>

<div class="divider"><hr></div>

<!-- EDUCATION -->
<section class="section" id="education">
  <div class="section-head reveal">
    <span class="section-number">03</span>
    <h2 class="section-title">Education</h2>
    <div class="section-rule"></div>
  </div>

  <div class="edu-grid">
    <div class="edu-card reveal">
      <div class="edu-year">2023 – 2024</div>
      <div class="edu-degree">Master of Data Science</div>
      <div class="edu-school">University of British Columbia</div>
    </div>
    <div class="edu-card reveal">
      <div class="edu-year">2020 – 2021</div>
      <div class="edu-degree">Master of Applied Business Analytics</div>
      <div class="edu-school">Boston University</div>
    </div>
    <div class="edu-card reveal">
      <div class="edu-year">2015 – 2019</div>
      <div class="edu-degree">Bachelor of Applied Statistics</div>
      <div class="edu-school">Pennsylvania State University</div>
    </div>
  </div>
</section>

<div class="divider"><hr></div>

<!-- SKILLS -->
<section class="section" id="skills">
  <div class="section-head reveal">
    <span class="section-number">04</span>
    <h2 class="section-title">Skills & tools</h2>
    <div class="section-rule"></div>
  </div>

  <div class="skills-layout">
    <div class="skill-category reveal">
      <div class="skill-cat-name">Languages</div>
      <div class="skill-tags">
        <span class="skill-tag">Python</span>
        <span class="skill-tag">SQL</span>
        <span class="skill-tag">R</span>
      </div>
    </div>
    <div class="skill-category reveal">
      <div class="skill-cat-name">Machine Learning & Statistics</div>
      <div class="skill-tags">
        <span class="skill-tag">LSTM / Deep Learning</span>
        <span class="skill-tag">Regression</span>
        <span class="skill-tag">SVM</span>
        <span class="skill-tag">A/B Testing</span>
        <span class="skill-tag">Statistical Inference</span>
        <span class="skill-tag">Forecasting</span>
      </div>
    </div>
    <div class="skill-category reveal">
      <div class="skill-cat-name">Data & Infrastructure</div>
      <div class="skill-tags">
        <span class="skill-tag">BigQuery</span>
        <span class="skill-tag">MySQL</span>
        <span class="skill-tag">REST APIs</span>
        <span class="skill-tag">Flask</span>
        <span class="skill-tag">Git</span>
        <span class="skill-tag">Docker</span>
      </div>
    </div>
    <div class="skill-category reveal">
      <div class="skill-cat-name">Business Intelligence</div>
      <div class="skill-tags">
        <span class="skill-tag">Power BI</span>
        <span class="skill-tag">Tableau</span>
        <span class="skill-tag">Dash / Plotly</span>
        <span class="skill-tag">Executive Dashboards</span>
        <span class="skill-tag">Data Storytelling</span>
      </div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<div class="contact-section">
  <div class="contact-inner">
    <div class="reveal">
      <h2 class="contact-headline">Let's build<br>something <em>together.</em></h2>
      <p class="contact-sub">Open to full-time roles in data analytics, data science, and business intelligence. Based in Vancouver, BC.</p>
    </div>
    <div class="contact-details reveal">
      <a href="mailto:sunjoshua64@gmail.com" class="contact-row">
        <span class="contact-row-label">Email</span>
        <span class="contact-row-value">sunjoshua64@gmail.com</span>
      </a>
      <a href="https://linkedin.com/in/ruocongsun" target="_blank" class="contact-row">
        <span class="contact-row-label">LinkedIn</span>
        <span class="contact-row-value">linkedin.com/in/ruocongsun</span>
      </a>
      <a href="https://github.com/sungg888" target="_blank" class="contact-row">
        <span class="contact-row-label">GitHub</span>
        <span class="contact-row-value">github.com/sungg888</span>
      </a>
      <div class="contact-row">
        <span class="contact-row-label">Phone</span>
        <span class="contact-row-value">+1-778-865-5320</span>
      </div>
    </div>
  </div>
</div>

<footer>
  <p>&copy; 2025 Ruocong (Josh) Sun</p>
</footer>

<script>
  const observer = new IntersectionObserver((entries) => {
    entries.forEach((entry) => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.08, rootMargin: '0px 0px -40px 0px' });

  document.querySelectorAll('.reveal').forEach(el => observer.observe(el));
</script>
</body>
</html>
