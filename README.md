<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Meet Pally — Your AI tugger for any situation | Cyngn (concept)</title>

<!-- Concept demo metadata -->
<meta name="description" content="Concept homepage redesign for Cyngn (NASDAQ: CYN) DriveMod Tugger — single-product hero with embedded configurator. Portfolio asset by Nizam Ali. Not affiliated with Cyngn Inc.">
<meta name="author" content="Nizam Ali">
<meta name="robots" content="noindex">

<!-- Open Graph -->
<meta property="og:type" content="website">
<meta property="og:title" content="Meet Pally — concept homepage for Cyngn DriveMod Tugger">
<meta property="og:description" content="Single-product hero. Named character. Configurator-driven funnel. A concept by Nizam Ali for the Cyngn Head of RevOps role. Not affiliated with Cyngn Inc.">

<!-- Twitter -->
<meta name="twitter:card" content="summary">
<meta name="twitter:title" content="Meet Pally — Your AI tugger for any situation">
<meta name="twitter:description" content="Concept homepage redesign by Nizam Ali. Not affiliated with Cyngn Inc.">

<!-- Favicon (Cyngn-style orange C mark) -->
<link rel="icon" type="image/svg+xml" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 32 32'%3E%3Crect width='32' height='32' rx='6' fill='%23FF5F1F'/%3E%3Ctext x='16' y='23' text-anchor='middle' font-family='Arial Black,sans-serif' font-weight='900' font-size='20' fill='white'%3EC%3C/text%3E%3C/svg%3E">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Archivo:wght@400;500;600;700;800;900&family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,500;0,9..144,600;0,9..144,700;0,9..144,800;0,9..144,900;1,9..144,400;1,9..144,700&family=Manrope:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;500;700&display=swap" rel="stylesheet">
<style>
  :root {
    /* Light industrial palette */
    --bg: #F5F1E8;          /* warm cream — Caterpillar/Deere feel */
    --bg-2: #EFEAE0;        /* slightly darker cream */
    --surface: #FFFFFF;     /* white card */
    --surface-2: #FAF7F2;   /* very light cream card */
    --border: #E5DDD0;
    --border-strong: #C7BCA9;
    --ink: #1B1B1F;         /* near-black with warmth */
    --ink-2: #3A3A40;
    --ink-muted: #6B6B72;
    --ink-dim: #9B9BA2;

    --accent: #FF5F1F;      /* high-vis safety orange */
    --accent-soft: rgba(255, 95, 31, 0.10);
    --accent-deep: #E04E12;
    --blue: #1E5BA8;        /* trust blue, used sparingly */
    --green: #2E8B57;       /* success */
    --yellow: #FFC233;      /* caution highlight */

    /* Typography */
    --serif: 'Fraunces', Georgia, serif;     /* Pally's voice */
    --display: 'Archivo', sans-serif;         /* Industrial structure */
    --body: 'Manrope', sans-serif;
    --mono: 'JetBrains Mono', monospace;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  html { scroll-behavior: smooth; }

  body {
    background: var(--bg);
    color: var(--ink);
    font-family: var(--body);
    font-weight: 400;
    line-height: 1.55;
    -webkit-font-smoothing: antialiased;
    overflow-x: hidden;
  }

  /* Subtle paper texture on the cream */
  body::before {
    content: "";
    position: fixed;
    inset: 0;
    pointer-events: none;
    z-index: 1;
    opacity: 0.4;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='200'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='2' stitchTiles='stitch'/%3E%3CfeColorMatrix values='0 0 0 0 0.4  0 0 0 0 0.35  0 0 0 0 0.25  0 0 0 0.04 0'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' /%3E%3C/svg%3E");
  }

  .container {
    max-width: 1280px;
    margin: 0 auto;
    padding: 0 32px;
    position: relative;
    z-index: 2;
  }

  /* ========== NAV ========== */
  nav {
    position: sticky;
    top: 0;
    z-index: 100;
    background: rgba(245, 241, 232, 0.9);
    backdrop-filter: blur(14px);
    -webkit-backdrop-filter: blur(14px);
    border-bottom: 1px solid var(--border);
  }
  .nav-inner {
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 68px;
  }
  .logo {
    display: flex;
    align-items: center;
    gap: 10px;
    color: var(--ink);
    text-decoration: none;
  }
  .logo-mark-svg {
    width: 34px;
    height: 34px;
    flex-shrink: 0;
    filter: drop-shadow(0 2px 6px rgba(0,0,0,0.15));
  }
  .logo-text {
    display: flex;
    flex-direction: column;
    line-height: 1;
    gap: 3px;
  }
  .logo-name {
    font-family: var(--display);
    font-weight: 900;
    font-size: 22px;
    letter-spacing: -0.025em;
    color: var(--ink);
  }
  .logo-by {
    font-family: var(--mono);
    font-size: 9px;
    text-transform: uppercase;
    letter-spacing: 0.14em;
    color: var(--ink-muted);
    font-weight: 500;
  }
  .nav-links {
    display: flex;
    gap: 36px;
    list-style: none;
  }
  .nav-links a {
    color: var(--ink-2);
    text-decoration: none;
    font-size: 14px;
    font-weight: 500;
    transition: color 0.2s;
  }
  .nav-links a:hover { color: var(--accent); }
  .nav-cta {
    display: flex;
    align-items: center;
    gap: 14px;
  }
  .nav-cta-secondary {
    color: var(--ink-2);
    text-decoration: none;
    font-size: 14px;
    font-weight: 500;
  }
  .nav-cta-primary {
    background: var(--ink);
    color: white;
    border: none;
    padding: 11px 20px;
    font-family: var(--body);
    font-weight: 700;
    font-size: 14px;
    border-radius: 100px;
    cursor: pointer;
    text-decoration: none;
    transition: background 0.2s, transform 0.2s;
    display: inline-flex;
    align-items: center;
    gap: 6px;
  }
  .nav-cta-primary:hover {
    background: var(--accent);
    transform: translateY(-1px);
  }

  /* ========== HERO ========== */
  .hero {
    padding: 64px 0 88px;
    position: relative;
  }

  .hero-grid {
    display: grid;
    grid-template-columns: 1.05fr 1fr;
    gap: 56px;
    align-items: center;
  }

  .hero-content {
    display: flex;
    flex-direction: column;
    gap: 0;
  }

  /* Hero photo — right column, large */
  .hero-image-wrap {
    border-radius: 16px;
    overflow: hidden;
    background: var(--ink);
    box-shadow: 0 32px 80px rgba(0,0,0,0.18), 0 4px 12px rgba(0,0,0,0.08);
    aspect-ratio: 4 / 5;
    position: relative;
  }
  .pally-hero-photo {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }

  /* Hero CTA row — under stats / customer logos */
  .hero-cta-row {
    display: flex;
    gap: 14px;
    margin-top: 36px;
    flex-wrap: wrap;
  }
  .hero-cta-primary {
    background: var(--ink);
    color: white;
    border: none;
    padding: 16px 30px;
    font-family: var(--body);
    font-weight: 700;
    font-size: 15px;
    border-radius: 100px;
    cursor: pointer;
    text-decoration: none;
    transition: background 0.2s, transform 0.2s;
    display: inline-flex;
    align-items: center;
    gap: 8px;
  }
  .hero-cta-primary:hover {
    background: var(--accent);
    transform: translateY(-1px);
  }
  .hero-cta-secondary {
    background: transparent;
    color: var(--ink);
    padding: 16px 28px;
    font-family: var(--body);
    font-weight: 600;
    font-size: 15px;
    border: 1px solid var(--border-strong);
    border-radius: 100px;
    cursor: pointer;
    text-decoration: none;
    transition: border-color 0.2s, color 0.2s;
    display: inline-flex;
    align-items: center;
  }
  .hero-cta-secondary:hover {
    border-color: var(--accent);
    color: var(--accent);
  }

  /* ========== CONFIGURATOR BAND (page 2) ========== */
  .config-band {
    background: var(--bg-2);
    padding: 96px 0 110px;
    border-top: 1px solid var(--border);
    border-bottom: 1px solid var(--border);
  }
  .config-band-inner {
    max-width: 760px;
    margin: 0 auto;
  }
  .config-band-header {
    text-align: center;
    margin-bottom: 40px;
  }
  .config-band-header .section-eyebrow {
    justify-content: center;
    display: inline-flex;
  }
  .config-band-title {
    font-family: var(--display);
    font-weight: 800;
    font-size: clamp(36px, 4vw, 52px);
    letter-spacing: -0.03em;
    line-height: 1.04;
    margin-bottom: 16px;
    color: var(--ink);
  }
  .config-band-title .accent {
    color: var(--accent);
    font-weight: 800;
  }
  .config-band-sub {
    font-family: var(--body);
    font-size: 17px;
    color: var(--ink-2);
    max-width: 560px;
    margin: 0 auto;
    line-height: 1.55;
  }

  .hero-eyebrow {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    font-family: var(--mono);
    font-size: 11px;
    font-weight: 500;
    color: var(--accent);
    text-transform: uppercase;
    letter-spacing: 0.14em;
    margin-bottom: 16px;
  }
  .hero-eyebrow::before {
    content: "";
    width: 6px;
    height: 6px;
    background: var(--accent);
    border-radius: 50%;
    animation: pulse 2s infinite;
    box-shadow: 0 0 0 4px rgba(255, 95, 31, 0.18);
  }
  @keyframes pulse {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.4; }
  }

  h1.hero-title {
    font-family: var(--display);
    font-weight: 800;
    font-size: clamp(48px, 5.4vw, 76px);
    line-height: 1.02;
    letter-spacing: -0.035em;
    margin-bottom: 28px;
    color: var(--ink);
  }
  h1.hero-title .accent {
    color: var(--accent);
    font-weight: 800;
  }

  .hero-sub {
    font-family: var(--body);
    font-size: 18px;
    line-height: 1.6;
    color: var(--ink-2);
    max-width: 580px;
    margin-bottom: 36px;
    font-weight: 400;
  }
  .hero-sub strong {
    color: var(--ink);
    font-weight: 700;
  }

  .hero-stats {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 0;
    padding: 28px 0;
    border-top: 2px solid var(--ink);
    border-bottom: 1px solid var(--border-strong);
    margin-bottom: 36px;
  }
  .stat {
    padding: 0 20px;
    border-right: 1px solid var(--border-strong);
  }
  .stat:first-child { padding-left: 0; }
  .stat:last-child { border-right: none; padding-right: 0; }
  .stat-num {
    font-family: var(--display);
    font-weight: 800;
    font-size: 38px;
    line-height: 1;
    letter-spacing: -0.03em;
    color: var(--ink);
  }
  .stat-num .unit {
    color: var(--accent);
    font-size: 22px;
    margin-left: 1px;
    font-weight: 700;
  }
  .stat-label {
    font-family: var(--mono);
    font-size: 10px;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    color: var(--ink-muted);
    margin-top: 6px;
  }

  .hero-references-label {
    font-family: var(--mono);
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 0.14em;
    color: var(--ink-muted);
    margin-bottom: 14px;
    font-weight: 500;
  }
  .hero-references {
    display: flex;
    gap: 28px;
    align-items: center;
    flex-wrap: wrap;
  }
  .reference-item {
    font-family: var(--display);
    font-weight: 700;
    font-size: 16px;
    color: var(--ink-2);
    letter-spacing: -0.005em;
    transition: color 0.2s;
  }
  .reference-item:hover { color: var(--accent); }

  /* ========== CONFIGURATOR ========== */
  .configurator {
    background: var(--surface);
    border: 1px solid var(--border-strong);
    border-radius: 16px;
    padding: 36px;
    box-shadow:
      0 2px 4px rgba(0,0,0,0.02),
      0 16px 40px rgba(0,0,0,0.10),
      0 32px 80px rgba(255, 95, 31, 0.06);
    overflow: hidden;
  }

  .config-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 24px;
    gap: 16px;
  }
  .config-title-block {
    display: flex;
    align-items: center;
    gap: 12px;
  }
  .config-titles {
    display: flex;
    flex-direction: column;
    gap: 2px;
  }
  .config-eyebrow {
    font-family: var(--mono);
    font-size: 10px;
    text-transform: uppercase;
    letter-spacing: 0.14em;
    color: var(--accent);
  }
  .config-title {
    font-family: var(--display);
    font-weight: 800;
    font-size: 20px;
    letter-spacing: -0.02em;
    color: var(--ink);
  }
  .step-indicator {
    font-family: var(--mono);
    font-size: 11px;
    color: var(--ink-muted);
    text-align: right;
    padding-top: 14px;
    flex-shrink: 0;
  }
  .step-indicator strong { color: var(--accent); font-weight: 700; }

  .progress-track {
    height: 4px;
    background: var(--bg-2);
    border-radius: 100px;
    margin-bottom: 28px;
    overflow: hidden;
  }
  .progress-fill {
    height: 100%;
    background: var(--accent);
    border-radius: 100px;
    width: 20%;
    transition: width 0.5s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .config-question {
    font-family: var(--display);
    font-weight: 700;
    font-size: 21px;
    line-height: 1.25;
    letter-spacing: -0.02em;
    margin-bottom: 8px;
    color: var(--ink);
  }
  .config-helper {
    font-size: 14px;
    color: var(--ink-muted);
    margin-bottom: 20px;
  }

  .config-options {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-bottom: 24px;
  }
  .config-option {
    background: var(--surface-2);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 16px 20px;
    text-align: left;
    color: var(--ink);
    font-family: var(--body);
    font-size: 15px;
    font-weight: 500;
    cursor: pointer;
    transition: all 0.2s;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .config-option:hover {
    border-color: var(--accent);
    background: var(--accent-soft);
    transform: translateX(2px);
  }
  .config-option.selected {
    border-color: var(--accent);
    background: var(--accent-soft);
  }
  .config-option .arrow {
    color: var(--ink-dim);
    font-family: var(--mono);
    transition: color 0.2s, transform 0.2s;
  }
  .config-option:hover .arrow {
    color: var(--accent);
    transform: translateX(4px);
  }

  .config-input-row {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-bottom: 20px;
  }
  .config-input {
    background: var(--surface-2);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 14px 16px;
    color: var(--ink);
    font-family: var(--body);
    font-size: 15px;
    width: 100%;
    transition: border-color 0.2s;
  }
  .config-input:focus {
    outline: none;
    border-color: var(--accent);
    background: var(--surface);
  }
  .config-input::placeholder {
    color: var(--ink-dim);
  }

  .config-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 8px;
  }
  .config-back {
    background: none;
    border: none;
    color: var(--ink-muted);
    font-family: var(--body);
    font-size: 14px;
    cursor: pointer;
    padding: 8px 0;
    transition: color 0.2s;
  }
  .config-back:hover { color: var(--ink); }
  .config-back:disabled { opacity: 0; pointer-events: none; }

  .config-submit {
    background: var(--ink);
    color: white;
    border: none;
    padding: 14px 24px;
    font-family: var(--body);
    font-weight: 700;
    font-size: 14px;
    border-radius: 100px;
    cursor: pointer;
    transition: background 0.2s, transform 0.2s;
    display: inline-flex;
    align-items: center;
    gap: 8px;
  }
  .config-submit:hover {
    background: var(--accent);
    transform: translateY(-1px);
  }

  /* === RESULT VIEW === */
  .config-result { text-align: left; }
  .result-headline {
    font-family: var(--display);
    font-weight: 800;
    font-size: 24px;
    line-height: 1.2;
    letter-spacing: -0.025em;
    margin-bottom: 6px;
    color: var(--ink);
  }
  .result-sub {
    font-size: 14px;
    color: var(--ink-muted);
    margin-bottom: 22px;
  }
  .result-card {
    background: linear-gradient(135deg, var(--accent-soft) 0%, transparent 100%);
    border: 1px solid var(--accent);
    border-radius: 12px;
    padding: 24px;
    margin-bottom: 18px;
  }
  .result-stat-label {
    font-family: var(--mono);
    font-size: 10px;
    text-transform: uppercase;
    letter-spacing: 0.14em;
    color: var(--accent-deep);
    margin-bottom: 10px;
  }
  .result-stat-value {
    font-family: var(--display);
    font-weight: 900;
    font-size: 44px;
    letter-spacing: -0.03em;
    line-height: 1;
    margin-bottom: 4px;
    color: var(--ink);
  }
  .result-stat-detail {
    font-size: 13px;
    color: var(--ink-muted);
  }
  .result-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 0;
    font-size: 14px;
    border-bottom: 1px solid var(--border);
  }
  .result-row:last-of-type { border-bottom: none; }
  .result-row .label { color: var(--ink-muted); }
  .result-row .value {
    font-family: var(--mono);
    font-weight: 500;
    color: var(--ink);
  }
  .result-row .value strong { color: var(--accent); font-weight: 700; }

  .result-cta-stack {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-top: 20px;
  }
  .result-cta-primary {
    background: var(--accent);
    color: white;
    padding: 15px;
    border: none;
    border-radius: 100px;
    font-family: var(--body);
    font-weight: 700;
    font-size: 14px;
    cursor: pointer;
    text-align: center;
    transition: background 0.2s, transform 0.2s;
  }
  .result-cta-primary:hover {
    background: var(--accent-deep);
    transform: translateY(-1px);
  }
  .result-cta-secondary {
    background: transparent;
    color: var(--ink);
    padding: 15px;
    border: 1px solid var(--border-strong);
    border-radius: 100px;
    font-family: var(--body);
    font-weight: 600;
    font-size: 14px;
    cursor: pointer;
    text-align: center;
  }
  .result-cta-secondary:hover {
    border-color: var(--accent);
    color: var(--accent);
  }

  /* ========== SECTIONS ========== */
  .section {
    padding: 110px 0;
    border-top: 1px solid var(--border);
    position: relative;
  }
  .section-eyebrow {
    font-family: var(--mono);
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 0.16em;
    color: var(--accent);
    margin-bottom: 16px;
    display: inline-flex;
    align-items: center;
    gap: 8px;
  }
  .section-title {
    font-family: var(--display);
    font-weight: 800;
    font-size: clamp(40px, 4.6vw, 60px);
    letter-spacing: -0.03em;
    line-height: 1.04;
    margin-bottom: 20px;
    max-width: 920px;
    color: var(--ink);
  }
  .section-title .accent {
    color: var(--accent);
    font-weight: 800;
  }
  .section-sub {
    font-size: 17px;
    color: var(--ink-2);
    max-width: 680px;
    margin-bottom: 56px;
    font-family: var(--body);
    font-weight: 400;
    line-height: 1.6;
  }

  /* ========== PALLY'S RESUME ========== */
  .resume-section {
    background: var(--surface);
    border-top: 1px solid var(--border);
  }
  .resume-grid {
    display: grid;
    grid-template-columns: 1fr 1.4fr;
    gap: 64px;
    align-items: start;
  }
  .resume-side {
    position: sticky;
    top: 96px;
  }
  .resume-portrait {
    background: var(--bg);
    border: 1px solid var(--border-strong);
    border-radius: 16px;
    overflow: hidden;
  }
  .pally-product-photo {
    width: 100%;
    height: auto;
    display: block;
    aspect-ratio: 5 / 4;
    object-fit: cover;
    background: var(--ink);
  }
  .resume-name {
    font-family: var(--display);
    font-weight: 900;
    font-size: 32px;
    letter-spacing: -0.025em;
    color: var(--ink);
    line-height: 1;
    margin: 28px 28px 6px;
  }
  .resume-role {
    font-family: var(--mono);
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 0.14em;
    color: var(--accent);
    margin: 0 28px 18px;
  }
  .resume-tagline {
    font-family: var(--body);
    font-size: 14px;
    color: var(--ink-2);
    line-height: 1.55;
    margin: 0 28px 28px;
    padding-top: 18px;
    border-top: 1px solid var(--border);
  }

  .resume-content {
    display: flex;
    flex-direction: column;
    gap: 40px;
  }
  .resume-block h3 {
    font-family: var(--mono);
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 0.16em;
    color: var(--ink-muted);
    margin-bottom: 16px;
    padding-bottom: 12px;
    border-bottom: 1px solid var(--border);
  }
  .resume-block p {
    font-family: var(--body);
    font-size: 16px;
    line-height: 1.65;
    color: var(--ink);
    margin-bottom: 14px;
  }
  .resume-block p strong { font-weight: 700; }
  .resume-block .quiet {
    font-family: var(--body);
    font-size: 14px;
    color: var(--ink-muted);
    line-height: 1.6;
  }

  .resume-skills {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
  }
  .skill {
    display: flex;
    align-items: flex-start;
    gap: 12px;
    padding: 14px 16px;
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 10px;
  }
  .skill-icon {
    width: 22px;
    height: 22px;
    flex-shrink: 0;
    color: var(--accent);
    margin-top: 1px;
  }
  .skill-text {
    font-size: 14px;
    line-height: 1.4;
    color: var(--ink);
    font-weight: 500;
  }
  .skill-text small {
    display: block;
    font-weight: 400;
    color: var(--ink-muted);
    font-size: 12px;
    margin-top: 2px;
  }

  /* ========== DAY IN THE LIFE ========== */
  .day-section {
    background: var(--bg-2);
  }
  .day-timeline {
    display: grid;
    grid-template-columns: 60px 1fr;
    gap: 0;
    max-width: 880px;
  }
  .day-row {
    display: contents;
  }
  .day-time {
    font-family: var(--mono);
    font-size: 13px;
    font-weight: 700;
    color: var(--accent);
    padding: 24px 0;
    text-align: right;
    padding-right: 28px;
    border-right: 2px solid var(--border-strong);
    position: relative;
  }
  .day-time::after {
    content: "";
    position: absolute;
    right: -7px;
    top: 30px;
    width: 12px;
    height: 12px;
    background: var(--accent);
    border-radius: 50%;
    border: 3px solid var(--bg-2);
  }
  .day-content {
    padding: 24px 0 24px 28px;
  }
  .day-event {
    font-family: var(--display);
    font-size: 20px;
    font-weight: 700;
    line-height: 1.25;
    color: var(--ink);
    margin-bottom: 6px;
    letter-spacing: -0.015em;
  }
  .day-detail {
    font-size: 14px;
    color: var(--ink-muted);
    line-height: 1.55;
  }

  /* ========== THE MATH ========== */
  .math-section {
    background: var(--ink);
    color: white;
    border-top: none;
  }
  .math-section .section-eyebrow { color: var(--yellow); }
  .math-section .section-title { color: white; }
  .math-section .section-title .accent { color: var(--accent); }
  .math-section .section-sub { color: rgba(255,255,255,0.7); }

  .math-comparison {
    display: grid;
    grid-template-columns: 1fr 80px 1fr;
    gap: 24px;
    align-items: stretch;
    margin-top: 32px;
  }
  .compare-card {
    background: rgba(255,255,255,0.04);
    border: 1px solid rgba(255,255,255,0.10);
    border-radius: 16px;
    padding: 36px;
    display: flex;
    flex-direction: column;
  }
  .compare-card.pally {
    background: var(--accent);
    border-color: var(--accent);
    color: white;
  }
  .compare-label {
    font-family: var(--mono);
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 0.14em;
    color: rgba(255,255,255,0.6);
    margin-bottom: 12px;
  }
  .compare-card.pally .compare-label { color: rgba(255,255,255,0.85); }
  .compare-name {
    font-family: var(--display);
    font-weight: 800;
    font-size: 28px;
    letter-spacing: -0.025em;
    line-height: 1.1;
    margin-bottom: 24px;
  }
  .compare-stats {
    flex: 1;
    display: flex;
    flex-direction: column;
    gap: 14px;
  }
  .compare-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-bottom: 10px;
    border-bottom: 1px solid rgba(255,255,255,0.10);
  }
  .compare-card.pally .compare-row {
    border-bottom-color: rgba(255,255,255,0.25);
  }
  .compare-row:last-child { border-bottom: none; }
  .compare-row .compare-key {
    font-size: 13px;
    color: rgba(255,255,255,0.7);
  }
  .compare-card.pally .compare-row .compare-key { color: rgba(255,255,255,0.9); }
  .compare-row .compare-value {
    font-family: var(--mono);
    font-weight: 700;
    font-size: 15px;
  }
  .compare-card .total-row {
    margin-top: auto;
    padding-top: 24px;
    border-top: 2px solid rgba(255,255,255,0.20);
    border-bottom: none !important;
  }
  .compare-card.pally .total-row {
    border-top-color: rgba(255,255,255,0.40);
  }
  .total-row .compare-key {
    font-size: 14px !important;
    color: white !important;
    font-weight: 600;
  }
  .total-row .compare-value {
    font-family: var(--display);
    font-size: 28px !important;
    font-weight: 800;
  }

  .compare-vs {
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: var(--serif);
    font-style: italic;
    font-weight: 600;
    font-size: 32px;
    color: rgba(255,255,255,0.4);
  }

  .math-callout {
    text-align: center;
    margin-top: 56px;
    padding: 32px;
    background: rgba(255, 95, 31, 0.08);
    border: 1px dashed var(--accent);
    border-radius: 16px;
  }
  .math-callout-text {
    font-family: var(--display);
    font-weight: 700;
    font-size: 22px;
    line-height: 1.4;
    color: white;
    letter-spacing: -0.02em;
  }
  .math-callout-text .highlight {
    background: var(--accent);
    color: white;
    padding: 0 8px;
    border-radius: 4px;
    font-weight: 700;
  }

  /* ========== REFERENCES ========== */
  .references-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 24px;
  }
  .reference-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 36px;
    transition: border-color 0.3s, transform 0.3s, box-shadow 0.3s;
  }
  .reference-card:hover {
    border-color: var(--accent);
    transform: translateY(-3px);
    box-shadow: 0 16px 40px rgba(0,0,0,0.08);
  }
  .reference-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 24px;
    padding-bottom: 24px;
    border-bottom: 1px solid var(--border);
  }
  .reference-name {
    font-family: var(--display);
    font-weight: 800;
    font-size: 22px;
    letter-spacing: -0.02em;
    color: var(--ink);
  }
  .reference-vertical {
    font-family: var(--mono);
    font-size: 10px;
    color: var(--accent);
    text-transform: uppercase;
    letter-spacing: 0.12em;
    padding: 5px 10px;
    background: var(--accent-soft);
    border-radius: 100px;
  }
  .reference-headline {
    font-family: var(--display);
    font-weight: 800;
    font-size: 22px;
    line-height: 1.25;
    letter-spacing: -0.02em;
    color: var(--ink);
    margin-bottom: 12px;
  }
  .reference-headline .num {
    color: var(--accent);
    font-weight: 800;
  }
  .reference-detail {
    font-size: 15px;
    color: var(--ink-muted);
    line-height: 1.55;
    margin-bottom: 20px;
  }
  .reference-quote {
    font-family: var(--serif);
    font-style: italic;
    font-size: 15px;
    line-height: 1.6;
    color: var(--ink);
    padding: 20px 0 0;
    border-top: 1px solid var(--border);
  }
  .reference-attribution {
    font-family: var(--mono);
    font-size: 11px;
    color: var(--ink-muted);
    text-transform: uppercase;
    letter-spacing: 0.1em;
    margin-top: 14px;
  }

  /* ========== TECHNICAL SPECS ========== */
  .specs-section {
    background: var(--bg-2);
  }
  .specs-grid-2col {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 56px;
    margin-top: 32px;
  }
  .specs-col h4 {
    font-family: var(--mono);
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 0.16em;
    color: var(--accent);
    margin-bottom: 20px;
    padding-bottom: 12px;
    border-bottom: 2px solid var(--ink);
  }
  .spec-row {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    padding: 14px 0;
    border-bottom: 1px solid var(--border);
    gap: 24px;
  }
  .spec-row:last-child { border-bottom: none; }
  .spec-key {
    font-family: var(--body);
    font-size: 14px;
    color: var(--ink-muted);
    flex-shrink: 0;
  }
  .spec-value {
    font-family: var(--mono);
    font-weight: 500;
    font-size: 14px;
    color: var(--ink);
    text-align: right;
  }
  .spec-value strong { color: var(--accent); font-weight: 700; }
  .specs-footnote {
    font-family: var(--mono);
    font-size: 11px;
    color: var(--ink-dim);
    text-transform: uppercase;
    letter-spacing: 0.1em;
    margin-top: 32px;
    padding-top: 24px;
    border-top: 1px solid var(--border);
  }

  /* ========== COMPARE PALLY VS AGV ========== */
  .compare-section {
    background: var(--surface);
    border-top: 1px solid var(--border);
  }
  .compare-table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 32px;
    background: var(--surface);
  }
  .compare-table thead th {
    font-family: var(--mono);
    font-size: 11px;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.14em;
    text-align: left;
    padding: 16px 20px;
    border-bottom: 2px solid var(--ink);
    color: var(--ink-muted);
  }
  .compare-table thead th.pally-col {
    background: var(--accent-soft);
    color: var(--accent-deep);
  }
  .compare-table tbody td {
    padding: 18px 20px;
    border-bottom: 1px solid var(--border);
    font-size: 15px;
    line-height: 1.5;
    vertical-align: top;
  }
  .compare-table tbody td.dimension {
    font-family: var(--display);
    font-weight: 700;
    color: var(--ink);
    width: 24%;
  }
  .compare-table tbody td.legacy {
    color: var(--ink-muted);
    width: 38%;
  }
  .compare-table tbody td.pally-col {
    background: var(--accent-soft);
    color: var(--ink);
    font-weight: 500;
    width: 38%;
  }
  .compare-table tbody td.pally-col strong { color: var(--accent-deep); }
  .compare-table tbody tr:last-child td { border-bottom: none; }

  /* ========== FAQ ========== */
  .faq-section {
    background: var(--bg-2);
  }
  .faq-list {
    max-width: 920px;
    margin-top: 32px;
  }
  .faq-item {
    border-bottom: 1px solid var(--border-strong);
    padding: 28px 0;
  }
  .faq-item:first-child { padding-top: 0; }
  .faq-q {
    font-family: var(--display);
    font-weight: 700;
    font-size: 22px;
    line-height: 1.3;
    letter-spacing: -0.015em;
    color: var(--ink);
    margin-bottom: 12px;
    display: flex;
    align-items: baseline;
    gap: 16px;
  }
  .faq-q-num {
    font-family: var(--mono);
    font-size: 13px;
    color: var(--accent);
    font-weight: 500;
    flex-shrink: 0;
  }
  .faq-a {
    font-family: var(--body);
    font-size: 16px;
    line-height: 1.65;
    color: var(--ink-2);
    padding-left: 40px;
  }
  .faq-a strong { color: var(--ink); font-weight: 600; }
  .faq-a .source {
    display: block;
    margin-top: 10px;
    font-family: var(--mono);
    font-size: 11px;
    color: var(--ink-dim);
    text-transform: uppercase;
    letter-spacing: 0.1em;
  }

  /* ========== MATH SOURCES FOOTNOTE ========== */
  .math-sources {
    margin-top: 40px;
    padding: 24px 28px;
    background: rgba(255,255,255,0.04);
    border-left: 2px solid var(--yellow);
    border-radius: 0 8px 8px 0;
  }
  .math-sources-label {
    font-family: var(--mono);
    font-size: 10px;
    text-transform: uppercase;
    letter-spacing: 0.16em;
    color: var(--yellow);
    margin-bottom: 12px;
  }
  .math-sources p {
    font-size: 13px;
    line-height: 1.6;
    color: rgba(255,255,255,0.7);
    margin-bottom: 8px;
  }
  .math-sources p:last-child { margin-bottom: 0; }
  .math-sources strong { color: white; }

  @media (max-width: 1100px) {
    .specs-grid-2col { grid-template-columns: 1fr; gap: 40px; }
    .compare-table thead th { font-size: 10px; padding: 12px 12px; }
    .compare-table tbody td { padding: 14px 12px; font-size: 13px; }
    .compare-table tbody td.dimension { font-size: 14px; }
  }
  .bottom-cta {
    padding: 130px 0;
    text-align: center;
    background:
      radial-gradient(ellipse at top, var(--accent-soft) 0%, transparent 60%),
      var(--bg);
    border-top: 1px solid var(--border);
    position: relative;
    overflow: hidden;
  }
  .bottom-cta-pally {
    width: 160px;
    height: auto;
    margin: 0 auto 20px;
    display: block;
    filter: drop-shadow(0 12px 28px rgba(0,0,0,0.12));
  }
  .bottom-cta h2 {
    font-family: var(--display);
    font-weight: 800;
    font-size: clamp(44px, 5.5vw, 76px);
    letter-spacing: -0.035em;
    line-height: 1.02;
    max-width: 920px;
    margin: 0 auto 24px;
    color: var(--ink);
  }
  .bottom-cta h2 .accent {
    color: var(--accent);
    font-weight: 800;
  }
  .bottom-cta p {
    font-family: var(--body);
    font-size: 17px;
    color: var(--ink-2);
    margin-bottom: 40px;
    max-width: 620px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.6;
  }
  .bottom-cta-buttons {
    display: flex;
    gap: 14px;
    justify-content: center;
    flex-wrap: wrap;
  }
  .btn-primary-large {
    background: var(--ink);
    color: white;
    border: none;
    padding: 18px 38px;
    font-family: var(--body);
    font-weight: 700;
    font-size: 16px;
    border-radius: 100px;
    cursor: pointer;
    text-decoration: none;
    display: inline-flex;
    align-items: center;
    gap: 10px;
    transition: transform 0.2s, background 0.2s;
  }
  .btn-primary-large:hover {
    background: var(--accent);
    transform: translateY(-2px);
  }
  .btn-secondary-large {
    background: transparent;
    color: var(--ink);
    border: 1px solid var(--border-strong);
    padding: 18px 38px;
    font-family: var(--body);
    font-weight: 600;
    font-size: 16px;
    border-radius: 100px;
    cursor: pointer;
    text-decoration: none;
    display: inline-flex;
    align-items: center;
    gap: 10px;
  }
  .btn-secondary-large:hover {
    border-color: var(--accent);
    color: var(--accent);
  }

  /* ========== FOOTER ========== */
  footer {
    padding: 56px 0 48px;
    border-top: 1px solid var(--border);
    background: var(--bg-2);
  }
  .footer-inner {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 13px;
    color: var(--ink-muted);
  }
  .footer-inner a {
    color: var(--ink-muted);
    text-decoration: none;
    margin-left: 24px;
  }
  .footer-inner a:hover { color: var(--accent); }

  /* ========== RESPONSIVE ========== */
  @media (max-width: 1100px) {
    .hero-grid {
      grid-template-columns: 1fr;
      gap: 36px;
    }
    .hero-image-wrap {
      order: -1;
      max-width: 560px;
      margin: 0 auto;
      width: 100%;
      aspect-ratio: 4 / 3;
    }
    .resume-grid { grid-template-columns: 1fr; gap: 40px; }
    .resume-side { position: static; }
    .references-grid { grid-template-columns: 1fr; }
    .math-comparison { grid-template-columns: 1fr; }
    .compare-vs { padding: 12px; }
    .resume-skills { grid-template-columns: 1fr; }
  }
  @media (max-width: 640px) {
    .container { padding: 0 20px; }
    .hero { padding: 40px 0 56px; }
    .config-band { padding: 64px 0 80px; }
    .nav-links { display: none; }
    .hero-stats { grid-template-columns: 1fr 1fr; gap: 24px; padding: 24px 0; }
    .stat { padding: 0; border-right: none; }
    .stat-num { font-size: 30px; }
    .day-timeline { grid-template-columns: 50px 1fr; }
    .hero-cta-row { flex-direction: column; align-items: stretch; }
    .hero-cta-primary, .hero-cta-secondary { justify-content: center; }
    .configurator { padding: 24px; }
  }

  /* ========== ANIMATION ========== */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(24px); }
    to { opacity: 1; transform: translateY(0); }
  }
  .reveal {
    opacity: 0;
    animation: fadeUp 0.9s cubic-bezier(0.16, 1, 0.3, 1) forwards;
  }
  .reveal-1 { animation-delay: 0.1s; }
  .reveal-2 { animation-delay: 0.2s; }
  .reveal-3 { animation-delay: 0.3s; }
  .reveal-4 { animation-delay: 0.4s; }
  .reveal-5 { animation-delay: 0.5s; }
  .reveal-6 { animation-delay: 0.6s; }

  /* Concept demo badge */
  .design-note {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background: var(--ink);
    color: white;
    padding: 12px 16px;
    border-radius: 100px;
    font-family: var(--mono);
    font-size: 11px;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    z-index: 1000;
    box-shadow: 0 8px 24px rgba(0,0,0,0.20);
    cursor: pointer;
    user-select: none;
    border: 2px solid var(--accent);
  }
  .design-note:hover { background: var(--accent); border-color: var(--ink); }
</style>
</head>
<body>

<!-- ============ NAV ============ -->
<nav>
  <div class="container nav-inner">
    <a href="#" class="logo">
      <svg class="logo-mark-svg" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
        <!-- Stylized Cyngn-style geometric diamond mark -->
        <polygon points="16,3 27,10 27,22 16,29 5,22 5,10" fill="none" stroke="#FF5F1F" stroke-width="2.4" stroke-linejoin="round"/>
        <polygon points="16,9 22,12.5 22,19.5 16,23 10,19.5 10,12.5" fill="#FF5F1F"/>
      </svg>
      <div class="logo-text">
        <div class="logo-name">pally</div>
        <div class="logo-by">by Cyngn · NASDAQ: CYN</div>
      </div>
    </a>
    <ul class="nav-links">
      <li><a href="#meet">Meet Pally</a></li>
      <li><a href="#specs">Specs</a></li>
      <li><a href="#compare">vs. AGVs</a></li>
      <li><a href="#math">The math</a></li>
      <li><a href="#references">Deployments</a></li>
      <li><a href="#faq">FAQ</a></li>
    </ul>
    <div class="nav-cta">
      <a href="#" class="nav-cta-secondary">Sign in</a>
      <a href="#configurator" class="nav-cta-primary">Configure pilot →</a>
    </div>
  </div>
</nav>

<!-- ============ HERO ============ -->
<section class="hero">
  <div class="container hero-grid">
    <div class="hero-content">
      <div class="hero-eyebrow reveal reveal-2">DriveMod-enabled · Built on Motrec MT-160</div>

      <h1 class="hero-title reveal reveal-3">
        Meet Pally.<br>
        Your <span class="accent">AI Tugger.</span>
      </h1>

      <p class="hero-sub reveal reveal-4">
        Pally hauls up to <strong>12,000 lbs</strong> indoors and out — handling the predictable, repeatable transport runs while your team focuses on machining, picking, and quality.
      </p>

      <div class="hero-stats reveal reveal-5">
        <div class="stat">
          <div class="stat-num">12,000<span class="unit">lb</span></div>
          <div class="stat-label">Tow capacity</div>
        </div>
        <div class="stat">
          <div class="stat-num">+33<span class="unit">%</span></div>
          <div class="stat-label">Productivity / shift</div>
        </div>
        <div class="stat">
          <div class="stat-num">−64<span class="unit">%</span></div>
          <div class="stat-label">Labor cost / route</div>
        </div>
        <div class="stat">
          <div class="stat-num">18<span class="unit">mo</span></div>
          <div class="stat-label">Avg. payback</div>
        </div>
      </div>

      <div class="reveal reveal-6">
        <div class="hero-references-label">Deployed today at</div>
        <div class="hero-references">
          <span class="reference-item">G&amp;J Pepsi</span>
          <span class="reference-item">DHL</span>
          <span class="reference-item">Coats</span>
          <span class="reference-item">Vann Family Orchards</span>
          <span class="reference-item">U.S. Continental</span>
          <span class="reference-item">Arauco</span>
        </div>
      </div>

      <div class="hero-cta-row reveal reveal-6">
        <a href="#configurator" class="hero-cta-primary">Configure your pilot ↓</a>
        <a href="#meet" class="hero-cta-secondary">Learn more about Pally</a>
      </div>
    </div>

    <div class="hero-image-wrap reveal reveal-1">
      <img src="img/pally-hero.jpg" alt="Pally — DriveMod-enabled Motrec MT-160 autonomous tow tractor" class="pally-hero-photo">
    </div>
  </div>
</section>

<!-- ============ CONFIGURATOR (full-width band) ============ -->
<section id="configurator" class="config-band">
  <div class="container">
    <div class="config-band-inner">
      <div class="config-band-header">
        <div class="section-eyebrow">→ Pilot configurator</div>
        <h2 class="config-band-title">Configure your <span class="accent">DriveMod pilot</span> in 60 seconds.</h2>
        <p class="config-band-sub">Five questions. We'll generate a customer-specific ROI estimate and route a real solutions engineer to follow up within 24 hours.</p>
      </div>

      <div class="configurator">
        <div class="config-header">
          <div class="config-title-block">
            <div class="config-titles">
              <div class="config-eyebrow">→ Pilot configurator</div>
              <div class="config-title">Tell us about your operation</div>
            </div>
          </div>
          <div class="step-indicator">
            Q&nbsp;<strong id="stepNum">1</strong>&nbsp;of&nbsp;<span>5</span>
          </div>
        </div>

        <div class="progress-track">
          <div class="progress-fill" id="progressFill"></div>
        </div>

        <div id="configContent">
          <!-- Dynamic content -->
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ MEET PALLY (PRODUCT OVERVIEW) ============ -->
<section id="meet" class="section resume-section">
  <div class="container">
    <div class="section-eyebrow">→ Meet Pally</div>
    <h2 class="section-title">The autonomous tugger, built on a <span class="accent">proven industrial chassis.</span></h2>
    <p class="section-sub">Pally is what happens when Cyngn's DriveMod autonomy stack runs on the Motrec MT-160 — the stand-up tow tractor used in casinos, manufacturing plants, and distribution centers across North America for over a decade. Real OEM hardware, real autonomy IP, deployed alongside the team you already have.</p>

    <div class="resume-grid">
      <div class="resume-side">
        <div class="resume-portrait">
          <img src="img/pally-product.jpg" alt="Pally — front three-quarter view with Cyngn branded backdrop" class="pally-product-photo">
          <div class="resume-name">Pally</div>
          <div class="resume-role">Autonomous tow tractor · 12,000 lb capacity</div>
          <div class="resume-tagline">DriveMod autonomy on the Motrec MT-160 chassis. Indoor and outdoor. WMS-integrated. Zero infrastructure required.</div>
        </div>
      </div>

      <div class="resume-content">
        <div class="resume-block">
          <h3>What Pally does</h3>
          <p>Pally automates predictable, repeatable material transport — the runs between machining and warehouse storage, between buildings, between zones in connected facilities. It tows up to 12,000 lbs across multi-cart trains, runs continuously across all three shifts, and reroutes in real time based on WMS-dispatched missions.</p>
          <p class="quiet">Cyngn's CEO Lior Tal frames it directly: "DriveMod handles predictable, repeatable movement, while forklifts and skilled labor stay focused on machining and warehouse operations." U.S. Continental absorbed roughly 200 forklift trips per week. Coats unlocked 500+ labor hours at their 150K sq ft Tennessee facility. WEG Electric Motor automated 60 pallets per day at their Bluffton, Indiana plant.</p>
        </div>

        <div class="resume-block">
          <h3>How Pally is built</h3>
          <p>The chassis is the Motrec MT-160 — a 30" stand-up tow tractor with a 15 HP brushless AC motor, regenerative braking, and a decade of industrial deployment behind it. The autonomy stack is Cyngn's DriveMod: 3D LiDAR perception, 3D semantic mapping, predictive trajectory tracking for pedestrian safety, and patented motion compensation (U.S. Patent No. 12,032,099).</p>
          <p class="quiet">Real OEM hardware, real autonomy IP. No retrofit project, no integration risk, no "phase two" that never ships.</p>
        </div>

        <div class="resume-block">
          <h3>Where Pally works</h3>
          <p>Indoor and outdoor environments, including transitions between buildings. Minimum aisle width of 55". Operates on facility maps generated during initial deployment — no magnetic strips, no QR markers, no infrastructure modifications. Three control surfaces: on-vehicle HMI, cloud FMS (Cyngn Insight), and tablet stations placed throughout the facility.</p>
          <p class="quiet">Currently deployed across food &amp; beverage, agriculture, manufacturing, and logistics. Hardware platform manufactured by Motrec in Quebec, Canada.</p>
        </div>

        <div class="resume-block">
          <h3>What Pally costs</h3>
          <p>Capex purchase or financed structure. Cyngn customer benchmarks show an average payback period of 18 months and 64% reduction in direct labor cost per route. Detailed pricing depends on fleet size, deployment scope, financing structure, and facility complexity — the configurator above generates a customer-specific estimate.</p>
        </div>

        <div class="resume-block">
          <h3>How long it takes</h3>
          <p>Roughly <strong>90 days</strong> from offer letter to first shift on the floor. Two weeks for facility assessment and ROI modeling. Four to six weeks for vehicle integration and shipping. Two to four weeks for on-site mapping, WMS integration, and operator training. No facility shutdown required at any phase.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ TECHNICAL SPECS ============ -->
<section id="specs" class="section specs-section">
  <div class="container">
    <div class="section-eyebrow">→ Technical specifications</div>
    <h2 class="section-title">The <span class="accent">datasheet.</span></h2>
    <p class="section-sub">For the plant engineers, procurement teams, and integrators who need real numbers before forwarding this to operations leadership.</p>

    <div class="specs-grid-2col">
      <div class="specs-col">
        <h4>Vehicle &amp; Platform</h4>
        <div class="spec-row">
          <span class="spec-key">Hardware platform</span>
          <span class="spec-value">Motrec MT-160</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Train towing capacity</span>
          <span class="spec-value"><strong>up to 12,000 lbs</strong></span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Vehicle width</span>
          <span class="spec-value">30 inches</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Minimum aisle width</span>
          <span class="spec-value">55 inches</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Max speed</span>
          <span class="spec-value">6 mph (configurable)</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Motor</span>
          <span class="spec-value">15 HP 48V brushless AC</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Power options</span>
          <span class="spec-value">Lithium-ion or lead-acid</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Braking</span>
          <span class="spec-value">Regenerative + drum + parking</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Operating environment</span>
          <span class="spec-value">Indoor + outdoor</span>
        </div>
      </div>

      <div class="specs-col">
        <h4>Autonomy &amp; Control</h4>
        <div class="spec-row">
          <span class="spec-key">Perception</span>
          <span class="spec-value">3D LiDAR + multi-layer</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Localization</span>
          <span class="spec-value">3D semantic map</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Infrastructure required</span>
          <span class="spec-value"><strong>None</strong></span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Operating modes</span>
          <span class="spec-value">Autonomous + manual</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Cart compatibility</span>
          <span class="spec-value">Any cart, quad-steer preferred</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Control interfaces</span>
          <span class="spec-value">On-vehicle HMI, cloud FMS, tablets</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Fleet management</span>
          <span class="spec-value">Cyngn Insight</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Safety system</span>
          <span class="spec-value">2× e-stop, LED status, audio cues</span>
        </div>
        <div class="spec-row">
          <span class="spec-key">Patented technology</span>
          <span class="spec-value">U.S. Patent No. 12,032,099</span>
        </div>
      </div>
    </div>

    <div class="specs-footnote">
      Source: Motrec MT-160 product specifications · Cyngn DriveMod Tugger FAQ &amp; spec sheet (cyngn.com) · USPTO patent records
    </div>
  </div>
</section>

<!-- ============ PALLY VS TRADITIONAL AGVs ============ -->
<section id="compare" class="section compare-section">
  <div class="container">
    <div class="section-eyebrow">→ How Pally compares</div>
    <h2 class="section-title">Pally vs. the <span class="accent">AGV you almost bought.</span></h2>
    <p class="section-sub">If you're evaluating Pally against traditional Automated Guided Vehicles — Seegrid, Otto, Vecna, MiR, Locus, Geek+ — these are the differences that matter to a 5-year capex decision.</p>

    <table class="compare-table">
      <thead>
        <tr>
          <th>Capability</th>
          <th>Traditional AGV</th>
          <th class="pally-col">Pally (Cyngn DriveMod)</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="dimension">Infrastructure</td>
          <td class="legacy">Magnetic strips, QR markers, beacons, or wire embedment</td>
          <td class="pally-col"><strong>None.</strong> 3D LiDAR navigation only.</td>
        </tr>
        <tr>
          <td class="dimension">Deployment timeline</td>
          <td class="legacy">4–6 months including facility prep and downtime</td>
          <td class="pally-col"><strong>~90 days</strong> from offer to first shift, no facility downtime</td>
        </tr>
        <tr>
          <td class="dimension">Route changes</td>
          <td class="legacy">Re-engineering: floor work, shutdown windows, integrator visits</td>
          <td class="pally-col">Software configuration update, no facility disruption</td>
        </tr>
        <tr>
          <td class="dimension">Pedestrian safety</td>
          <td class="legacy">Stop-on-contact or 2D obstacle detection</td>
          <td class="pally-col"><strong>Predictive trajectory tracking</strong> via 3D LiDAR — anticipates motion patterns</td>
        </tr>
        <tr>
          <td class="dimension">Map model</td>
          <td class="legacy">2D path-following</td>
          <td class="pally-col">3D semantic map — robust to dynamic environments</td>
        </tr>
        <tr>
          <td class="dimension">Cart compatibility</td>
          <td class="legacy">Vendor-specific carts often required</td>
          <td class="pally-col">Works with carts you already own</td>
        </tr>
        <tr>
          <td class="dimension">Mode flexibility</td>
          <td class="legacy">Autonomous-only — operator override is rare</td>
          <td class="pally-col">Manual mode at any time — driver takes over for edge cases</td>
        </tr>
        <tr>
          <td class="dimension">Mission orchestration</td>
          <td class="legacy">Pre-programmed paths, fixed sequences</td>
          <td class="pally-col">WMS-integrated dispatch, real-time mission re-routing</td>
        </tr>
      </tbody>
    </table>
  </div>
</section>

<!-- ============ DAY IN THE LIFE ============ -->
<section id="day" class="section day-section">
  <div class="container">
    <div class="section-eyebrow">→ A day with Pally</div>
    <h2 class="section-title">An illustrative shift at a <span class="accent">100K sq ft facility.</span></h2>
    <p class="section-sub">A composite scenario based on Cyngn deployment patterns. Not a transcript from a single customer — a synthesized day-in-the-life to show what Pally's role looks like on the floor.</p>

    <div class="day-timeline">
      <div class="day-row">
        <div class="day-time">05:58</div>
        <div class="day-content">
          <div class="day-event">Pre-shift diagnostics complete at the charging dock</div>
          <div class="day-detail">Battery at 98%. System checks pass. Pally is queued for first dispatch.</div>
        </div>
      </div>

      <div class="day-row">
        <div class="day-time">06:01</div>
        <div class="day-content">
          <div class="day-event">First mission picked up at staging</div>
          <div class="day-detail">A 4,200 lb load of WIP material from receiving. Pally executes the dispatched route to assembly bay 3.</div>
        </div>
      </div>

      <div class="day-row">
        <div class="day-time">07:34</div>
        <div class="day-content">
          <div class="day-event">Pedestrian detected — autonomous stop &amp; resume</div>
          <div class="day-detail">A forklift operator crosses the route. 3D LiDAR catches the trajectory at 8 meters out. Total stop duration: 4 seconds. The pedestrian doesn't break stride.</div>
        </div>
      </div>

      <div class="day-row">
        <div class="day-time">11:15</div>
        <div class="day-content">
          <div class="day-event">14 routes complete · 31,800 lb moved</div>
          <div class="day-detail">Material movement across the facility continues uninterrupted while human operators take lunch. No break required.</div>
        </div>
      </div>

      <div class="day-row">
        <div class="day-time">14:22</div>
        <div class="day-content">
          <div class="day-event">WMS dispatches an unscheduled priority pull</div>
          <div class="day-detail">Order changes upstream. The Cyngn Insight FMS reroutes Pally to expedite a hot order from finished goods to outbound. Mission complete in 11 minutes.</div>
        </div>
      </div>

      <div class="day-row">
        <div class="day-time">17:00</div>
        <div class="day-content">
          <div class="day-event">First shift ends · operations continue</div>
          <div class="day-detail">Second-shift supervisor confirms the route plan via the tablet station — 30 seconds of human interaction. Continuous operation across the shift change.</div>
        </div>
      </div>

      <div class="day-row">
        <div class="day-time">22:47</div>
        <div class="day-content">
          <div class="day-event">Second shift complete · headed to dock</div>
          <div class="day-detail">Total shift output: 89,400 lb moved across 38 routes. Average cart-cycle time 23% faster than the manual baseline from Q1.</div>
        </div>
      </div>

      <div class="day-row">
        <div class="day-time">23:15</div>
        <div class="day-content">
          <div class="day-event">Charging · diagnostics streaming to FMS</div>
          <div class="day-detail">Ready for 05:58 dispatch tomorrow. Same configuration. Same reliability. Year over year.</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ THE MATH ============ -->
<section id="math" class="section math-section">
  <div class="container">
    <div class="section-eyebrow">→ The math</div>
    <h2 class="section-title">Pally's hourly rate vs. the human you <span class="accent">can't hire.</span></h2>
    <p class="section-sub">Year-one cost comparison for a single 24/7 tugger route. Conservative inputs. Numbers based on Cyngn customer ROI analyses.</p>

    <div class="math-comparison">
      <div class="compare-card">
        <div class="compare-label">Option A — Status quo</div>
        <div class="compare-name">A human driver<br>across 3 shifts</div>
        <div class="compare-stats">
          <div class="compare-row">
            <span class="compare-key">Annual fully-loaded labor</span>
            <span class="compare-value">$165,000</span>
          </div>
          <div class="compare-row">
            <span class="compare-key">Avg. turnover replacement / yr</span>
            <span class="compare-value">~$8,400</span>
          </div>
          <div class="compare-row">
            <span class="compare-key">Time off / sick / PTO coverage</span>
            <span class="compare-value">~$12,000</span>
          </div>
          <div class="compare-row">
            <span class="compare-key">Safety incident reserve</span>
            <span class="compare-value">~$6,500</span>
          </div>
          <div class="compare-row">
            <span class="compare-key">Productivity (% of theoretical)</span>
            <span class="compare-value">~78%</span>
          </div>
          <div class="compare-row total-row">
            <span class="compare-key">Year-one total</span>
            <span class="compare-value">$191,900</span>
          </div>
        </div>
      </div>

      <div class="compare-vs">vs.</div>

      <div class="compare-card pally">
        <div class="compare-label">Option B — Deploy Pally</div>
        <div class="compare-name">One Pally,<br>same route, 24/7</div>
        <div class="compare-stats">
          <div class="compare-row">
            <span class="compare-key">Capex (amortized year 1)</span>
            <span class="compare-value">~$60,000</span>
          </div>
          <div class="compare-row">
            <span class="compare-key">Software + FMS subscription</span>
            <span class="compare-value">~$9,000</span>
          </div>
          <div class="compare-row">
            <span class="compare-key">Energy + maintenance</span>
            <span class="compare-value">~$3,400</span>
          </div>
          <div class="compare-row">
            <span class="compare-key">Safety incidents (LiDAR-protected)</span>
            <span class="compare-value">→ 0</span>
          </div>
          <div class="compare-row">
            <span class="compare-key">Productivity (% of theoretical)</span>
            <span class="compare-value">~96%</span>
          </div>
          <div class="compare-row total-row">
            <span class="compare-key">Year-one total</span>
            <span class="compare-value">$72,400</span>
          </div>
        </div>
      </div>
    </div>

    <div class="math-callout">
      <div class="math-callout-text">
        Net year-one savings: <span class="highlight">$119,500 per route</span><br>
        Payback in roughly <span class="highlight">14 months</span>. Compounding every year after.
      </div>
    </div>

    <div class="math-sources">
      <div class="math-sources-label">Sources &amp; methodology</div>
      <p><strong>Annual labor cost ($165K / 24-7 facility):</strong> Calculated from BLS Occupational Employment and Wage Statistics, May 2024 — median annual wage for "Hand Laborers and Material Movers" of $37,680 (bls.gov/ooh). Fully loaded with employer payroll taxes, benefits, PTO, and turnover replacement costs (~1.45× multiplier ≈ $54,600/operator/shift). Three shifts × $54,600 ≈ $164,000.</p>
      <p><strong>33% productivity boost · 64% labor cost reduction · 18-month payback:</strong> Cyngn published metrics, sourced from Cyngn customer ROI analyses across deployed DriveMod Tugger installations (cyngn.com).</p>
      <p><strong>Capex / software / energy estimates:</strong> Illustrative inputs intended to demonstrate a customer-facing comparison framework. Customer-specific quotes will vary based on fleet size, deployment scope, financing structure, and facility complexity. Request your customer-specific ROI model below.</p>
    </div>
  </div>
</section>

<!-- ============ REFERENCES ============ -->
<section id="references" class="section">
  <div class="container">
    <div class="section-eyebrow">→ Customer deployments</div>
    <h2 class="section-title">Already on the floor at <span class="accent">production scale.</span></h2>
    <p class="section-sub">Six commercial deployments across food &amp; beverage, agriculture, manufacturing, and logistics. These aren't pilots — they're production fleets running shifts you don't have to staff.</p>

    <div class="references-grid">
      <div class="reference-card">
        <div class="reference-header">
          <div class="reference-name">U.S. Continental</div>
          <div class="reference-vertical">Manufacturing</div>
        </div>
        <div class="reference-headline"><span class="num">200</span> manual forklift trips per week, absorbed.</div>
        <div class="reference-detail">Before DriveMod, U.S. Continental's facility relied on roughly 200 forklift trips per week to handle pallet deliveries between two buildings. Pally automated the workload entirely, contributing to a 4× operational efficiency increase.</div>
        <div class="reference-quote">"I'd definitely recommend the DriveMod Tugger."</div>
        <div class="reference-attribution">— Dave Hoover, VP of Technical Services, U.S. Continental</div>
      </div>

      <div class="reference-card">
        <div class="reference-header">
          <div class="reference-name">Coats</div>
          <div class="reference-vertical">Manufacturing</div>
        </div>
        <div class="reference-headline"><span class="num">500+</span> labor hours unlocked at 150K sq ft facility</div>
        <div class="reference-detail">Coats deployed DriveMod at their 150,000+ sq ft facility in La Vergne, Tennessee, automating wheel service component transport across production lines. The deployment freed 500+ labor hours for higher-judgment work.</div>
        <div class="reference-quote">"I wish we'd found it sooner."</div>
        <div class="reference-attribution">— Steven Finley, VP of Operations, Coats</div>
      </div>

      <div class="reference-card">
        <div class="reference-header">
          <div class="reference-name">G&amp;J Pepsi</div>
          <div class="reference-vertical">Beverage</div>
        </div>
        <div class="reference-headline"><span class="num">#1</span> independent Pepsi bottler in the U.S.</div>
        <div class="reference-detail">DriveMod is deployed at G&amp;J Pepsi's 77,000 sq ft beverage distribution facility, automating high-frequency repetitive transport in a sector where labor turnover and seasonal demand swings hit hardest.</div>
        <div class="reference-quote">"By integrating Cyngn's DriveMod Tugger into our material handling processes, we're addressing today's labor challenges and positioning our business to meet the growing demands of tomorrow."</div>
        <div class="reference-attribution">— Jeff Erwin, VP of Manufacturing &amp; Quality, G&amp;J Pepsi</div>
      </div>

      <div class="reference-card">
        <div class="reference-header">
          <div class="reference-name">Vann Family Orchards</div>
          <div class="reference-vertical">Agriculture</div>
        </div>
        <div class="reference-headline"><span class="num">4</span> Pallys deployed across processing facilities</div>
        <div class="reference-detail">Pally automates raw material transport between storage and processing zones across connected agricultural facilities. Hybrid workflow keeps humans on loading and product handling — where judgment matters most. Deployed via Chandler Automation, Cyngn's systems integration partner.</div>
        <div class="reference-quote">"DriveMod handles material transport between zones. Our team focuses on loading, picking, and quality. Right division of labor."</div>
        <div class="reference-attribution">— Vann Family Orchards deployment, March 2026</div>
      </div>
    </div>
  </div>
</section>

<!-- ============ FAQ ============ -->
<section id="faq" class="section faq-section">
  <div class="container">
    <div class="section-eyebrow">→ Pre-empted objections</div>
    <h2 class="section-title">The questions that come up <span class="accent">on every call.</span></h2>
    <p class="section-sub">Answered upfront, sourced from Cyngn's published documentation. If your question isn't here, the configurator routes it to a real solutions engineer.</p>

    <div class="faq-list">
      <div class="faq-item">
        <div class="faq-q"><span class="faq-q-num">01</span><span>Do I need to change my warehouse infrastructure?</span></div>
        <div class="faq-a">No. <strong>Pally uses 3D LiDAR perception and onboard intelligence</strong> — not magnetic strips, QR markers, beacons, or wire embedment. There's no facility prep, no shutdown window, and no integrator floor work. Pally maps your facility on first deployment and operates from that map thereafter.<span class="source">Source: Cyngn DriveMod Tugger FAQ</span></div>
      </div>

      <div class="faq-item">
        <div class="faq-q"><span class="faq-q-num">02</span><span>What if I need to change a route after Pally is deployed?</span></div>
        <div class="faq-a">Routes are software-defined. <strong>Changing or adding a route is a configuration update</strong>, not a facility re-engineering project. No floor work, no downtime, no integrator return visits. Operations can adjust mission flow as the business changes.</div>
      </div>

      <div class="faq-item">
        <div class="faq-q"><span class="faq-q-num">03</span><span>Will Pally work with my existing carts?</span></div>
        <div class="faq-a">Yes. <strong>Pally tows nearly any cart system already in use</strong>, including standard tugger carts. Quad-steer carts are preferred for narrow aisles because they track behind Pally with much higher fidelity than non-quad-steer carts, but standard carts work as well — capacity calculations adjust accordingly.<span class="source">Source: Cyngn DriveMod Tugger FAQ</span></div>
      </div>

      <div class="faq-item">
        <div class="faq-q"><span class="faq-q-num">04</span><span>What's the minimum aisle width Pally can operate in?</span></div>
        <div class="faq-a"><strong>55 inches minimum</strong> — increasing if cart width exceeds Pally's vehicle width. Pally itself is 30 inches wide; the platform is purpose-built for tight industrial corridors. If your facility has aisles narrower than 55", we'll flag it during the assessment phase before any capital commits.<span class="source">Source: Cyngn DriveMod Tugger FAQ &amp; Motrec MT-160 specifications</span></div>
      </div>

      <div class="faq-item">
        <div class="faq-q"><span class="faq-q-num">05</span><span>What happens if Pally encounters something unexpected?</span></div>
        <div class="faq-a">Pally stops, switches LED indicators to alert color, and triggers configurable audio cues. <strong>If Pally is driven outside the mapped route by a human in manual mode, autonomous operation is disabled until manual return to the drivable path.</strong> Two e-stop buttons allow immediate shutdown at any time. The full safety stack — predictive trajectory tracking via 3D LiDAR, multi-layer perception, redundant e-stops — is designed for facilities where humans and robots share floor space.</div>
      </div>

      <div class="faq-item">
        <div class="faq-q"><span class="faq-q-num">06</span><span>How does Pally integrate with our WMS?</span></div>
        <div class="faq-a">Pally integrates with your warehouse management system via Cyngn Insight, the cloud-based fleet management platform. <strong>Three control surfaces are supported simultaneously:</strong> the on-vehicle HMI (touchscreen on Pally itself), the cloud FMS (web dashboard for ops leadership), and tablet stations placed throughout the facility (elevator-button-style mission dispatch for floor teams). Mission orchestration responds to WMS-triggered events in real time.</div>
      </div>

      <div class="faq-item">
        <div class="faq-q"><span class="faq-q-num">07</span><span>What's the safety record?</span></div>
        <div class="faq-a">Cyngn reports <strong>zero collisions</strong> across deployed Enterprise Autonomy Suite installations. The DriveMod safety architecture relies on patented technology (U.S. Patent No. 12,032,099 for motion compensation in LiDAR perception channels) that improves sensor reliability in dynamic industrial environments — the conditions where most legacy AGV safety systems struggle.<span class="source">Source: Cyngn DriveMod Tugger FAQ &amp; USPTO patent records</span></div>
      </div>
    </div>
  </div>
</section>

<!-- ============ BOTTOM CTA ============ -->
<section class="bottom-cta">
  <div class="container">
    <h2>Free your team for the work that <span class="accent">actually matters.</span></h2>
    <p>The repetitive transport runs are the easiest thing to automate. The judgment work — loading, picking, quality, machining — is where your operators add the most value. Configure your DriveMod pilot in 60 seconds and a solutions engineer will reply within 24 hours with a customer-specific ROI model.</p>
    <div class="bottom-cta-buttons">
      <a href="#configurator" class="btn-primary-large">Configure my pilot →</a>
      <a href="#" class="btn-secondary-large">Talk to a solutions engineer</a>
    </div>
  </div>
</section>

<!-- ============ FOOTER ============ -->
<footer>
  <div class="container footer-inner">
    <div>© 2026 Cyngn Inc. (NASDAQ: CYN) — Mountain View, CA · Pally™ is built on Motrec MT-160 hardware</div>
    <div>
      <a href="#">Privacy</a>
      <a href="#">Terms</a>
      <a href="#">Investors</a>
    </div>
  </div>
</footer>

<div class="design-note" onclick="alert('PALLY v3 — concept homepage by Nizam Ali\n\nNOT AFFILIATED WITH CYNGN INC.\nThis is a portfolio mockup created as an interview demo for the Cyngn (NASDAQ: CYN) Head of Revenue Operations role. Cyngn name, customer references, and product details are drawn from publicly available sources and used illustratively.\n\nStrategic moves:\n• Single-product hero: DriveMod Tugger reframed as Pally\n• Named product (Roomba/Servi/Oura model) — not a mascot\n• Industrial design read: isometric product render, confident sans, photographic-style restraint\n• Embedded configurator captures qualification context before sales\n• Light industrial palette mirrors Caterpillar/Crown/Toyota MH visual code\n• ROI math front and center vs. the labor you cannot hire\n• Sourced claims: BLS, Cyngn FAQ, USPTO patent, named-executive quotes')">
  ⚡ Concept demo — click for notes
</div>

<script>
  // ============ CONFIGURATOR LOGIC ============
  // Same flow as v1, copy rewritten in Pally's voice.

  const STEPS = [
    {
      type: 'select',
      key: 'size',
      question: "How big is your facility?",
      helper: "Square footage of your main operations area.",
      options: [
        { label: 'Under 50,000 sq ft', value: 'small', mult: 0.6 },
        { label: '50,000 – 200,000 sq ft', value: 'medium', mult: 1.0 },
        { label: '200,000 – 500,000 sq ft', value: 'large', mult: 1.6 },
        { label: '500,000+ sq ft (multi-building campus)', value: 'xlarge', mult: 2.4 }
      ]
    },
    {
      type: 'select',
      key: 'fleet',
      question: "How many tuggers are you running today?",
      helper: "Manual and autonomous combined. Pally fits alongside your existing fleet.",
      options: [
        { label: '1 – 5 tuggers', value: '1-5', units: 3 },
        { label: '6 – 15 tuggers', value: '6-15', units: 10 },
        { label: '16 – 50 tuggers', value: '16-50', units: 30 },
        { label: '50+ tuggers', value: '50+', units: 70 },
        { label: "We're new to tuggers — evaluating first deployment", value: 'none', units: 5 }
      ]
    },
    {
      type: 'select',
      key: 'shifts',
      question: "How many shifts per day?",
      helper: "Pally runs all of them. The math just shifts a lot depending on the answer.",
      options: [
        { label: '1 shift', value: '1', mult: 1.0 },
        { label: '2 shifts', value: '2', mult: 1.85 },
        { label: '3 shifts (24/7)', value: '3', mult: 2.6 }
      ]
    },
    {
      type: 'select',
      key: 'pain',
      question: "What's the biggest pain you're solving?",
      helper: "Pick the one that hurts most. We'll tailor the pilot scope to it.",
      options: [
        { label: "Filling jobs you can't hire (labor shortage)", value: 'labor' },
        { label: 'Reducing safety incidents on the floor', value: 'safety' },
        { label: 'Scaling throughput without adding headcount', value: 'throughput' },
        { label: 'Cutting operating cost / margin pressure', value: 'cost' },
        { label: 'Future-proofing the operation', value: 'strategic' }
      ]
    },
    {
      type: 'form',
      key: 'contact',
      question: "Where should we send your ROI model?",
      helper: "A solutions engineer will follow up within 24 hours. No sequences, no spam — one human reply.",
      fields: [
        { name: 'name', placeholder: 'Your name' },
        { name: 'email', placeholder: 'Work email', type: 'email' },
        { name: 'company', placeholder: 'Company name' },
        { name: 'title', placeholder: 'Your title' }
      ]
    }
  ];

  let currentStep = 0;
  const answers = {};

  const stepNumEl = document.getElementById('stepNum');
  const progressFill = document.getElementById('progressFill');
  const configContent = document.getElementById('configContent');

  function updateProgress() {
    const pct = ((currentStep + 1) / (STEPS.length + 1)) * 100;
    progressFill.style.width = pct + '%';
    stepNumEl.textContent = Math.min(currentStep + 1, STEPS.length);
  }

  function renderStep() {
    if (currentStep >= STEPS.length) {
      renderResult();
      return;
    }

    const step = STEPS[currentStep];
    let html = `
      <div class="config-question">${step.question}</div>
      <div class="config-helper">${step.helper}</div>
    `;

    if (step.type === 'select') {
      html += '<div class="config-options">';
      step.options.forEach((opt, i) => {
        html += `
          <button class="config-option" data-step="${currentStep}" data-idx="${i}">
            <span>${opt.label}</span>
            <span class="arrow">→</span>
          </button>
        `;
      });
      html += '</div>';
      html += `
        <div class="config-nav">
          <button class="config-back" ${currentStep === 0 ? 'disabled' : ''}>← Back</button>
          <span style="font-family: var(--mono); font-size: 11px; color: var(--ink-dim); text-transform: uppercase; letter-spacing: 0.1em;">Click to continue →</span>
        </div>
      `;
    } else if (step.type === 'form') {
      html += '<div class="config-input-row">';
      step.fields.forEach(f => {
        html += `<input class="config-input" type="${f.type || 'text'}" name="${f.name}" placeholder="${f.placeholder}" />`;
      });
      html += '</div>';
      html += `
        <div class="config-nav">
          <button class="config-back">← Back</button>
          <button class="config-submit" id="submitBtn">Get my ROI estimate →</button>
        </div>
      `;
    }

    configContent.innerHTML = html;
    updateProgress();

    document.querySelectorAll('.config-option').forEach(btn => {
      btn.addEventListener('click', () => {
        const step = STEPS[currentStep];
        const idx = parseInt(btn.dataset.idx);
        answers[step.key] = step.options[idx];
        currentStep++;
        renderStep();
      });
    });

    const backBtn = document.querySelector('.config-back');
    if (backBtn) {
      backBtn.addEventListener('click', () => {
        if (currentStep > 0) {
          currentStep--;
          renderStep();
        }
      });
    }

    const submitBtn = document.getElementById('submitBtn');
    if (submitBtn) {
      submitBtn.addEventListener('click', () => {
        const inputs = document.querySelectorAll('.config-input');
        const contact = {};
        let valid = true;
        inputs.forEach(input => {
          contact[input.name] = input.value;
          if (!input.value) valid = false;
        });
        if (!valid) {
          alert("Please complete all four fields so we can route your ROI model correctly.");
          return;
        }
        answers.contact = contact;
        currentStep++;
        renderStep();
      });
    }
  }

  function renderResult() {
    const sizeMult = answers.size?.mult || 1.0;
    const units = answers.fleet?.units || 5;
    const shiftsMult = answers.shifts?.mult || 1.0;

    const baseSavings = units * shiftsMult * 35000 * (sizeMult * 0.7 + 0.3);
    const annualSavings = Math.round(baseSavings / 10000) * 10000;

    const paybackMonths = annualSavings > 1500000 ? 11 :
                         annualSavings > 800000 ? 14 :
                         annualSavings > 400000 ? 17 : 22;

    const teamSize = units >= 30 ? '4–6 Pallys' :
                    units >= 10 ? '2–4 Pallys' :
                    units >= 3 ? '2 Pallys' : '1 Pally';

    const formatNum = n => '$' + n.toLocaleString();

    const sizeLabel = answers.size?.label || '';
    const fleetLabel = answers.fleet?.label || '';
    const shiftsLabel = answers.shifts?.label || '';
    const painMap = {
      labor: 'labor shortage',
      safety: 'safety',
      throughput: 'throughput scaling',
      cost: 'cost reduction',
      strategic: 'strategic automation'
    };
    const painLabel = painMap[answers.pain?.value] || 'operations';
    const firstName = (answers.contact?.name || 'there').split(' ')[0];

    configContent.innerHTML = `
      <div class="config-result">
        <div class="result-headline">${firstName}, here's your estimate.</div>
        <div class="result-sub">${sizeLabel.toLowerCase()} · ${fleetLabel.toLowerCase()} · ${shiftsLabel.toLowerCase()} · prioritizing ${painLabel}</div>

        <div class="result-card">
          <div class="result-stat-label">Estimated annual labor savings</div>
          <div class="result-stat-value">${formatNum(annualSavings)}</div>
          <div class="result-stat-detail">Range based on Cyngn customer benchmarks. Detailed model arrives within 24 hours.</div>
        </div>

        <div class="result-row">
          <span class="label">Recommended pilot size</span>
          <span class="value"><strong>${teamSize}</strong></span>
        </div>
        <div class="result-row">
          <span class="label">Estimated payback</span>
          <span class="value"><strong>${paybackMonths} months</strong></span>
        </div>
        <div class="result-row">
          <span class="label">Time to first deployment</span>
          <span class="value"><strong>~90 days</strong></span>
        </div>
        <div class="result-row">
          <span class="label">Hardware platform</span>
          <span class="value">Motrec MT-160</span>
        </div>

        <div class="result-cta-stack">
          <button class="result-cta-primary" onclick="alert('In a live build: this triggers a Salesforce/HubSpot lead create with full configurator context, books a calendar slot via Chili Piper, and triggers a Slack alert to the assigned solutions engineer. Email confirmation sent automatically.')">📅 Schedule a 30-min strategy call</button>
          <button class="result-cta-secondary" onclick="alert('In a live build: this generates a personalized PDF ROI model, gated download, and adds the contact to a 7-day nurture sequence with case studies matching their vertical.')">📊 Email me the detailed ROI model</button>
        </div>
      </div>
    `;

    progressFill.style.width = '100%';
    stepNumEl.textContent = '5';
  }

  renderStep();

  document.querySelectorAll('a[href^="#"]').forEach(link => {
    link.addEventListener('click', e => {
      const target = document.querySelector(link.getAttribute('href'));
      if (target) {
        e.preventDefault();
        target.scrollIntoView({ behavior: 'smooth', block: 'start' });
      }
    });
  });
</script>

</body>
</html>
