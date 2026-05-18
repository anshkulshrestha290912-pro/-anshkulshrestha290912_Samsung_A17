# -anshkulshrestha290912_Samsung_A17
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Samsung Galaxy A17 5G — Official</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
<link href="https://fonts.googleapis.com/css2?family=Rajdhani:wght@300;400;500;600;700&family=Barlow:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;1,200;1,300&family=Barlow+Condensed:wght@200;300;400;500;600;700;800&display=swap" rel="stylesheet"/>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --bg:#04060a;
  --surface:#080c12;
  --surface2:#0d1219;
  --border:rgba(255,255,255,0.06);
  --border2:rgba(255,255,255,0.12);
  --text:#e8ecf2;
  --muted:#6b7a8d;
  --dim:#2a3040;
  --blue:#1a6cff;
  --blue-light:#4d94ff;
  --cyan:#00d4ff;
  --glow:rgba(26,108,255,0.25);
  --font-head:'Barlow Condensed',sans-serif;
  --font-body:'Barlow',sans-serif;
  --font-ui:'Rajdhani',sans-serif;
}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--text);font-family:var(--font-body);overflow-x:hidden;line-height:1.6}

/* ── Scanline overlay ── */
body::after{
  content:'';position:fixed;inset:0;
  background:repeating-linear-gradient(0deg,transparent,transparent 2px,rgba(0,0,0,0.03) 2px,rgba(0,0,0,0.03) 4px);
  pointer-events:none;z-index:9999;
}

/* ── Nav ── */
nav{
  position:fixed;top:0;left:0;right:0;z-index:100;
  display:flex;align-items:center;justify-content:space-between;
  padding:1rem 3rem;
  background:rgba(4,6,10,0.88);
  backdrop-filter:blur(16px);
  border-bottom:1px solid var(--border);
}
.nav-brand{
  font-family:var(--font-head);font-size:1.2rem;font-weight:700;
  letter-spacing:0.1em;color:var(--text);text-transform:uppercase;
}
.nav-brand span{color:var(--blue-light)}
.nav-links{display:flex;gap:2rem;list-style:none}
.nav-links a{
  font-family:var(--font-ui);font-size:0.95rem;font-weight:500;
  letter-spacing:0.08em;text-transform:uppercase;
  color:var(--muted);text-decoration:none;transition:color 0.2s;
}
.nav-links a:hover{color:var(--text)}
.nav-buy{
  font-family:var(--font-ui);font-size:0.9rem;font-weight:600;
  letter-spacing:0.1em;text-transform:uppercase;
  background:var(--blue);color:#fff;border:none;
  padding:0.55rem 1.5rem;cursor:pointer;
  clip-path:polygon(8px 0%,100% 0%,calc(100% - 8px) 100%,0% 100%);
  transition:background 0.2s,transform 0.15s;
}
.nav-buy:hover{background:var(--blue-light);transform:scale(0.97)}

/* ── Hero ── */
.hero{
  min-height:100vh;display:grid;
  grid-template-columns:1fr 1fr;
  align-items:center;gap:0;
  padding:6rem 3rem 3rem;
  position:relative;overflow:hidden;
}
/* Radial glow behind phone */
.hero::before{
  content:'';position:absolute;right:5%;top:50%;transform:translateY(-50%);
  width:600px;height:600px;border-radius:50%;
  background:radial-gradient(circle,rgba(26,108,255,0.18) 0%,transparent 70%);
  pointer-events:none;
}
/* Grid overlay hero */
.hero-grid-bg{
  position:absolute;inset:0;
  background-image:
    linear-gradient(rgba(26,108,255,0.04) 1px,transparent 1px),
    linear-gradient(90deg,rgba(26,108,255,0.04) 1px,transparent 1px);
  background-size:60px 60px;
  mask-image:radial-gradient(ellipse 80% 80% at 50% 50%,black 0%,transparent 100%);
}

.hero-left{position:relative;z-index:2}
.hero-eyebrow{
  font-family:var(--font-ui);font-size:0.8rem;font-weight:600;
  letter-spacing:0.25em;text-transform:uppercase;
  color:var(--cyan);margin-bottom:1.5rem;
  display:flex;align-items:center;gap:0.75rem;
}
.hero-eyebrow::before{content:'';display:block;width:28px;height:1px;background:var(--cyan)}
.hero-title{
  font-family:var(--font-head);
  font-size:clamp(3.5rem,8vw,7.5rem);
  font-weight:800;line-height:0.9;
  letter-spacing:-0.01em;
  text-transform:uppercase;
  margin-bottom:0.5rem;
}
.hero-title .line-muted{
  color:transparent;
  -webkit-text-stroke:1px rgba(255,255,255,0.18);
}
.hero-title .line-blue{color:var(--blue-light)}
.hero-title .line-5g{
  color:var(--cyan);
  font-size:0.55em;
  vertical-align:super;
  font-weight:700;
}
.hero-tagline{
  font-size:1.05rem;font-weight:300;
  color:var(--muted);max-width:400px;
  margin:1.5rem 0 2.5rem;line-height:1.8;
  font-style:italic;
}
.hero-price-row{display:flex;align-items:baseline;gap:0.75rem;margin-bottom:2.5rem}
.hero-price-label{font-family:var(--font-ui);font-size:0.75rem;letter-spacing:0.1em;color:var(--muted);text-transform:uppercase}
.hero-price{font-family:var(--font-head);font-size:2.8rem;font-weight:700;color:var(--text);letter-spacing:-0.02em}
.hero-price sup{font-size:0.5em;vertical-align:super;color:var(--muted)}

.hero-actions{display:flex;gap:1rem;flex-wrap:wrap}
.btn-primary{
  font-family:var(--font-ui);font-size:0.9rem;font-weight:600;
  letter-spacing:0.12em;text-transform:uppercase;
  background:var(--blue);color:#fff;border:none;
  padding:0.9rem 2.2rem;cursor:pointer;
  clip-path:polygon(10px 0%,100% 0%,calc(100% - 10px) 100%,0% 100%);
  transition:all 0.2s;text-decoration:none;display:inline-block;
}
.btn-primary:hover{background:var(--blue-light);transform:translateY(-2px)}
.btn-outline{
  font-family:var(--font-ui);font-size:0.9rem;font-weight:600;
  letter-spacing:0.12em;text-transform:uppercase;
  background:transparent;color:var(--text);
  border:1px solid var(--border2);
  padding:0.9rem 2.2rem;cursor:pointer;
  transition:all 0.2s;text-decoration:none;display:inline-block;
}
.btn-outline:hover{border-color:var(--blue-light);color:var(--blue-light)}

/* Phone illustration */
.hero-right{
  position:relative;z-index:2;
  display:flex;justify-content:center;align-items:center;
}
.phone-wrap{
  position:relative;width:300px;height:580px;
  animation:float 5s ease-in-out infinite;
}
@keyframes float{
  0%,100%{transform:translateY(0)}
  50%{transform:translateY(-18px)}
}
.phone-body{
  width:100%;height:100%;
  background:linear-gradient(145deg,#1a1f2e 0%,#0d1018 40%,#141824 100%);
  border-radius:40px;
  border:1px solid rgba(255,255,255,0.12);
  position:relative;overflow:hidden;
  box-shadow:
    0 0 0 1px rgba(255,255,255,0.05),
    0 40px 80px rgba(0,0,0,0.6),
    0 0 60px rgba(26,108,255,0.12),
    inset 0 1px 0 rgba(255,255,255,0.08);
}
/* Screen */
.phone-screen{
  position:absolute;top:14px;left:8px;right:8px;bottom:14px;
  background:linear-gradient(160deg,#0a1628 0%,#050d1a 50%,#0c1220 100%);
  border-radius:33px;overflow:hidden;
}
/* Wallpaper-like screen content */
.phone-screen-content{
  width:100%;height:100%;
  background:
    radial-gradient(ellipse 80% 60% at 50% 30%,rgba(26,108,255,0.3) 0%,transparent 60%),
    radial-gradient(ellipse 60% 40% at 80% 80%,rgba(0,212,255,0.12) 0%,transparent 60%),
    linear-gradient(180deg,#060d1a 0%,#0a1528 100%);
  display:flex;flex-direction:column;align-items:center;padding-top:60px;gap:8px;
}
/* Status bar -->
.phone-status{
  position:absolute;top:18px;left:20px;right:20px;
  display:flex;justify-content:space-between;align-items:center;
  font-family:var(--font-ui);font-size:10px;color:rgba(255,255,255,0.7);z-index:5;
}
/* Punch hole camera -->
.phone-camera{
  position:absolute;top:24px;left:50%;transform:translateX(-50%);
  width:14px;height:14px;background:#000;border-radius:50%;z-index:6;
  box-shadow:0 0 0 1px rgba(255,255,255,0.1);
}
/* screen UI elements -->
.screen-time{font-family:var(--font-head);font-size:2.8rem;font-weight:300;color:#fff;letter-spacing:-0.02em;margin-top:30px}
.screen-date{font-family:var(--font-body);font-size:0.75rem;color:rgba(255,255,255,0.5);margin-bottom:16px}
.screen-icons{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;padding:0 16px;margin-top:auto;margin-bottom:24px;width:100%}
.screen-icon{
  aspect-ratio:1;border-radius:14px;
  display:flex;align-items:center;justify-content:center;
  font-size:1.4rem;
}
.screen-icon.blue{background:rgba(26,108,255,0.5)}
.screen-icon.green{background:rgba(0,180,80,0.5)}
.screen-icon.orange{background:rgba(255,120,20,0.5)}
.screen-icon.purple{background:rgba(140,50,220,0.5)}
.screen-icon.teal{background:rgba(0,190,200,0.5)}
.screen-icon.red{background:rgba(220,40,60,0.5)}
.screen-icon.yellow{background:rgba(220,180,0,0.5)}
.screen-icon.pink{background:rgba(220,60,160,0.5)}

/* 5G badge -->
.badge-5g{
  position:absolute;top:-12px;right:-12px;
  background:var(--cyan);color:#04060a;
  font-family:var(--font-head);font-size:0.9rem;font-weight:800;
  letter-spacing:0.1em;padding:0.3rem 0.75rem;
  clip-path:polygon(6px 0%,100% 0%,calc(100% - 6px) 100%,0% 100%);
}
/* Glow rings around phone -->
.phone-ring{
  position:absolute;top:50%;left:50%;
  border-radius:50%;border:1px solid rgba(26,108,255,0.15);
  transform:translate(-50%,-50%);
  animation:pulse 4s ease-in-out infinite;
}
.phone-ring:nth-child(1){width:380px;height:380px;animation-delay:0s}
.phone-ring:nth-child(2){width:460px;height:460px;animation-delay:1s}
.phone-ring:nth-child(3){width:540px;height:540px;animation-delay:2s}
@keyframes pulse{0%,100%{opacity:0.4}50%{opacity:0.1}}

/* Side buttons -->
.phone-btn-vol{
  position:absolute;left:-3px;top:120px;
  width:4px;height:36px;background:rgba(255,255,255,0.15);border-radius:2px 0 0 2px;
}
.phone-btn-vol2{
  position:absolute;left:-3px;top:166px;
  width:4px;height:36px;background:rgba(255,255,255,0.15);border-radius:2px 0 0 2px;
}
.phone-btn-power{
  position:absolute;right:-3px;top:140px;
  width:4px;height:55px;background:rgba(255,255,255,0.15);border-radius:0 2px 2px 0;
}

/* ── Specs Bar ── */
.specs-bar{
  background:var(--surface);
  border-top:1px solid var(--border);
  border-bottom:1px solid var(--border);
  padding:1.5rem 3rem;
  display:flex;align-items:center;justify-content:space-between;
  gap:1rem;overflow-x:auto;
}
.spec-item{
  display:flex;flex-direction:column;align-items:center;
  gap:0.3rem;text-align:center;flex-shrink:0;
}
.spec-icon{font-size:1.5rem;margin-bottom:0.2rem}
.spec-val{font-family:var(--font-head);font-size:1.3rem;font-weight:700;color:var(--text);letter-spacing:0.02em}
.spec-label{font-family:var(--font-ui);font-size:0.7rem;letter-spacing:0.12em;text-transform:uppercase;color:var(--muted)}
.spec-sep{width:1px;height:40px;background:var(--border);flex-shrink:0}

/* ── Section shared ── */
section{position:relative;z-index:1}
.section-tag{
  font-family:var(--font-ui);font-size:0.72rem;font-weight:600;
  letter-spacing:0.2em;text-transform:uppercase;color:var(--cyan);
  margin-bottom:0.75rem;
}
.section-title{
  font-family:var(--font-head);
  font-size:clamp(2rem,5vw,3.8rem);
  font-weight:800;text-transform:uppercase;
  letter-spacing:-0.01em;line-height:1;
  margin-bottom:1rem;
}
.section-sub{
  font-size:1rem;font-weight:300;color:var(--muted);
  max-width:480px;line-height:1.8;
}

/* ── Features ── */
.features{padding:6rem 3rem;border-top:1px solid var(--border)}
.features-grid{
  display:grid;grid-template-columns:1fr 1fr 1fr;
  gap:1px;background:var(--border);
  border:1px solid var(--border);margin-top:4rem;
  overflow:hidden;
}
.feat-card{
  background:var(--bg);padding:2.5rem 2rem;
  transition:background 0.25s;position:relative;overflow:hidden;
}
.feat-card::before{
  content:'';position:absolute;top:0;left:0;right:0;height:1px;
  background:linear-gradient(90deg,transparent,var(--blue),transparent);
  opacity:0;transition:opacity 0.3s;
}
.feat-card:hover{background:var(--surface)}
.feat-card:hover::before{opacity:1}
.feat-icon{font-size:2.2rem;margin-bottom:1.2rem;display:block}
.feat-title{
  font-family:var(--font-head);font-size:1.3rem;font-weight:700;
  text-transform:uppercase;letter-spacing:0.03em;
  margin-bottom:0.75rem;color:var(--text);
}
.feat-desc{
  font-size:0.88rem;font-weight:300;color:var(--muted);
  line-height:1.8;
}
.feat-highlight{
  font-family:var(--font-head);font-size:2rem;font-weight:800;
  color:var(--blue-light);letter-spacing:-0.02em;
  display:block;margin-top:1.2rem;
}

/* ── Specs Full ── */
.specs-full{padding:6rem 3rem;border-top:1px solid var(--border);background:var(--surface)}
.specs-table-wrap{margin-top:3rem}
.specs-table{width:100%;border-collapse:collapse}
.specs-table tr{border-bottom:1px solid var(--border)}
.specs-table tr:hover td{background:rgba(255,255,255,0.02)}
.specs-table td{padding:1.1rem 0;font-size:0.92rem}
.specs-table td:first-child{
  font-family:var(--font-ui);font-size:0.78rem;letter-spacing:0.1em;
  text-transform:uppercase;color:var(--muted);width:35%;
  padding-right:2rem;
}
.specs-table td:last-child{color:var(--text);font-weight:300}
.specs-table td strong{color:var(--blue-light);font-weight:600}

/* ── Colors Section ── */
.colors-section{padding:6rem 3rem;border-top:1px solid var(--border)}
.color-options{
  display:flex;gap:2.5rem;margin-top:3rem;flex-wrap:wrap;align-items:center;
}
.color-option{
  display:flex;flex-direction:column;align-items:center;gap:0.75rem;
  cursor:pointer;
}
.color-swatch{
  width:64px;height:64px;border-radius:50%;
  border:2px solid transparent;transition:all 0.2s;
  position:relative;
}
.color-swatch.active,
.color-swatch:hover{border-color:rgba(255,255,255,0.4);transform:scale(1.1)}
.color-name{
  font-family:var(--font-ui);font-size:0.7rem;letter-spacing:0.1em;
  text-transform:uppercase;color:var(--muted);text-align:center;
}

/* ── CTA ── */
.cta{
  padding:7rem 3rem;border-top:1px solid var(--border);
  text-align:center;position:relative;overflow:hidden;
}
.cta::before{
  content:'';position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);
  width:700px;height:400px;border-radius:50%;
  background:radial-gradient(ellipse,rgba(26,108,255,0.12) 0%,transparent 70%);
  pointer-events:none;
}
.cta .section-title{font-size:clamp(2.5rem,7vw,5.5rem)}
.cta .section-sub{margin:1.5rem auto 3rem;text-align:center}
.cta-buttons{display:flex;gap:1.2rem;justify-content:center;flex-wrap:wrap}

/* ── Footer ── */
footer{
  background:var(--surface);border-top:1px solid var(--border);
  padding:2.5rem 3rem;
  display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:1rem;
}
.footer-brand{font-family:var(--font-head);font-size:1rem;font-weight:700;letter-spacing:0.1em;text-transform:uppercase;color:var(--muted)}
.footer-brand span{color:var(--blue-light)}
.footer-copy{font-family:var(--font-ui);font-size:0.72rem;letter-spacing:0.08em;color:var(--dim);text-transform:uppercase}

/* ── Animations ── */
@keyframes fadeUp{from{opacity:0;transform:translateY(28px)}to{opacity:1;transform:translateY(0)}}
.hero-eyebrow{animation:fadeUp 0.6s 0.1s both}
.hero-title{animation:fadeUp 0.6s 0.2s both}
.hero-tagline{animation:fadeUp 0.6s 0.35s both}
.hero-price-row{animation:fadeUp 0.6s 0.45s both}
.hero-actions{animation:fadeUp 0.6s 0.55s both}
.phone-wrap{animation:fadeUp 0.8s 0.3s both, float 5s 1.1s ease-in-out infinite}

/* ── Responsive ── */
@media(max-width:900px){
  nav{padding:1rem 1.5rem}
  .nav-links{display:none}
  .hero{grid-template-columns:1fr;padding:7rem 1.5rem 3rem;gap:3rem}
  .hero-right{order:-1}
  .phone-wrap{width:220px;height:420px}
  .features-grid{grid-template-columns:1fr}
  .specs-bar{padding:1.5rem}
  .features,.specs-full,.colors-section,.cta{padding:4rem 1.5rem}
  footer{padding:1.5rem;flex-direction:column;text-align:center}
}
</style>
</head>
<body>

<!-- Nav -->
<nav>
  <div class="nav-brand">Samsung <span>Galaxy</span></div>
  <ul class="nav-links">
    <li><a href="#features">Features</a></li>
    <li><a href="#specs">Specs</a></li>
    <li><a href="#colors">Colors</a></li>
    <li><a href="#buy">Buy</a></li>
  </ul>
  <button class="nav-buy">Buy Now</button>
</nav>

<!-- Hero -->
<section class="hero">
  <div class="hero-grid-bg"></div>

  <div class="hero-left">
    <p class="hero-eyebrow">Introducing</p>
    <h1 class="hero-title">
      Galaxy<br/>
      <span class="line-blue">A17</span><span class="line-5g">5G</span><br/>
      <span class="line-muted">Series</span>
    </h1>
    <p class="hero-tagline">Blazing 5G speed. Brilliant display.<br/>Built for the ones who never stop.</p>
    <div class="hero-price-row">
      <span class="hero-price-label">Starting at</span>
      <span class="hero-price"><sup>₹</sup>18,999</span>
    </div>
    <div class="hero-actions">
      <a href="#buy" class="btn-primary">Order Now</a>
      <a href="#specs" class="btn-outline">Explore Specs</a>
    </div>
  </div>

  <div class="hero-right">
    <div class="phone-ring"></div>
    <div class="phone-ring"></div>
    <div class="phone-ring"></div>
    <div class="phone-wrap">
      <div class="badge-5g">5G</div>
      <div class="phone-body">
        <div class="phone-btn-vol"></div>
        <div class="phone-btn-vol2"></div>
        <div class="phone-btn-power"></div>
        <div class="phone-screen">
          <div class="phone-camera"></div>
          <div class="phone-status">
            <span>9:41</span>
            <span>5G ▐▐▐ 🔋</span>
          </div>
          <div class="phone-screen-content">
            <div class="screen-time">9:41</div>
            <div class="screen-date">Monday, May 18</div>
            <div class="screen-icons">
              <div class="screen-icon blue">📷</div>
              <div class="screen-icon green">💬</div>
              <div class="screen-icon orange">🎵</div>
              <div class="screen-icon purple">🎮</div>
              <div class="screen-icon teal">🌐</div>
              <div class="screen-icon red">📺</div>
              <div class="screen-icon yellow">⭐</div>
              <div class="screen-icon pink">📸</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Specs Bar -->
<div class="specs-bar">
  <div class="spec-item"><div class="spec-icon">📶</div><div class="spec-val">5G</div><div class="spec-label">Connectivity</div></div>
  <div class="spec-sep"></div>
  <div class="spec-item"><div class="spec-icon">🧠</div><div class="spec-val">8 GB</div><div class="spec-label">RAM</div></div>
  <div class="spec-sep"></div>
  <div class="spec-item"><div class="spec-icon">💾</div><div class="spec-val">128 GB</div><div class="spec-label">Storage</div></div>
  <div class="spec-sep"></div>
  <div class="spec-item"><div class="spec-icon">🖥️</div><div class="spec-val">6.7"</div><div class="spec-label">Display</div></div>
  <div class="spec-sep"></div>
  <div class="spec-item"><div class="spec-icon">🔋</div><div class="spec-val">5000</div><div class="spec-label">mAh Battery</div></div>
  <div class="spec-sep"></div>
  <div class="spec-item"><div class="spec-icon">📷</div><div class="spec-val">50 MP</div><div class="spec-label">Main Camera</div></div>
  <div class="spec-sep"></div>
  <div class="spec-item"><div class="spec-icon">⚡</div><div class="spec-val">25W</div><div class="spec-label">Fast Charging</div></div>
</div>

<!-- Features -->
<section class="features" id="features">
  <div class="section-tag">Why Galaxy A17</div>
  <h2 class="section-title">Built Different.</h2>
  <p class="section-sub">Every detail engineered to give you more — more speed, more power, more life.</p>

  <div class="features-grid">
    <div class="feat-card">
      <span class="feat-icon">📶</span>
      <h3 class="feat-title">5G Ready</h3>
      <p class="feat-desc">Experience next-generation 5G speeds. Stream, download, and connect faster than ever before — wherever you go.</p>
      <span class="feat-highlight">10× Faster</span>
    </div>
    <div class="feat-card">
      <span class="feat-icon">🧠</span>
      <h3 class="feat-title">8 GB RAM</h3>
      <p class="feat-desc">Multitask like a pro. Switch between apps, games, and streams without a single stutter. More RAM, more freedom.</p>
      <span class="feat-highlight">8 GB RAM</span>
    </div>
    <div class="feat-card">
      <span class="feat-icon">💾</span>
      <h3 class="feat-title">128 GB Storage</h3>
      <p class="feat-desc">Store every moment. 128 GB of onboard storage means thousands of photos, videos, and apps — all at your fingertips.</p>
      <span class="feat-highlight">128 GB</span>
    </div>
    <div class="feat-card">
      <span class="feat-icon">📷</span>
      <h3 class="feat-title">50 MP Camera</h3>
      <p class="feat-desc">Capture life in stunning detail. The 50MP AI-enhanced main camera delivers sharp, vibrant shots day and night.</p>
      <span class="feat-highlight">50 MP AI</span>
    </div>
    <div class="feat-card">
      <span class="feat-icon">🔋</span>
      <h3 class="feat-title">All-Day Battery</h3>
      <p class="feat-desc">A massive 5000 mAh battery keeps you going all day and beyond. And with 25W fast charging, you're back up in no time.</p>
      <span class="feat-highlight">5000 mAh</span>
    </div>
    <div class="feat-card">
      <span class="feat-icon">🖥️</span>
      <h3 class="feat-title">Super AMOLED</h3>
      <p class="feat-desc">A 6.7-inch Super AMOLED display with 90Hz refresh rate brings everything to life — vivid colors, smooth scrolling.</p>
      <span class="feat-highlight">90 Hz</span>
    </div>
  </div>
</section>

<!-- Full Specs -->
<section class="specs-full" id="specs">
  <div class="section-tag">Technical Details</div>
  <h2 class="section-title">Full Specifications</h2>
  <div class="specs-table-wrap">
    <table class="specs-table">
      <tr><td>Model</td><td><strong>Samsung Galaxy A17 5G</strong></td></tr>
      <tr><td>Display</td><td>6.7" Super AMOLED, 1080 × 2400 px, <strong>90Hz</strong></td></tr>
      <tr><td>Processor</td><td>Octa-core 2.4 GHz (5G-enabled SoC)</td></tr>
      <tr><td>RAM</td><td><strong>8 GB</strong> LPDDR5</td></tr>
      <tr><td>Storage</td><td><strong>128 GB</strong> UFS 3.1, expandable via microSD</td></tr>
      <tr><td>Rear Camera</td><td><strong>50 MP</strong> (f/1.8) + 8 MP Ultra-wide + 2 MP Depth</td></tr>
      <tr><td>Front Camera</td><td><strong>13 MP</strong>, f/2.2, Auto-focus</td></tr>
      <tr><td>Battery</td><td><strong>5000 mAh</strong> with 25W fast charging</td></tr>
      <tr><td>OS</td><td>Android 14, One UI 6.0</td></tr>
      <tr><td>Connectivity</td><td><strong>5G</strong>, Wi-Fi 6, Bluetooth 5.3, NFC, USB-C</td></tr>
      <tr><td>Security</td><td>In-display Fingerprint + Face Unlock</td></tr>
      <tr><td>Dimensions</td><td>164.2 × 76.8 × 7.8 mm</td></tr>
      <tr><td>Weight</td><td>190 g</td></tr>
      <tr><td>Colors</td><td>Midnight Black, Ice Blue, Lavender Dusk, Sage Green</td></tr>
    </table>
  </div>
</section>

<!-- Colors -->
<section class="colors-section" id="colors">
  <div class="section-tag">Choose Your Style</div>
  <h2 class="section-title">Four Stunning<br/>Colors</h2>
  <div class="color-options">
    <div class="color-option">
      <div class="color-swatch active" style="background:linear-gradient(135deg,#1a1c22,#0d0f14);box-shadow:0 0 0 1px rgba(255,255,255,0.15)"></div>
      <span class="color-name">Midnight<br/>Black</span>
    </div>
    <div class="color-option">
      <div class="color-swatch" style="background:linear-gradient(135deg,#b8d8e8,#7ab3cc)"></div>
      <span class="color-name">Ice<br/>Blue</span>
    </div>
    <div class="color-option">
      <div class="color-swatch" style="background:linear-gradient(135deg,#c9b8d8,#a690be)"></div>
      <span class="color-name">Lavender<br/>Dusk</span>
    </div>
    <div class="color-option">
      <div class="color-swatch" style="background:linear-gradient(135deg,#a8c5a0,#7a9e72)"></div>
      <span class="color-name">Sage<br/>Green</span>
    </div>
  </div>
</section>

<!-- CTA -->
<section class="cta" id="buy">
  <div class="section-tag">Get Yours Today</div>
  <h2 class="section-title">Ready to<br/>Upgrade?</h2>
  <p class="section-sub">Samsung Galaxy A17 5G — 8 GB RAM, 128 GB Storage. Starting at ₹18,999.</p>
  <div class="cta-buttons">
    <a href="#" class="btn-primary">Buy Now — ₹18,999</a>
    <a href="#" class="btn-outline">Find a Store</a>
  </div>
</section>

<!-- Footer -->
<footer>
  <div class="footer-brand">Samsung <span>Galaxy</span> A17 5G</div>
  <div class="footer-copy">© 2026 Samsung Electronics — All specifications subject to change</div>
</footer>

<script>
// Scroll reveal
const observer = new IntersectionObserver(entries => {
  entries.forEach(e => {
    if(e.isIntersecting){
      e.target.style.opacity='1';
      e.target.style.transform='translateY(0)';
    }
  });
},{threshold:0.08});

document.querySelectorAll('.feat-card,.spec-item,.color-option').forEach(el=>{
  el.style.opacity='0';
  el.style.transform='translateY(24px)';
  el.style.transition='opacity 0.55s ease, transform 0.55s ease';
  observer.observe(el);
});

// Color swatch selector
document.querySelectorAll('.color-swatch').forEach(sw=>{
  sw.addEventListener('click',()=>{
    document.querySelectorAll('.color-swatch').forEach(s=>s.classList.remove('active'));
    sw.classList.add('active');
  });
});
</script>
</body>
</html>

