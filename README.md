<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Rms_dragon — About Me</title>
  <meta name="description" content="Personal one‑page bio website for Rms (aka Rms_dragon): gamer, music lover, coder, ethical cyberhacker, cybersecurity enthusiast."/>
  <meta name="theme-color" content="#0ea5e9"/>
  <link rel="icon" href="logo.png" /> <!-- Your custom logo -->
  <style>
    :root {
      --bg: #0b1220;
      --panel: #0f172a;
      --text: #e5e7eb;
      --muted: #94a3b8;
      --brand: #0ea5e9;
      --accent: #22d3ee;
      --ring: 0 0 0 3px rgba(14,165,233,.35);
    }
    :root.light {
      --bg: #f8fafc;
      --panel: #ffffff;
      --text: #0f172a;
      --muted: #475569;
      --brand: #0284c7;
      --accent: #0ea5e9;
    }
    * { box-sizing: border-box; }
    html, body { height: 100%; }
    body {
      margin: 0; font-family: system-ui, -apple-system, Segoe UI, Roboto, "Inter", Arial, sans-serif;
      background: radial-gradient(1200px 600px at 80% -100px, rgba(14,165,233,.15), transparent), var(--bg);
      color: var(--text);
    }
    a { color: var(--accent); text-decoration: none; }
    a:hover { text-decoration: underline; }
    .container { max-width: 1000px; margin: 0 auto; padding: 24px; }
    header {
      display: flex; align-items: center; justify-content: space-between; gap: 12px; padding: 12px 0 16px;
    }
    .logo { display: inline-flex; align-items: center; gap: 10px; font-weight: 800; letter-spacing: .5px; }
    .logo img { width: 36px; height: 36px; border-radius: 8px; }
    .theme-toggle { border: 1px solid rgba(148,163,184,.25); background: var(--panel); color: var(--text); padding: 10px 14px; border-radius: 999px; cursor: pointer; backdrop-filter: blur(8px); }
    .theme-toggle:focus { outline: none; box-shadow: var(--ring); }

    .hero {
      display: grid; grid-template-columns: 1.2fr .8fr; gap: 24px; align-items: center; margin-top: 8px;
    }
    .card {
      background: linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,.02));
      border: 1px solid rgba(148,163,184,.15);
      border-radius: 20px; padding: 22px; box-shadow: 0 10px 40px rgba(2,6,23,.35);
    }
    .tag { display:inline-flex; align-items:center; gap:8px; font-size: 12px; color: var(--muted); background: rgba(148,163,184,.08); padding: 6px 10px; border-radius: 999px; border:1px solid rgba(148,163,184,.18); }
    h1 { font-size: clamp(28px, 4vw, 44px); margin: 8px 0 10px; line-height: 1.1; }
    .typing { font-weight: 600; color: var(--accent); border-right: 2px solid var(--accent); padding-right: 4px; animation: caret 1s steps(1) infinite; }
    @keyframes caret { 50% { border-color: transparent; } }
    .sub { color: var(--muted); font-size: 15px; line-height: 1.6; }
    .cta-row { display: flex; gap: 12px; margin-top: 18px; flex-wrap: wrap; }
    .btn { display:inline-flex; align-items:center; gap:10px; border: 1px solid rgba(148,163,184,.25); background: var(--panel); color: var(--text); padding: 12px 16px; border-radius: 14px; cursor: pointer; text-decoration: none; font-weight: 600; }
    .btn.primary { background: linear-gradient(90deg, var(--brand), var(--accent)); border-color: transparent; color: #001018; }
    .btn:hover { transform: translateY(-1px); }

    .avatar {
      width: 100%; aspect-ratio: 1 / 1; border-radius: 18px; object-fit: cover; display:block; background: rgba(148,163,184,.12);
      border: 1px solid rgba(148,163,184,.18);
    }

    .grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; margin-top: 24px; }
    .pill { font-size: 13px; color: var(--muted); background: rgba(148,163,184,.08); border:1px solid rgba(148,163,184,.18); padding: 6px 10px; border-radius: 999px; }

    section { margin-top: 28px; }
    h2 { font-size: 20px; margin: 0 0 10px; letter-spacing: .3px; }
    ul { padding-left: 18px; }

    footer { margin: 40px 0 10px; color: var(--muted); font-size: 13px; text-align: center; }

    @media (max-width: 900px) {
      .hero { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo" aria-label="Site logo">
        <img src="logo.png" alt="Site Logo" />
        <span>Rms_dragon</span>
      </div>
      <button class="theme-toggle" id="themeBtn" title="Toggle light/dark">Toggle Theme</button>
    </header>

    <main class="hero">
      <div class="card">
        <span class="tag">👋 Hello! I'm</span>
        <h1>Rms <span class="typing" id="typing"></span></h1>
        <p class="sub">
          Gamer • Music lover • Coder • Ethical <b>cyberhacker</b> • <b>Cybersecurity</b> enthusiast from Bangladesh. My dream is to become a <b>computer engineer</b> and someday build cool things at <b>Microsoft</b> or <b>Google</b>.
        </p>
        <div class="cta-row">
          <a class="btn primary" href="#contact">Contact Me</a>
          <button class="btn" id="copyEmail">Copy Email</button>
          <a class="btn" href="#projects">Projects</a>
        </div>
        <section>
          <h2>About me</h2>
          <p class="sub">I love building web things, breaking stuff <i>the safe way</i>, and helping people stay secure online. When I'm not coding, you'll probably find me testing games on mobile or tweaking my own code studio UI.</p>
        </section>
        <section>
          <h2>Skills</h2>
          <div class="grid">
            <span class="pill">HTML • CSS • JS</span>
            <span class="pill">Responsive UI</span>
            <span class="pill">Cybersecurity Basics</span>
            <span class="pill">Ethical Hacking</span>
            <span class="pill">Minecraft: PE</span>
            <span class="pill">Roblox (HD Admin)</span>
          </div>
        </section>
        <section id="projects">
          <h2>Projects</h2>
          <ul>
            <li>Dragon Code Studio — a VS Code‑inspired online code editor UI.</li>
            <li>Animated Fanta drink website — playful UI with sounds and motion.</li>
            <li>Cyber-safety mini site — explains safe vs admin‑level malware risks.</li>
          </ul>
        </section>
        <section id="contact">
          <h2>Contact</h2>
          <p class="sub">Email: <a href="mailto:jabirai4779@gmail.com" id="email">jabirai4779@gmail.com</a> • Facebook: <a href="#" target="_blank" rel="noreferrer">Rms Rms</a></p>
        </section>
      </div>

      <div>
        <img class="avatar" src="IMG_20250622_160938.jpg" alt="Your avatar or logo" />
        <section class="card" style="margin-top:16px">
          <h2>Quick Facts</h2>
          <ul>
            <li>Timezone: Asia/Dhaka (UTC+6)</li>
            <li>Goal: Become a Computer Engineer</li>
            <li>Dream: Work at Microsoft or Google</li>
          </ul>
        </section>
        <section class="card" style="margin-top:16px">
          <h2>Visit my media</h2>
          <div class="grid">
            <a class="pill" href="#" target="_blank" rel="noreferrer">Facebook:Rms Rms</a>
            <a class="pill" href="#" target="_blank" rel="noreferrer">Discord:rms_dragon</a>
          </div>
        </section>
      </div>
    </main>

    <footer>
      © <span id="year"></span> Rms (aka Rms_dragon). Built with vanilla HTML/CSS/JS.
    </footer>
  </div>

  <script>
    // ---- Theme toggle ----
    const root = document.documentElement;
    const themeBtn = document.getElementById('themeBtn');
    const savedTheme = localStorage.getItem('theme');
    if (savedTheme === 'light') root.classList.add('light');
    themeBtn.addEventListener('click', () => {
      root.classList.toggle('light');
      localStorage.setItem('theme', root.classList.contains('light') ? 'light' : 'dark');
    });

    // ---- Typing effect ----
    const roles = ['Music Lover','Coder','Cyberhacker','Cybersecurity'];
    const typingEl = document.getElementById('typing');
    let idx = 0, ch = 0, back = false;
    function type() {
      const word = roles[idx % roles.length];
      typingEl.textContent = back ? word.slice(0, ch--) : word.slice(0, ch++);
      if (!back && ch > word.length + 6) back = true;
      if (back && ch < 0) { back = false; idx++; }
      setTimeout(type, back ? 60 : 90);
    }
    type();

    // ---- Copy email ----
    const email = document.getElementById('email');
    document.getElementById('copyEmail').addEventListener('click', async () => {
      try {
        await navigator.clipboard.writeText(email.textContent);
        const btn = event.currentTarget; const old = btn.textContent;
        btn.textContent = 'Copied!';
        btn.style.boxShadow = 'var(--ring)';
        setTimeout(() => { btn.textContent = old; btn.style.boxShadow = 'none'; }, 1200);
      } catch (e) { alert('Copy failed'); }
    });

    // ---- Year ----
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
