<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kaushal Dalwala · AI & Systems · ISRO Contributor</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    :root {
      --bg-primary: #0a0e14;
      --bg-secondary: #111820;
      --bg-card: #161c26;
      --text-primary: #d4d9e2;
      --text-secondary: #8b95a5;
      --accent-blue: #5b8def;
      --accent-teal: #4db8b0;
      --accent-amber: #d4a853;
      --accent-rose: #c77d8d;
      --border-subtle: #252d38;
      --border-accent: #3a4d6b;
      --shadow-sm: 0 2px 8px rgba(0,0,0,0.3);
      --shadow-md: 0 4px 16px rgba(0,0,0,0.4);
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: var(--bg-primary);
      color: var(--text-primary);
      font-family: 'Inter', -apple-system, sans-serif;
      line-height: 1.7;
      padding: 2rem 2rem;
      min-height: 100vh;
      letter-spacing: 0.01em;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
    }

    /* Header */
    .header {
      text-align: center;
      margin-bottom: 3rem;
      padding: 2rem 0;
    }

    .header-name {
      font-family: 'JetBrains Mono', monospace;
      font-size: 3.2rem;
      font-weight: 700;
      color: #e8ecf1;
      letter-spacing: 2px;
      margin-bottom: 0.5rem;
    }

    .header-role {
      font-size: 1.05rem;
      color: var(--text-secondary);
      font-weight: 400;
      letter-spacing: 0.5px;
      margin-bottom: 1.5rem;
    }

    .header-role span {
      color: var(--accent-blue);
      font-weight: 500;
    }

    .typing-line {
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.95rem;
      color: var(--accent-teal);
      margin: 1rem auto 1.8rem;
      display: inline-block;
      padding: 0.4rem 1.2rem;
      border: 1px solid var(--border-accent);
      border-radius: 6px;
      background: rgba(91, 141, 239, 0.04);
    }

    .social-links {
      display: flex;
      justify-content: center;
      gap: 1.2rem;
      margin-top: 1.5rem;
    }

    .social-link {
      color: var(--text-secondary);
      font-size: 1.4rem;
      transition: color 0.2s ease;
      text-decoration: none;
    }

    .social-link:hover {
      color: var(--accent-blue);
    }

    /* Section titles */
    .section-title {
      font-family: 'JetBrains Mono', monospace;
      font-size: 1.5rem;
      font-weight: 600;
      color: #c8d0da;
      margin: 3rem 0 1.5rem;
      padding-bottom: 0.6rem;
      border-bottom: 2px solid var(--border-subtle);
      letter-spacing: 1px;
    }

    .section-subtitle {
      font-size: 1.05rem;
      font-weight: 500;
      color: var(--text-secondary);
      margin: 1.8rem 0 1rem 0.5rem;
      letter-spacing: 0.5px;
    }

    /* Tech stack */
    .tech-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem 0.8rem;
      margin-bottom: 1rem;
    }

    .tech-badge {
      background: var(--bg-card);
      border: 1px solid var(--border-subtle);
      color: var(--text-secondary);
      padding: 0.35rem 0.9rem;
      border-radius: 5px;
      font-size: 0.85rem;
      font-family: 'JetBrains Mono', monospace;
      transition: all 0.2s ease;
    }

    .tech-badge:hover {
      border-color: var(--accent-blue);
      color: #c8d4e8;
      background: #1a2332;
    }

    /* Project cards */
    .project-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(330px, 1fr));
      gap: 1.2rem;
    }

    .project-card {
      background: var(--bg-card);
      border: 1px solid var(--border-subtle);
      border-radius: 10px;
      padding: 1.5rem;
      transition: all 0.25s ease;
      box-shadow: var(--shadow-sm);
      position: relative;
    }

    .project-card:hover {
      border-color: var(--border-accent);
      box-shadow: var(--shadow-md);
      transform: translateY(-1px);
    }

    .project-card a {
      font-family: 'JetBrains Mono', monospace;
      font-size: 1.15rem;
      font-weight: 600;
      color: #c8d8f0;
      text-decoration: none;
      display: inline-block;
      margin-bottom: 0.7rem;
      transition: color 0.2s ease;
    }

    .project-card a:hover {
      color: var(--accent-blue);
    }

    .project-card p {
      color: var(--text-secondary);
      font-size: 0.9rem;
      line-height: 1.6;
      margin-bottom: 1rem;
    }

    .tag-list {
      display: flex;
      flex-wrap: wrap;
      gap: 0.4rem;
    }

    .tag {
      background: rgba(91, 141, 239, 0.08);
      border: 1px solid rgba(91, 141, 239, 0.2);
      color: var(--accent-blue);
      padding: 0.2rem 0.6rem;
      border-radius: 4px;
      font-size: 0.75rem;
      font-family: 'JetBrains Mono', monospace;
    }

    .tag.teal {
      background: rgba(77, 184, 176, 0.08);
      border-color: rgba(77, 184, 176, 0.2);
      color: var(--accent-teal);
    }

    .tag.amber {
      background: rgba(212, 168, 83, 0.08);
      border-color: rgba(212, 168, 83, 0.2);
      color: var(--accent-amber);
    }

    /* ISRO card special */
    .project-card.isro {
      border-left: 3px solid var(--accent-amber);
      background: linear-gradient(135deg, #161c26 0%, #1a1f2b 100%);
    }

    .isro-label {
      display: inline-block;
      background: rgba(212, 168, 83, 0.1);
      border: 1px solid rgba(212, 168, 83, 0.3);
      color: var(--accent-amber);
      padding: 0.2rem 0.7rem;
      border-radius: 4px;
      font-size: 0.75rem;
      font-weight: 500;
      letter-spacing: 0.5px;
      margin-bottom: 0.8rem;
    }

    /* Stats section */
    .stats-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin: 1.5rem 0;
    }

    .stats-container img {
      border-radius: 8px;
      border: 1px solid var(--border-subtle);
    }

    /* Competencies */
    .comp-card {
      background: var(--bg-card);
      border: 1px solid var(--border-subtle);
      border-radius: 10px;
      padding: 1.8rem;
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.9rem;
      color: var(--text-secondary);
      line-height: 1.8;
      box-shadow: var(--shadow-sm);
    }

    .comp-card .highlight {
      color: #bcc8d8;
      font-weight: 500;
    }

    /* Contact */
    .contact-section {
      text-align: center;
      margin-top: 2rem;
      padding: 2rem 0;
    }

    .contact-text {
      color: var(--text-secondary);
      margin-bottom: 1.5rem;
      font-size: 0.95rem;
    }

    .contact-badges {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 0.8rem;
    }

    .contact-badges img {
      border-radius: 6px;
    }

    /* Footer */
    footer {
      text-align: center;
      margin-top: 3rem;
      padding-top: 2rem;
      border-top: 1px solid var(--border-subtle);
      color: var(--text-secondary);
      font-size: 0.85rem;
    }

    footer .quote {
      font-style: italic;
      color: #8b95a5;
      margin-bottom: 0.5rem;
    }

    footer .signature {
      color: #a0aab8;
      font-weight: 500;
    }

    hr {
      border: none;
      border-top: 1px solid var(--border-subtle);
      margin: 2.5rem 0;
    }

    @media (max-width: 700px) {
      body {
        padding: 1rem;
      }
      .header-name {
        font-size: 2.2rem;
      }
      .project-grid {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>
  <div class="container">

    <!-- Header -->
    <header class="header">
      <h1 class="header-name">Kaushal Dalwala</h1>
      <p class="header-role">Engineer · <span>ISRO Contributor</span> · AI & Systems Developer</p>
      <div class="typing-line">
        <i class="fas fa-satellite" style="margin-right: 8px;"></i> mission-critical software · IPv6 · MRI AI · Flask · C++
      </div>
      <div class="social-links">
        <a href="https://www.linkedin.com/in/kaushaldalwala" class="social-link" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
        <a href="mailto:kaushaldalwala1503@gmail.com" class="social-link" title="Email"><i class="fas fa-envelope"></i></a>
        <a href="https://github.com/Kaushaldalwala" class="social-link" title="GitHub"><i class="fab fa-github"></i></a>
      </div>
    </header>

    <hr>

    <!-- Tech Stack -->
    <h2 class="section-title">// Tech Stack</h2>
    <div class="tech-grid">
      <span class="tech-badge">Python</span>
      <span class="tech-badge">C++</span>
      <span class="tech-badge">Java</span>
      <span class="tech-badge">Dart</span>
      <span class="tech-badge">JavaScript</span>
      <span class="tech-badge">Flask</span>
      <span class="tech-badge">Flutter</span>
      <span class="tech-badge">YOLOv8</span>
      <span class="tech-badge">OpenCV</span>
      <span class="tech-badge">IPv6 Sockets</span>
      <span class="tech-badge">HTML5</span>
      <span class="tech-badge">CSS3</span>
      <span class="tech-badge">MongoDB</span>
      <span class="tech-badge">SQL</span>
      <span class="tech-badge">ODBC</span>
    </div>

    <!-- Projects -->
    <h2 class="section-title">// Projects</h2>

    <h3 class="section-subtitle">🤖 AI / ML</h3>
    <div class="project-grid">
      <div class="project-card">
        <a href="https://github.com/Kaushaldalwala/Gartner-Duct-Detection-System-Using-MRIs">Gartner Duct Detection — MRI AI</a>
        <p>AI diagnostic tool for automatic analysis of axial T1-weighted MRI scans. Detects duct and tissue abnormalities using a YOLO-based object detection pipeline.</p>
        <div class="tag-list">
          <span class="tag">Python</span>
          <span class="tag">Jupyter</span>
          <span class="tag">YOLOv8</span>
          <span class="tag teal">Computer Vision</span>
        </div>
      </div>
      <div class="project-card">
        <a href="https://github.com/Kaushaldalwala/cpp-ml-library">C++ ML Library</a>
        <p>Custom implementation of machine learning concepts and algorithms in C++ from scratch. Deep dive into ML fundamentals with systems-level programming.</p>
        <div class="tag-list">
          <span class="tag">C++</span>
          <span class="tag teal">Machine Learning</span>
          <span class="tag amber">Algorithms</span>
        </div>
      </div>
    </div>

    <h3 class="section-subtitle">🌐 Systems / Networking</h3>
    <div class="project-grid">
      <div class="project-card">
        <a href="https://github.com/Kaushaldalwala/IPv6-Socket-Communication">IPv6 Socket Communication</a>
        <p>Lightweight Python client–server project over IPv6 sockets. Built for learning low-level network communication with zero dependencies.</p>
        <div class="tag-list">
          <span class="tag">Python</span>
          <span class="tag">IPv6</span>
          <span class="tag teal">Socket Programming</span>
          <span class="tag amber">Networking</span>
        </div>
      </div>
    </div>

    <h3 class="section-subtitle">🛠️ Backend</h3>
    <div class="project-grid">
      <div class="project-card">
        <a href="https://github.com/Kaushaldalwala/CRUD-with-Flask-HTML-JavaScript">CRUD with Flask, HTML & JavaScript</a>
        <p>Full-stack web application using Python Flask, connected to a relational database via ODBC. Complete CRUD operations with integrated frontend.</p>
        <div class="tag-list">
          <span class="tag">Python</span>
          <span class="tag">Flask</span>
          <span class="tag">HTML</span>
          <span class="tag">JavaScript</span>
          <span class="tag teal">ODBC</span>
        </div>
      </div>
    </div>

    <h3 class="section-subtitle">📱 Apps</h3>
    <div class="project-grid">
      <div class="project-card">
        <a href="https://github.com/Kaushaldalwala/Weather-App">Weather App — Java</a>
        <p>Terminal-based weather retrieval using OpenWeather REST API. Clean command-line interface for quick weather information.</p>
        <div class="tag-list">
          <span class="tag">Java</span>
          <span class="tag">REST API</span>
          <span class="tag teal">OpenWeather</span>
        </div>
      </div>
      <div class="project-card">
        <a href="https://github.com/Kaushaldalwala/flutter_weather_app">Flutter Weather App</a>
        <p>Cross-platform mobile application built with Flutter and Dart. Real-time weather data with polished user interface.</p>
        <div class="tag-list">
          <span class="tag">Flutter</span>
          <span class="tag">Dart</span>
          <span class="tag teal">API Integration</span>
        </div>
      </div>
    </div>

    <h3 class="section-subtitle">🛰️ ISRO Mission</h3>
    <div class="project-grid">
      <div class="project-card isro">
        <span class="isro-label">PAHAL Phase-04</span>
        <p style="font-weight: 500; color: #c8d4e0;">SPACE APPLICATIONS CENTRE (SAC) — ISRO, Ahmedabad</p>
        <strong>Domain:</strong> Satellite Ground Systems · TC & TM Engineering<br>
        <strong>Focus:</strong> Telecommand/Telemetry CRUD interface, mission-control web UI, configuration management.</p>
        <div class="tag-list">
          <span class="tag amber">Flask</span>
          <span class="tag amber">CRUD</span>
          <span class="tag amber">Ground Systems</span>
          <span class="tag amber">TC&TM</span>
        </div>
        <p style="margin-top: 0.8rem; font-size: 0.85rem; color: var(--accent-amber); opacity: 0.9;">
          <i class="fas fa-circle" style="font-size: 0.5rem; vertical-align: middle;"></i> Contributing to India's satellite communication infrastructure
        </p>
      </div>
    </div>

    <!-- GitHub Analytics -->
    <h2 class="section-title">// GitHub Analytics</h2>
    <div class="stats-container">
      <img height="170em" src="https://github-readme-stats.vercel.app/api?username=Kaushaldalwala&show_icons=true&theme=tokyonight&hide_border=true&bg_color=111820&title_color=5b8def&icon_color=4db8b0&text_color=8b95a5" alt="GitHub Stats">
      <img height="170em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Kaushaldalwala&layout=compact&theme=tokyonight&hide_border=true&bg_color=111820&title_color=5b8def&text_color=8b95a5" alt="Top Languages">
    </div>
    <div class="stats-container">
      <img src="https://github-readme-streak-stats.herokuapp.com/?user=Kaushaldalwala&theme=tokyonight&hide_border=true&background=111820&ring=5b8def&fire=d4a853&currStreakLabel=4db8b0" alt="GitHub Streak">
    </div>

    <!-- Core Competencies -->
    <h2 class="section-title">// Core Competencies</h2>
    <div class="comp-card">
      <span class="highlight">AI / Machine Learning</span> — Computer Vision · YOLO · MRI Analysis · Custom ML Libraries<br>
      <span class="highlight">Systems Programming</span> — C++ · IPv6 · Socket Communication · Low-level Networking<br>
      <span class="highlight">Backend Development</span> — Flask · REST APIs · ODBC · SQL · MongoDB<br>
      <span class="highlight">Mobile Development</span> — Flutter · Dart · Cross-platform Applications<br>
      <span class="highlight">Web Development</span> — HTML · CSS · JavaScript · Full-stack Integration<br>
      <span class="highlight">Ground Systems</span> — Telecommand · Telemetry · ISRO TC&TM · Mission Control
    </div>

    <!-- Contact -->
    <h2 class="section-title">// Contact</h2>
    <div class="contact-section">
      <p class="contact-text">Open to research collaborations, DRDO/ISRO-aligned projects, and systems-level engineering roles.</p>
      <div class="contact-badges">
        <a href="mailto:kaushaldalwala1503@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
        <a href="https://www.linkedin.com/in/kaushaldalwala"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
        <a href="https://github.com/Kaushaldalwala"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>
      </div>
      <div style="margin-top: 1.5rem;">
        <img src="https://komarev.com/ghpvc/?username=Kaushaldalwala&style=for-the-badge&color=5b8def&label=PROFILE+VIEWS" alt="Profile Views">
      </div>
    </div>

    <footer>
      <p class="quote">"Precision in code. Clarity in systems. Purpose in every commit."</p>
      <p class="signature">— Kaushal Dalwala · ISRO PAHAL Phase-04</p>
    </footer>
  </div>
</body>
</html>
