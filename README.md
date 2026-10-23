<!DOCTYPE html>
<html lang="nl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Café de Nachtegaal — Uden</title>
<meta name="description" content="Café de Nachtegaal in Uden: het donkerbruinste café van de stad. Zachte Premium van de tap, biljarten, darten, live muziek, sport op groot scherm en feesten tot 120 personen.">
<meta name="theme-color" content="#120a05">
<link rel="icon" href="favicon.svg" type="image/svg+xml">
<meta property="og:title" content="Café de Nachtegaal — Uden">
<meta property="og:description" content="Het donkerbruinste café van Uden: Zachte Premium van de tap, biljarten, darten, live muziek, sport en feesten tot 120 personen.">
<meta property="og:type" content="website">
<meta property="og:locale" content="nl_NL">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,600;0,9..144,800;1,9..144,400;1,9..144,600&family=Karla:wght@400;500;700&family=Caveat:wght@600&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#120a05; --bg2:#1a0f08; --panel:#241509; --panel2:#2e1b0c;
  --brass:#d1993f; --brass-hi:#f3cd85; --brass-lo:#8f6428;
  --cream:#f3e6c9; --muted:#bfae8f; --red:#a22d1f; --ink:#0c0603;
  --line:rgba(243,230,201,.14);
  --serif:'Fraunces',Georgia,'Times New Roman',serif;
  --sans:'Karla',system-ui,-apple-system,'Segoe UI',sans-serif;
  --hand:'Caveat','Segoe Script',cursive;
  --maxw:1220px; --gut:clamp(20px,5vw,64px);
}
*{box-sizing:border-box}
html{scroll-behavior:smooth;-webkit-text-size-adjust:100%}
body{margin:0;background:var(--bg);color:var(--cream);font-family:var(--sans);font-size:16px;line-height:1.6;overflow-x:hidden}
img{display:block;max-width:100%}
a{color:var(--brass-hi)}
h1,h2,h3,h4{font-family:var(--serif);font-weight:600;margin:0;color:var(--cream);letter-spacing:.2px;line-height:1.1}
p{margin:0 0 1em;color:var(--muted);max-width:60ch}
[hidden]{display:none!important}
.wrap{max-width:var(--maxw);margin:0 auto;padding:0 var(--gut)}
.eyebrow{display:inline-flex;align-items:center;gap:12px;font-family:var(--serif);font-style:italic;font-weight:400;color:var(--brass);font-size:1.05rem}
.eyebrow::before{content:"";width:34px;height:1px;background:var(--brass-lo)}
h2.big{font-size:clamp(1.75rem,3.4vw,2.7rem);margin:8px 0 14px;font-weight:600}
h2.big em{font-style:italic;color:var(--brass-hi);font-weight:400}
section{position:relative;padding:clamp(36px,4.6vw,66px) 0;scroll-margin-top:64px}
.grain{position:fixed;inset:0;pointer-events:none;z-index:90;opacity:.07;mix-blend-mode:overlay;background-image:url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='180' height='180'><filter id='n'><feTurbulence type='fractalNoise' baseFrequency='.9' numOctaves='2' stitchTiles='stitch'/></filter><rect width='100%25' height='100%25' filter='url(%23n)'/></svg>")}
a:focus-visible,button:focus-visible,input:focus-visible,select:focus-visible,textarea:focus-visible{outline:2px solid var(--brass-hi);outline-offset:3px}

/* ---------- buttons ---------- */
.btn{display:inline-flex;align-items:center;gap:10px;padding:14px 26px;border-radius:2px;font-family:var(--sans);font-weight:700;font-size:.95rem;letter-spacing:.3px;text-decoration:none;cursor:pointer;border:1px solid var(--brass);transition:transform .25s,background .25s,color .25s,box-shadow .25s}
.btn.solid{background:linear-gradient(180deg,var(--brass-hi),var(--brass));color:var(--ink);box-shadow:0 10px 30px -10px rgba(209,153,63,.6)}
.btn.solid:hover{transform:translateY(-2px);box-shadow:0 16px 36px -10px rgba(209,153,63,.8)}
.btn.ghost{background:transparent;color:var(--brass-hi)}
.btn.ghost:hover{background:rgba(209,153,63,.12);transform:translateY(-2px)}
.btn svg{width:18px;height:18px;flex:none}

/* ---------- nav ---------- */
.nav{position:fixed;top:0;left:0;right:0;z-index:80;display:flex;align-items:center;justify-content:space-between;gap:20px;padding:16px var(--gut);transition:background .35s,backdrop-filter .35s,border-color .35s;border-bottom:1px solid transparent}
.nav.solid{background:rgba(18,10,5,.78);backdrop-filter:blur(12px);-webkit-backdrop-filter:blur(12px);border-color:var(--line)}
.brand{display:flex;align-items:center;gap:12px;text-decoration:none;color:var(--cream)}
.brand svg{width:34px;height:28px;color:var(--brass)}
.brand span{font-family:var(--serif);font-size:1.12rem;font-weight:600;letter-spacing:.3px}
.nav-links{display:flex;gap:26px;align-items:center}
.nav-links a{color:var(--cream);text-decoration:none;font-size:.92rem;opacity:.82;transition:opacity .2s,color .2s}
.nav-links a:hover{opacity:1;color:var(--brass-hi)}
.nav .btn{padding:10px 20px;font-size:.88rem}
.nav-links .btn{display:none}
.burger{display:none;background:none;border:1px solid var(--line);color:var(--cream);padding:9px 14px;border-radius:2px;font:inherit;font-size:.9rem;cursor:pointer}
@media(max-width:940px){
  .nav-links{position:fixed;inset:0;flex-direction:column;justify-content:center;gap:26px;background:rgba(14,8,4,.97);opacity:0;pointer-events:none;transition:opacity .3s}
  .nav-links a{font-family:var(--serif);font-size:1.7rem;opacity:1}
  .nav.open .nav-links{opacity:1;pointer-events:auto}
  .burger{display:block;position:relative;z-index:2}
  .nav>.btn{display:none}
  .nav-links .btn{display:inline-flex;margin-top:10px}
}

/* ---------- hero ---------- */
.hero{position:relative;min-height:100svh;padding:0;display:flex;flex-direction:column;overflow:hidden;background:radial-gradient(ellipse 70% 55% at 50% 30%,#3a2110 0%,var(--bg) 70%)}
.hero-stage{position:relative;flex:1;display:flex;align-items:center;justify-content:center;perspective:1300px;padding:120px var(--gut) 90px}
.bokeh{position:absolute;inset:0;pointer-events:none;overflow:hidden}
.bokeh i{position:absolute;border-radius:50%;background:radial-gradient(circle,rgba(243,205,133,.55),rgba(243,205,133,0) 70%);filter:blur(3px);animation:rise linear infinite}
@keyframes rise{from{transform:translateY(20vh) scale(.8);opacity:0}15%{opacity:1}to{transform:translateY(-110vh) scale(1.2);opacity:0}}
.hero-glow{position:absolute;left:50%;top:38%;width:70vmin;height:70vmin;transform:translate(-50%,-50%);background:radial-gradient(circle,rgba(209,153,63,.28),transparent 65%);pointer-events:none;animation:breathe 7s ease-in-out infinite}
@keyframes breathe{50%{transform:translate(-50%,-50%) scale(1.12);opacity:.8}}
.float{position:absolute;margin:0;transform-style:preserve-3d;will-change:transform;border-radius:3px;overflow:hidden;box-shadow:0 40px 80px -20px rgba(0,0,0,.85),0 0 0 1px rgba(243,230,201,.12)}
.float img{width:100%;height:100%;object-fit:cover}
.float::after{content:"";position:absolute;inset:0;background:linear-gradient(160deg,rgba(209,153,63,.18),rgba(12,6,3,.45))}
.f1{left:5%;top:20%;width:clamp(130px,16vw,250px);aspect-ratio:855 / 1680;--d:60;transform:translate3d(calc(var(--mx,0)*calc(var(--d)*1px)),calc(var(--sy,0)*-.12px + var(--my,0)*calc(var(--d)*1px)),0) rotateY(24deg) rotateZ(-3deg)}
.f2{right:4%;top:14%;width:clamp(140px,17vw,270px);aspect-ratio:855 / 1389;--d:80;transform:translate3d(calc(var(--mx,0)*calc(var(--d)*1px)),calc(var(--sy,0)*-.2px + var(--my,0)*calc(var(--d)*1px)),0) rotateY(-24deg) rotateZ(3deg)}
.f3{left:15%;bottom:7%;width:clamp(100px,11vw,180px);aspect-ratio:837 / 1398;--d:30;filter:blur(2px);opacity:.75;transform:translate3d(calc(var(--mx,0)*calc(var(--d)*1px)),calc(var(--sy,0)*-.06px + var(--my,0)*calc(var(--d)*1px)),-80px) rotateY(18deg) rotateZ(4deg)}
.f4{right:14%;bottom:9%;width:clamp(100px,11vw,170px);aspect-ratio:855 / 1299;--d:35;filter:blur(2px);opacity:.75;transform:translate3d(calc(var(--mx,0)*calc(var(--d)*1px)),calc(var(--sy,0)*-.08px + var(--my,0)*calc(var(--d)*1px)),-80px) rotateY(-18deg) rotateZ(-4deg)}
.hero-copy{position:relative;z-index:3;text-align:center;max-width:860px;transform:translate3d(0,calc(var(--sy,0)*.12px),0)}
.status{display:inline-flex;align-items:center;gap:10px;padding:8px 16px;border:1px solid var(--line);border-radius:30px;font-size:.88rem;color:var(--cream);background:rgba(18,10,5,.6);backdrop-filter:blur(6px)}
.status i{width:9px;height:9px;border-radius:50%;background:#7bd389;box-shadow:0 0 0 0 rgba(123,211,137,.6);animation:ping 2s infinite}
.status.closed i{background:#c9693f;animation:none}
@keyframes ping{70%{box-shadow:0 0 0 10px rgba(123,211,137,0)}100%{box-shadow:0 0 0 0 rgba(123,211,137,0)}}
.hero h1{font-size:clamp(3rem,10.5vw,8.6rem);font-weight:800;line-height:.92;margin:26px 0 8px;letter-spacing:-.5px;text-shadow:0 10px 50px rgba(0,0,0,.7)}
.hero h1 small{display:block;font-family:var(--serif);font-style:italic;font-weight:400;font-size:.32em;color:var(--brass);letter-spacing:.5px;margin-bottom:.15em}
.hero h1 b{display:block;background:linear-gradient(180deg,var(--cream) 30%,var(--brass-hi) 70%,var(--brass-lo));-webkit-background-clip:text;background-clip:text;color:transparent}
.tagline{font-family:var(--serif);font-style:italic;font-size:clamp(1.1rem,2.2vw,1.55rem);color:var(--cream);margin:10px auto 34px;max-width:34ch;opacity:.92}
.hero-cta{display:flex;gap:14px;justify-content:center;flex-wrap:wrap}
.hero-meta{display:flex;gap:10px 26px;justify-content:center;flex-wrap:wrap;margin-top:34px;font-size:.92rem;color:var(--brass-hi)}
.hero-meta span{display:inline-flex;align-items:center;gap:8px}
.scroll-cue{position:absolute;left:50%;bottom:62px;transform:translateX(-50%);z-index:3;display:flex;flex-direction:column;align-items:center;gap:8px;font-size:.72rem;letter-spacing:2px;text-transform:uppercase;color:var(--brass-lo)}
.scroll-cue b{width:1px;height:38px;background:linear-gradient(var(--brass),transparent);animation:cue 2s ease-in-out infinite}
@keyframes cue{50%{opacity:.25}}
.marquee{position:relative;z-index:3;border-block:1px solid var(--line);background:rgba(10,5,2,.7);overflow:hidden;padding:15px 0}
.marquee-track{display:flex;width:max-content;animation:slide 38s linear infinite}
.marquee span{font-family:var(--serif);font-style:italic;font-size:1.05rem;color:var(--brass-hi);white-space:nowrap;padding:0 22px}
.marquee span::after{content:"✦";margin-left:44px;color:var(--brass-lo);font-style:normal;font-size:.8em}
@keyframes slide{to{transform:translateX(-50%)}}
@media(max-width:700px){.f3,.f4{display:none}.f1{left:-4%;top:12%;opacity:.7}.f2{right:-4%;top:9%;opacity:.7}.scroll-cue{display:none}}

/* ---------- 3D tour ---------- */
.tour{padding:0;height:205vh;background:linear-gradient(180deg,var(--bg),#0c0603 12%,#0c0603 88%,var(--bg))}
.tour-sticky{position:sticky;top:0;height:100vh;overflow:hidden;perspective:900px;perspective-origin:50% 42%}
.tour-world{position:absolute;inset:0;transform-style:preserve-3d;will-change:transform}
.plane{position:absolute;left:50%;top:50%;margin:0;width:clamp(170px,23vw,340px);transform-style:preserve-3d;will-change:opacity;opacity:0;border-radius:3px;overflow:hidden;box-shadow:0 50px 90px -20px #000,0 0 0 1px rgba(243,230,201,.16),0 0 60px -10px rgba(209,153,63,.35)}
.plane img{width:100%;height:auto;aspect-ratio:var(--ar);object-fit:cover}
.plane::after{content:"";position:absolute;inset:0;background:linear-gradient(170deg,rgba(209,153,63,.14),rgba(12,6,3,.28));pointer-events:none}
.dust{position:absolute;left:50%;top:50%;width:6px;height:6px;border-radius:50%;background:var(--brass-hi);box-shadow:0 0 14px 4px rgba(243,205,133,.55);will-change:opacity}
.tour-ui{position:absolute;inset:0;pointer-events:none;display:flex;flex-direction:column;justify-content:space-between;padding:96px var(--gut) 38px}
.tour-top{display:flex;justify-content:space-between;align-items:flex-start;gap:20px}
.tour-top .eyebrow{background:rgba(12,6,3,.6);padding:6px 14px 6px 0}
.tour-count{font-family:var(--serif);font-size:1rem;color:var(--brass);letter-spacing:2px}
.tour-caps{position:relative;height:clamp(150px,26vh,230px);display:flex;align-items:flex-end;justify-content:center}
.tour-caps::before{content:"";position:absolute;left:-10vw;right:-10vw;bottom:-60px;height:140%;background:radial-gradient(ellipse 60% 70% at 50% 100%,rgba(8,4,2,.92),transparent 75%);z-index:-1}
.cap{position:absolute;left:0;right:0;bottom:0;text-align:center;font-family:var(--serif);font-size:clamp(1.55rem,4vw,3.1rem);line-height:1.15;font-weight:400;font-style:italic;color:var(--cream);opacity:0;transform:translateY(26px);transition:opacity .22s,transform .22s;max-width:20em;margin:0 auto;text-shadow:0 4px 30px #000}
.cap em{color:var(--brass-hi)}
.cap.on{opacity:1;transform:none;transition:opacity .6s .25s,transform .6s .25s}
.tour-bar{height:2px;background:var(--line);margin-top:22px;position:relative}
.tour-bar i{position:absolute;left:0;top:0;bottom:0;width:100%;transform-origin:left;transform:scaleX(0);background:linear-gradient(90deg,var(--brass-lo),var(--brass-hi))}
.tour-hint{position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);z-index:4;text-align:center;width:150px;line-height:1.3;font-family:var(--serif);font-style:italic;color:var(--brass-hi);font-size:1.1rem;transition:opacity .5s;pointer-events:none;text-shadow:0 2px 20px #000}
.tour-hint b{display:block;font-size:.72rem;letter-spacing:3px;text-transform:uppercase;font-family:var(--sans);font-style:normal;color:var(--brass-lo);margin-top:8px}
@media(max-width:700px){.tour{height:190vh}.plane{width:clamp(150px,50vw,230px)}}

/* ---------- welkom ---------- */
.welkom{display:grid;grid-template-columns:1.05fr .95fr;gap:clamp(36px,7vw,100px);align-items:center}
.welkom-copy p{font-size:1rem;margin-bottom:.8em}
.welkom-copy p.lead{font-family:var(--serif);font-size:clamp(1.25rem,2.2vw,1.6rem);color:var(--cream);line-height:1.4}
.hand{font-family:var(--hand);font-size:1.75rem;color:var(--brass-hi);transform:rotate(-2deg);display:inline-block;margin:2px 0 0}
.prints{position:relative;aspect-ratio:1/.9;perspective:1100px}
.print{position:absolute;margin:0;background:#e9dcc0;padding:12px 12px 12px;box-shadow:0 40px 70px -20px #000;transition:transform .5s cubic-bezier(.2,.7,.2,1)}
.print img{width:100%;object-fit:cover;filter:sepia(.15) contrast(1.03)}
.print figcaption{margin-top:10px;text-align:center;font-family:var(--hand);font-size:1.25rem;color:#3a2410;line-height:1.1}
.print.p1{width:66%;left:0;top:0;transform:rotate(-4deg) rotateY(8deg)}
.print.p2{width:60%;right:0;bottom:0;transform:rotate(3.5deg) rotateY(-8deg)}
.prints:hover .p1{transform:rotate(-2deg) rotateY(0) translateY(-6px)}
.prints:hover .p2{transform:rotate(2deg) rotateY(0) translateY(6px)}
@media(max-width:860px){.welkom{grid-template-columns:1fr}.prints{order:-1}}

/* ---------- agenda ---------- */
.agenda{background:var(--bg2)}
.agenda-grid{display:grid;grid-template-columns:minmax(0,.7fr) minmax(0,1.3fr);gap:clamp(24px,5vw,64px);align-items:center}
.agenda-grid.solo{grid-template-columns:1fr}
.posters{display:flex;justify-content:center;perspective:1400px}
.poster{position:relative;width:min(100%,290px);margin:0;border-radius:3px;overflow:hidden;box-shadow:0 50px 90px -24px #000,0 0 0 1px rgba(243,230,201,.14);transition:transform .6s cubic-bezier(.2,.7,.2,1);transform-style:preserve-3d}
.poster img{width:100%;height:auto}
.poster.a{transform:rotateY(14deg) rotateZ(-2deg)}
.poster.b{transform:rotateY(-14deg) rotateZ(2deg);margin-left:-36px}
.posters:hover .poster.a{transform:rotateY(4deg) rotateZ(-1deg)}
.posters:hover .poster.b{transform:rotateY(-4deg) rotateZ(1deg)}
.events{list-style:none;margin:0;padding:0;border-top:1px solid var(--line)}
.event{display:grid;grid-template-columns:64px 1fr auto;gap:18px;align-items:center;padding:11px 4px;border-bottom:1px solid var(--line);transition:background .3s,transform .3s}
.event:hover{background:rgba(209,153,63,.06);transform:translateX(6px)}
.date{text-align:center;font-family:var(--serif);line-height:1}
.date b{display:block;font-size:1.9rem;font-weight:800;color:var(--brass-hi)}
.date span{display:block;font-size:.78rem;letter-spacing:2px;text-transform:uppercase;color:var(--muted);margin-top:4px}
.event h3{font-size:1.1rem;font-weight:600;margin-bottom:1px}
.event p{margin:0;font-size:.88rem}
.price{font-size:.82rem;font-weight:700;color:var(--ink);background:var(--brass);padding:6px 12px;border-radius:30px;white-space:nowrap}
.price.free{background:#7bd389}
.event.next{background:linear-gradient(90deg,rgba(209,153,63,.14),transparent)}
.event.next .nxt{display:inline-block;font-size:.68rem;letter-spacing:2px;text-transform:uppercase;color:var(--brass-hi)}
.note{font-size:.85rem;color:var(--brass-lo);margin:12px 0 0}
@media(max-width:900px){.agenda-grid{grid-template-columns:1fr}.event{grid-template-columns:52px 1fr}.event .price{grid-column:2;justify-self:start}.poster{width:min(100%,230px)}}

/* ---------- feest ---------- */
.feest{background:radial-gradient(ellipse 80% 70% at 75% 40%,#4a1b10 0%,transparent 70%),linear-gradient(180deg,var(--bg),#1b0a05)}
.feest-grid{display:grid;grid-template-columns:1.1fr .9fr;gap:clamp(30px,7vw,100px);align-items:center}
.big-num{font-family:var(--serif);font-weight:800;line-height:.9;font-size:clamp(3.2rem,8vw,5.6rem);background:linear-gradient(180deg,var(--brass-hi),var(--brass-lo));-webkit-background-clip:text;background-clip:text;color:transparent;margin:6px 0 6px}
.big-num small{font-size:.3em;font-weight:400;font-style:italic;-webkit-text-fill-color:var(--cream);margin-left:10px}
.pull{border-left:2px solid var(--brass);padding-left:18px;margin:14px 0;font-family:var(--serif);font-style:italic;font-size:clamp(1.1rem,2vw,1.4rem);line-height:1.35;color:var(--cream);max-width:30ch}
.feest-poster{perspective:1200px;max-width:380px;justify-self:center}
.feest-poster figure{margin:0;transform:rotateY(-14deg) rotateX(3deg);transition:transform .7s cubic-bezier(.2,.7,.2,1);box-shadow:40px 50px 90px -20px #000,0 0 0 1px rgba(243,230,201,.15);border-radius:3px;overflow:hidden}
.feest-poster:hover figure{transform:rotateY(-3deg) rotateX(0)}
@media(max-width:900px){.feest-grid{grid-template-columns:1fr}.feest-poster{max-width:230px;margin:0 auto}}

/* ---------- sport, biljart & darten ---------- */
.sport{background:var(--bg2)}
.duo{display:grid;grid-template-columns:1fr 1fr;gap:clamp(24px,5vw,72px);align-items:start}
.duo h2.big{font-size:clamp(1.6rem,3vw,2.3rem)}
.biljart-col{display:grid;grid-template-columns:minmax(0,170px) 1fr;column-gap:20px;align-items:start}
.biljart-col>.eyebrow,.biljart-col>h2{grid-column:1/-1}
.biljart-col>.eyebrow{justify-self:start}
.biljart-poster{perspective:900px;grid-row:3/5}
.biljart-poster figure{margin:0;border-radius:3px;overflow:hidden;box-shadow:-20px 30px 50px -20px #000,0 0 0 1px var(--line);transform:rotateY(14deg) rotateX(2deg);transition:transform .7s cubic-bezier(.2,.7,.2,1)}
.biljart-poster:hover figure{transform:rotateY(2deg) rotateX(0)}
@media(max-width:900px){.duo{grid-template-columns:1fr;gap:34px}}
@media(max-width:480px){.biljart-col{grid-template-columns:minmax(0,120px) 1fr;column-gap:14px}}

/* ---------- drankjes ---------- */
.drank-grid{display:grid;grid-template-columns:.8fr 1.2fr;gap:clamp(30px,7vw,100px);align-items:center}
.glass{perspective:1100px;max-width:190px;margin:0 auto}
.glass figure{margin:0;border-radius:3px;overflow:hidden;box-shadow:0 60px 90px -20px #000,0 0 0 1px var(--line);transform:rotateY(12deg) rotateZ(2deg);transition:transform .7s cubic-bezier(.2,.7,.2,1)}
.glass:hover figure{transform:rotateY(0) rotateZ(0) scale(1.02)}
.menu-list{list-style:none;margin:0 0 18px;padding:0;border-top:1px solid var(--line)}
.menu-list li{display:grid;grid-template-columns:auto 1fr;gap:2px 18px;padding:9px 0;border-bottom:1px solid var(--line);align-items:baseline}
.menu-list h3{font-size:1.1rem}
.menu-list p{margin:0;font-size:.9rem;grid-column:2}
.menu-list .k{font-family:var(--serif);font-style:italic;color:var(--brass);min-width:3.6em}
.bierkaart{position:relative;perspective:1000px}
.bk{position:relative;border-radius:14px;padding:18px 24px;background:linear-gradient(135deg,#3a2410 0%,#5a3a17 45%,#2c1a0a 100%);border:1px solid var(--brass-lo);box-shadow:0 40px 70px -24px #000,inset 0 0 0 1px rgba(243,205,133,.18);overflow:hidden;transform:rotateX(6deg) rotateY(-6deg);transition:transform .6s cubic-bezier(.2,.7,.2,1);max-width:560px}
.bk:hover{transform:rotateX(0) rotateY(0) translateY(-4px)}
.bk::after{content:"";position:absolute;top:-60%;left:-40%;width:50%;height:220%;background:linear-gradient(90deg,transparent,rgba(255,255,255,.14),transparent);transform:rotate(18deg);animation:shine 5s ease-in-out infinite}
@keyframes shine{0%,55%{left:-60%}100%{left:130%}}
.bk .lbl{font-size:.74rem;letter-spacing:3px;text-transform:uppercase;color:var(--brass-hi)}
.bk .eq{display:flex;align-items:baseline;gap:12px;font-family:var(--serif);margin:4px 0 6px}
.bk .eq b{font-size:2rem;font-weight:800;color:var(--cream)}
.bk .eq i{color:var(--brass);font-size:1.6rem}
.bk .eq u{text-decoration:none;font-size:2.5rem;font-weight:800;color:var(--brass-hi)}
.bk p{margin:0;color:var(--cream);opacity:.85;font-size:.95rem}
@media(max-width:900px){.drank-grid{grid-template-columns:1fr}.glass{max-width:150px}}

/* ---------- biljart ---------- */
.biljart{background:linear-gradient(180deg,var(--bg),#0f1a12 120%)}
.biljart-grid{display:grid;grid-template-columns:.8fr 1.2fr;gap:clamp(30px,7vw,100px);align-items:center}
.biljart-poster{perspective:1200px;max-width:360px;margin:0 auto}
.biljart-poster figure{margin:0;border-radius:3px;overflow:hidden;box-shadow:-40px 50px 90px -20px #000,0 0 0 1px var(--line);transform:rotateY(14deg) rotateX(2deg);transition:transform .7s cubic-bezier(.2,.7,.2,1)}
.biljart-poster:hover figure{transform:rotateY(2deg) rotateX(0)}
@media(max-width:900px){.biljart-grid{grid-template-columns:1fr}.biljart-poster{max-width:250px}}

/* ---------- reviews ---------- */
.rev-head{display:flex;align-items:flex-end;justify-content:space-between;gap:30px;flex-wrap:wrap;margin-bottom:20px}
.score{display:flex;align-items:center;gap:20px}
.score b{font-family:var(--serif);font-size:clamp(2.8rem,6vw,4.2rem);font-weight:800;line-height:.9;color:var(--brass-hi)}
.stars{color:var(--brass);letter-spacing:4px;font-size:1.3rem}
.score span{display:block;font-size:.9rem;color:var(--muted)}
.rev-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:18px;perspective:1300px}
.rev{background:var(--panel);border:1px solid var(--line);padding:18px 20px;border-radius:2px;transform-style:preserve-3d;transition:transform .5s cubic-bezier(.2,.7,.2,1),border-color .3s,box-shadow .5s;gap:12px;display:flex;flex-direction:column;justify-content:space-between}
.rev:hover{transform:translateY(-8px) rotateX(4deg);border-color:var(--brass-lo);box-shadow:0 30px 50px -20px #000}
.rev q{quotes:"“" "”";font-family:var(--serif);font-style:italic;font-size:1rem;line-height:1.4;color:var(--cream)}
.rev cite{display:block;margin-top:0;font-style:normal;font-size:.8rem;color:var(--brass);letter-spacing:.5px}
@media(max-width:1000px){.rev-grid{grid-template-columns:1fr 1fr}}

/* ---------- contact (in het reserveer-blok) ---------- */
.hours{width:100%;border-collapse:collapse;margin:0 0 14px}
.hours td{padding:7px 0;border-bottom:1px solid var(--line);font-size:.95rem}
.hours td:first-child{font-family:var(--serif);color:var(--cream)}
.hours td:last-child{text-align:right;color:var(--muted)}
.hours tr.closed td:last-child{font-style:italic;color:var(--brass-lo)}
.hours tr.today td{color:var(--brass-hi)}
.hours tr.today td:first-child::after{content:"vandaag";margin-left:10px;font-family:var(--sans);font-size:.66rem;letter-spacing:2px;text-transform:uppercase;color:var(--ink);background:var(--brass);padding:3px 8px;border-radius:20px;vertical-align:2px}
.addr{font-style:normal;font-size:1rem;color:var(--cream);line-height:1.5;margin:0 0 14px}
.map{border:1px solid var(--line);border-radius:3px;overflow:hidden;height:170px;margin:0 0 14px;background:var(--panel)}
.map iframe{width:100%;height:100%;border:0;filter:invert(.92) hue-rotate(180deg) saturate(.5) sepia(.35) brightness(.9) contrast(.95)}
.social{display:flex;align-items:center;gap:10px;flex-wrap:wrap;margin-top:14px;padding-top:14px;border-top:1px solid var(--line);font-size:.9rem;color:var(--muted)}
.social .btn{padding:8px 16px;font-size:.85rem}
.btns{display:flex;gap:10px;flex-wrap:wrap}

/* ---------- footer ---------- */
footer{border-top:1px solid var(--line);padding:30px 0 22px;background:var(--ink)}
.foot{display:flex;justify-content:space-between;align-items:flex-start;gap:30px;flex-wrap:wrap}
.foot p{margin:0 0 4px;font-size:.92rem}
.foot .brand{margin-bottom:12px}
.foot-end{margin-top:18px;padding-top:14px;border-top:1px solid var(--line);font-size:.8rem;color:var(--brass-lo);display:flex;justify-content:space-between;gap:12px;flex-wrap:wrap}

/* ---------- reveal ---------- */
.reveal{opacity:0;transform:translate3d(0,40px,0) perspective(900px) rotateX(-10deg);transform-origin:50% 100%;transition:opacity .9s ease,transform .9s cubic-bezier(.2,.7,.2,1)}
.reveal.in{opacity:1;transform:none}
.reveal.d1{transition-delay:.1s}.reveal.d2{transition-delay:.2s}.reveal.d3{transition-delay:.3s}

/* ---------- reserveren ---------- */
.reserveren{background:var(--bg2)}
.res-intro{margin:0 0 20px}
.res-grid{display:grid;grid-template-columns:1.15fr .85fr;gap:clamp(20px,4vw,48px);align-items:start}
.card{background:var(--panel);border:1px solid var(--line);padding:clamp(18px,3vw,30px);border-radius:3px;box-shadow:0 40px 80px -40px #000}
.side h3{font-size:1.25rem;margin-bottom:12px}
fieldset{border:0;padding:0;margin:0 0 16px}
legend,.lab{font-size:.74rem;letter-spacing:2px;text-transform:uppercase;color:var(--brass);margin-bottom:6px;display:block;padding:0}
.types{position:relative;display:grid;grid-template-columns:repeat(4,1fr);gap:8px}
.types input{position:absolute;opacity:0;pointer-events:none}
.types label{display:block;padding:10px 8px;border:1px solid var(--line);border-radius:2px;cursor:pointer;font-weight:700;font-size:.88rem;text-align:center;color:var(--cream);transition:border-color .2s,background .2s}
.types input:checked+label{border-color:var(--brass);background:rgba(209,153,63,.14);color:var(--brass-hi)}
.types input:focus-visible+label{outline:2px solid var(--brass-hi);outline-offset:2px}
.row{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:12px}
.row.r3{grid-template-columns:1.2fr 1fr 1.1fr}
.field{display:flex;flex-direction:column;min-width:0}
.field input,.field select{background:var(--bg);color:var(--cream);border:1px solid var(--line);border-radius:2px;padding:11px 12px;font:inherit;font-size:1rem;width:100%;color-scheme:dark}
.field input:focus,.field select:focus{border-color:var(--brass)}
.stepper{display:flex;border:1px solid var(--line);border-radius:2px;background:var(--bg)}
.stepper button{width:40px;background:none;border:0;color:var(--brass-hi);font-size:1.3rem;cursor:pointer}
.stepper button:hover{background:rgba(209,153,63,.12)}
.stepper input{border:0;text-align:center;-moz-appearance:textfield;padding:11px 0;background:none}
.stepper input::-webkit-outer-spin-button,.stepper input::-webkit-inner-spin-button{-webkit-appearance:none}
.err{color:#ff9d7a;font-size:.88rem;min-height:1.2em;margin:0 0 8px}
.hint{font-size:.82rem;color:var(--muted);margin:10px 0 0}
.done{display:none;margin-top:14px;padding:16px 18px;border:1px solid var(--brass);background:rgba(209,153,63,.08)}
.done.on{display:block}
.done p{color:var(--cream);margin-bottom:10px}
.done .acts{display:flex;gap:10px;flex-wrap:wrap}
@media(max-width:900px){.res-grid{grid-template-columns:1fr}}
@media(max-width:560px){.row.r3{grid-template-columns:1fr 1fr}.row.r3 .field:last-child{grid-column:1/-1}.row{grid-template-columns:1fr}.types{grid-template-columns:1fr 1fr}.map{display:none}}

@media(max-width:700px){
  .foot{flex-direction:column;gap:14px}
  .foot>div:last-child{display:none}
  .foot-end span:last-child{display:none}
  .glass{display:none}
  .feest-poster{max-width:200px}
  .poster{width:min(100%,180px)}
  .rev-grid{display:grid;grid-auto-flow:column;grid-auto-columns:82%;grid-template-columns:none;overflow-x:auto;scroll-snap-type:x mandatory;gap:12px;padding-bottom:6px;margin-right:calc(var(--gut)*-1);padding-right:var(--gut);-webkit-overflow-scrolling:touch}
  .rev{scroll-snap-align:start}
  .hero-stage{padding-top:96px;padding-bottom:64px}
  .welkom-copy p.lead{font-size:1.15rem}
  .prints{aspect-ratio:1/.78}
  .print{padding:8px 8px 8px}
  .print figcaption{font-size:1rem;margin-top:6px}
  .big-num{font-size:3.4rem}
}
/* ---------- reduced motion ---------- */
@media (prefers-reduced-motion:reduce){
  html{scroll-behavior:auto}
  *,*::before,*::after{animation:none!important;transition:none!important}
  .reveal{opacity:1;transform:none}
  .tour{height:auto;padding:90px 0}
  .tour-sticky{position:static;height:auto;perspective:none;overflow:visible}
  .tour-world{position:static;display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:16px;padding:0 var(--gut);max-width:var(--maxw);margin:0 auto;transform:none!important}
  .plane{position:static;width:auto;opacity:1!important;transform:none!important}
  .tour-ui,.dust,.tour-hint{display:none}
}
</style>
<script type="application/ld+json">{"@context": "https://schema.org", "@type": "BarOrPub", "name": "Café de Nachtegaal", "description": "Het donkerbruinste café van Uden: Zachte Premium van de tap, biljarten, darten, live muziek, sport op groot scherm en feesten tot 120 personen.", "telephone": "+31630862200", "priceRange": "€€", "address": {"@type": "PostalAddress", "streetAddress": "Elisabethstraat 25", "postalCode": "5402 VD", "addressLocality": "Uden", "addressCountry": "NL"}, "aggregateRating": {"@type": "AggregateRating", "ratingValue": "4.7", "reviewCount": "77"}, "openingHoursSpecification": [{"@type": "OpeningHoursSpecification", "dayOfWeek": "Monday", "opens": "13:00", "closes": "22:00"}, {"@type": "OpeningHoursSpecification", "dayOfWeek": ["Thursday", "Friday"], "opens": "15:00", "closes": "01:00"}, {"@type": "OpeningHoursSpecification", "dayOfWeek": "Saturday", "opens": "13:00", "closes": "01:00"}, {"@type": "OpeningHoursSpecification", "dayOfWeek": "Sunday", "opens": "13:00", "closes": "00:00"}]}</script>
<noscript><style>.reveal{opacity:1!important;transform:none!important}.tour{height:auto}.tour-sticky{position:static;height:auto}.tour-world{position:static;display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:12px;padding:0 var(--gut)}.plane{position:static;width:auto;opacity:1;transform:none!important}.tour-ui,.dust,.tour-hint{display:none}</style></noscript>
</head>
<body>
<div class="grain" aria-hidden="true"></div>

<!-- ================= NAV ================= -->
<header class="nav" id="nav">
  <a class="brand" href="#top" aria-label="Café de Nachtegaal — naar boven">
    <svg viewBox="0 0 48 40" aria-hidden="true"><path fill="currentColor" d="M3 33 15 25C14 14 22 7 31 9c4 1 6 4 6 8l9 2-9 2c0 10-9 17-20 15L7 39z"/><circle cx="32" cy="14" r="1.4" fill="#120a05"/></svg>
    <span>Café de Nachtegaal</span>
  </a>
  <nav class="nav-links" id="navlinks" aria-label="Hoofdmenu">
    <a href="#rondleiding">Rondleiding</a>
    <a href="#agenda">Agenda</a>
    <a href="#feesten">Feesten</a>
    <a href="#drankjes">Drankjes</a>
    <a href="#reviews">Reviews</a>
    <a href="#reserveren">Contact</a>
    <a class="btn solid" href="#reserveren">Reserveren</a>
  </nav>
  <a class="btn solid" href="#reserveren">Reserveren</a>
  <button class="burger" id="burger" aria-expanded="false" aria-controls="navlinks">Menu</button>
</header>

<!-- ======================================================= -->
<!-- ===================== HOME VIEW ======================= -->
<!-- ======================================================= -->
<main id="view-home">

<!-- HERO -->
<section class="hero" id="top" style="padding:0">
  <div class="hero-stage" id="heroStage">
    <div class="hero-glow"></div>
    <div class="bokeh" id="bokeh" aria-hidden="true"></div>
    <figure class="float f1" aria-hidden="true"><img src="images/bar_hoorn.jpg" alt=""></figure>
    <figure class="float f2" aria-hidden="true"><img src="images/bar_krukken.jpg" alt=""></figure>
    <figure class="float f3" aria-hidden="true"><img src="images/bar_hout.jpg" alt=""></figure>
    <figure class="float f4" aria-hidden="true"><img src="images/bar_glazen.jpg" alt=""></figure>
    <div class="hero-copy">
      <div class="status" id="status" role="status"><i></i><span>Openingstijden laden…</span></div>
      <h1><small>Café de</small><b>Nachtegaal</b></h1>
      <p class="tagline">Welkom in het donkerbruinste café van Uden.</p>
      <div class="hero-cta">
        <a class="btn solid" href="#reserveren">Reserveer een tafel</a>
        <a class="btn ghost" href="#agenda">Bekijk de agenda</a>
      </div>
      <div class="hero-meta">
        <span>★ 4,7 · 77 reviews op Google</span>
        <span>Elisabethstraat 25, Uden</span>
        <span><a href="tel:+31630862200" style="color:inherit;text-decoration:none">06-30862200</a></span>
      </div>
    </div>
    <div class="scroll-cue" aria-hidden="true"><span>scroll</span><b></b></div>
  </div>
  <div class="marquee" aria-hidden="true">
    <div class="marquee-track" id="marq"></div>
  </div>
</section>

<!-- 3D RONDLEIDING -->
<section class="tour" id="rondleiding" aria-label="Rondleiding door het café">
  <div class="tour-sticky" id="tourSticky">
    <div class="tour-world" id="tourWorld">
      <figure class="plane" data-i="0" data-x="-27" data-y="-6" data-r="16"><img src="images/bar_hoorn.jpg" alt="De bar met de koperen hoorn en de Casablanca-poster" style="--ar:855 / 1680"></figure>
      <figure class="plane" data-i="1" data-x="26" data-y="4" data-r="-16"><img src="images/bar_glazen.jpg" alt="De bar met hangende bierglazen en houten kasten" style="--ar:855 / 1299"></figure>
      <figure class="plane" data-i="2" data-x="-25" data-y="3" data-r="15"><img src="images/bar_krukken.jpg" alt="De bar met krukken en glas-in-lood lampen" style="--ar:855 / 1389"></figure>
      <figure class="plane" data-i="3" data-x="27" data-y="-5" data-r="-15"><img src="images/bar_hout.jpg" alt="Het gesneden houten barfront met kruk" style="--ar:837 / 1398"></figure>
      <figure class="plane" data-i="4" data-x="-26" data-y="-3" data-r="16"><img src="images/cowboy.jpg" alt="De zithoek met saloondeurtjes en houten beeld" style="--ar:855 / 1521"></figure>
      <figure class="plane" data-i="5" data-x="26" data-y="2" data-r="-16"><img src="images/bar_bel.jpg" alt="De bar in de avond met de grote bel" style="--ar:855 / 1830"></figure>
      <figure class="plane" data-i="6" data-x="-24" data-y="-2" data-r="14"><img src="images/taps.jpg" alt="De tapkranen op de bar" style="--ar:855 / 1281"></figure>
    </div>
    <div class="tour-hint" id="tourHint">Scroll en loop mee naar binnen<b>Rondleiding</b></div>
    <div class="tour-ui">
      <div class="tour-top"><span class="eyebrow">De rondleiding</span><span class="tour-count" id="tourCount">01 / 06</span></div>
      <div>
        <div class="tour-caps" id="tourCaps">
          <p class="cap">Welkom in het <em>donkerbruinste café</em> van Uden.</p>
          <p class="cap">Een plek waar de sfeer <em>warm</em> is, de drankjes <em>betaalbaar</em> zijn.</p>
          <p class="cap">Altijd tijd voor <em>gezelligheid</em>.</p>
          <p class="cap">Bij ons hoef je niks, <em>behalve jezelf zijn.</em></p>
          <p class="cap">Altijd plek voor een goed gesprek en een flinke dosis <em>Brabantse gezelligheid!</em></p>
          <p class="cap">Bij de Nachtegaal maken we er <em>samen iets moois</em> van!</p>
        </div>
        <div class="tour-bar"><i id="tourBar"></i></div>
      </div>
    </div>
  </div>
</section>

<!-- WELKOM -->
<section id="welkom">
  <div class="wrap welkom">
    <div class="welkom-copy">
      <span class="eyebrow reveal">Café de Nachtegaal</span>
      <h2 class="big reveal d1">Het donkerbruinste café <em>van Uden</em></h2>
      <p class="lead reveal d2">Een plek waar de sfeer warm is, de drankjes betaalbaar zijn en het altijd tijd is voor gezelligheid.</p>
      <p class="reveal d2">Schuif aan voor een koud tap-pilsje uit Duitsland, een goed glas wijn of gewoon een gezellige babbel. Bij ons hoef je niks, behalve jezelf zijn.</p>
      <p class="reveal d3">Kom je alleen of met vrienden? Er is altijd plek voor een goed gesprek en een flinke dosis Brabantse gezelligheid!</p>
      <p class="reveal d3">Wij houden ook wel van een feestje! Van live muziek en gezellige middagen, tot avonden waarbij het dak er bijna afgaat. Bij de Nachtegaal maken we er samen iets moois van!</p>
      <span class="hand reveal d3">Ook kunt u biljarten en darten in dit café.</span>
    </div>
    <div class="prints reveal d2">
      <figure class="print p1"><img src="images/duo.jpg" alt="Twee gasten proosten met bier aan de bar" style="aspect-ratio:855 / 573"><figcaption>Proost!</figcaption></figure>
      <figure class="print p2"><img src="images/team.jpg" alt="Groepsfoto achter de bar van Café de Nachtegaal" style="aspect-ratio:798 / 480"><figcaption>Café de Nachtegaal Uden<br>1 dec. 1995 – 2025</figcaption></figure>
    </div>
  </div>
</section>

<!-- AGENDA -->
<section class="agenda" id="agenda">
  <div class="wrap">
    <span class="eyebrow reveal">Agenda</span>
    <h2 class="big reveal d1">Wanneer gaat het <em>dak eraf?</em></h2>
    <p class="reveal d2" style="margin-bottom:22px">Hieronder zie je wie er komt optreden en welke sportwedstrijd we samen gaan kijken.</p>
    <div class="agenda-grid">
      <div class="poster-col reveal"><div class="posters" id="posters">
        <figure class="poster a" data-until="2026-10-25"><img src="images/poster_okt.jpg" alt="Poster Oktoberfest met Thorsten von Lippe Biesterfeld, zondag 25 oktober, aanvang 15.00 uur, kaarten € 15" style="aspect-ratio:837 / 882"></figure>
        <figure class="poster b" data-until="2026-10-17"><img src="images/poster_dave.jpg" alt="Poster Dave Brokken, zaterdag 17 oktober, gratis entree, aanvang 19.00 uur" style="aspect-ratio:852 / 1185"></figure>
      </div></div>
      <div>
        <ul class="events" id="events"></ul>
        <p class="note">Wil je weten wie er komt optreden of welke wedstrijd we kijken? Plaats je verzoek via social media en wij worden vrienden!</p>
      </div>
    </div>
  </div>
</section>

<!-- FEESTEN -->
<section class="feest" id="feesten">
  <div class="wrap feest-grid">
    <div>
      <span class="eyebrow reveal">Feesten &amp; partijen</span>
      <h2 class="big reveal d1">Heb je een reden <em>voor een feestje?</em></h2>
      <div class="big-num reveal d1">120<small>personen</small></div>
      <p class="reveal d2" style="font-size:1.15rem;color:var(--cream)">Wij de perfecte plek!! Ruimte voor 120 personen!</p>
      <p class="reveal d2">Een verjaardag, jubileum, personeelsfeest of gewoon zin om het leven te vieren?</p>
      <p class="reveal d3">Bij café de Nachtegaal in Uden maken we er samen een gezellig feest van!! Een sfeervol donkerbruin café, betaalbare drankjes en een hele vlotte bediening: alle ingrediënten voor een zeer geslaagde middag of avond.</p>
      <blockquote class="pull reveal d3" style="margin-left:0">Jij geniet van je gasten, wij zorgen voor de gezelligheid in het glas!</blockquote>
      <div class="hero-cta reveal d3" style="justify-content:flex-start">
        <a class="btn solid" href="#reserveren" data-type="feest">Plan je feest</a>
        <a class="btn ghost" href="tel:+31630862200">Bel 06-30862200</a>
      </div>
      <p class="note">Voor verdere info neem contact op met 06-30862200 of loop even binnen…</p>
    </div>
    <div class="feest-poster reveal d2"><figure><img src="images/poster_feest.jpg" alt="Poster: stop met zoeken, ruimte voor tot 120 personen, € 27,50 alle drankjes" style="aspect-ratio:855 / 1068"></figure></div>
  </div>
</section>

<!-- DRANKJES -->
<section id="drankjes">
  <div class="wrap drank-grid">
    <div class="glass reveal"><figure><img src="images/bier.jpg" alt="Een vers getapt glas Zachte Premium met een dikke schuimkraag"></figure></div>
    <div>
      <span class="eyebrow reveal">Onze drankjes</span>
      <h2 class="big reveal d1">Een Duits engeltje <em>op je tong</em></h2>
      <ul class="menu-list reveal d2">
        <li><span class="k">Van de tap</span><h3>Zachte Premium</h3><p>Een Duits engeltje op je tong.</p></li>
        <li><span class="k">Fris</span><h3>Frisdranken en sapjes</h3></li>
        <li><span class="k">Op fles</span><h3>Speciaalbieren</h3><p>Zoals Hoegaarden en Hertog Jan 0.0, Radler 2.0 en Radler 0.0, Liefmans Rosé en Desperados, donker bier en meer.</p></li>
        <li><span class="k">Mixen</span><h3>Diverse alcoholische dranken</h3><p>Om te mixen.</p></li>
      </ul>
      <div class="bierkaart reveal d3">
        <div class="bk">
          <span class="lbl">De bierkaart</span>
          <div class="eq"><b>€ 50</b><i>→</i><u>€ 55</u></div>
          <p>Wist u dat u bij ons ook bierkaarten kunt kopen? U betaalt voor zo’n kaart € 50,00 (onbeperkt geldig) en wij schenken u alle drankjes ter waarde van € 55,00.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- SPORT, BILJART & DARTEN -->
<section class="sport" id="sport">
  <div class="wrap duo">
    <div>
      <span class="eyebrow reveal">Sportwedstrijden</span>
      <h2 class="big reveal d1">Samen kijken, <em>samen juichen!</em></h2>
      <p class="reveal d2">Van spannende Formule 1 races en mooie voetbalwedstrijden tot boksen en andere sportkrakers… Bij café de Nachtegaal beleef je sport op een groot scherm.</p>
      <p class="reveal d2">Met een koud biertje en een flinke dosis Brabantse gezelligheid zit je bij ons goed. Hier mag je juichen, en natuurlijk vertellen hoe jij het veel beter had gedaan!!!</p>
      <p class="reveal d3" style="color:var(--cream)">Weten welke sportwedstrijd we samen gaan kijken? Plaats je verzoek en wij worden vrienden!</p>
    </div>
    <div class="biljart-col" id="biljart">
      <span class="eyebrow reveal">Biljarten &amp; darten</span>
      <h2 class="big reveal d1">Ook kunt u <em>biljarten en darten</em> in dit café</h2>
      <div class="biljart-poster reveal d2"><figure><img src="images/poster_biljart.jpg" alt="Poster Biljartvereniging K.O.T. in Café de Nachtegaal: nieuwe leden van harte welkom, wij spelen op vrijdagavond" style="aspect-ratio:1101 / 1099"></figure></div>
      <div>
        <p class="reveal d2">Het nieuwe seizoen met onderlinge competitie van Biljartvereniging K.O.T. gaat weer van start. Sportief, gezellig en voor iedereen: nieuwe leden zijn van harte welkom! Er wordt gespeeld op vrijdagavond.</p>
        <p class="reveal d3" style="color:var(--cream)">Opgeven of meer info? Bel het nummer op de poster.</p>
      </div>
    </div>
  </div>
</section>

<!-- REVIEWS -->
<section id="reviews">
  <div class="wrap">
    <div class="rev-head">
      <div>
        <span class="eyebrow reveal">Reviews van Google</span>
        <h2 class="big reveal d1" style="margin-bottom:0">Wat gasten <em>zeggen</em></h2>
      </div>
      <div class="score reveal d2"><b>4,7</b><div><div class="stars" aria-label="4,7 van de 5 sterren">★★★★★</div><span>77 reviews op Google</span></div></div>
    </div>
    <div class="rev-grid">
      <div class="rev reveal"><q>Enige plek in Uden met betaalbaar bier</q><cite>Google review</cite></div>
      <div class="rev reveal d1"><q>Gezellige avond gehad, snelle bediening, leuke muziek gehad van Dave Brokken.</q><cite>Google review</cite></div>
      <div class="rev reveal d2"><q>Super een horeca ondernemer die zijn gasten centraal stelt.</q><cite>Google review</cite></div>
      <div class="rev reveal d3"><q>Super leuke avond gehad in dit super gezellige cafe. Echt een aanrader!</q><cite>Google review</cite></div>
    </div>
    <p class="reveal" style="margin:20px 0 0"><a class="btn ghost" href="https://www.google.com/maps/search/?api=1&query=Caf%C3%A9+de+Nachtegaal+Elisabethstraat+25+Uden" target="_blank" rel="noopener">Lees alle reviews op Google</a></p>
  </div>
</section>

<!-- RESERVEREN & CONTACT -->
<section class="reserveren" id="reserveren">
  <div class="wrap">
    <span class="eyebrow reveal">Reserveren &amp; contact</span>
    <h2 class="big reveal d1">Schuif aan <em>bij de Nachtegaal</em></h2>
    <p class="res-intro reveal d2">Een tafel, een feest of mosselen: laat het ons weten, bel gerust of loop even binnen.</p>
    <div class="res-grid">
      <form class="card" id="resForm" novalidate>
        <fieldset>
          <legend>Waar gaat het om?</legend>
          <div class="types" id="types">
            <input type="radio" name="type" id="t1" value="tafel" checked><label for="t1">Tafel</label>
            <input type="radio" name="type" id="t2" value="feest"><label for="t2">Feest of groep</label>
            <input type="radio" name="type" id="t3" value="mosselen"><label for="t3">Mosselen 1 nov</label>
            <input type="radio" name="type" id="t4" value="vraag"><label for="t4">Vraag stellen</label>
          </div>
        </fieldset>
        <div class="row r3">
          <div class="field"><label class="lab" for="fDate">Datum</label><input type="date" id="fDate" required></div>
          <div class="field"><label class="lab" for="fTime">Tijd</label><select id="fTime" required></select></div>
          <div class="field">
            <span class="lab" id="lblPers">Personen</span>
            <div class="stepper" role="group" aria-labelledby="lblPers">
              <button type="button" id="minus" aria-label="Eén persoon minder">−</button>
              <input type="number" id="fPers" min="1" max="120" value="2" inputmode="numeric" aria-labelledby="lblPers">
              <button type="button" id="plus" aria-label="Eén persoon meer">+</button>
            </div>
          </div>
        </div>
        <div class="err" id="errDate" role="alert" aria-live="polite"></div>
        <div class="row">
          <div class="field"><label class="lab" for="fName">Naam</label><input type="text" id="fName" autocomplete="name" required placeholder="Voor- en achternaam"></div>
          <div class="field"><label class="lab" for="fTel">Telefoonnummer</label><input type="tel" id="fTel" autocomplete="tel" required placeholder="06-12345678"></div>
        </div>
        <div class="field" style="margin-bottom:12px"><label class="lab" for="fNote">Opmerking (niet verplicht)</label><input type="text" id="fNote" placeholder="Bijvoorbeeld een verjaardag of kinderstoel"></div>
        <div class="err" id="errForm" role="alert" aria-live="polite"></div>
        <button class="btn solid" type="submit" id="send"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M20.5 3.5A11.9 11.9 0 0 0 .1 11.9c0 2.1.6 4.2 1.6 6L0 24l6.3-1.6a11.9 11.9 0 0 0 5.7 1.5h0A11.9 11.9 0 0 0 20.5 3.5zM12 21.8a9.9 9.9 0 0 1-5-1.4l-.4-.2-3.7 1 1-3.6-.2-.4A9.9 9.9 0 1 1 12 21.8zm5.4-7.4c-.3-.1-1.8-.9-2-1s-.5-.1-.7.1-.8 1-1 1.2-.4.2-.7.1a8 8 0 0 1-4-3.5c-.3-.5.3-.5.9-1.6.1-.2 0-.4 0-.5l-1-2.3c-.2-.6-.5-.5-.7-.5h-.6a1.2 1.2 0 0 0-.9.4 3.7 3.7 0 0 0-1.1 2.7 6.4 6.4 0 0 0 1.4 3.4 14.6 14.6 0 0 0 5.6 5c2 .8 2.8.9 3.8.7a3.2 3.2 0 0 0 2.1-1.5 2.6 2.6 0 0 0 .2-1.5c-.1-.1-.3-.2-.6-.3z"/></svg>Verstuur via WhatsApp</button>
        <p class="hint">Je aanvraag wordt klaargezet in WhatsApp. Je reservering is definitief zodra het café hem bevestigt.</p>
        <div class="done" id="done" role="status">
          <p><strong id="doneTitle">Bedankt!</strong> WhatsApp is geopend met je aanvraag. Druk daar op verzenden, dan ontvangt het café je reservering en bevestigt die zo snel mogelijk.</p>
          <div class="acts"><a class="btn solid" id="waLink" href="https://wa.me/31630862200" target="_blank" rel="noopener">Open WhatsApp</a><a class="btn ghost" href="tel:+31630862200">Bel 06-30862200</a></div>
        </div>
      </form>
      <aside class="side">
        <div class="card">
          <h3>Bel of loop binnen</h3>
          <address class="addr"><strong style="font-family:var(--serif);font-size:1.1rem;font-weight:600">Café de Nachtegaal</strong><br>Elisabethstraat 25, 5402 VD Uden</address>
          <div class="btns" style="margin-bottom:16px"><a class="btn solid" href="tel:+31630862200">06-30862200</a><a class="btn ghost" href="https://www.google.com/maps/dir/?api=1&destination=Caf%C3%A9+de+Nachtegaal+Elisabethstraat+25+Uden" target="_blank" rel="noopener">Plan je route</a></div>
          <table class="hours" id="hoursTable" aria-label="Openingstijden"></table>
          <div class="map"><iframe title="Kaart van Café de Nachtegaal, Elisabethstraat 25 Uden" loading="lazy" referrerpolicy="no-referrer-when-downgrade" src="https://www.google.com/maps?q=Caf%C3%A9+de+Nachtegaal+Elisabethstraat+25+Uden&output=embed"></iframe></div>
          <div class="social"><span>Mis geen feestje, volg ons op</span><a class="btn ghost" href="https://www.facebook.com/search/top?q=Caf%C3%A9%20de%20Nachtegaal%20Uden" target="_blank" rel="noopener">Facebook</a><a class="btn ghost" href="https://www.instagram.com/explore/search/keyword/?q=Caf%C3%A9%20de%20Nachtegaal%20Uden" target="_blank" rel="noopener">Instagram</a></div>
        </div>
      </aside>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="wrap">
    <div class="foot">
      <div>
        <a class="brand" href="#top"><svg viewBox="0 0 48 40" aria-hidden="true"><path fill="currentColor" d="M3 33 15 25C14 14 22 7 31 9c4 1 6 4 6 8l9 2-9 2c0 10-9 17-20 15L7 39z"/><circle cx="32" cy="14" r="1.4" fill="#0c0603"/></svg><span>Café de Nachtegaal</span></a>
        <p>Elisabethstraat 25 · 5402 VD Uden</p>
        <p><a href="tel:+31630862200">06-30862200</a></p>
      </div>
      <div>
        <p style="color:var(--cream)">Het donkerbruinste café van Uden.</p>
        <p>Volg ons op Facebook en Instagram</p>
      </div>
      <div><a class="btn solid" href="#reserveren">Reserveren</a></div>
    </div>
    <div class="foot-end"><span>© <span id="yr"></span> Café de Nachtegaal, Uden</span><span>Zachte Premium van de tap · biljarten · darten · feesten tot 120 personen</span></div>
  </div>
</footer>

<script>
(function(){
'use strict';
const $=(s,r=document)=>r.querySelector(s), $$=(s,r=document)=>Array.from(r.querySelectorAll(s));
const reduced=matchMedia('(prefers-reduced-motion: reduce)').matches;
const clamp=(v,a,b)=>Math.min(Math.max(v,a),b);

/* ----- images ----- */
$('#yr').textContent=new Date().getFullYear();

/* ----- opening hours (Europe/Amsterdam) ----- */
const DAYS=['zondag','maandag','dinsdag','woensdag','donderdag','vrijdag','zaterdag'];
const HOURS={0:[13,24],1:[13,22],2:null,3:null,4:[15,25],5:[15,25],6:[13,25]};
const hh=h=>String(h%24).padStart(2,'0')+'.00';
function nowAms(){
  const f=new Intl.DateTimeFormat('en-GB',{timeZone:'Europe/Amsterdam',weekday:'short',hour:'2-digit',minute:'2-digit',hourCycle:'h23'}).formatToParts(new Date());
  const g=t=>f.find(p=>p.type===t).value;
  const wd=['Sun','Mon','Tue','Wed','Thu','Fri','Sat'].indexOf(g('weekday'));
  return {wd,min:(+g('hour'))*60+(+g('minute'))};
}
function openState(){
  const {wd,min}=nowAms();
  const t=HOURS[wd], y=HOURS[(wd+6)%7];
  if(y&&y[1]>24&&min<(y[1]-24)*60) return {open:true,until:hh(y[1])};
  if(t&&min>=t[0]*60&&min<t[1]*60) return {open:true,until:hh(t[1])};
  for(let i=0;i<=7;i++){
    const d=(wd+i)%7, h=HOURS[d]; if(!h) continue;
    if(i===0&&min>=h[0]*60) continue;
    return {open:false,next:i===0?'vandaag':(i===1?'morgen':DAYS[d]),at:hh(h[0])};
  }
  return {open:false};
}
function paintStatus(){
  const s=openState(), el=$('#status'); if(!el) return;
  el.classList.toggle('closed',!s.open);
  el.querySelector('span').textContent=s.open?`Nu open · tot ${s.until} uur`:`Gesloten · open ${s.next} om ${s.at} uur`;
}
paintStatus(); setInterval(paintStatus,60000);
function paintHours(sel){
  const t=$(sel); if(!t) return; const today=nowAms().wd;
  t.innerHTML=[1,2,3,4,5,6,0].map(d=>{const h=HOURS[d];
    return `<tr class="${h?'':'closed'} ${d===today?'today':''}"><td>${DAYS[d][0].toUpperCase()+DAYS[d].slice(1)}</td><td>${h?`${hh(h[0])} tot ${hh(h[1])} uur`:'Gesloten'}</td></tr>`}).join('');
}
paintHours('#hoursTable'); paintHours('#hoursTable2');

/* ----- marquee ----- */
(function(){
  const items=['Zachte Premium van de tap','Biljarten','Darten','Live muziek','Sport op groot scherm','Feesten tot 120 personen','Brabantse gezelligheid'];
  const html=items.map(t=>`<span>${t}</span>`).join('');
  $('#marq').innerHTML=html+html+html+html;
})();

/* ----- bokeh ----- */
(function(){
  if(reduced) return; const b=$('#bokeh'); let h='';
  for(let i=0;i<22;i++){const s=8+Math.random()*34;
    h+=`<i style="left:${Math.random()*100}%;bottom:${-10+Math.random()*20}%;width:${s}px;height:${s}px;animation-duration:${14+Math.random()*22}s;animation-delay:-${Math.random()*30}s;opacity:${.3+Math.random()*.6}"></i>`;}
  b.innerHTML=h;
})();

/* ----- nav ----- */
const nav=$('#nav'), burger=$('#burger');
burger.addEventListener('click',()=>{const o=nav.classList.toggle('open');burger.setAttribute('aria-expanded',o);burger.textContent=o?'Sluiten':'Menu';document.body.style.overflow=o?'hidden':'';});
$$('#navlinks a').forEach(a=>a.addEventListener('click',()=>{nav.classList.remove('open');burger.setAttribute('aria-expanded',false);burger.textContent='Menu';document.body.style.overflow='';}));

/* ----- anchor links: altijd soepel naar de sectie, ook zonder hash-routing ----- */
function goTo(id,type){
  const t=document.getElementById(id); if(!t) return;
  if(type){const r=$(`input[name=type][value="${type}"]`); if(r){r.checked=true; onType();}}
  const y=t.getBoundingClientRect().top+scrollY-62;
  window.scrollTo({top:Math.max(0,y),behavior:reduced?'auto':'smooth'});
}
document.addEventListener('click',e=>{
  const a=e.target.closest('a[href^="#"]'); if(!a) return;
  const id=a.getAttribute('href').slice(1);
  if(id==='top'){e.preventDefault();window.scrollTo({top:0,behavior:reduced?'auto':'smooth'});return;}
  if(document.getElementById(id)){e.preventDefault();goTo(id,a.dataset.type);}
});

/* ----- scroll state ----- */
let sy=0, ticking=false;
const stage=$('#heroStage');
const tour=$('#rondleiding'), world=$('#tourWorld'), planes=$$('.plane'), caps=$$('.cap'), bar=$('#tourBar'), count=$('#tourCount'), hint=$('#tourHint');
const SP=620, TRAVEL=SP*(planes.length-1)+180;
function layoutPlanes(){
  const k=innerWidth<700?.55:1;
  planes.forEach((p,i)=>{
    const x=+p.dataset.x*k,y=+p.dataset.y,r=+p.dataset.r, z=-(500+i*SP);
    p._z=z;
    p.style.transform=`translate3d(calc(-50% + ${x}vw),calc(-50% + ${y}vh),${z}px) rotateY(${r}deg)`;
  });
}
layoutPlanes();
const dust=[];
if(!reduced){
  for(let i=0;i<46;i++){
    const d=document.createElement('div'); d.className='dust';
    const z=-Math.random()*(TRAVEL+900), x=(Math.random()-.5)*110, y=(Math.random()-.5)*90, s=.5+Math.random()*1.2;
    d._z=z; d.style.transform=`translate3d(calc(-50% + ${x}vw),calc(-50% + ${y}vh),${z}px) scale(${s})`;
    world.appendChild(d); dust.push(d);
  }
}
let curCap=-1;
function onScroll(){
  ticking=false; sy=window.scrollY;
  nav.classList.toggle('solid',sy>40);
  stage.style.setProperty('--sy',Math.min(sy,900));
  if(reduced) return;
  const r=tour.getBoundingClientRect(), total=tour.offsetHeight-innerHeight;
  const p=clamp(-r.top/total,0,1);
  if(r.bottom<-200||r.top>innerHeight+200) return;
  const T=p*TRAVEL;
  world.style.transform=`translateZ(${T}px) rotateY(${(p-.5)*-5}deg)`;
  planes.forEach(pl=>{
    const z=pl._z+T; let o=1;
    if(z<-1900) o=0; else if(z<-1000) o=(z+1900)/900;
    if(z>-120) o=clamp(1-(z+120)/520,0,1);
    pl.style.opacity=o.toFixed(3);
  });
  dust.forEach(d=>{const z=d._z+T; let o=z<-1800?0:z<-900?(z+1800)/900:1; if(z>200)o=clamp(1-(z-200)/500,0,1); d.style.opacity=(o*.8).toFixed(3);});
  const idx=clamp(Math.floor(p*caps.length*.999),0,caps.length-1);
  if(idx!==curCap){curCap=idx;caps.forEach((c,i)=>c.classList.toggle('on',i===idx));count.textContent=String(idx+1).padStart(2,'0')+' / '+String(caps.length).padStart(2,'0');}
  bar.style.transform=`scaleX(${p})`;
  hint.style.opacity=p<.03?1:0;
}
addEventListener('scroll',()=>{if(!ticking){ticking=true;requestAnimationFrame(onScroll);}},{passive:true});
addEventListener('resize',()=>{layoutPlanes();onScroll();});
if(reduced){caps.forEach(c=>c.classList.remove('on'));}

/* ----- hero mouse parallax ----- */
if(!reduced&&matchMedia('(pointer:fine)').matches){
  addEventListener('pointermove',e=>{
    stage.style.setProperty('--mx',((e.clientX/innerWidth)-.5).toFixed(3));
    stage.style.setProperty('--my',((e.clientY/innerHeight)-.5).toFixed(3));
  },{passive:true});
}

/* ----- reveal ----- */
let io;
function reveal(){
  const els=$$('.reveal:not(.in)');
  if(!('IntersectionObserver' in window)||reduced){els.forEach(e=>e.classList.add('in'));return;}
  if(!io) io=new IntersectionObserver(es=>es.forEach(e=>{if(e.isIntersecting){e.target.classList.add('in');io.unobserve(e.target);}}),{threshold:.12,rootMargin:'0px 0px -6% 0px'});
  els.forEach(e=>io.observe(e));
}

/* ----- agenda (automatisch: komend vs. geweest) ----- */
const EVENTS=[
  {d:'2026-10-11',wd:'Zondag',t:'Formule 1 Singapore',p:'Samen kijken, samen juichen!'},
  {d:'2026-10-17',wd:'Zaterdag',t:'Dave Brokken',p:'Aanvang 19.00 uur',tag:'Gratis entree',free:1},
  {d:'2026-10-25',wd:'Zondag',t:'Oktoberfest met Thorsten von Lippe Biesterfeld',p:'Aanvang 15.00 uur · kaarten te koop bij de Nachtegaal',tag:'Kaarten € 15,00'},
  {d:'2026-11-01',wd:'Zondag',t:'ONBEPERKT mosselen eten',p:'Opgeven aan de bar of telefonisch.',tag:'€ 17,50 p.p.',cta:'mosselen'},
  {d:'2026-11-28',wd:'',t:'Houseparty met T.H.I.I.S',p:'',tag:'Gratis entree',free:1},
  {d:'2026-12-20',wd:'Zondag',t:'Kerstshow met NO Expectations',p:''},
  {d:'2026-12-26',wd:'Zaterdag',t:'2e Kerstdag met Lootjes en Kadootjes!',p:''},
  {d:'2027-01-01',wd:'',t:'Nieuwjaarsdag met Dave Brokken',p:''}
];
const MON=['jan','feb','mrt','apr','mei','jun','jul','aug','sep','okt','nov','dec'];
(function(){
  const pad=n=>String(n).padStart(2,'0'); const n=new Date();
  const today=n.getFullYear()+'-'+pad(n.getMonth()+1)+'-'+pad(n.getDate());
  const up=EVENTS.filter(e=>e.d>=today);
  const row=(e,i)=>{const [y,m,d]=e.d.split('-');
    const meta=[e.wd,e.p].filter(Boolean).join(' · ');
    return `<li class="event ${i===0?'next':''}"><div class="date"><b>${+d}</b><span>${MON[+m-1]}</span></div><div>${i===0?'<span class="nxt">Eerstvolgende</span>':''}<h3>${e.t}</h3>${meta?`<p>${meta}</p>`:''}${e.cta?`<p style="margin-top:4px"><a href="#reserveren" data-type="${e.cta}">Opgeven →</a></p>`:''}</div>${e.tag?`<span class="price ${e.free?'free':''}">${e.tag}</span>`:''}</li>`;};
  $('#events').innerHTML=up.length?up.map(row).join(''):'<li class="event"><div></div><div><h3>Binnenkort meer</h3><p>Volg ons op social media voor de volgende optredens.</p></div></li>';
  /* posters verdwijnen na de datum van het evenement */
  let shown=0;
  $$('.poster[data-until]').forEach(f=>{if(f.dataset.until<today) f.hidden=true; else shown++;});
  if(!shown){$('.poster-col').hidden=true; $('.agenda-grid').classList.add('solo');}
})();

/* ----- poster tilt on pointer ----- */
$$('.posters,.feest-poster,.biljart-poster,.glass').forEach(el=>{
  if(reduced||!matchMedia('(pointer:fine)').matches) return;
  el.addEventListener('pointermove',e=>{const r=el.getBoundingClientRect();const x=(e.clientX-r.left)/r.width-.5,y=(e.clientY-r.top)/r.height-.5;
    const f=el.querySelector('figure'); if(f&&!el.classList.contains('posters')) f.style.transform=`rotateY(${x*14}deg) rotateX(${-y*10}deg) scale(1.02)`;});
  el.addEventListener('pointerleave',()=>{const f=el.querySelector('figure'); if(f&&!el.classList.contains('posters')) f.style.transform='';});
});

/* ======================= RESERVEREN ======================= */
const fDate=$('#fDate'), fTime=$('#fTime'), fPers=$('#fPers'), errDate=$('#errDate'), errForm=$('#errForm');
const iso=d=>d.getFullYear()+'-'+String(d.getMonth()+1).padStart(2,'0')+'-'+String(d.getDate()).padStart(2,'0');
fDate.min=iso(new Date());
function wdOf(v){const [y,m,d]=v.split('-').map(Number);return new Date(y,m-1,d).getDay();}
function buildTimes(){
  fTime.innerHTML=''; errDate.textContent='';
  const type=$('input[name=type]:checked').value;
  if(!fDate.value){fTime.innerHTML='<option value="">Kies datum</option>';return false;}
  const h=HOURS[wdOf(fDate.value)];
  if(!h){fTime.innerHTML='<option value="">Gesloten</option>';errDate.textContent='Op dinsdag en woensdag zijn we gesloten. Kies een andere dag.';return false;}
  const end=type==='feest'?h[1]-1:h[1]-1;
  let html='';
  for(let m=h[0]*60;m<=end*60;m+=30){const H=Math.floor(m/60)%24,M=m%60;const t=String(H).padStart(2,'0')+':'+String(M).padStart(2,'0');html+=`<option value="${t}">${t}</option>`;}
  fTime.innerHTML=html; return true;
}
function onType(){
  const type=$('input[name=type]:checked').value;
  if(type==='mosselen'){fDate.value='2026-11-01'; fDate.readOnly=true; if(+fPers.value<1)fPers.value=2;}
  else {fDate.readOnly=false;}
  if(type==='feest'&&+fPers.value<10) fPers.value=30;
  buildTimes();
}
$$('input[name=type]').forEach(r=>r.addEventListener('change',onType));
fDate.addEventListener('change',buildTimes);
$('#minus').addEventListener('click',()=>{fPers.value=Math.max(1,(+fPers.value||1)-1);});
$('#plus').addEventListener('click',()=>{fPers.value=Math.min(120,(+fPers.value||1)+1);});
if(iso(new Date())>'2026-11-01'){$('#t3').hidden=true;$('label[for=t3]').hidden=true;}
buildTimes();
const TYPE={tafel:'Tafel reserveren',feest:'Feest of groep',mosselen:'Mosselen eten (zondag 1 november, € 17,50 p.p.)',vraag:'Vraag of overig'};
function fmtDate(v){const [y,m,d]=v.split('-').map(Number);const dt=new Date(y,m-1,d);return DAYS[dt.getDay()]+' '+d+' '+['januari','februari','maart','april','mei','juni','juli','augustus','september','oktober','november','december'][m-1]+' '+y;}
let lastMsg='';
$('#resForm').addEventListener('submit',e=>{
  e.preventDefault(); errForm.textContent='';
  const type=$('input[name=type]:checked').value, name=$('#fName').value.trim(), tel=$('#fTel').value.trim();
  if(type!=='vraag'){
    if(!fDate.value){errForm.textContent='Kies een datum.';fDate.focus();return;}
    if(!HOURS[wdOf(fDate.value)]){errDate.textContent='Op dinsdag en woensdag zijn we gesloten. Kies een andere dag.';fDate.focus();return;}
  }
  if(!name){errForm.textContent='Vul je naam in.';$('#fName').focus();return;}
  if(tel.replace(/\D/g,'').length<9){errForm.textContent='Vul een geldig telefoonnummer in, dan kan het café je bereiken.';$('#fTel').focus();return;}
  const pers=clamp(+fPers.value||1,1,120);
  const lines=['Hallo Café de Nachtegaal, ik wil graag het volgende doorgeven:','',`Soort: ${TYPE[type]}`];
  if(fDate.value){lines.push(`Datum: ${fmtDate(fDate.value)}`); if(fTime.value) lines.push(`Tijd: ${fTime.value} uur`);}
  lines.push(`Aantal personen: ${pers}`,`Naam: ${name}`,`Telefoon: ${tel}`);
  if($('#fNote').value.trim()) lines.push(`Opmerking: ${$('#fNote').value.trim()}`);
  lines.push('','Kunt u dit bevestigen? Alvast bedankt!');
  lastMsg=lines.join('\n');
  $('#doneTitle').textContent='Bedankt, '+name.split(' ')[0]+'!'; $('#done').classList.add('on');
  const wa='https://wa.me/31630862200?text='+encodeURIComponent(lastMsg);
  $('#waLink').href=wa; window.open(wa,'_blank','noopener');
  $('#done').scrollIntoView({behavior:'smooth',block:'center'});
});

onScroll(); reveal();
})();
</script>
</body>
</html>

onScroll(); reveal();
})();
</script>
</body>
</html>
