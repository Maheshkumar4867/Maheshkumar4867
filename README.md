
<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap');

*{box-sizing:border-box;margin:0;padding:0}
body{background:#0d1117;color:#e6edf3;font-family:'Inter',sans-serif;-webkit-font-smoothing:antialiased}

.page{max-width:860px;margin:0 auto;padding:0 0 60px}

/* HERO */
.hero{padding:48px 40px 40px;border-bottom:1px solid #21262d;position:relative;overflow:hidden}
.hero-bg{position:absolute;top:-60px;right:-60px;width:300px;height:300px;border-radius:50%;background:radial-gradient(circle,rgba(29,158,117,.08) 0%,transparent 70%);pointer-events:none}
.hero-bg2{position:absolute;bottom:-40px;left:20%;width:200px;height:200px;border-radius:50%;background:radial-gradient(circle,rgba(88,166,255,.05) 0%,transparent 70%);pointer-events:none}
.hero-top{display:flex;align-items:flex-start;justify-content:space-between;margin-bottom:20px}
.hero-left{}
.hero-eyebrow{display:flex;align-items:center;gap:8px;font-family:'JetBrains Mono',monospace;font-size:11px;color:#7d8590;letter-spacing:.5px;margin-bottom:14px}
.hero-eyebrow-dot{width:6px;height:6px;border-radius:50%;background:#1D9E75;animation:pulse 2.5s ease-in-out infinite}
@keyframes pulse{0%,100%{box-shadow:0 0 0 0 rgba(29,158,117,.4)}50%{box-shadow:0 0 0 6px rgba(29,158,117,0)}}
.hero-name{font-size:46px;font-weight:700;letter-spacing:-2px;line-height:1;color:#f0f6fc;margin-bottom:10px}
.hero-name span{color:#1D9E75}
.hero-title{font-size:14px;color:#7d8590;font-weight:400;line-height:1.6;max-width:440px}
.hero-avatar{width:72px;height:72px;border-radius:16px;background:linear-gradient(135deg,#1D9E75,#0d5c42);display:flex;align-items:center;justify-content:center;font-size:22px;font-weight:700;color:#fff;letter-spacing:-1px;flex-shrink:0;border:1px solid rgba(29,158,117,.3)}
.hero-links{display:flex;gap:8px;flex-wrap:wrap;margin-top:24px}
.hl{display:inline-flex;align-items:center;gap:6px;font-size:12px;font-weight:500;padding:6px 14px;border-radius:8px;text-decoration:none;border:1px solid #30363d;color:#8b949e;background:#161b22;transition:border-color .15s,color .15s}
.hl:hover{border-color:#1D9E75;color:#1D9E75}
.hl svg{opacity:.7}
.avail-chip{display:inline-flex;align-items:center;gap:6px;font-size:11px;font-weight:500;font-family:'JetBrains Mono',monospace;padding:5px 12px;border-radius:20px;border:1px solid rgba(29,158,117,.3);color:#3fb950;background:rgba(29,158,117,.07);letter-spacing:.3px}

/* SECTION */
.section{padding:32px 40px;border-bottom:1px solid #21262d}
.sec-head{display:flex;align-items:center;gap:10px;margin-bottom:24px}
.sec-num{font-family:'JetBrains Mono',monospace;font-size:10px;color:#484f58;letter-spacing:1px}
.sec-title{font-size:13px;font-weight:600;color:#f0f6fc;letter-spacing:.5px;text-transform:uppercase}
.sec-line{flex:1;height:1px;background:#21262d}

/* ABOUT */
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:6px}
.about-row{display:flex;align-items:flex-start;gap:10px;padding:10px 12px;border-radius:8px;background:#161b22;border:1px solid #21262d;font-size:13px;color:#8b949e;line-height:1.5;transition:border-color .15s}
.about-row:hover{border-color:#30363d}
.about-icon{width:26px;height:26px;border-radius:6px;display:flex;align-items:center;justify-content:center;flex-shrink:0;font-size:13px}

/* EXPERTISE */
.exp-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:10px}
.exp-card{padding:18px;border-radius:12px;border:1px solid #21262d;background:#161b22;transition:border-color .15s}
.exp-card:hover{border-color:#30363d}
.exp-card-icon{width:36px;height:36px;border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:16px;margin-bottom:12px}
.exp-card-title{font-size:13px;font-weight:600;color:#f0f6fc;margin-bottom:10px}
.exp-tags{display:flex;flex-wrap:wrap;gap:4px}
.etag{font-family:'JetBrains Mono',monospace;font-size:10px;padding:2px 8px;border-radius:4px;color:#8b949e;background:#0d1117;border:1px solid #30363d}

/* STACK */
.stack-group{margin-bottom:20px}
.stack-label{font-family:'JetBrains Mono',monospace;font-size:10px;letter-spacing:2px;color:#484f58;text-transform:uppercase;margin-bottom:10px}
.stack-row{display:flex;flex-wrap:wrap;gap:6px}
.spill{display:inline-flex;align-items:center;gap:6px;padding:6px 12px;border-radius:8px;border:1px solid #30363d;background:#161b22;font-size:12px;font-weight:500;color:#8b949e;transition:border-color .15s,color .15s}
.spill:hover{border-color:#1D9E75;color:#e6edf3}
.spill.core{border-color:rgba(29,158,117,.4);color:#3fb950;background:rgba(29,158,117,.06)}
.spill svg{flex-shrink:0}

/* EXPERIENCE */
.tl{position:relative;padding-left:20px}
.tl::before{content:'';position:absolute;left:5px;top:10px;bottom:10px;width:1px;background:#21262d}
.tl-item{position:relative;margin-bottom:8px}
.tl-item+.tl-item{margin-top:8px}
.tl-dot{position:absolute;left:-17px;top:20px;width:11px;height:11px;border-radius:50%;background:#0d1117;border:2px solid #30363d}
.tl-dot.active{background:#1D9E75;border-color:#1D9E75;box-shadow:0 0 0 3px rgba(29,158,117,.2)}
.job-card{border:1px solid #21262d;border-radius:12px;padding:20px;background:#161b22;transition:border-color .2s}
.job-card:hover{border-color:#30363d}
.job-top{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:4px}
.job-title{font-size:15px;font-weight:600;color:#f0f6fc}
.job-badge{font-family:'JetBrains Mono',monospace;font-size:10px;padding:3px 10px;border-radius:20px;background:#161b22;border:1px solid #30363d;color:#7d8590;white-space:nowrap}
.job-badge.current{border-color:rgba(29,158,117,.4);color:#3fb950;background:rgba(29,158,117,.07)}
.job-company{display:inline-flex;align-items:center;gap:5px;font-family:'JetBrains Mono',monospace;font-size:11px;color:#484f58;margin-bottom:10px}
.job-company-bullet{width:4px;height:4px;border-radius:50%;background:#1D9E75}
.job-desc{font-size:13px;color:#7d8590;line-height:1.75;margin-bottom:14px}
.ach-grid{display:grid;grid-template-columns:1fr 1fr;gap:5px}
.ach{display:flex;gap:8px;align-items:flex-start;font-size:12px;color:#7d8590;line-height:1.6;padding:8px 10px;background:#0d1117;border-radius:7px;border:1px solid #21262d}
.ach-bullet{width:4px;height:4px;border-radius:50%;background:#1D9E75;flex-shrink:0;margin-top:6px}

/* STATS */
.stats-row{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:8px;margin-bottom:20px}
.stat-box{background:#161b22;border:1px solid #21262d;border-radius:10px;padding:16px;text-align:center}
.stat-num{font-size:26px;font-weight:700;color:#f0f6fc;line-height:1;letter-spacing:-1px}
.stat-label{font-family:'JetBrains Mono',monospace;font-size:9px;color:#484f58;letter-spacing:1px;text-transform:uppercase;margin-top:4px}
.gh-img{width:100%;border-radius:10px;display:block;border:1px solid #21262d}
.gh-imgs{display:flex;flex-direction:column;gap:8px}

/* CONTACT */
.contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px}
.contact-card{display:flex;align-items:center;gap:12px;padding:14px 16px;border-radius:10px;border:1px solid #21262d;background:#161b22;text-decoration:none;transition:border-color .15s}
.contact-card:hover{border-color:#1D9E75}
.contact-icon{width:34px;height:34px;border-radius:8px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.contact-label{font-family:'JetBrains Mono',monospace;font-size:10px;color:#484f58;letter-spacing:1px;text-transform:uppercase;margin-bottom:3px}
.contact-val{font-size:13px;font-weight:500;color:#8b949e}
.contact-card:hover .contact-val{color:#e6edf3}

/* FOOTER */
.footer{padding:28px 40px;text-align:center;font-family:'JetBrains Mono',monospace;font-size:11px;color:#484f58;letter-spacing:.5px}
.footer-bar{height:3px;background:linear-gradient(90deg,transparent,#1D9E75,transparent);margin-bottom:24px;border-radius:2px}
</style>

<div class="page">

<!-- HERO -->
<div class="hero">
  <div class="hero-bg"></div>
  <div class="hero-bg2"></div>
  <div class="hero-top">
    <div class="hero-left">
      <div class="hero-eyebrow">
        <div class="hero-eyebrow-dot"></div>
        Full Stack Developer &nbsp;·&nbsp; Bangalore, India
      </div>
      <div class="hero-name">Mahesh <span>Kumar</span></div>
      <div class="hero-title">OTT & Video Streaming Specialist &nbsp;·&nbsp; Smart TV Engineer &nbsp;·&nbsp; 3+ Years</div>
    </div>
    <div class="hero-avatar">MK</div>
  </div>
  <div class="hero-links">
    <a class="hl" href="https://www.linkedin.com/in/maheshkumardev/" target="_blank">
      <svg width="13" height="13" viewBox="0 0 24 24" fill="#0A66C2"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
      LinkedIn
    </a>
    <a class="hl" href="mailto:k.maheshkumar8522@gmail.com">
      <svg width="13" height="13" viewBox="0 0 24 24" fill="#EA4335"><path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></svg>
      Email
    </a>
    <a class="hl" href="https://maheshkumardev.com" target="_blank">
      <svg width="13" height="13" viewBox="0 0 24 24" fill="#1D9E75"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"/></svg>
      Portfolio
    </a>
    <a class="hl" href="https://github.com/Maheshkumar4867" target="_blank">
      <svg width="13" height="13" viewBox="0 0 24 24" fill="#f0f6fc"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg>
      GitHub
    </a>
    <div class="avail-chip">
      <svg width="8" height="8" viewBox="0 0 8 8"><circle cx="4" cy="4" r="4" fill="#3fb950"/></svg>
      Open to opportunities
    </div>
  </div>
</div>

<!-- ABOUT -->
<div class="section">
  <div class="sec-head"><span class="sec-num">01</span><span class="sec-title">About</span><div class="sec-line"></div></div>
  <div class="about-grid">
    <div class="about-row"><div class="about-icon" style="background:rgba(29,158,117,.1)">🎬</div><span><strong style="color:#e6edf3">3+ years</strong> building OTT & video streaming apps</span></div>
    <div class="about-row"><div class="about-icon" style="background:rgba(88,166,255,.1)">📺</div><span>Smart TV dev — Samsung Tizen & LG WebOS</span></div>
    <div class="about-row"><div class="about-icon" style="background:rgba(255,166,77,.1)">⚡</div><span>HLS/DASH adaptive streaming & DRM</span></div>
    <div class="about-row"><div class="about-icon" style="background:rgba(29,158,117,.1)">⚛️</div><span>React · TypeScript · Node.js · Redux Toolkit</span></div>
    <div class="about-row"><div class="about-icon" style="background:rgba(255,120,120,.1)">🚀</div><span>Focused on performance, scalability & UX</span></div>
    <div class="about-row"><div class="about-icon" style="background:rgba(150,150,150,.1)">📍</div><span>Bangalore, Karnataka, India</span></div>
  </div>
</div>

<!-- EXPERTISE -->
<div class="section">
  <div class="sec-head"><span class="sec-num">02</span><span class="sec-title">Core Expertise</span><div class="sec-line"></div></div>
  <div class="exp-grid">
    <div class="exp-card">
      <div class="exp-card-icon" style="background:rgba(29,158,117,.12)">🎥</div>
      <div class="exp-card-title">OTT & Streaming</div>
      <div class="exp-tags"><span class="etag">HLS/DASH</span><span class="etag">DRM</span><span class="etag">HLS.js</span><span class="etag">Dash.js</span><span class="etag">Google IMA</span><span class="etag">FFmpeg</span><span class="etag">Seekbar</span></div>
    </div>
    <div class="exp-card">
      <div class="exp-card-icon" style="background:rgba(88,166,255,.12)">⚛️</div>
      <div class="exp-card-title">Frontend Engineering</div>
      <div class="exp-tags"><span class="etag">React.js</span><span class="etag">TypeScript</span><span class="etag">Next.js</span><span class="etag">Redux</span><span class="etag">TailwindCSS</span><span class="etag">Vite</span><span class="etag">Webpack</span></div>
    </div>
    <div class="exp-card">
      <div class="exp-card-icon" style="background:rgba(188,103,255,.12)">📺</div>
      <div class="exp-card-title">Smart TV Platforms</div>
      <div class="exp-tags"><span class="etag">Samsung Tizen</span><span class="etag">LG WebOS</span><span class="etag">Remote Nav</span><span class="etag">EPG</span><span class="etag">TV SDKs</span></div>
    </div>
  </div>
</div>

<!-- STACK -->
<div class="section">
  <div class="sec-head"><span class="sec-num">03</span><span class="sec-title">Tech Stack</span><div class="sec-line"></div></div>

  <div class="stack-group">
    <div class="stack-label">Core</div>
    <div class="stack-row">
      <span class="spill core"><svg width="14" height="14" viewBox="0 0 24 24" fill="#61DAFB"><circle cx="12" cy="12" r="2.139"/><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 3c.89 0 1.74.13 2.55.37-1.56 1.08-2.55 2.88-2.55 4.88S12.99 13.55 14.55 14.63c-.81.24-1.66.37-2.55.37-3.86 0-7-3.14-7-7s3.14-7 7-7z" opacity="0"/></svg>React.js</span>
      <span class="spill core"><svg width="14" height="14" viewBox="0 0 24 24" fill="#3178C6"><path d="M1.125 0C.502 0 0 .502 0 1.125v21.75C0 23.498.502 24 1.125 24h21.75c.623 0 1.125-.502 1.125-1.125V1.125C24 .502 23.498 0 22.875 0zm17.363 9.75c.612 0 1.154.037 1.627.111v2.458a3.95 3.95 0 00-1.36-.601 5.453 5.453 0 00-1.426-.2c-.3 0-.573.028-.819.086a2.1 2.1 0 00-.623.242.888.888 0 00-.14.49c0 .373.332.693.996.96l.926.416c.94.395 1.61.865 2.009 1.41.4.545.599 1.188.599 1.927 0 1.18-.43 2.082-1.291 2.705-.86.624-2.047.935-3.56.935-1.275 0-2.547-.26-3.818-.779v-2.5c.977.544 2.018.815 3.12.815.594 0 1.055-.112 1.382-.337.327-.225.49-.527.49-.906 0-.435-.351-.804-1.053-1.107l-.96-.41c-.828-.352-1.44-.778-1.836-1.279a2.95 2.95 0 01-.594-1.842c0-1.078.394-1.921 1.181-2.53.788-.61 1.843-.914 3.165-.914zm-8.99.151h3.276L7.5 24H4.224z"/></svg>TypeScript</span>
      <span class="spill core"><svg width="14" height="14" viewBox="0 0 24 24"><rect width="24" height="24" rx="3" fill="#F7DF1E"/><path d="M6.3 20.573l1.855-1.124c.357.633.683 1.169 1.464 1.169.749 0 1.222-.292 1.222-1.43V12.62h2.283v6.6c0 2.356-1.381 3.429-3.398 3.429-1.821 0-2.878-.942-3.426-2.076zm8.262-.456l1.855-1.095c.49.798 1.124 1.384 2.248 1.384 1.946 0 2.021-.491 2.021-1.095V6.558h2.283v12.81c0 2.907-1.673 4.225-4.113 4.225-2.203 0-3.477-1.17-4.294-2.476z" fill="#000"/></svg>JavaScript</span>
      <span class="spill core"><svg width="14" height="14" viewBox="0 0 24 24" fill="#339933"><path d="M11.998 24c-.321 0-.641-.084-.924-.251l-2.937-1.737c-.439-.245-.225-.332-.08-.383.585-.203.703-.25 1.328-.604.065-.037.151-.023.219.015l2.256 1.339c.082.045.198.045.275 0l8.795-5.076c.082-.047.134-.141.134-.238V6.921c0-.099-.053-.19-.137-.242l-8.791-5.072a.276.276 0 00-.277 0L3.063 6.68c-.085.05-.139.145-.139.243v10.147c0 .097.054.19.137.235l2.409 1.392c1.307.654 2.108-.116 2.108-.89V7.359c0-.142.114-.253.255-.253h1.115c.139 0 .255.112.255.253v10.447c0 1.745-.95 2.745-2.604 2.745-.508 0-.909 0-2.026-.551l-2.307-1.328A1.851 1.851 0 010 17.068V6.921a1.849 1.849 0 01.924-1.6l8.79-5.08a1.924 1.924 0 011.852 0l8.79 5.08a1.85 1.85 0 01.924 1.6v10.147a1.852 1.852 0 01-.924 1.601l-8.79 5.078a1.858 1.858 0 01-.57.253z"/></svg>Node.js</span>
      <span class="spill core">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="#1D9E75"><path d="M4 8h16v2H4zm0 4h16v2H4zm0 4h8v2H4z"/></svg>HLS / DASH</span>
      <span class="spill core">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="#CC0000"><path d="M12 1L3 5v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V5l-9-4z"/></svg>DRM</span>
    </div>
  </div>

  <div class="stack-group">
    <div class="stack-label">Frontend</div>
    <div class="stack-row">
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#fff"><path d="M11.572 0c-.176 0-.31.001-.358.007a19.76 19.76 0 01-.364.033C7.443.346 4.25 2.185 2.228 5.012a11.875 11.875 0 00-2.119 5.243c-.096.659-.108.854-.108 1.747s.012 1.089.108 1.748c.652 4.506 3.86 8.292 8.209 9.695.779.25 1.6.422 2.534.525.363.04 1.935.04 2.299 0 1.611-.178 2.977-.577 4.323-1.264.207-.106.247-.134.219-.158-.02-.013-.9-1.193-1.955-2.62l-1.919-2.592-2.404-3.558a338.739 338.739 0 00-2.422-3.556c-.009-.002-.018 1.579-.023 3.51-.007 3.38-.01 3.515-.052 3.595a.426.426 0 01-.206.214c-.075.037-.14.044-.495.044H7.81l-.108-.068a.438.438 0 01-.157-.171l-.05-.106.006-4.703.007-4.705.072-.092a.645.645 0 01.174-.143c.096-.047.134-.052.54-.052.479 0 .558.019.683.156.035.038 1.337 1.999 2.895 4.361a10760.433 10760.433 0 004.735 7.17l1.9 2.879.096-.063a12.317 12.317 0 002.466-2.163 11.944 11.944 0 002.824-6.134c.096-.66.108-.854.108-1.748 0-.893-.012-1.088-.108-1.747-.652-4.506-3.859-8.292-8.208-9.695a12.597 12.597 0 00-2.499-.523A33.119 33.119 0 0011.573 0z"/></svg>Next.js</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#764ABC"><path d="M16.634 16.504c.87-.075 1.543-.84 1.499-1.754-.046-.914-.796-1.648-1.709-1.648h-.06c-.943.03-1.679.793-1.648 1.709.03.479.226.869.494 1.153-1.048 2.038-2.621 3.536-5.005 4.795-1.603.838-3.296 1.154-4.944.93-1.378-.195-2.456-.81-3.116-1.798-.988-1.499-1.078-3.116-.255-4.734.6-1.169 1.499-2.023 2.099-2.443-.15-.389-.27-.943-.315-1.378-4.509 3.206-4.045 7.532-2.682 9.569 1.018 1.499 3.101 2.442 5.394 2.442.618 0 1.244-.075 1.86-.224 3.987-.784 7.009-3.146 8.388-6.619zm5.634-4.045c-2.367-2.756-5.843-4.275-9.839-4.275h-.51c-.27-.554-.868-.898-1.498-.898h-.045c-.943 0-1.678.769-1.648 1.708.03.915.796 1.648 1.709 1.648h.06c.674-.03 1.244-.435 1.529-.988h.558c2.367 0 4.61.674 6.648 2.008 1.559 1.004 2.682 2.308 3.326 3.896.538 1.288.509 2.547-.045 3.597-.855 1.589-2.279 2.443-4.168 2.443-1.214 0-2.382-.375-2.995-.749-.345.284-.99.749-1.439.989 1.318.629 2.652.943 3.94.943 2.937 0 5.125-1.618 5.964-3.236.898-1.769.838-4.824-1.547-7.086z"/></svg>Redux Toolkit</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#06B6D4"><path d="M12.001 4.8c-3.2 0-5.2 1.6-6 4.8 1.2-1.6 2.6-2.2 4.2-1.8.913.228 1.565.89 2.288 1.624C13.666 10.618 15.027 12 18.001 12c3.2 0 5.2-1.6 6-4.8-1.2 1.6-2.6 2.2-4.2 1.8-.913-.228-1.565-.89-2.288-1.624C16.337 6.182 14.976 4.8 12.001 4.8zm-6 7.2c-3.2 0-5.2 1.6-6 4.8 1.2-1.6 2.6-2.2 4.2-1.8.913.228 1.565.89 2.288 1.624 1.177 1.194 2.538 2.576 5.512 2.576 3.2 0 5.2-1.6 6-4.8-1.2 1.6-2.6 2.2-4.2 1.8-.913-.228-1.565-.89-2.288-1.624C10.337 13.382 8.976 12 6.001 12z"/></svg>TailwindCSS</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#646CFF"><path d="M12 0C5.52 0 0 5.52 0 12s5.52 12 12 12 12-5.52 12-12S18.48 0 12 0zm.5 3.5l7 13h-3l-4-7.5-4 7.5H5.5l7-13z"/></svg>Vite</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#FF4154"><circle cx="12" cy="12" r="10"/></svg>React Query</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#CA4245"><path d="M12.118 5.466L4.18 9.755v8.57l2.008-1.154V11.1l5.929-3.406 5.93 3.406v6.075l2.005 1.152V9.755z"/></svg>React Router</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#8b949e"><circle cx="12" cy="12" r="11" fill="none" stroke="#8b949e" stroke-width="2"/><circle cx="12" cy="12" r="4" fill="#8b949e"/></svg>Socket.io</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#8DD6F9"><path d="M.395 0H23.61c.217 0 .395.177.395.395v23.21a.395.395 0 01-.395.395H.395A.395.395 0 010 23.605V.395C0 .177.177 0 .395 0zm11.27 13.74l-5.948-6.553H2.44l9.226 10.148 9.226-10.148h-3.278l-5.948 6.553z"/></svg>Webpack</span>
    </div>
  </div>

  <div class="stack-group">
    <div class="stack-label">Backend & Data</div>
    <div class="stack-row">
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#8b949e"><path d="M24 18.588a1.529 1.529 0 01-1.895-.72l-3.45-4.771-.5-.667-4.003 5.444a1.466 1.466 0 01-1.802.708l5.158-6.92-4.798-6.251a1.595 1.595 0 011.9.666l3.576 4.83 3.596-4.81a1.435 1.435 0 011.788-.668L21.708 7.9l-2.522 3.283a.666.666 0 000 .994l4.804 6.412zM.002 11.576l.42-2.205 9.875-9.875a1.153 1.153 0 011.75.15l7.08 9.773-1.08 1.447-6.43-8.93-.59 3.97C5.38 5.07 4.78 4.18 3.83 4.18L2.62 4.18C1.14 4.18 0 5.32 0 6.8v14.4l4.07-2.25-.46-.644C2.97 17.57 2.14 16.51 2.14 16.51L.002 11.576z"/></svg>Express.js</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#4DB33D"><path d="M17.193 9.555c-1.264-5.58-4.252-7.507-4.573-8.227-.36-.635-.42-.862-.438-1.328a3.83 3.83 0 01.078-.581 4.05 4.05 0 01-.075.527c-.547 3.874-2.548 4.276-3.674 6.045-1.17 1.85-1.261 3.47-.94 4.597-.212-.114-.41-.239-.574-.396-.526-.518-.773-1.319-.773-2.18 0-1.18.342-2.293 1.09-3.29-1.055 1.072-1.84 2.46-1.84 4.102 0 1.29.342 2.478 1.09 3.492.77 1.03 1.953 1.729 3.317 1.86-.04.02-.079.04-.116.063-1.073.65-1.558 1.92-1.558 3.01 0 .844.334 1.617.931 2.172.583.543 1.386.843 2.255.843.87 0 1.67-.3 2.254-.843.596-.555.93-1.328.93-2.172 0-1.09-.485-2.36-1.556-3.01a2.8 2.8 0 00-.116-.063c1.364-.131 2.547-.83 3.317-1.86.748-1.014 1.09-2.202 1.09-3.492 0-1.642-.785-3.03-1.84-4.102.748.997 1.09 2.11 1.09 3.29 0 .861-.247 1.662-.773 2.18-.164.157-.362.282-.574.396.32-1.127.23-2.747-.94-4.597z" fill="#4DB33D"/></svg>MongoDB</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#003B57"><path d="M21.678.521C20.467-.174 18.895.004 17.53.906L12 4.585 6.47.906C5.104.004 3.533-.174 2.322.521.9 1.338 0 2.89 0 4.646v14.708c0 1.756.9 3.308 2.322 4.125C2.977 23.826 3.668 24 4.362 24c.69 0 1.38-.174 2.023-.52L12 19.955l5.615 3.525c.643.346 1.334.52 2.023.52.694 0 1.385-.174 2.04-.52C23.1 22.662 24 21.11 24 19.354V4.646C24 2.89 23.1 1.338 21.678.521z" fill="#003B57"/></svg>SQLite</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#009639"><path d="M12 0L1.605 6v12L12 24l10.395-6V6L12 0zm6 16.59c0 .705-.646 1.29-1.529 1.29-.631 0-1.351-.255-1.801-.78l-5.209-6.225v5.966c0 .735-.57 1.29-1.346 1.29H7.88c-.721 0-1.346-.6-1.346-1.29V7.41c0-.705.645-1.29 1.529-1.29.646 0 1.351.255 1.801.78l5.209 6.225V7.155c0-.735.57-1.29 1.346-1.29h.255c.72 0 1.346.6 1.346 1.29V16.59z"/></svg>Nginx</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 16 16" fill="#5cb85c"><path d="M8 0a8 8 0 100 16A8 8 0 008 0zm3.5 5.5l-5 5-2-2 1-1 1 1 4-4 1 1z"/></svg>FFmpeg</span>
    </div>
  </div>

  <div class="stack-group">
    <div class="stack-label">Smart TV & Media SDKs</div>
    <div class="stack-row">
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#1428A0"><rect width="24" height="24" rx="4" fill="#1428A0"/><text x="4" y="17" font-size="11" fill="#fff" font-family="Arial" font-weight="bold">S</text></svg>Samsung Tizen</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24"><rect width="24" height="24" rx="4" fill="#A50034"/><text x="4" y="17" font-size="11" fill="#fff" font-family="Arial" font-weight="bold">L</text></svg>LG WebOS</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#CC0000"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 14H8V8h2v8zm4 0h-2V8h2v8z"/></svg>HLS.js / Dash.js</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#FF0000"><path d="M23.495 6.205a3.007 3.007 0 00-2.088-2.088c-1.87-.501-9.396-.501-9.396-.501s-7.507-.01-9.396.501A3.007 3.007 0 00.527 6.205a31.247 31.247 0 00-.522 5.805 31.247 31.247 0 00.522 5.783 3.007 3.007 0 002.088 2.088c1.868.502 9.396.502 9.396.502s7.506 0 9.396-.502a3.007 3.007 0 002.088-2.088 31.247 31.247 0 00.5-5.783 31.247 31.247 0 00-.5-5.805zM9.609 15.601V8.408l6.264 3.602z"/></svg>Google IMA SDK</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#4285F4"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-6h2v6zm0-8h-2V7h2v2z"/></svg>Norigin Spatial Nav</span>
    </div>
  </div>

  <div class="stack-group">
    <div class="stack-label">Tooling</div>
    <div class="stack-row">
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#F05032"><path d="M23.546 10.93L13.067.452a1.55 1.55 0 00-2.188 0L8.708 2.627l2.76 2.76a1.838 1.838 0 012.327 2.341l2.658 2.66a1.838 1.838 0 012.09 2.82 1.842 1.842 0 01-2.256-.294 1.837 1.837 0 01-.404-2.002L13.26 8.5v6.627a1.833 1.833 0 01.483 3.582 1.84 1.84 0 01-2.264-1.794 1.837 1.837 0 01.96-1.614V8.355a1.832 1.832 0 01-.96-1.616 1.84 1.84 0 012.264-1.793L11.07 2.285 1.454 11.902a1.55 1.55 0 000 2.188l10.48 10.479a1.55 1.55 0 002.186 0l10.426-10.427a1.55 1.55 0 000-2.212"/></svg>Git</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#F69220"><path d="M12 1.27a11 11 0 100 21.46A11 11 0 0012 1.27zm0 1.5a9.5 9.5 0 110 19 9.5 9.5 0 010-19z"/></svg>PNPM</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#2C8EBB"><path d="M12 0C5.375 0 0 5.375 0 12s5.375 12 12 12 12-5.375 12-12S18.625 0 12 0zm.703 16.852l-3.584-3.585 3.584-3.583 3.583 3.583-3.583 3.585z"/></svg>Yarn</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#CB3837"><path d="M0 0v24h24V0H0zm13 19.5H6v-15h7v3.5H9.5V16H13v3.5zm5.5 0h-4V4.5h4v15z"/></svg>NPM</span>
      <span class="spill"><svg width="14" height="14" viewBox="0 0 24 24" fill="#BBDEAD"><path d="M12 0C5.373 0 0 5.373 0 12s5.373 12 12 12 12-5.373 12-12S18.627 0 12 0zm1 16h-2v-4h2v4zm0-6h-2V8h2v2z"/></svg>Nodemon</span>
    </div>
  </div>
</div>

<!-- EXPERIENCE -->
<div class="section">
  <div class="sec-head"><span class="sec-num">04</span><span class="sec-title">Experience</span><div class="sec-line"></div></div>
  <div class="tl">
    <div class="tl-item">
      <div class="tl-dot active"></div>
      <div class="job-card">
        <div class="job-top"><div class="job-title">Software Engineer</div><div class="job-badge current">Oct 2023 – Present</div></div>
        <div class="job-company"><div class="job-company-bullet"></div>Saranyu Technologies</div>
        <div class="job-desc">Building and optimizing Smart TV OTT applications for Samsung Tizen and LG WebOS using React.js, Redux Toolkit, and custom video player SDKs — focused on advanced playback, monetization, and performance across 50+ TV models.</div>
        <div class="ach-grid">
          <div class="ach"><div class="ach-bullet"></div>Custom HLS/DASH thumbnail seekbar for video preview during seek</div>
          <div class="ach"><div class="ach-bullet"></div>Google IMA SDK — pre/mid/post-roll ad monetization integration</div>
          <div class="ach"><div class="ach-bullet"></div>Adaptive streaming (HLS.js, Dash.js) with multi-audio & subtitle UI</div>
          <div class="ach"><div class="ach-bullet"></div>TV remote navigation via Norigin Spatial Navigation</div>
          <div class="ach"><div class="ach-bullet"></div>Redux Toolkit state scaling across 50+ Smart TV models</div>
          <div class="ach"><div class="ach-bullet"></div>Deployed to LG Content Store & Samsung Smart Hub</div>
        </div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-dot"></div>
      <div class="job-card">
        <div class="job-top"><div class="job-title">Trainee Software Engineer</div><div class="job-badge">Nov 2022 – Oct 2023</div></div>
        <div class="job-company"><div class="job-company-bullet"></div>Saranyu Technologies</div>
        <div class="job-desc">Built Smart TV apps on WebOS & Tizen with React, real-time video playback, EPG system, and remote-optimized UI for large-screen devices.</div>
        <div class="ach-grid">
          <div class="ach"><div class="ach-bullet"></div>TV apps from scratch — WebOS & TizenOS responsive layouts</div>
          <div class="ach"><div class="ach-bullet"></div>EPG with real-time schedule data integration</div>
          <div class="ach"><div class="ach-bullet"></div>Reusable video player components with remote navigation</div>
          <div class="ach"><div class="ach-bullet"></div>Redux Toolkit for scalable app state management</div>
        </div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-dot"></div>
      <div class="job-card">
        <div class="job-top"><div class="job-title">Web Development Intern</div><div class="job-badge">Jun 2022</div></div>
        <div class="job-company"><div class="job-company-bullet"></div>Null Class</div>
        <div class="job-desc">End-to-end web dev with React and REST APIs on live client projects — UI components, performance optimization, and clean architecture.</div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-dot"></div>
      <div class="job-card">
        <div class="job-top"><div class="job-title">MERN Stack Trainee</div><div class="job-badge">Dec 2021 – May 2022</div></div>
        <div class="job-company"><div class="job-company-bullet"></div>NxtWave Disruptive Technologies</div>
        <div class="job-desc">Intensive full-stack MERN program — MongoDB, Express, React, Node.js. Built end-to-end apps with auth, REST APIs, and deployment.</div>
      </div>
    </div>
  </div>
</div>

<!-- STATS -->
<div class="section">
  <div class="sec-head"><span class="sec-num">05</span><span class="sec-title">GitHub Stats</span><div class="sec-line"></div></div>
  <div class="stats-row">
    <div class="stat-box"><div class="stat-num">3+</div><div class="stat-label">Years Exp</div></div>
    <div class="stat-box"><div class="stat-num">4</div><div class="stat-label">Companies</div></div>
    <div class="stat-box"><div class="stat-num">2</div><div class="stat-label">Smart TV OS</div></div>
    <div class="stat-box"><div class="stat-num">20+</div><div class="stat-label">Technologies</div></div>
  </div>
  <div class="gh-imgs">
    <img class="gh-img" src="https://github-readme-stats.vercel.app/api?username=Maheshkumar4867&theme=github_dark&hide_border=true&bg_color=161b22&title_color=3fb950&text_color=8b949e&icon_color=1D9E75" alt="stats"/>
    <img class="gh-img" src="https://nirzak-streak-stats.vercel.app/?user=Maheshkumar4867&theme=github-dark-blue&hide_border=true&background=161b22&ring=1D9E75&fire=3fb950&currStreakLabel=8b949e" alt="streak"/>
    <img class="gh-img" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Maheshkumar4867&theme=github_dark&hide_border=true&bg_color=161b22&title_color=3fb950&text_color=8b949e&layout=compact" alt="langs"/>
  </div>
</div>

<!-- CONTACT -->
<div class="section">
  <div class="sec-head"><span class="sec-num">06</span><span class="sec-title">Get In Touch</span><div class="sec-line"></div></div>
  <div class="contact-grid">
    <a class="contact-card" href="mailto:k.maheshkumar8522@gmail.com">
      <div class="contact-icon" style="background:rgba(234,67,53,.1)"><svg width="18" height="18" viewBox="0 0 24 24" fill="#EA4335"><path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></svg></div>
      <div><div class="contact-label">Email</div><div class="contact-val">k.maheshkumar8522@gmail.com</div></div>
    </a>
    <a class="contact-card" href="https://maheshkumardev.com" target="_blank">
      <div class="contact-icon" style="background:rgba(29,158,117,.1)"><svg width="18" height="18" viewBox="0 0 24 24" fill="#1D9E75"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"/></svg></div>
      <div><div class="contact-label">Portfolio</div><div class="contact-val">maheshkumardev.com</div></div>
    </a>
    <a class="contact-card" href="https://www.linkedin.com/in/maheshkumardev/" target="_blank">
      <div class="contact-icon" style="background:rgba(10,102,194,.1)"><svg width="18" height="18" viewBox="0 0 24 24" fill="#0A66C2"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg></div>
      <div><div class="contact-label">LinkedIn</div><div class="contact-val">in/maheshkumardev</div></div>
    </a>
    <a class="contact-card" href="https://github.com/Maheshkumar4867" target="_blank">
      <div class="contact-icon" style="background:rgba(240,246,252,.05)"><svg width="18" height="18" viewBox="0 0 24 24" fill="#f0f6fc"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg></div>
      <div><div class="contact-label">GitHub</div><div class="contact-val">Maheshkumar4867</div></div>
    </a>
  </div>
</div>

<div class="footer">
  <div class="footer-bar"></div>
  mahesh kumar · full stack developer · bangalore · 2025
</div>

</div>
