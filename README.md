<!DOCTYPE html>
<html lang="nl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Café de Nachtegaal — Uden</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,600;9..144,700;9..144,900&family=Fraunces:ital,opsz,wght@1,9..144,500&family=Karla:wght@400;500;700&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #191009;
    --bg-alt: #221609;
    --wood: #33210f;
    --wood-light: #422c17;
    --brass: #c8903f;
    --brass-light: #e6b978;
    --brass-dim: #8a622f;
    --cream: #efe2c6;
    --muted: #b7a284;
    --ink: #0d0805;
    --line: rgba(239,226,198,0.14);
    --maxw: 1180px;
  }

  *{ box-sizing: border-box; }
  html{ scroll-behavior: smooth; }
  body{
    margin:0;
    background: var(--bg);
    color: var(--cream);
    font-family: 'Karla', sans-serif;
    font-size: 17px;
    line-height: 1.6;
    overflow-x: hidden;
    background-image:
      repeating-linear-gradient(115deg, rgba(255,255,255,0.012) 0px, rgba(255,255,255,0.012) 1px, transparent 1px, transparent 3px);
  }
  h1,h2,h3{
    font-family: 'Fraunces', serif;
    margin: 0;
    font-weight: 600;
    color: var(--cream);
    letter-spacing: 0.2px;
  }
  a{ color: var(--brass-light); }
  p{ color: var(--muted); max-width: 62ch; }
  .wrap{ max-width: var(--maxw); margin: 0 auto; padding: 0 clamp(20px, 5vw, 56px); }
  .eyebrow{ color: var(--brass); font-family: 'Fraunces', serif; font-style: italic; font-weight: 500; font-size: 1.05rem; }

  /* ---------- top nav ---------- */
  .nav{
    position: fixed; top:0; left:0; right:0; z-index: 50;
    display:flex; align-items:center; justify-content:space-between;
    padding: 18px clamp(20px,5vw,56px);
    opacity: 0; transform: translateY(-12px);
    transition: opacity .5s ease, transform .5s ease, background .3s ease;
    pointer-events: none;
  }
  .nav.show{ opacity:1; transform:none; pointer-events:auto; background: rgba(20,13,7,0.72); backdrop-filter: blur(8px); border-bottom: 1px solid var(--line); }
  .nav-name{ font-family:'Fraunces',serif; font-size:1.05rem; color:var(--cream); }
  .nav-cta{
    font-family:'Karla',sans-serif; font-size:0.9rem; font-weight:700;
    color: var(--ink); background: var(--brass); padding: 9px 18px;
    border-radius: 2px; text-decoration:none; letter-spacing:0.2px;
    transition: background .2s ease;
  }
  .nav-cta:hover{ background: var(--brass-light); }

  /* ---------- hero ---------- */
  .hero{
    position:relative; min-height: 100svh;
    display:flex; align-items:center; justify-content:center;
    perspective: 1300px;
    background:
      radial-gradient(ellipse 60% 45% at 50% 28%, rgba(200,144,63,0.16), transparent 60%),
      linear-gradient(180deg, var(--bg) 0%, var(--bg-alt) 100%);
    overflow: hidden;
    padding-top: 60px;
  }
  .hero-scene{
    position:relative; width:100%; height:100%;
    display:flex; flex-direction:column; align-items:center; justify-content:center;
    transform-style: preserve-3d;
  }
  .lantern-wrap{
    position:relative; width: 150px; height: 210px; margin-bottom: 10px;
    transform-style: preserve-3d;
    animation: sway 6.5s ease-in-out infinite;
    transform-origin: top center;
  }
  @keyframes sway{
    0%,100%{ transform: rotateZ(-3.2deg); }
    50%{ transform: rotateZ(3.2deg); }
  }
  .lantern-wrap svg{ width:100%; height:100%; overflow: visible; }
  .glow{
    position:absolute; left:50%; top:56%; width:230px; height:230px;
    transform: translate(-50%,-50%);
    background: radial-gradient(circle, rgba(230,185,120,0.5), rgba(230,185,120,0) 68%);
    filter: blur(2px);
    pointer-events:none;
  }
  .hero h1{
    font-size: clamp(2.6rem, 6.4vw, 5rem);
    text-align:center; line-height: 1.02; margin-top: 6px;
  }
  .hero .tagline{
    font-family:'Fraunces',serif; font-style: italic; font-weight:500;
    color: var(--muted); font-size: clamp(1.05rem,2vw,1.35rem);
    text-align:center; margin: 18px auto 0; max-width: 46ch;
  }
  .hero-meta{
    display:flex; gap: 22px; flex-wrap:wrap; justify-content:center;
    margin-top: 34px; font-size: 0.92rem; color: var(--brass-light);
  }
  .hero-meta span{ display:flex; align-items:center; gap:7px; }
  .dot{ width:4px;height:4px;border-radius:50%; background: var(--brass-dim); display:inline-block; }
  .scroll-cue{
    position:absolute; bottom: 34px; left:50%; transform: translateX(-50%);
    display:flex; flex-direction:column; align-items:center; gap:8px;
    color: var(--brass-dim); font-size: 0.78rem; letter-spacing: 0.5px;
  }
  .scroll-cue .bar{
    width:1px; height: 34px; background: linear-gradient(var(--brass), transparent);
    animation: cue 1.8s ease-in-out infinite;
  }
  @keyframes cue{ 0%{ opacity:.2; } 50%{ opacity:1; } 100%{ opacity:.2; } }

  /* ---------- generic section ---------- */
  section{ position:relative; padding: clamp(72px,11vw,132px) 0; }
  .section-head{ max-width: 58ch; margin-bottom: 52px; }
  .section-head h2{ font-size: clamp(1.9rem,3.6vw,2.7rem); margin-top:10px; }

  /* ---------- story (sfeer) ---------- */
  .story{
    display:grid; grid-template-columns: 1.05fr 0.95fr; gap: clamp(30px,6vw,72px);
    align-items:center;
  }
  .story-copy p + p{ margin-top: 14px; }
  .stage{
    perspective: 1200px;
  }
  .scene-card{
    position:relative; border-radius: 3px; aspect-ratio: 4/5;
    background: linear-gradient(155deg, var(--wood-light), var(--wood) 60%, #251809 100%);
    border: 1px solid var(--line);
    transform-style: preserve-3d;
    transform: rotateY(-8deg) rotateX(3deg);
    transition: transform .15s ease-out;
    box-shadow: 30px 40px 70px rgba(0,0,0,0.45);
    overflow: hidden;
  }
  .scene-card .bar-illust{ position:absolute; inset:0; }
  .scene-card .frame-label{
    position:absolute; left:20px; bottom:18px; font-family:'Fraunces',serif;
    font-style:italic; color: var(--brass-light); font-size: 0.95rem;
  }

  /* ---------- menu ---------- */
  .menu-grid{
    display:grid; grid-template-columns: repeat(3, 1fr); gap: 22px;
    perspective: 1400px;
  }
  .tilt-card{
    background: var(--wood);
    border: 1px solid var(--line);
    padding: 30px 26px;
    border-radius: 2px;
    transform-style: preserve-3d;
    transform: rotateX(-18deg) translateY(24px);
    opacity: 0;
    transition: transform .8s cubic-bezier(.2,.7,.25,1), opacity .8s ease;
  }
  .tilt-card.in-view{ transform: rotateX(0) translateY(0); opacity:1; }
  .tilt-card h3{ font-size: 1.18rem; margin-bottom: 8px; }
  .tilt-card .price{ color: var(--brass-light); font-family:'Fraunces',serif; font-style:italic; font-size:0.98rem; }
  .tilt-card p{ margin-top:10px; font-size: 0.93rem; }
  .menu-note{ margin-top:26px; font-size: 0.85rem; color: var(--brass-dim); }

  /* ---------- reviews ---------- */
  .rating-row{ display:flex; align-items:baseline; gap:14px; margin-bottom: 44px; }
  .rating-num{ font-family:'Fraunces',serif; font-size: 3rem; color: var(--brass-light); }
  .rating-sub{ color: var(--muted); font-size:0.92rem; }
  .reviews-grid{
    display:grid; grid-template-columns: repeat(3,1fr); gap: 22px;
    perspective: 1400px;
  }
  .review-card{
    background: var(--bg-alt); border:1px solid var(--line); border-radius: 2px;
    padding: 28px 24px; transform-style:preserve-3d;
    transform: rotateY(14deg) translateX(-18px); opacity:0;
    transition: transform .8s cubic-bezier(.2,.7,.25,1), opacity .8s ease;
  }
  .review-card:nth-child(2){ transform: rotateX(-14deg) translateY(18px); }
  .review-card:nth-child(3){ transform: rotateY(-14deg) translateX(18px); }
  .review-card.in-view{ transform: none; opacity:1; }
  .review-card .quote{ font-family:'Fraunces',serif; font-style:italic; font-size:1.02rem; color:var(--cream); }
  .review-card .who{ margin-top:16px; font-size:0.85rem; color:var(--brass-dim); }

  /* ---------- hours / location ---------- */
  .hours{
    display:grid; grid-template-columns: 1fr 1fr; gap: clamp(30px,6vw,72px);
  }
  .hours-table{ width:100%; border-collapse: collapse; }
  .hours-table tr{ border-bottom: 1px solid var(--line); }
  .hours-table td{ padding: 13px 0; font-size:0.95rem; }
  .hours-table td:first-child{ color: var(--cream); font-family:'Fraunces',serif; }
  .hours-table td:last-child{ text-align:right; color: var(--muted); }
  .hours-table tr.closed td:last-child{ color: var(--brass-dim); font-style: italic; }
  .addr-block p{ margin: 4px 0; }
  .addr-block a{ text-decoration:none; border-bottom: 1px solid var(--brass-dim); }
  .btn{
    display:inline-block; margin-top: 22px; padding: 13px 26px;
    background: var(--brass); color: var(--ink); font-weight:700; font-size:0.92rem;
    text-decoration:none; border-radius: 2px; transition: background .2s ease, transform .2s ease;
  }
  .btn:hover{ background: var(--brass-light); transform: translateY(-1px); }

  /* ---------- footer ---------- */
  footer{
    border-top: 1px solid var(--line); padding: 44px 0 30px;
    display:flex; align-items:center; justify-content:space-between; flex-wrap:wrap; gap:16px;
  }
  footer .fname{ font-family:'Fraunces',serif; font-style:italic; color:var(--muted); font-size:0.95rem; }
  footer .fmeta{ font-size:0.82rem; color: var(--brass-dim); }

  @media (max-width: 880px){
    .story, .hours{ grid-template-columns: 1fr; }
    .menu-grid, .reviews-grid{ grid-template-columns: 1fr; }
    .stage{ order: -1; }
  }

  @media (prefers-reduced-motion: reduce){
    html{ scroll-behavior:auto; }
    .lantern-wrap{ animation:none; }
    .scene-card{ transform:none !important; }
    .tilt-card, .review-card{ transition:none; transform:none; opacity:1; }
    .scroll-cue .bar{ animation:none; }
  }

  a:focus-visible, button:focus-visible{ outline: 2px solid var(--brass-light); outline-offset: 3px; }
</style>
</head>
<body>

<nav class="nav" id="nav">
  <span class="nav-name">Café de Nachtegaal</span>
  <a class="nav-cta" href="tel:+31630862200">Bel &amp; reserveer</a>
</nav>

<header class="hero" id="hero">
  <div class="hero-scene" id="heroScene">
    <div class="lantern-wrap" id="lantern">
      <div class="glow"></div>
      <svg viewBox="0 0 150 210">
        <line x1="75" y1="0" x2="75" y2="26" stroke="var(--brass-dim)" stroke-width="2"/>
        <path d="M55 26 h40 l-6 14 h-28 z" fill="var(--brass)"/>
        <path d="M50 40 h50 v88 a25 25 0 0 1 -50 0 z" fill="var(--wood-light)" stroke="var(--brass)" stroke-width="1.5"/>
        <path d="M58 46 h34 v78 a17 17 0 0 1 -34 0 z" fill="#f2c98a" opacity="0.85"/>
        <path d="M58 46 h34 v78 a17 17 0 0 1 -34 0 z" fill="none" stroke="var(--brass-light)" stroke-width="1"/>
        <ellipse cx="75" cy="128" rx="25" ry="6" fill="var(--brass)"/>
        <path d="M60 134 q15 10 30 0 l-4 14 q-11 8 -22 0 z" fill="var(--brass)"/>
        <g transform="translate(100,4) scale(0.9)" opacity="0.92">
          <path d="M0 14 q10 -14 26 -10 q-4 4 -3 9 q7 -2 11 4 q-9 3 -9 10 q-9 -2 -14 -7 q-8 -1 -11 -6 z" fill="var(--brass-light)"/>
        </g>
      </svg>
    </div>
    <h1>Café de<br>Nachtegaal</h1>
    <p class="tagline">Een bruin café in het hart van Uden — bier dat betaalbaar blijft, avonden die dat niet snel doen.</p>
    <div class="hero-meta">
      <span>★ 4,7 <span style="color:var(--muted)">— 77 reviews</span></span>
      <span class="dot"></span>
      <span>€ 10–50 p.p.</span>
      <span class="dot"></span>
      <span>Elisabethstraat 25, Uden</span>
    </div>
  </div>
  <div class="scroll-cue"><span class="bar"></span>scroll</div>
</header>

<main>
  <section id="sfeer">
    <div class="wrap story">
      <div class="story-copy">
        <p class="eyebrow">De sfeer</p>
        <h2>Waar de avond zichzelf regelt</h2>
        <p>Geen kaarsjes-en-decor-verhaal nodig: gewoon een bar, koel bier tegen een eerlijke prijs, en een eigenaar die zijn gasten kent bij naam. Op donderdag- en vrijdagavond schuift het geluid van live muziek — vaste gast Dave Brokken speelt geregeld — moeiteloos tussen de gesprekken door.</p>
        <p>Het is de plek waar Uden nog gewoon een biertje drinkt zonder dat het een gelegenheid hoeft te zijn.</p>
      </div>
      <div class="stage">
        <div class="scene-card" id="sceneCard">
          <svg class="bar-illust" viewBox="0 0 400 500" preserveAspectRatio="xMidYMid slice">
            <rect width="400" height="500" fill="none"/>
            <rect x="0" y="330" width="400" height="170" fill="#2a1b0d"/>
            <rect x="0" y="330" width="400" height="6" fill="var(--brass)" opacity="0.6"/>
            <g opacity="0.9">
              <rect x="40" y="80" width="8" height="250" fill="#5a3d1e"/>
              <rect x="150" y="60" width="8" height="270" fill="#5a3d1e"/>
              <rect x="260" y="90" width="8" height="240" fill="#5a3d1e"/>
              <rect x="340" y="70" width="8" height="260" fill="#5a3d1e"/>
            </g>
            <g fill="var(--brass-light)" opacity="0.85">
              <circle cx="44" cy="80" r="5"/>
              <circle cx="154" cy="60" r="5"/>
              <circle cx="264" cy="90" r="5"/>
              <circle cx="344" cy="70" r="5"/>
            </g>
            <g stroke="var(--brass)" stroke-width="1.4" opacity="0.5">
              <path d="M44 85 q6 40 -4 80" fill="none"/>
              <path d="M154 65 q-8 40 4 80" fill="none"/>
              <path d="M264 95 q6 40 -4 80" fill="none"/>
              <path d="M344 75 q-8 40 4 80" fill="none"/>
            </g>
            <g fill="#8a5a24" opacity="0.7">
              <rect x="90" y="360" width="26" height="60" rx="2"/>
              <rect x="130" y="350" width="26" height="70" rx="2"/>
              <rect x="230" y="355" width="26" height="65" rx="2"/>
              <rect x="270" y="345" width="26" height="75" rx="2"/>
            </g>
          </svg>
          <span class="frame-label">donderdag, 21:40 uur</span>
        </div>
      </div>
    </div>
  </section>

  <section id="kaart" style="background: var(--bg-alt);">
    <div class="wrap">
      <div class="section-head">
        <p class="eyebrow">Op de kaart</p>
        <h2>Simpel, goed, niet duur</h2>
        <p>Een greep uit wat er getapt en geserveerd wordt — de volledige kaart hangt aan de muur, zoals het hoort.</p>
      </div>
      <div class="menu-grid">
        <div class="tilt-card">
          <h3>Getapt bier</h3>
          <span class="price">vanaf € 2,60</span>
          <p>Fris getapt, eerlijk geprijsd — inclusief het Duitse pils dat hier de vaste vervanger is van de grote merken.</p>
        </div>
        <div class="tilt-card">
          <h3>Borrelplank</h3>
          <span class="price">€ 12,50</span>
          <p>Kaas, worst en bitterballen, gemaakt om gedeeld te worden bij een tweede rondje.</p>
        </div>
        <div class="tilt-card">
          <h3>Uitsmijter &amp; broodjes</h3>
          <span class="price">vanaf € 8,-</span>
          <p>Voor wie eet voordat het avond wordt — ook gewoon om af te halen.</p>
        </div>
      </div>
      <p class="menu-note">Voorbeeldkaart — vervang door de actuele gerechten en prijzen van het café.</p>
    </div>
  </section>

  <section id="reviews">
    <div class="wrap">
      <div class="rating-row">
        <span class="rating-num">4,7</span>
        <span class="rating-sub">gebaseerd op 77 reviews</span>
      </div>
      <div class="reviews-grid">
        <div class="review-card">
          <p class="quote">"De enige plek in Uden waar een biertje nog betaalbaar is."</p>
          <p class="who">— Vaste gast, Google Reviews</p>
        </div>
        <div class="review-card">
          <p class="quote">"Gezellige avond, snelle bediening en goede live muziek van Dave Brokken."</p>
          <p class="who">— Local Guide, 200+ reviews</p>
        </div>
        <div class="review-card">
          <p class="quote">"Een horecaondernemer die zijn gasten écht centraal stelt."</p>
          <p class="who">— Kim B., stamgast</p>
        </div>
      </div>
    </div>
  </section>

  <section id="route" style="background: var(--bg-alt);">
    <div class="wrap hours">
      <div>
        <p class="eyebrow">Openingstijden</p>
        <h2 style="font-size:1.9rem; margin-bottom:22px;">Wanneer we open zijn</h2>
        <table class="hours-table">
          <tr class="closed"><td>Dinsdag</td><td>Gesloten</td></tr>
          <tr><td>Woensdag</td><td>15:00 – 01:00</td></tr>
          <tr><td>Donderdag</td><td>15:00 – 01:00</td></tr>
          <tr><td>Vrijdag</td><td>15:00 – 02:00</td></tr>
          <tr><td>Zaterdag</td><td>14:00 – 02:00</td></tr>
          <tr><td>Zondag</td><td>14:00 – 00:00</td></tr>
          <tr><td>Maandag</td><td>15:00 – 01:00</td></tr>
        </table>
      </div>
      <div class="addr-block">
        <p class="eyebrow">Route &amp; contact</p>
        <h2 style="font-size:1.9rem; margin: 10px 0 18px;">Elisabethstraat 25</h2>
        <p>5402 VD Uden</p>
        <p><a href="tel:+31630862200">06 30 86 22 00</a></p>
        <a class="btn" href="https://www.google.com/maps/search/?api=1&query=Caf%C3%A9+de+Nachtegaal+Elisabethstraat+25+Uden" target="_blank" rel="noopener">Plan je route</a>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="wrap" style="width:100%; display:flex; align-items:center; justify-content:space-between; flex-wrap:wrap; gap:16px;">
    <span class="fname">Café de Nachtegaal — Uden</span>
    <span class="fmeta">Ter plaatse eten · Afhalen · Bezorging</span>
  </div>
</footer>

<script>
(function(){
  var reduced = window.matchMedia('(prefers-reduced-motion: reduce)').matches;

  // Nav reveal
  var nav = document.getElementById('nav');
  var hero = document.getElementById('hero');
  window.addEventListener('scroll', function(){
    var y = window.scrollY;
    if(y > hero.offsetHeight * 0.6){ nav.classList.add('show'); }
    else{ nav.classList.remove('show'); }
  }, {passive:true});

  if(!reduced){
    // Continuous 3D scroll-linked scene: lantern + bar illustration
    var lantern = document.getElementById('lantern');
    var sceneCard = document.getElementById('sceneCard');
    var heroH = hero.offsetHeight;

    function raf(){
      var y = window.scrollY;

      // hero progress 0 -> 1 over the hero's height
      var hp = Math.min(Math.max(y / heroH, 0), 1);
      lantern.style.transform = 'translateY(' + (hp * 60) + 'px) scale(' + (1 - hp*0.12) + ')';

      // bar scene tilts as it enters the viewport
      var rect = sceneCard.getBoundingClientRect();
      var vh = window.innerHeight;
      var center = rect.top + rect.height/2;
      var progress = (vh/2 - center) / (vh/2); // -1 .. 1
      progress = Math.min(Math.max(progress, -1), 1);
      var rotY = -8 + progress * 10;
      var rotX = 3 - progress * 6;
      sceneCard.style.transform = 'rotateY(' + rotY + 'deg) rotateX(' + rotX + 'deg) translateZ(' + (progress*10) + 'px)';

      requestAnimationFrame(raf);
    }
    requestAnimationFrame(raf);
  }

  // Entrance reveals for cards
  var targets = document.querySelectorAll('.tilt-card, .review-card');
  if('IntersectionObserver' in window){
    var io = new IntersectionObserver(function(entries){
      entries.forEach(function(e, i){
        if(e.isIntersecting){
          setTimeout(function(){ e.target.classList.add('in-view'); }, i % 3 * 90);
          io.unobserve(e.target);
        }
      });
    }, {threshold: 0.2});
    targets.forEach(function(t){ io.observe(t); });
  } else {
    targets.forEach(function(t){ t.classList.add('in-view'); });
  }
})();
</script>

</body>
</html>
