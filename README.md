<!DOCTYPE html>
<html lang="en" data-theme="light">
<head>
  <script async src="https://www.googletagmanager.com/gtag/js?id=G-0ZKZN59YGS"></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());

    // 기본 페이지 조회 및 실시간 방문자 수 수집 활성화
    gtag('config', 'G-0ZKZN59YGS', {
      'send_page_view': true
    });
  </script>

  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>ACBM | Adaptive Compensation-Based Methodology</title> 
  <meta name="description" content="ACBM introduces adaptive compensation methodology for display uniformity, luminance control, and scalable calibration across advanced display systems.">
  <style>
    :root {
      --bg: #f6f4ef;
      --surface: #fcfbf8;
      --surface-2: #efebe3;
      --text: #1f1f1b;
      --muted: #66645f;
      --line: #d8d2c7;
      --primary: #0c6a6f;
      --primary-dark: #084d51;
      --accent: #d9eee9;
      --max: 1120px;
      --radius: 18px;
      --shadow: 0 12px 30px rgba(0,0,0,.08);
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
      color: var(--text);
      background: linear-gradient(180deg, #f6f4ef 0%, #fbfaf7 100%);
      line-height: 1.6;
    }
    img { max-width: 100%; display: block; height: auto; }
    a { color: inherit; text-decoration: none; }
    .container { width: min(calc(100% - 32px), var(--max)); margin: 0 auto; }
    .site-header {
      position: sticky; top: 0; z-index: 20;
      backdrop-filter: blur(10px);
      background: rgba(246,244,239,.84);
      border-bottom: 1px solid rgba(31,31,27,.08);
    }
    .nav {
      display: flex; align-items: center; justify-content: space-between;
      min-height: 72px; gap: 16px;
    }
    .brand { display: flex; align-items: center; gap: 12px; font-weight: 700; letter-spacing: .02em; }
    .brand-mark {
      width: 40px; height: 40px; border-radius: 12px; background: var(--primary); color: white;
      display: grid; place-items: center; font-size: 14px; font-weight: 800;
      box-shadow: inset 0 0 0 1px rgba(255,255,255,.18);
    }
    .nav-links { display: flex; gap: 18px; color: var(--muted); font-size: 14px; }
    .btn {
      display: inline-flex; align-items: center; justify-content: center; gap: 8px;
      padding: 12px 18px; border-radius: 999px; font-weight: 600; border: 1px solid transparent;
      transition: .2s ease;
    }
    .btn-primary { background: var(--primary); color: #fff; }
    .btn-primary:hover { background: var(--primary-dark); }
    .btn-secondary { border-color: var(--line); background: rgba(255,255,255,.65); }
    .hero { padding: 72px 0 44px; }
    .hero-grid {
      display: grid; grid-template-columns: 1fr 1fr; gap: 28px; align-items: stretch;
    }
    .eyebrow {
      display: inline-flex; padding: 8px 12px; border-radius: 999px; background: var(--accent);
      color: var(--primary-dark); font-size: 13px; font-weight: 700; margin-bottom: 18px;
    }
    h1 {
      margin: 0 0 18px; font-size: clamp(2.4rem, 4vw, 4.8rem); line-height: 1.02; letter-spacing: -.04em;
    }
    .hero p { color: var(--muted); font-size: 18px; margin: 0 0 26px; max-width: 62ch; }
    .actions { display: flex; gap: 12px; flex-wrap: wrap; }
    .hero-card, .panel, .feature, .contact-card {
      height: 100%; display: flex; flex-direction: column;
      margin: 0;
      background: var(--surface); border: 1px solid var(--line); border-radius: var(--radius); box-shadow: var(--shadow);
    }
    .hero-card { padding: 22px; display: grid; gap: 16px; }
    .stat { padding: 16px; background: var(--surface-2); border-radius: 14px; }
    .stat strong { display: block; font-size: 14px; color: var(--muted); margin-bottom: 6px; }
    .stat span { font-size: 28px; font-weight: 750; letter-spacing: -.03em; }
    section { padding: 28px 0; }
    .section-title { margin: 0 0 14px; font-size: 30px; letter-spacing: -.03em; }
    .section-copy { color: var(--muted); margin: 0 0 22px; max-width: 70ch; }
    .grid-3 { display: grid; grid-template-columns: repeat(3, 1fr); gap: 18px; }
    .feature { padding: 22px; }
    .feature h3 { margin: 0 0 10px; font-size: 20px; }
    .feature p { margin: 0; color: var(--muted); }

    .two-col { 
      display: grid; 
      grid-template-columns: 1fr 1fr; 
      gap: 24px; 
      align-items: stretch; 
    }

    .panel, .contact-card {
      height: 100%;
      margin: 0 !important; 
      display: flex;
      flex-direction: column;
    }

    .contact-card {
      justify-content: space-between;
    }

    .media-wrap {
      overflow: hidden; border-radius: 16px; border: 1px solid var(--line); background: #e8e2d8;
    }
    .media-wrap img { width: 100%; aspect-ratio: 16 / 10; object-fit: cover; }
    .contact-card { padding: 24px; display: grid; gap: 14px; }
    footer { padding: 38px 0 56px; color: var(--muted); font-size: 14px; }
    .footer-box {
      padding-top: 20px; border-top: 1px solid rgba(31,31,27,.1);
      display: flex; justify-content: space-between; gap: 12px; flex-wrap: wrap;
    }
    
    /* YouTube 아이프레임 중앙 정렬 및 여백 */
    iframe {
      display: block;
      margin: 20px auto;
      max-width: 100%;
      border: none;
      border-radius: 12px;
      box-shadow: var(--shadow);
    }

    @media (max-width: 900px) {
      .hero-grid, .grid-3, .two-col { grid-template-columns: 1fr; }
      .nav { align-items: flex-start; padding: 14px 0; }
      .nav-links { flex-wrap: wrap; }
    }
    @media (max-width: 560px) {
      h1 { font-size: 2.4rem; }
      .hero p { font-size: 16px; }
      .nav-links { display: none; }
    }
  </style>
</head>
<body>
  <header class="site-header">
    <div class="container nav">
      <a class="brand" href="#top" aria-label="ACBM home">
        <span class="brand-mark">AI</span>
        <span>ACBM</span>
      </a>
      <nav class="nav-links" aria-label="Primary">
        <a href="#technology">Technology</a>
        <a href="#applications">Applications</a>
        <a href="#ip">IP</a>
        <a href="#contact">Contact</a>
      </nav>
      <a class="btn btn-secondary" href="https://www.acbmai.de/dataroom/index.html" onclick="trackGA4Event('dataroom_click', 'top_nav_button')">DATA ROOM</a>
    </div>
  </header>

  <img src="./images/acbmsoftware1.jpg" alt="ACBM software1" width="1200" height="750" loading="lazy">

  <main id="top">
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <h1>Adaptive Compensation for Advanced Displays</h1>
          <p> Scalable display compensation designed for uniformity, luminance control, and manufacturable calibration. ACBM introduces a practical methodology for display compensation, with emphasis on real-time correction, reduced memory burden, and implementation paths relevant to OLED, MicroLED, and emerging XR display systems.</p>
          <div class="actions">
            <a class="btn btn-primary" href="#technology" onclick="trackGA4Event('hero_action_click', 'explore_technology')">Explore technology</a>
            <a class="btn btn-secondary" href="#ip" onclick="trackGA4Event('hero_action_click', 'view_ip_focus')">View IP focus</a>
          </div>
        </div>
        <aside class="hero-card" aria-label="Highlights">
          <div class="stat"><strong>Core idea</strong><span>Adaptive compensation</span></div>
          <div class="stat"><strong>Target domains</strong><span>OLED · MicroLED · XR</span></div>
          <div class="stat"><strong>Implementation focus</strong><span>Calibration + driver architecture</span></div>
        </aside>
      </div>
    </section>

    <img src="./images/acbmsoftware2.jpg" alt="ACBM software2" width="1200" height="750" loading="lazy">

    <iframe
      width="560"
      height="315"
      src="https://www.youtube.com/embed/LOXqIPtEQxk"
      title="YouTube video player"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen>
    </iframe>

    <section id="technology">
      <div class="container">
        <h2 class="section-title">Technology</h2>
        <p class="section-copy">Parametric Transfer function based LUT-less technology.</p>
        <div class="two-col">
          <div class="panel">
            <h3>What ACBM addresses</h3>
            <ul class="list">
              <li>Grid based uniformity and luminance variation.</li>
              <li>Compensation strategies that remain practical at scale.</li>
              <li>Integration of calibration logic with driver and manufacturing workflows.</li>
              <li>Architecture choices that reduce memory overhead compared with brute-force LUT storage.</li>
            </ul>
          </div>
          <div class="panel media-wrap">
            <img src="./images/acbmlogo.jpg" alt="ACBM technology logo" width="1200" height="750" loading="lazy">
          </div>    
        </div>
      </div>
    </section>

    <iframe
      width="560"
      height="315"
      src="https
