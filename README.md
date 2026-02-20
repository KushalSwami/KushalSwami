<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kushal Swami — IT Program Coordinator</title>
<meta name="description" content="IT Program Coordinator and Project Manager with 4+ years of enterprise delivery experience. Smartsheet & SharePoint Administrator.">
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>

/* ============================================================
   GLOBAL VARIABLES & RESET
   ============================================================ */
:root {
  --bg: #141820;
  --surface: #1c2130;
  --surface2: #161b28;
  --border: #2a2f3d;
  --line: #2a2f3d;
  --text: #dde2ec;
  --muted: #5a6070;
  --work-accent: #4e9e7a;
  --work-light: #1a2e25;
  --edu-accent: #7a6eb8;
  --edu-light: #1e1a30;
  --vol-accent: #c8a44a;
  --vol-light: #2a2010;
  --hover-shadow: 0 8px 32px rgba(0,0,0,0.4);
  --nav-height: 64px;
}

* { box-sizing: border-box; margin: 0; padding: 0; }

html { scroll-behavior: smooth; }

body {
  background: var(--bg);
  color: var(--text);
  font-family: 'DM Mono', monospace;
  font-size: 13px;
  line-height: 1.6;
  overflow-x: hidden;
}

/* ============================================================
   NAVIGATION
   ============================================================ */
nav {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: var(--nav-height);
  background: rgba(20, 24, 32, 0.92);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--border);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 40px;
  z-index: 100;
}

.nav-logo {
  font-family: 'Cormorant Garamond', serif;
  font-size: 20px;
  font-weight: 300;
  color: var(--text);
  text-decoration: none;
  letter-spacing: -0.5px;
}

.nav-links {
  display: flex;
  gap: 32px;
  list-style: none;
}

.nav-links a {
  color: var(--muted);
  text-decoration: none;
  font-size: 11px;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  transition: color 0.2s;
}

.nav-links a:hover { color: var(--work-accent); }

.nav-cta {
  background: transparent;
  border: 1px solid var(--work-accent);
  color: var(--work-accent) !important;
  padding: 6px 16px;
  border-radius: 4px;
  transition: all 0.2s !important;
}

.nav-cta:hover {
  background: var(--work-accent) !important;
  color: var(--bg) !important;
}

/* ============================================================
   HERO SECTION
   ============================================================ */
#hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: calc(var(--nav-height) + 40px) 24px 80px;
  position: relative;
  overflow: hidden;
}

/* Subtle grid background */
#hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(var(--border) 1px, transparent 1px),
    linear-gradient(90deg, var(--border) 1px, transparent 1px);
  background-size: 60px 60px;
  opacity: 0.3;
  pointer-events: none;
}

/* Radial glow */
#hero::after {
  content: '';
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 600px;
  height: 600px;
  background: radial-gradient(circle, rgba(78,158,122,0.08) 0%, transparent 70%);
  pointer-events: none;
}

.hero-eyebrow {
  font-size: 10px;
  letter-spacing: 4px;
  text-transform: uppercase;
  color: var(--work-accent);
  margin-bottom: 24px;
  animation: fadeUp 0.8s ease both;
}

.hero-name {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(56px, 8vw, 96px);
  font-weight: 300;
  line-height: 1;
  letter-spacing: -2px;
  color: var(--text);
  margin-bottom: 24px;
  animation: fadeUp 0.8s 0.1s ease both;
  position: relative;
  z-index: 1;
}

.hero-title {
  font-size: 12px;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--muted);
  margin-bottom: 40px;
  animation: fadeUp 0.8s 0.2s ease both;
}

.hero-tagline {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(18px, 3vw, 26px);
  font-weight: 300;
  font-style: italic;
  color: #8a9ab8;
  max-width: 640px;
  margin-bottom: 48px;
  animation: fadeUp 0.8s 0.3s ease both;
  line-height: 1.5;
  position: relative;
  z-index: 1;
}

.hero-buttons {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
  justify-content: center;
  animation: fadeUp 0.8s 0.4s ease both;
  position: relative;
  z-index: 1;
}

.btn-primary {
  background: var(--work-accent);
  color: var(--bg);
  border: none;
  padding: 12px 28px;
  font-family: 'DM Mono', monospace;
  font-size: 11px;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  border-radius: 4px;
  cursor: pointer;
  text-decoration: none;
  transition: all 0.2s;
}

.btn-primary:hover {
  background: #5db88c;
  transform: translateY(-1px);
}

.btn-secondary {
  background: transparent;
  color: var(--text);
  border: 1px solid var(--border);
  padding: 12px 28px;
  font-family: 'DM Mono', monospace;
  font-size: 11px;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  border-radius: 4px;
  cursor: pointer;
  text-decoration: none;
  transition: all 0.2s;
}

.btn-secondary:hover {
  border-color: var(--text);
  transform: translateY(-1px);
}

.hero-scroll {
  position: absolute;
  bottom: 32px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
  color: var(--muted);
  font-size: 10px;
  letter-spacing: 2px;
  text-transform: uppercase;
  animation: fadeUp 1s 0.8s ease both;
}

.scroll-line {
  width: 1px;
  height: 40px;
  background: linear-gradient(to bottom, var(--work-accent), transparent);
  animation: scrollPulse 2s infinite;
}

/* ============================================================
   STATS STRIP
   ============================================================ */
#stats {
  border-top: 1px solid var(--border);
  border-bottom: 1px solid var(--border);
  background: var(--surface);
  padding: 32px 40px;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0;
}

.stat {
  text-align: center;
  padding: 16px;
  border-right: 1px solid var(--border);
}

.stat:last-child { border-right: none; }

.stat-number {
  font-family: 'Cormorant Garamond', serif;
  font-size: 42px;
  font-weight: 300;
  color: var(--work-accent);
  line-height: 1;
  margin-bottom: 8px;
}

.stat-label {
  font-size: 10px;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--muted);
}

/* ============================================================
   HIGHLIGHTS / FEATURED ACCOMPLISHMENTS
   ============================================================ */
#highlights {
  padding: 96px 40px;
  max-width: 1100px;
  margin: 0 auto;
}

.section-label {
  font-size: 10px;
  letter-spacing: 4px;
  text-transform: uppercase;
  color: var(--work-accent);
  margin-bottom: 12px;
}

.section-title {
  font-family: 'Cormorant Garamond', serif;
  font-size: 40px;
  font-weight: 300;
  color: var(--text);
  margin-bottom: 48px;
  letter-spacing: -0.5px;
}

.highlights-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.highlight-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 8px;
  padding: 28px 24px;
  transition: all 0.25s;
  position: relative;
  overflow: hidden;
}

.highlight-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--work-accent);
  transform: scaleX(0);
  transition: transform 0.3s ease;
}

.highlight-card:hover::before { transform: scaleX(1); }
.highlight-card:hover {
  transform: translateY(-3px);
  box-shadow: var(--hover-shadow);
  border-color: #3a4050;
}

.highlight-icon {
  font-size: 24px;
  margin-bottom: 16px;
}

.highlight-title {
  font-family: 'Cormorant Garamond', serif;
  font-size: 20px;
  font-weight: 600;
  color: var(--text);
  margin-bottom: 10px;
  line-height: 1.2;
}

.highlight-desc {
  color: #8a9ab8;
  font-size: 11px;
  line-height: 1.7;
}

/* ============================================================
   SKILLS SECTION
   ============================================================ */
#skills {
  background: var(--surface);
  border-top: 1px solid var(--border);
  border-bottom: 1px solid var(--border);
  padding: 80px 40px;
}

.skills-inner {
  max-width: 1100px;
  margin: 0 auto;
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 32px;
  margin-top: 48px;
}

.skill-group-title {
  font-size: 10px;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--work-accent);
  margin-bottom: 16px;
  padding-bottom: 8px;
  border-bottom: 1px solid var(--border);
}

.skill-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.skill-tag {
  background: var(--bg);
  border: 1px solid var(--border);
  color: #8a9ab8;
  font-size: 11px;
  padding: 5px 12px;
  border-radius: 4px;
  transition: all 0.2s;
}

.skill-tag:hover {
  border-color: var(--work-accent);
  color: var(--work-accent);
}

/* ============================================================
   TIMELINE SECTION
   ============================================================ */
#timeline {
  padding: 96px 24px 80px;
}

.timeline-header {
  text-align: center;
  margin-bottom: 56px;
  max-width: 1100px;
  margin-left: auto;
  margin-right: auto;
}

/* Timeline component styles (carried from career_timeline.html) */
  .legend {
    display: flex;
    justify-content: center;
    gap: 24px;
    margin-bottom: 32px;
    flex-wrap: wrap;
  }

  .legend-item {
    display: flex;
    align-items: center;
    gap: 8px;
    font-size: 11px;
    color: var(--muted);
    letter-spacing: 1px;
    text-transform: uppercase;
  }

  .legend-dot {
    width: 10px;
    height: 10px;
    border-radius: 50%;
  }

  .legend-dot.work { background: var(--work-accent); }
  .legend-dot.edu { background: var(--edu-accent); }
  .legend-dot.vol { background: var(--vol-accent); }

  .timeline {
    position: relative;
    max-width: 900px;
    margin: 0 auto;
  }

  .timeline::before {
    content: '';
    position: absolute;
    left: 50%;
    top: 0;
    bottom: 0;
    width: 1px;
    background: var(--line);
    transform: translateX(-50%);
  }

  .year-marker {
    position: relative;
    text-align: center;
    margin: 0 0 8px;
    z-index: 2;
  }

  .year-marker span {
    display: inline-block;
    background: var(--bg);
    padding: 4px 12px;
    font-size: 11px;
    color: var(--muted);
    letter-spacing: 2px;
    border: 1px solid var(--border);
    border-radius: 20px;
  }

  .timeline-row {
    display: flex;
    margin-bottom: 8px;
    position: relative;
    min-height: 20px;
  }

  .timeline-row.left {
    justify-content: flex-start;
    padding-right: calc(50% + 24px);
  }

  .timeline-row.right {
    justify-content: flex-end;
    padding-left: calc(50% + 24px);
  }

  .card {
    background: #1c2130;
    border: 1px solid var(--border);
    border-radius: 6px;
    padding: 16px 18px;
    width: 100%;
    position: relative;
    cursor: default;
    transition: box-shadow 0.25s ease, transform 0.25s ease;
  }

  .card:hover {
    box-shadow: var(--hover-shadow);
    transform: translateY(-2px);
  }

  .card::after {
    content: '';
    position: absolute;
    top: 20px;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    border: 2px solid var(--bg);
    z-index: 3;
  }

  .timeline-row.left .card::after { right: -33px; }
  .timeline-row.right .card::after { left: -33px; }

  .card::before {
    content: '';
    position: absolute;
    top: 24px;
    width: 22px;
    height: 1px;
    background: var(--border);
  }

  .timeline-row.left .card::before { right: -23px; }
  .timeline-row.right .card::before { left: -23px; }

  .card.work { border-left: 3px solid var(--work-accent); }
  .card.work::after { background: var(--work-accent); }
  .card.edu { border-left: 3px solid var(--edu-accent); }
  .card.edu::after { background: var(--edu-accent); }
  .card.vol { border-left: 3px solid var(--vol-accent); }
  .card.vol::after { background: var(--vol-accent); }

  .card-type {
    font-size: 9px;
    letter-spacing: 2px;
    text-transform: uppercase;
    margin-bottom: 4px;
  }

  .card.work .card-type { color: var(--work-accent); }
  .card.edu .card-type { color: var(--edu-accent); }
  .card.vol .card-type { color: var(--vol-accent); }

  .card-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 18px;
    font-weight: 600;
    line-height: 1.2;
    margin-bottom: 2px;
    color: var(--text);
    transition: color 0.2s ease;
  }

  .card:hover .card-title { color: #ffffff; }

  .card-org {
    font-size: 11px;
    color: #8a9ab8;
    margin-bottom: 8px;
  }

  .card-dates {
    font-size: 10px;
    color: #8a9ab8;
    letter-spacing: 1px;
    margin-bottom: 10px;
    padding-bottom: 10px;
    border-bottom: 1px solid var(--border);
  }

  .card-details {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.35s ease, opacity 0.3s ease;
    opacity: 0;
  }

  .card:hover .card-details {
    max-height: 600px;
    opacity: 1;
  }

  .card.edu .card-details {
    max-height: 600px;
    opacity: 1;
  }

  .card-details ul { list-style: none; padding: 0; }

  .card-details ul li {
    padding: 3px 0 3px 12px;
    position: relative;
    line-height: 1.6;
    color: #b8c4d4;
    font-size: 11px;
  }

  .card-details ul li::before {
    content: '—';
    position: absolute;
    left: 0;
    color: var(--border);
  }

  .card-tag {
    display: inline-block;
    font-size: 9px;
    padding: 2px 7px;
    border-radius: 3px;
    margin: 8px 4px 0 0;
    letter-spacing: 0.5px;
  }

  .card.work .card-tag { background: var(--work-light); color: var(--work-accent); }
  .card.edu .card-tag { background: var(--edu-light); color: var(--edu-accent); }
  .card.vol .card-tag { background: var(--vol-light); color: var(--vol-accent); }

  .hover-hint {
    text-align: center;
    color: var(--muted);
    font-size: 10px;
    letter-spacing: 1px;
    margin-bottom: 32px;
    text-transform: uppercase;
  }

  .spacer { margin-bottom: 16px; }

/* ============================================================
   CONTACT SECTION
   ============================================================ */
#contact {
  background: var(--surface);
  border-top: 1px solid var(--border);
  padding: 96px 40px;
  text-align: center;
}

.contact-inner { max-width: 600px; margin: 0 auto; }

.contact-inner .section-title { margin-bottom: 16px; }

.contact-sub {
  color: #8a9ab8;
  font-size: 12px;
  margin-bottom: 48px;
  line-height: 1.8;
}

.contact-links {
  display: flex;
  justify-content: center;
  gap: 16px;
  flex-wrap: wrap;
  margin-bottom: 48px;
}

.contact-link {
  display: flex;
  align-items: center;
  gap: 8px;
  background: var(--bg);
  border: 1px solid var(--border);
  color: var(--text);
  text-decoration: none;
  padding: 12px 20px;
  border-radius: 6px;
  font-size: 11px;
  letter-spacing: 1px;
  transition: all 0.2s;
}

.contact-link:hover {
  border-color: var(--work-accent);
  color: var(--work-accent);
  transform: translateY(-2px);
}

.contact-email {
  font-family: 'Cormorant Garamond', serif;
  font-size: 22px;
  font-weight: 300;
  color: var(--work-accent);
  text-decoration: none;
  letter-spacing: -0.5px;
  border-bottom: 1px solid transparent;
  transition: border-color 0.2s;
}

.contact-email:hover { border-color: var(--work-accent); }

/* ============================================================
   FOOTER
   ============================================================ */
footer {
  border-top: 1px solid var(--border);
  padding: 24px 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: var(--muted);
  font-size: 10px;
  letter-spacing: 1px;
}

/* ============================================================
   ANIMATIONS
   ============================================================ */
@keyframes fadeUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes scrollPulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.3; }
}

/* ============================================================
   RESPONSIVE
   ============================================================ */
@media (max-width: 768px) {
  nav { padding: 0 20px; }
  .nav-links { display: none; }
  #stats { grid-template-columns: repeat(2, 1fr); }
  .highlights-grid { grid-template-columns: 1fr; }
  .skills-grid { grid-template-columns: 1fr; }
  #highlights, #skills, #contact { padding: 60px 20px; }
  .timeline::before { left: 16px; }
  .timeline-row.left,
  .timeline-row.right {
    padding-left: 40px;
    padding-right: 0;
    justify-content: flex-start;
  }
  .card::after { left: -31px !important; right: auto !important; }
  .card::before { left: -21px !important; right: auto !important; }
  footer { flex-direction: column; gap: 8px; text-align: center; }
}

</style>
</head>
<body>

<!-- NAV -->
<nav>
  <a href="#hero" class="nav-logo">Kushal Swami</a>
  <ul class="nav-links">
    <li><a href="#highlights">Highlights</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#timeline">Timeline</a></li>
    <li><a href="#contact" class="nav-cta">Contact</a></li>
  </ul>
</nav>

<!-- HERO -->
<section id="hero">
  <p class="hero-eyebrow">Available for new opportunities</p>
  <h1 class="hero-name">Kushal Swami</h1>
  <p class="hero-title">IT Program Coordinator &nbsp;·&nbsp; Project Manager &nbsp;·&nbsp; PMO Analyst</p>
  <p class="hero-tagline">Building scalable delivery systems for enterprise teams — 4+ years coordinating a $90M program across 30+ subprojects.</p>
  <div class="hero-buttons">
    <a href="#timeline" class="btn-primary">View My Timeline</a>
    <a href="#contact" class="btn-secondary">Get In Touch</a>
  </div>
  <div class="hero-scroll">
    <div class="scroll-line"></div>
    <span>Scroll</span>
  </div>
</section>

<!-- STATS STRIP -->
<div id="stats">
  <div class="stat">
    <div class="stat-number">$90M</div>
    <div class="stat-label">Program Budget</div>
  </div>
  <div class="stat">
    <div class="stat-number">30+</div>
    <div class="stat-label">Subprojects Managed</div>
  </div>
  <div class="stat">
    <div class="stat-number">4+</div>
    <div class="stat-label">Years Experience</div>
  </div>
  <div class="stat">
    <div class="stat-number">150%</div>
    <div class="stat-label">Team Growth Supported</div>
  </div>
</div>

<!-- HIGHLIGHTS -->
<section id="highlights">
  <p class="section-label">Featured Accomplishments</p>
  <h2 class="section-title">Where I've Made an Impact</h2>
  <div class="highlights-grid">
    <div class="highlight-card">
      <div class="highlight-icon">⚡</div>
      <div class="highlight-title">Enterprise Program Delivery</div>
      <div class="highlight-desc">Coordinated delivery across a $90M POS modernization initiative spanning 30+ subprojects and 5 grocery retail brands at Ahold Delhaize — scaled from 15 workstreams without additional coordinator headcount as the team grew 150%.</div>
    </div>
    <div class="highlight-card">
      <div class="highlight-icon">🛠</div>
      <div class="highlight-title">Platform Administration</div>
      <div class="highlight-desc">Served as System Administrator for both Smartsheet and SharePoint environments — managing access governance, workflow automation, and reporting standards across an enterprise-scale program.</div>
    </div>
    <div class="highlight-card">
      <div class="highlight-icon">🔄</div>
      <div class="highlight-title">Automation & Recovery</div>
      <div class="highlight-desc">Spearheaded restoration of an enterprise ERP system (ConnectWise) following a ransomware attack by building an AutoHotKey automation pipeline — significantly reducing recovery time and resource hours required.</div>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="skills-inner">
    <p class="section-label">Technical Proficiencies</p>
    <h2 class="section-title">Skills & Tools</h2>
    <div class="skills-grid">
      <div class="skill-group">
        <div class="skill-group-title">Program & Delivery</div>
        <div class="skill-tags">
          <span class="skill-tag">Program Governance</span>
          <span class="skill-tag">Risk Tracking</span>
          <span class="skill-tag">Dependency Management</span>
          <span class="skill-tag">Executive Reporting</span>
          <span class="skill-tag">Milestone Tracking</span>
          <span class="skill-tag">Change Management</span>
        </div>
      </div>
      <div class="skill-group">
        <div class="skill-group-title">Tools & Platforms</div>
        <div class="skill-tags">
          <span class="skill-tag">Smartsheet (Admin)</span>
          <span class="skill-tag">SharePoint (Admin)</span>
          <span class="skill-tag">Jira</span>
          <span class="skill-tag">ServiceNow</span>
          <span class="skill-tag">MS Project</span>
          <span class="skill-tag">Confluence</span>
          <span class="skill-tag">O365</span>
          <span class="skill-tag">Trello</span>
        </div>
      </div>
      <div class="skill-group">
        <div class="skill-group-title">Data & Automation</div>
        <div class="skill-tags">
          <span class="skill-tag">SQL</span>
          <span class="skill-tag">Python</span>
          <span class="skill-tag">AutoHotKey</span>
          <span class="skill-tag">Dashboard Development</span>
          <span class="skill-tag">Trend Analysis</span>
          <span class="skill-tag">Data Visualization</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- TIMELINE -->
<section id="timeline">
  <div class="timeline-header">
    <p class="section-label">Career & Education</p>
    <h2 class="section-title">My Journey</h2>
    <div class="legend">
      <div class="legend-item"><div class="legend-dot work"></div> Work Experience</div>
      <div class="legend-item"><div class="legend-dot edu"></div> Education</div>
      <div class="legend-item"><div class="legend-dot vol"></div> Volunteer / Other</div>
    </div>
    <p class="hover-hint">↓ Hover over any card to expand details</p>
  </div>

  <div class="timeline">

  <!-- 2026 -->
  <div class="year-marker"><span>2026</span></div>

  <!-- Ahold Delhaize -->
  <div class="timeline-row left">
    <div class="card work">
      <div class="card-type">Work · Contract (W2)</div>
      <div class="card-title">IT Program Coordinator</div>
      <div class="card-org">Ahold Delhaize · Salisbury, NC (Remote)</div>
      <div class="card-dates">Feb 2022 – Feb 2026 · 4 yrs 1 mo</div>
      <div class="card-details">
        <ul>
          <li>Coordinated $90M enterprise POS modernization spanning 30+ subprojects across 5 grocery retail brands following M&A integration</li>
          <li>Designed and scaled Subproject Timeline Management System from 15 to 30+ workstreams — team grew 150% without additional coordinator headcount</li>
          <li>Owned program governance & reporting cadence; produced executive-ready dashboards and trend analyses</li>
          <li>System Administrator for Smartsheet & SharePoint — access controls, workflow automation, reporting standards</li>
          <li>Served as bridge between technical teams and non-technical stakeholders across engineering, product, and business</li>
        </ul>
        <div>
          <span class="card-tag">Smartsheet Admin</span>
          <span class="card-tag">SharePoint Admin</span>
          <span class="card-tag">Program Governance</span>
          <span class="card-tag">Executive Reporting</span>
          <span class="card-tag">Jira</span>
        </div>
      </div>
    </div>
  </div>

  <div class="spacer"></div>

  <!-- Rutgers -->
  <div class="timeline-row right">
    <div class="card edu">
      <div class="card-type">Education</div>
      <div class="card-title">B.S. Management Information Systems</div>
      <div class="card-org">Rutgers Business School</div>
      <div class="card-dates">2020 – 2023 · Magna Cum Laude · 3.97 GPA</div>
      <div class="card-details">
        <ul>
          <li>Completed degree while working full-time as an IT Program Coordinator</li>
          <li>Graduated Magna Cum Laude with a 3.97 GPA</li>
          <li>3SP STEM Research Scholar</li>
          <li>Phi Theta Kappa Honor Society — Board Director of Service</li>
        </ul>
        <div>
          <span class="card-tag">MIS</span>
          <span class="card-tag">Magna Cum Laude</span>
          <span class="card-tag">3.97 GPA</span>
        </div>
      </div>
    </div>
  </div>

  <div class="spacer"></div>
  <div class="year-marker"><span>2022</span></div>
  <div class="spacer"></div>

  <!-- Diversified -->
  <div class="timeline-row left">
    <div class="card work">
      <div class="card-type">Work · Contract</div>
      <div class="card-title">Technical Project Coordinator</div>
      <div class="card-org">Diversified Media Group · Kenilworth, NJ</div>
      <div class="card-dates">Jun 2019 – Dec 2019 · 7 mos</div>
      <div class="card-details">
        <ul>
          <li>Spearheaded restoration of enterprise ERP system (ConnectWise) following ransomware-induced data loss via AutoHotKey automation</li>
          <li>Coordinated nationwide digital signage installations for JPMorgan Chase & AdSpace Networks</li>
          <li>Managed end-to-end logistics: procurement, IT/AV configuration, scheduling, post-install verification, asset management</li>
        </ul>
        <div>
          <span class="card-tag">ConnectWise</span>
          <span class="card-tag">AutoHotKey</span>
          <span class="card-tag">Asset Management</span>
          <span class="card-tag">IT/AV</span>
        </div>
      </div>
    </div>
  </div>

  <div class="spacer"></div>
  <div class="year-marker"><span>2019</span></div>
  <div class="spacer"></div>

  <!-- Steve Rich -->

  <div class="spacer"></div>

  <!-- NJ Governor -->
  <div class="timeline-row left">
    <div class="card work">
      <div class="card-type">Work · Internship</div>
      <div class="card-title">Cyber Security Intern</div>
      <div class="card-org">Office of the NJ Governor · Trenton, NJ</div>
      <div class="card-dates">Summer 2018</div>
      <div class="card-details">
        <ul>
          <li>Advised elections officials on newly enacted cybersecurity guidelines under the Director of Communications</li>
        </ul>
        <div>
          <span class="card-tag">Cybersecurity</span>
          <span class="card-tag">Government</span>
          <span class="card-tag">Policy</span>
        </div>
      </div>
    </div>
  </div>
  <div class="timeline-row left">
    <div class="card work">
      <div class="card-type">Work</div>
      <div class="card-title">IT Project Coordinator &amp; Backend Manager</div>
      <div class="card-org">Steve Rich Environmental Contractors (Versatile Products) · Clifton, NJ</div>
      <div class="card-dates">May 2017 – Jun 2019 · 2 yrs 1 mo</div>
      <div class="card-details">
        <ul>
          <li>Established full operational workflow for company subsidiary including website, POS (Square), logistics, and customer relations</li>
          <li>Reorganized and maintained CRM database (Act!); increased Google AdWords conversion rates</li>
          <li>Designed and standardized electronic form templates for proposal production</li>
          <li>Coordinated IT systems upgrades and provided in-house desktop support</li>
        </ul>
        <div>
          <span class="card-tag">CRM</span>
          <span class="card-tag">IT Support</span>
          <span class="card-tag">Google AdWords</span>
          <span class="card-tag">Microsoft Office</span>
        </div>
      </div>
    </div>
  </div>

  <div class="spacer"></div>
  <div class="year-marker"><span>2017</span></div>
  <div class="spacer"></div>

  <!-- Bergen Community College -->
  <div class="timeline-row right">
    <div class="card edu">
      <div class="card-type">Education</div>
      <div class="card-title">A.S. Information Technology</div>
      <div class="card-org">Bergen Community College</div>
      <div class="card-dates">Graduated 2018 · Magna Cum Laude · 3.97 GPA</div>
      <div class="card-details">
        <ul>
          <li>Graduated Magna Cum Laude with a 3.97 GPA</li>
          <li>Phi Theta Kappa Honor Society — Director of Service</li>
          <li>STEM Student Scholars — Cyber Security Internship Program Manager</li>
        </ul>
        <div>
          <span class="card-tag">Information Technology</span>
          <span class="card-tag">Magna Cum Laude</span>
          <span class="card-tag">Phi Theta Kappa</span>
        </div>
      </div>
    </div>
  </div>

  <div class="spacer"></div>

  <!-- Congressional Intern -->
  <div class="timeline-row left">
    <div class="card work">
      <div class="card-type">Work · Internship</div>
      <div class="card-title">IT Project Management Intern</div>
      <div class="card-org">9th District Congressional Office of NJ · Paterson, NJ</div>
      <div class="card-dates">Summer 2017</div>
      <div class="card-details">
        <ul>
          <li>Performed hardware refresh for local workstations and provided desktop support</li>
          <li>Remodeled and rebuilt CRM database (Internet Quorum for Congress)</li>
          <li>Led team of interns for general data processing</li>
        </ul>
        <div>
          <span class="card-tag">IT Support</span>
          <span class="card-tag">CRM</span>
          <span class="card-tag">Government</span>
        </div>
      </div>
    </div>
  </div>

  <div class="spacer"></div>
  <div class="year-marker"><span>2015</span></div>
  <div class="spacer"></div>

  <!-- Volunteer -->
  <div class="timeline-row left">
    <div class="card vol">
      <div class="card-type">Volunteer · Bergen Community College</div>
      <div class="card-title">Service Director &amp; Liaison</div>
      <div class="card-org">Be the Match — National Bone Marrow Donor Program</div>
      <div class="card-dates">During BCC enrollment · Phi Theta Kappa Honor Society</div>
      <div class="card-details">
        <ul>
          <li>Elected Service Director of Bergen Community College's Phi Theta Kappa Honor Society chapter</li>
          <li>Served as official liaison between BCC and Be the Match, the National Bone Marrow Donor Program</li>
          <li>Organized and ran blood and bone marrow donor drives on the BCC campus</li>
        </ul>
        <div>
          <span class="card-tag">Bergen Community College</span>
          <span class="card-tag">Phi Theta Kappa</span>
          <span class="card-tag">Be the Match</span>
          <span class="card-tag">Event Coordination</span>
        </div>
      </div>
    </div>
  </div>

  <div class="spacer"></div>

    <!-- Alliance Advisors -->
  <div class="timeline-row left">
    <div class="card work">
      <div class="card-type">Work</div>
      <div class="card-title">Sr. Proxy Information Specialist</div>
      <div class="card-org">Alliance Advisors · Bloomfield, NJ</div>
      <div class="card-dates">Sep 2015 – Dec 2016 · 1 yr 4 mos</div>
      <div class="card-details">
        <ul>
          <li>Reviewed proxy information for annual and semiannual shareholder meetings</li>
          <li>Provided customer service and performed interim supervisor duties</li>
          <li>Handled desktop support issues for the team</li>
        </ul>
        <div>
          <span class="card-tag">Proxy Information</span>
          <span class="card-tag">Customer Service</span>
          <span class="card-tag">Desktop Support</span>
        </div>
      </div>
    </div>
  </div>



</div>



</section>

<!-- CONTACT -->
<section id="contact">
  <div class="contact-inner">
    <p class="section-label">Get In Touch</p>
    <h2 class="section-title">Let's Connect</h2>
    <p class="contact-sub">Open to IT Program Coordinator, Project Manager, PMO Analyst, and Senior Project Coordinator opportunities — remote, hybrid, or onsite with relocation.</p>
    <div class="contact-links">
      <a href="mailto:Kswami96@outlook.com" class="contact-link">✉ Email</a>
      <a href="https://linkedin.com/in/kushalswami" target="_blank" class="contact-link">⟶ LinkedIn</a>
    </div>
    <a href="mailto:Kswami96@outlook.com" class="contact-email">Kswami96@outlook.com</a>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <span>© 2026 Kushal Swami</span>
  <span>Clifton, NJ · Open to Relocation</span>
</footer>

</body>
</html>
