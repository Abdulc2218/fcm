<html>
<head>
  <title>FC Mobile Community – Landing Page</title>
  <meta name="description" content="Join the ultimate FC Mobile community. Track updates, explore Shadows League, and stay connected with other football fans." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg: #0b0c10;             
      --panel: #101218;          
      --card: #151827;           
      --muted: #a8b0c2;          
      --text: #f5f7ff;           
      --accent: #06b6d4;         
      --accent-2: #34dbeb;       
      --ring: rgba(6,182,212,.55);
      --grad: conic-gradient(from 160deg at 50% 50%, #06b6d4 0%, #34ebb1 40%, #34dbeb 70%, #06b6d4 100%);
      --radius-xl: 20px;
      --radius-2xl: 28px;
      --shadow-1: 0 10px 30px rgba(0,0,0,.45);
      --shadow-2: 0 24px 70px rgba(0,0,0,.6);
      --border: 1px solid rgba(255,255,255,.06);
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial;
      color:var(--text);
      background: radial-gradient(1200px 800px at 10% -10%, rgba(6,182,212,.08), transparent 50%),
                  radial-gradient(800px 600px at 110% 10%, rgba(52,219,235,.1), transparent 40%),
                  var(--bg);
      line-height:1.6;
    }

    a{color:inherit;text-decoration:none}
    .container{width:min(1200px, 92vw); margin-inline:auto}
    .section{padding:72px 0}
    .grid{display:grid; gap:24px}

    header{
      position:sticky; top:0; z-index:50;
      backdrop-filter:saturate(160%) blur(12px);
      background:linear-gradient(to bottom, rgba(16,18,24,.9), rgba(16,18,24,.65));
      border-bottom:var(--border);
    }
    .nav{display:flex; align-items:center; justify-content:space-between; padding:16px 0}
    .brand{display:flex; align-items:center; gap:12px; font-weight:800; letter-spacing:.2px}
    .logo{
      width:36px; height:36px; border-radius:10px; position:relative; overflow:hidden; flex:0 0 auto;
      box-shadow: inset 0 0 0 1px rgba(255,255,255,.08), 0 8px 24px rgba(6,182,212,.25);
      background: radial-gradient(120% 120% at 10% 10%, #06b6d4 0%, #34dbeb 60%, #34ebb1 100%);
    }
    nav a{opacity:.9; font-weight:500; padding:10px 12px; border-radius:10px}
    nav a:hover{background:rgba(255,255,255,.04)}

    .btn{display:inline-flex; align-items:center; justify-content:center; gap:10px; font-weight:700;
      padding:12px 18px; border-radius:14px; border:var(--border); position:relative; overflow:hidden}
    .btn-primary{
      background:linear-gradient(180deg, var(--accent), #0284c7);
      box-shadow: 0 10px 24px rgba(6,182,212,.4);
      border-color: transparent;
    }
    .btn-ghost{background:rgba(255,255,255,.02)}

    .hero{display:grid; grid-template-columns: 1.15fr .85fr; gap:40px; align-items:center; padding:56px 0}
    h1{font-size: clamp(36px, 4.2vw, 56px); line-height:1.05; margin:16px 0 18px}
    h1 .accent{background:linear-gradient(90deg, var(--accent), #34dbeb 55%, #34ebb1); -webkit-background-clip:text; background-clip:text; -webkit-text-fill-color:transparent}
    .lead{font-size: clamp(16px, 1.2vw, 18px); color:var(--muted); max-width:60ch}
    .cta{display:flex; gap:12px; flex-wrap:wrap; margin-top:24px}

    .title{font-size: clamp(28px, 3.2vw, 42px); margin:10px 0 18px}
    .title .accent{color:var(--accent)}
    .subtitle{color:var(--muted); max-width:70ch}

    .card{background:linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,.02)); border:var(--border); border-radius:var(--radius-xl); padding:24px; box-shadow:var(--shadow-1)}
    .card h3{margin:16px 0 8px}
    .card p{color:var(--muted)}

    footer{border-top:var(--border); padding:36px 0 60px; color:#c5cad6}
    .foot{display:grid; grid-template-columns: 1.1fr .9fr; gap:24px}
    .links{display:grid; grid-template-columns: repeat(3, 1fr); gap:16px}
    .links a{display:block; padding:6px 0; opacity:.85}
    .links a:hover{opacity:1}
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="logo" aria-hidden="true"></div>
        <span>FC Mobile Community</span>
      </div>
      <nav aria-label="Primary">
        <a href="#features">Features</a>
        <a href="#updates">Updates</a>
        <a href="#league">Shadows League</a>
      </nav>
      <div style="display:flex; gap:10px">
        <a href="#join" class="btn btn-primary">Join Server</a>
      </div>
    </div>
  </header>

  <main>
    <section class="container hero">
      <div>
        <h1>The Home of <span class="accent">FC Mobile</span> Players</h1>
        <p class="lead">Stay updated with the latest FC Mobile news, events, and guides. Connect with other players and take part in the exclusive Shadows League.</p>
        <div class="cta">
          <a class="btn btn-primary" href="#join">Join Now</a>
          <a class="btn btn-ghost" href="#features">Learn More</a>
        </div>
      </div>
    </section>

    <section id="features" class="container section">
      <div>
        <div class="eyebrow">Features</div>
        <h2 class="title">Why Join <span class="accent">Our Server?</span></h2>
        <p class="subtitle">From guides and live updates to a thriving competitive league, our FC Mobile community has everything you need.</p>
      </div>
      <div class="grid steps" style="margin-top:24px; grid-template-columns:repeat(3,1fr)">
        <article class="card"><h3>📢 Updates</h3><p>Get the fastest FC Mobile news, leaks, and patch notes directly.</p></article>
        <article class="card"><h3>🎮 Community</h3><p>Meet players worldwide, trade tips, and share your squads.</p></article>
        <article class="card"><h3>🏆 Shadows League</h3><p>Compete in our exclusive server league and prove your skills.</p></article>
      </div>
    </section>

    <section id="league" class="container section">
      <h2 class="title">Enter the <span class="accent">Shadows League</span></h2>
      <p class="subtitle">Challenge the best players in our server-exclusive competition. Seasonal rewards, rankings, and ultimate bragging rights await!</p>
      <div class="cta" style="margin-top:20px">
        <a class="btn btn-primary" href="#join">Join the League</a>
      </div>
    </section>

    <section id="join" class="container section">
      <div class="card" style="text-align:center; padding:40px">
        <h2 class="title">Join the <span class="accent">FC Mobile Community</span> Today</h2>
        <p class="subtitle">Be part of the fastest growing FC Mobile Discord. Share, compete, and stay ahead of the game.</p>
        <div class="cta" style="margin-top:20px">
          <a class="btn btn-primary" href="#">Join Server</a>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container foot">
      <div>
        <div class="brand" style="margin-bottom:8px">
          <div class="logo" aria-hidden="true"></div>
          <strong>FC Mobile Community</strong>
        </div>
        <p style="color:var(--muted); max-width:50ch">The ultimate hub for FC Mobile players. News, leagues, and a global community all in one place.</p>
      </div>
      <div class="links">
        <div>
          <strong>Community</strong>
          <a href="#features">Features</a>
          <a href="#league">Shadows League</a>
          <a href="#join">Join</a>
        </div>
        <div>
          <strong>Resources</strong>
          <a href="#updates">Updates</a>
          <a href="#">Guides</a>
          <a href="#">Support</a>
        </div>
        <div>
          <strong>Follow</strong>
          <a href="#">Twitter</a>
          <a href="#">YouTube</a>
          <a href="#">Discord</a>
        </div>
      </div>
    </div>
  </footer>
</body>
</html>
