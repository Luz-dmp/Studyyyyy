<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ruta de preparación — Vacaciones 2026</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500;600&family=Source+Serif+4:opsz,wght@8..60,400;8..60,500;8..60,600&display=swap" rel="stylesheet">
<style>
  :root{
    --paper:#EAEDF1;
    --paper-2:#E1E5EC;
    --grid-line:#C6D0DC;
    --ink:#16233B;
    --ink-soft:#3E4C67;
    --copper:#9C5A28;
    --copper-bright:#B5652D;
    --teal:#1F7A72;
    --amber:#B98A25;
    --white:#FBFAF7;
  }
  *{box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    margin:0;
    background:
      repeating-linear-gradient(0deg, transparent, transparent 27px, var(--grid-line) 27px, var(--grid-line) 28px),
      repeating-linear-gradient(90deg, transparent, transparent 27px, var(--grid-line) 27px, var(--grid-line) 28px),
      var(--paper);
    color:var(--ink);
    font-family:'Source Serif 4', serif;
    line-height:1.6;
  }
  .wrap{max-width:920px; margin:0 auto; padding:0 24px;}
  .eyebrow{
    font-family:'JetBrains Mono', monospace;
    font-size:12px;
    letter-spacing:.14em;
    text-transform:uppercase;
    color:var(--copper);
    font-weight:600;
  }
  h1,h2,h3{font-family:'Space Grotesk', sans-serif; color:var(--ink); margin:0;}

  /* ---------- HERO ---------- */
  header.hero{padding:72px 0 40px; position:relative; animation:fade-in .6s ease;}
  .hero .eyebrow{margin-bottom:14px; animation:slide-in .6s ease .1s backwards;}
  .hero h1{font-size:clamp(34px,6vw,56px); font-weight:700; line-height:1.05; letter-spacing:-0.01em; animation:slide-in .6s ease .2s backwards;}
  .hero h1 span{color:var(--copper-bright); transition:all .3s ease;}
  .hero h1:hover span{text-shadow:0 0 10px rgba(181, 101, 45, 0.3); letter-spacing:0.02em;}
  .hero p.lede{max-width:560px; font-size:18px; color:var(--ink-soft); margin-top:18px; animation:slide-in .6s ease .3s backwards;}
  .hero .meta-row{
    display:flex; gap:28px; margin-top:32px; flex-wrap:wrap;
    font-family:'JetBrains Mono', monospace; font-size:12.5px; color:var(--ink-soft);
    animation:slide-in .6s ease .4s backwards;
  }
  .hero .meta-row div{border-left:2px solid var(--copper-bright); padding-left:10px; transition:all .2s ease;}
  .hero .meta-row div:hover{padding-left:14px; color:var(--ink);}
  .hero .meta-row b{display:block; color:var(--ink); font-size:15px; font-family:'Space Grotesk',sans-serif;}
  @keyframes slide-in{from{opacity:0; transform:translateY(10px);} to{opacity:1; transform:translateY(0);}}
  @keyframes fade-in{from{opacity:0;} to{opacity:1;}}
  /* ---------- CIRCUIT PRIORITY TRACE ---------- */
  section.trace{padding:20px 0 56px;}
  .trace-title{margin-bottom:22px;}
  .trace-svg-holder{width:100%; overflow-x:auto;}
  svg.trace-svg{display:block; min-width:760px; width:100%; height:auto;}
  .node-card{
    font-family:'JetBrains Mono', monospace;
  }
  .node-label{fill:var(--ink); font-size:13px; font-family:'Space Grotesk', sans-serif; font-weight:600;}
  .node-sub{fill:var(--ink-soft); font-size:10.5px;}
  .node-hours{fill:var(--copper-bright); font-size:10.5px; font-weight:600;}
  .node-flag{fill:var(--amber); font-size:9.5px; font-weight:600;}
  .trace-note{
    font-size:14px; color:var(--ink-soft); margin-top:10px; max-width:640px;
  }

  /* ---------- SUBJECT ACCORDION ---------- */
  section.subjects{padding:20px 0 30px;}
  .subject{
    background:var(--white);
    border:1px solid var(--grid-line);
    border-left:5px solid var(--copper-bright);
    border-radius:2px;
    margin-bottom:16px;
    box-shadow:0 1px 0 rgba(22,35,59,.04);
    transition:all .2s ease;
  }
  .subject:hover{box-shadow:0 2px 6px rgba(22,35,59,.08); border-color:#B5652D;}
  .subject.teal-accent{border-left-color:var(--teal);}
  .subject.teal-accent:hover{border-color:var(--teal);}
  .subject.amber-accent{border-left-color:var(--amber);}
  .subject.amber-accent:hover{border-color:var(--amber);}
  .subject-head{
    display:flex; align-items:center; justify-content:space-between; gap:16px;
    padding:20px 22px; cursor:pointer; user-select:none; transition:all .2s ease;
  }
  .subject-head:active{background:rgba(156, 90, 40, 0.05);}
  .subject-head-left{display:flex; align-items:baseline; gap:14px;}
  .subject-num{font-family:'JetBrains Mono',monospace; color:var(--copper-bright); font-size:13px; font-weight:600; transition:all .2s ease;}
  .subject.open .subject-num{transform:scale(1.1);}
  .subject-head h3{font-size:21px; font-weight:600; transition:color .2s ease;}
  .subject:hover .subject-head h3{color:var(--copper-bright);}
  .subject-stars{font-size:12px; color:var(--copper-bright); font-family:'JetBrains Mono',monospace; margin-left:8px; letter-spacing:.05em;}
  .chev{
    width:22px; height:22px; flex-shrink:0; transition:transform .35s cubic-bezier(0.34, 1.56, 0.64, 1);
    color:var(--ink-soft);
  }
  .subject.open .chev{transform:rotate(180deg);}
  .subject-body{
    max-height:0; overflow:hidden; transition:max-height .35s cubic-bezier(0.34, 1.56, 0.64, 1);
  }
  .subject.open .subject-body{max-height:2400px; transition:max-height .4s ease;}
  .subject-body-inner{padding:0 22px 26px 22px;}
  .why-box{
    font-size:15px; color:var(--ink-soft); margin-bottom:18px; padding-bottom:16px;
    border-bottom:1px dashed var(--grid-line);
  }
  .col-heading{
    font-family:'JetBrains Mono', monospace; font-size:11px; letter-spacing:.1em;
    text-transform:uppercase; color:var(--ink); font-weight:600; margin-bottom:8px; margin-top:18px;
  }
  ol.topics{margin:0; padding-left:20px;}
  ol.topics li{margin-bottom:5px; font-size:15px;}
  .formula{
    font-family:'JetBrains Mono', monospace; background:var(--paper-2); padding:2px 7px; border-radius:3px; font-size:14px;
  }
  .resource-row{
    display:flex; gap:10px; align-items:flex-start; font-size:14.5px; margin-bottom:6px;
  }
  .resource-row .tag{
    font-family:'JetBrains Mono',monospace; font-size:10px; background:var(--ink); color:var(--white);
    padding:2px 6px; border-radius:2px; flex-shrink:0; margin-top:3px;
  }
  .plan-line{font-size:14.5px; color:var(--ink-soft);}

  /* Yamil sticky note */
  .yamil-note{
    margin-top:18px;
    background:#F3EAD3;
    border:1px solid #DECFA0;
    border-radius:3px;
    padding:14px 16px;
    position:relative;
    font-size:14.5px;
    color:#4a3c1a;
  }
  .yamil-note::before{
    content:"NOTA DE CAMPO — YAMIL";
    display:block;
    font-family:'JetBrains Mono',monospace;
    font-size:10px;
    letter-spacing:.08em;
    color:var(--amber);
    font-weight:700;
    margin-bottom:6px;
  }
  .yamil-note.warn{background:#F5E4D9; border-color:#E0BFA3;}
  .yamil-note.warn::before{content:"⚠ OJO — YAMIL";}

  /* ---------- SCHEDULE ---------- */
  section.schedule{padding:30px 0 40px;}
  .schedule-grid{
    display:grid;
    grid-template-columns:repeat(6, 1fr);
    gap:8px;
    margin-top:20px;
  }
  .day-col{
    background:var(--white); border:1px solid var(--grid-line); border-radius:3px; padding:10px 8px; 
    text-align:center; transition:all .2s ease; cursor:default;
  }
  .day-col:hover{box-shadow:0 3px 8px rgba(156, 90, 40, 0.15); transform:translateY(-2px);}
  .day-col .day-name{font-family:'JetBrains Mono',monospace; font-size:11px; font-weight:600; letter-spacing:.06em; color:var(--ink-soft); text-transform:uppercase;}
  .day-col .cell{
    margin-top:8px; padding:8px 4px; border-radius:3px; font-size:12px; font-family:'Space Grotesk',sans-serif; 
    font-weight:600; color:var(--white); transition:all .2s ease; cursor:pointer;
  }
  .day-col .cell:hover{transform:scale(1.05); box-shadow:0 2px 4px rgba(0,0,0,.2);}
  .cell.circ{background:var(--copper-bright);}
  .cell.fis{background:var(--teal);}
  .cell.est{background:#5B6B8C;}
  .cell.edo{background:#7C8A55;}
  .cell.sis{background:var(--amber);}
  .cell.free{background:var(--paper-2); color:var(--ink-soft); font-weight:400;}
  .legend{display:flex; flex-wrap:wrap; gap:14px; margin-top:16px; font-family:'JetBrains Mono',monospace; font-size:11.5px; color:var(--ink-soft); transition:all .2s ease;}
  .legend span{display:inline-flex; align-items:center; gap:6px; transition:transform .2s ease;}
  .legend span:hover{transform:translateX(2px);}
  .legend i{width:10px; height:10px; display:inline-block; border-radius:2px;}

  .distribution{margin-top:26px;}
  .bar-row{display:flex; align-items:center; gap:12px; margin-bottom:9px;}
  .bar-row .bar-label{width:150px; font-size:13px; font-family:'JetBrains Mono',monospace; flex-shrink:0;}
  .bar-track{flex:1; background:var(--paper-2); height:16px; border-radius:2px; overflow:hidden;}
  .bar-fill{height:100%;}
  .bar-row .bar-pct{width:40px; text-align:right; font-family:'JetBrains Mono',monospace; font-size:12.5px; color:var(--ink-soft); flex-shrink:0;}

  /* ---------- GOLDEN KEY (IC chip) ---------- */
  section.golden{padding:30px 0 60px;}
  .chip{
    background:var(--ink);
    color:var(--white);
    border-radius:8px;
    padding:34px 30px;
    position:relative;
    max-width:720px;
    margin:0 auto;
    transition:all .3s ease;
    box-shadow:0 4px 12px rgba(22,35,59,.15);
  }
  .chip:hover{transform:translateY(-2px); box-shadow:0 8px 24px rgba(156, 90, 40, 0.2);}
  .chip::before, .chip::after{
    content:"";
    position:absolute; top:24px; bottom:24px; width:14px;
    background-image:repeating-linear-gradient(0deg, var(--copper-bright), var(--copper-bright) 4px, transparent 4px, transparent 12px);
    transition:all .3s ease;
  }
  .chip::before{left:-10px;}
  .chip::after{right:-10px;}
  .chip:hover::before, .chip:hover::after{width:16px; left:-12px;}
  .chip h2{color:var(--white); font-size:24px; margin-bottom:16px; transition:color .3s ease;}
  .chip p{color:#C9D1E0; font-size:15px; margin:0 0 14px; transition:color .3s ease;}
  .chip ul{margin:0; padding-left:20px; color:#E6E9F2;}
  .chip ul li{margin-bottom:8px; font-size:15px; transition:transform .2s ease;}
  .chip ul li:hover{transform:translateX(3px);}
  .chip .kicker{font-family:'JetBrains Mono',monospace; font-size:11px; letter-spacing:.14em; text-transform:uppercase; color:var(--copper-bright); margin-bottom:10px; display:block; animation:kicker-pulse 2s ease-in-out infinite;}
  @keyframes kicker-pulse{0%,100%{opacity:1;} 50%{opacity:0.7;}}
  section.dashboard{padding:8px 0 34px;}
  .dash-grid{display:grid; grid-template-columns:1.1fr 1.6fr; gap:14px; margin-top:18px;}
  .dash-card{background:var(--white); border:1px solid var(--grid-line); border-radius:3px; padding:18px 20px;}
  .dash-card h4{font-family:'JetBrains Mono',monospace; font-size:11px; letter-spacing:.08em; text-transform:uppercase; color:var(--ink-soft); margin:0 0 10px; font-weight:600;}
  .countdown-num{font-family:'Space Grotesk',sans-serif; font-size:44px; font-weight:700; color:var(--copper-bright); line-height:1; transition:all .5s ease; animation:pulse-countdown 2s ease-in-out infinite;}
  .countdown-label{font-size:14px; color:var(--ink-soft); margin-top:4px; transition:color .3s ease;}
  @keyframes pulse-countdown{0%,100%{transform:scale(1);} 50%{transform:scale(1.02);}}
  .date-row{display:flex; align-items:center; gap:8px; margin-top:14px;}
  .date-row label{font-size:12.5px; color:var(--ink-soft); font-family:'JetBrains Mono',monospace;}
  .date-row input[type=date]{
    font-family:'JetBrains Mono',monospace; font-size:12.5px; border:2px solid var(--grid-line);
    border-radius:3px; padding:8px 10px; background:var(--paper-2); color:var(--ink); 
    cursor:pointer; transition:all .2s ease;
  }
  .date-row input[type=date]:hover{border-color:var(--copper-bright); background:var(--white);}
  .date-row input[type=date]:focus{outline:none; border-color:var(--copper-bright); box-shadow:0 0 0 3px rgba(181, 101, 45, 0.1);}
  .overall-bar{margin-top:14px;}
  .overall-bar .bar-track{height:10px; box-shadow:inset 0 1px 2px rgba(22,35,59,.1);}
  .overall-pct{font-family:'JetBrains Mono',monospace; font-size:12.5px; color:var(--ink-soft); margin-top:6px; transition:color .3s ease;}

  .bar-row{display:flex; align-items:center; gap:12px; margin-bottom:9px; transition:all .2s ease;}
  .bar-row:hover{transform:translateX(2px);}
  .bar-row .bar-label{width:150px; font-size:13px; font-family:'JetBrains Mono',monospace; flex-shrink:0;}
  .bar-track{flex:1; background:var(--paper-2); height:16px; border-radius:2px; overflow:hidden; box-shadow:inset 0 1px 2px rgba(22,35,59,.08);}
  .bar-fill{height:100%; transition:width .4s cubic-bezier(0.34, 1.56, 0.64, 1); position:relative;}
  .bar-fill::after{content:''; position:absolute; top:0; left:0; right:0; bottom:0; background:linear-gradient(90deg, transparent, rgba(255,255,255,.3), transparent); animation:shimmer 2s infinite;}
  @keyframes shimmer{0%{transform:translateX(-100%);} 100%{transform:translateX(100%);}}
  .bar-row .bar-pct{width:40px; text-align:right; font-family:'JetBrains Mono',monospace; font-size:12.5px; color:var(--ink-soft); flex-shrink:0;}

  .hours-item{display:flex; align-items:center; gap:10px; padding:6px 8px; border-radius:3px; transition:background .2s ease;}
  .hours-item:hover{background:rgba(156, 90, 40, 0.03);}
  .hours-item .h-name{width:118px; font-size:13px; font-family:'JetBrains Mono',monospace; flex-shrink:0;}
  .hours-item .h-track{flex:1; background:var(--paper-2); height:12px; border-radius:2px; overflow:hidden; position:relative; box-shadow:inset 0 1px 1px rgba(22,35,59,.08);}
  .hours-item .h-fill{height:100%; transition:width .3s ease; position:relative;}
  .hours-item .h-total{width:64px; text-align:right; font-family:'JetBrains Mono',monospace; font-size:12px; color:var(--ink-soft); flex-shrink:0;}
  .hours-item .h-btns{display:flex; gap:4px; flex-shrink:0;}

  .subject-progress{
    font-family:'JetBrains Mono',monospace; font-size:11.5px; color:var(--ink-soft); margin-left:10px; transition:color .2s ease;
  }
  .head-bar-track{width:56px; height:6px; background:var(--paper-2); border-radius:3px; overflow:hidden; display:inline-block; margin-left:8px; vertical-align:middle;}
  .head-bar-fill{height:100%; background:var(--copper-bright); transition:width .3s ease;}

  /* Enhanced button styles */
  .subject-head{transition:background .2s ease;}
  .subject-head:hover{background:rgba(156, 90, 40, 0.04);}

  @media (max-width:640px){
    .dash-grid{grid-template-columns:1fr;}
  }

  @media (max-width:640px){
    .schedule-grid{grid-template-columns:repeat(3,1fr);}
    .hero{padding:48px 0 30px;}
    .chip::before,.chip::after{display:none;}
  }
</style>
</head>
<body>

<div class="wrap">

  <header class="hero">
    <div class="eyebrow">Vacaciones · Antes del semestre</div>
    <h1>Ruta de preparación <span>— Ingeniería</span></h1>
    <p class="lede">No se trata de "aprender la materia completa", sino de llegar al primer día de clases con las bases listas — para que la clase funcione como repaso, no como primer contacto. Esta guía cruza dos rutas de estudio con la experiencia real de alguien que ya cursó estas materias.</p>
    <div class="meta-row">
      <div><b>5</b>materias cubiertas</div>
      <div><b>~11-13h</b>por semana</div>
      <div><b>2</b>fuentes cruzadas y verificadas</div>
    </div>
  </header>

  <section class="dashboard" id="seguimiento">
    <div class="eyebrow">Panel de seguimiento</div>
    <h2 style="font-size:24px; margin-top:6px;">Tu avance real</h2>
    <div class="dash-grid">
      <div class="dash-card">
        <h4>Cuenta regresiva</h4>
        <div class="countdown-num" id="countdownNum">—</div>
        <div class="countdown-label" id="countdownLabel">configura la fecha de inicio</div>
        <div class="date-row">
          <label for="semDate">Inicio de semestre:</label>
          <input type="date" id="semDate">
        </div>
        <div class="overall-bar">
          <div class="bar-track"><div class="bar-fill" id="overallFill" style="width:0%; background:var(--copper-bright);"></div></div>
          <div class="overall-pct" id="overallPct">0/33 temas completados</div>
        </div>
      </div>
      <div class="dash-card">
        <h4>Horas acumuladas por materia</h4>
        <div class="hours-list" id="hoursList"><!-- filled by JS --></div>
      </div>
    </div>
  </section>

  <section class="trace" id="prioridades">
    <div class="trace-title">
      <div class="eyebrow">Orden de prioridad</div>
      <h2 style="font-size:26px; margin-top:6px;">El circuito de estudio</h2>
      <p class="trace-note">Ordenado según lo que realmente pesa en el semestre — no por el orden en que aparecen en el pénsum. El grosor de la traza indica horas semanales recomendadas.</p>
    </div>
    <div class="trace-svg-holder">
      <svg class="trace-svg" viewBox="0 0 780 190" xmlns="http://www.w3.org/2000/svg">
        <!-- main trace -->
        <path d="M60 95 L720 95" stroke="#9C5A28" stroke-width="5" fill="none" stroke-linecap="round"/>
        <!-- drop lines -->
        <line x1="60" y1="95" x2="60" y2="95"/>
        <g font-family="JetBrains Mono">
          <!-- Node 1: Circuitos -->
          <circle cx="60" cy="95" r="26" fill="#FBFAF7" stroke="#9C5A28" stroke-width="4"/>
          <text x="60" y="100" text-anchor="middle" class="node-hours" font-size="13" font-weight="700" fill="#9C5A28">01</text>
          <text x="60" y="140" text-anchor="middle" class="node-label">Circuitos I</text>
          <text x="60" y="155" text-anchor="middle" class="node-sub">4h/sem</text>

          <!-- Node 2: Fisica -->
          <circle cx="225" cy="95" r="24" fill="#FBFAF7" stroke="#1F7A72" stroke-width="4"/>
          <text x="225" y="100" text-anchor="middle" font-size="13" font-weight="700" fill="#1F7A72">02</text>
          <text x="225" y="140" text-anchor="middle" class="node-label">Física · Calor y Ondas</text>
          <text x="225" y="155" text-anchor="middle" class="node-sub">3h/sem</text>

          <!-- Node 3: Estadistica -->
          <circle cx="400" cy="95" r="21" fill="#FBFAF7" stroke="#5B6B8C" stroke-width="4"/>
          <text x="400" y="100" text-anchor="middle" font-size="13" font-weight="700" fill="#5B6B8C">03</text>
          <text x="400" y="135" text-anchor="middle" class="node-label">Estadística</text>
          <text x="400" y="150" text-anchor="middle" class="node-sub">2h/sem</text>
          <text x="400" y="164" text-anchor="middle" class="node-flag">condicional ⚑</text>

          <!-- Node 4: EDO -->
          <circle cx="565" cy="95" r="20" fill="#FBFAF7" stroke="#7C8A55" stroke-width="4"/>
          <text x="565" y="100" text-anchor="middle" font-size="13" font-weight="700" fill="#7C8A55">04</text>
          <text x="565" y="135" text-anchor="middle" class="node-label">Ecuaciones Dif.</text>
          <text x="565" y="150" text-anchor="middle" class="node-sub">2-3h/sem</text>

          <!-- Node 5: Sistemas -->
          <circle cx="720" cy="95" r="19" fill="#FBFAF7" stroke="#B98A25" stroke-width="4"/>
          <text x="720" y="100" text-anchor="middle" font-size="13" font-weight="700" fill="#B98A25">05</text>
          <text x="720" y="135" text-anchor="middle" class="node-label">Sistemas Digit.</text>
          <text x="720" y="150" text-anchor="middle" class="node-sub">2h/sem</text>
          <text x="720" y="164" text-anchor="middle" class="node-flag">sin libro guía ⚑</text>
        </g>
      </svg>
    </div>
    <p class="trace-note"><b>Por qué este orden:</b> las dos rutas coinciden en que Circuitos I y Física (Calor y Ondas) van primero. La diferencia la marca la experiencia real: Estadística sube al puesto 3 <i>solo si es la Inferencial</i> — si es la básica, prácticamente ya la diste en el colegio y baja de prioridad. Ecuaciones Diferenciales, aunque parezca intensa, es la más "regalada" de las cinco si la ves con el profesor Palomino. Sistemas Digitales queda última porque no depende de un solo libro — es la más dispersa.</p>
  </section>

  <section class="subjects" id="materias">
    <div class="eyebrow" style="margin-bottom:6px;">Detalle por materia</div>
    <h2 style="font-size:26px; margin-bottom:20px;">Qué estudiar y en qué orden</h2>

    <!-- CIRCUITOS -->
    <div class="subject open">
      <div class="subject-head" onclick="toggleSubject(this)">
        <div class="subject-head-left">
          <span class="subject-num">01</span>
          <h3>Circuitos Eléctricos I</h3>
          <span class="subject-stars">★★★★★</span>
          <span class="head-bar-track"><span class="head-bar-fill" data-head-bar="circuitos" style="width:0%"></span></span>
        </div>
        <svg class="chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>
      </div>
      <div class="subject-body">
        <div class="subject-body-inner">
          <p class="why-box">Es la materia con más impacto en cursos posteriores. Todo lo que viene después de este curso — electrónica, máquinas, control — se apoya en estos fundamentos.</p>

          <div class="col-heading">Temas en orden <span class="subject-progress" data-progress-label="circuitos">0/7</span></div>
          <ul class="topics" data-subject="circuitos">
            <li class="topic-row"><input type="checkbox" id="circuitos-0" data-subject="circuitos" data-idx="0"><label for="circuitos-0">Qué es la electricidad: carga (Coulomb), corriente (A), voltaje (V), potencia (W), energía. Pregúntate: ¿qué hace realmente una batería? ¿qué diferencia hay entre voltaje y corriente?</label></li>
            <li class="topic-row"><input type="checkbox" id="circuitos-1" data-subject="circuitos" data-idx="1"><label for="circuitos-1">Componentes básicos: resistencia, fuentes de voltaje y corriente. Luego capacitores e inductores — entender qué almacena cada uno, sin resolver circuitos todavía.</label></li>
            <li class="topic-row"><input type="checkbox" id="circuitos-2" data-subject="circuitos" data-idx="2"><label for="circuitos-2">Ley de Ohm: <span class="formula">V = IR</span> — despejarla de memoria (<span class="formula">I=V/R</span>, <span class="formula">R=V/I</span>) y hacer muchos ejercicios.</label></li>
            <li class="topic-row"><input type="checkbox" id="circuitos-3" data-subject="circuitos" data-idx="3"><label for="circuitos-3">Potencia: <span class="formula">P = VI</span>, <span class="formula">P = I²R</span>, <span class="formula">P = V²/R</span>.</label></li>
            <li class="topic-row"><input type="checkbox" id="circuitos-4" data-subject="circuitos" data-idx="4"><label for="circuitos-4">Leyes de Kirchhoff: KCL (la suma de corrientes que entran a un nodo = la suma de las que salen) y KVL (la suma de voltajes en una malla cerrada es cero).</label></li>
            <li class="topic-row"><input type="checkbox" id="circuitos-5" data-subject="circuitos" data-idx="5"><label for="circuitos-5">Métodos de análisis: análisis nodal y análisis de mallas. Dominar esto es "media materia ganada".</label></li>
            <li class="topic-row"><input type="checkbox" id="circuitos-6" data-subject="circuitos" data-idx="6"><label for="circuitos-6">Teoremas: Thévenin, Norton, superposición, transformación de fuentes, divisores de voltaje y corriente.</label></li>
          </ul>

          <div class="col-heading">Recursos</div>
          <div class="resource-row"><span class="tag">LIBRO PRINCIPAL</span><span><i>Fundamentos de Circuitos Eléctricos</i> — Alexander &amp; Sadiku. Sigue el orden de capítulos: cantidades básicas → elementos de circuitos → leyes básicas → métodos de análisis → teoremas. No saltes capítulos.</span></div>
          <div class="resource-row"><span class="tag">PARA PROFUNDIZAR</span><span><i>Análisis de Circuitos</i> — Hayt.</span></div>

          <div class="col-heading">Plan de estudio</div>
          <p class="plan-line">4 horas semanales. Prioriza hacer ejercicios sobre leer teoría — la teoría se fija resolviendo.</p>

          <div class="yamil-note warn">De los libros de circuitos que te compartí, no todo se usa — solo algunas cosas básicas para Circuitos 1. Aun así, no está de más revisar el resto.</div>
        </div>
      </div>
    </div>

    <!-- FISICA -->
    <div class="subject teal-accent open">
      <div class="subject-head" onclick="toggleSubject(this)">
        <div class="subject-head-left">
          <span class="subject-num">02</span>
          <h3>Física · Calor y Ondas</h3>
          <span class="subject-stars" style="color:#1F7A72;">★★★★★</span>
          <span class="head-bar-track"><span class="head-bar-fill" data-head-bar="fisica" style="width:0%; background:var(--teal);"></span></span>
        </div>
        <svg class="chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>
      </div>
      <div class="subject-body">
        <div class="subject-body-inner">
          <p class="why-box">Suele castigar a quienes llegan débiles en física y matemáticas básicas. Aquí los ejercicios son los que realmente dan la nota, más que la teoría.</p>

          <div class="col-heading">Repaso previo <span class="subject-progress" data-progress-label="fisica">0/9</span></div>
          <ul class="topics" data-subject="fisica">
            <li class="topic-row"><input type="checkbox" id="fisica-0" data-subject="fisica" data-idx="0"><label for="fisica-0">Unidades SI, vectores, fuerzas, energía, trabajo, potencia — todo esto vuelve constantemente.</label></li>
          </ul>

          <div class="col-heading">Calor</div>
          <ul class="topics" data-subject="fisica">
            <li class="topic-row"><input type="checkbox" id="fisica-1" data-subject="fisica" data-idx="1"><label for="fisica-1">Diferencia entre temperatura y calor (la mayoría los confunde).</label></li>
            <li class="topic-row"><input type="checkbox" id="fisica-2" data-subject="fisica" data-idx="2"><label for="fisica-2">Calor específico: qué significa y cómo calcularlo.</label></li>
            <li class="topic-row"><input type="checkbox" id="fisica-3" data-subject="fisica" data-idx="3"><label for="fisica-3">Dilatación: lineal, superficial, volumétrica.</label></li>
            <li class="topic-row"><input type="checkbox" id="fisica-4" data-subject="fisica" data-idx="4"><label for="fisica-4">Calorimetría.</label></li>
            <li class="topic-row"><input type="checkbox" id="fisica-5" data-subject="fisica" data-idx="5"><label for="fisica-5">Termodinámica — especialmente la Primera Ley.</label></li>
          </ul>

          <div class="col-heading">Ondas</div>
          <ul class="topics" data-subject="fisica">
            <li class="topic-row"><input type="checkbox" id="fisica-6" data-subject="fisica" data-idx="6"><label for="fisica-6">Movimiento armónico simple: periodo, frecuencia, amplitud.</label></li>
            <li class="topic-row"><input type="checkbox" id="fisica-7" data-subject="fisica" data-idx="7"><label for="fisica-7">Ondas mecánicas: longitud de onda, frecuencia, velocidad — <span class="formula">v = fλ</span>.</label></li>
            <li class="topic-row"><input type="checkbox" id="fisica-8" data-subject="fisica" data-idx="8"><label for="fisica-8">Sonido: intensidad, resonancia, efecto Doppler, interferencia.</label></li>
          </ul>

          <div class="col-heading">Recursos</div>
          <div class="resource-row"><span class="tag">LIBRO PRINCIPAL</span><span><i>Física Universitaria</i> — Young &amp; Freedman (probablemente el segundo tomo). Orden sugerido: temperatura → calor → primera ley → oscilaciones → ondas → sonido.</span></div>

          <div class="col-heading">Plan de estudio</div>
          <p class="plan-line">3 horas semanales: 1h teoría + 2h ejercicios.</p>

          <div class="yamil-note">En el curso sí abordan toda la parte de ondas del libro de Física Universitaria. Trata de hacer todos los ejercicios del libro y estar pendiente a los que deje el profe — todos tienen solucionario.</div>
        </div>
      </div>
    </div>

    <!-- ESTADISTICA -->
    <div class="subject" style="border-left-color:#5B6B8C;">
      <div class="subject-head" onclick="toggleSubject(this)">
        <div class="subject-head-left">
          <span class="subject-num">03</span>
          <h3>Estadística</h3>
          <span class="subject-stars" style="color:#5B6B8C;">★★★☆☆</span>
          <span class="head-bar-track"><span class="head-bar-fill" data-head-bar="estadistica" style="width:0%; background:#5B6B8C;"></span></span>
        </div>
        <svg class="chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>
      </div>
      <div class="subject-body">
        <div class="subject-body-inner">
          <p class="why-box">Esta es la materia que más depende de un dato que solo tú puedes confirmar: <b>qué Estadística te toca.</b> No estaba en la primera ruta de estudio — es un aporte directo de la experiencia de Yamil, y cambia todo el plan.</p>

          <div class="col-heading">Si es Estadística I (básica) <span class="subject-progress" data-progress-label="estadistica">0/5</span></div>
          <ul class="topics" data-subject="estadistica">
            <li class="topic-row"><input type="checkbox" id="estadistica-0" data-subject="estadistica" data-idx="0"><label for="estadistica-0">Es literalmente lo que ya diste en el colegio.</label></li>
            <li class="topic-row"><input type="checkbox" id="estadistica-1" data-subject="estadistica" data-idx="1"><label for="estadistica-1">La diferencia es que probablemente usen un software para los cálculos: Excel, R, u otro.</label></li>
            <li class="topic-row"><input type="checkbox" id="estadistica-2" data-subject="estadistica" data-idx="2"><label for="estadistica-2">Prioridad baja — puede quedar de última en tu semana.</label></li>
          </ul>

          <div class="col-heading">Si es Estadística Inferencial</div>
          <ul class="topics" data-subject="estadistica">
            <li class="topic-row"><input type="checkbox" id="estadistica-3" data-subject="estadistica" data-idx="3"><label for="estadistica-3">No hay una ruta clara de referencia — depende mucho de lo que dé cada profesor.</label></li>
            <li class="topic-row"><input type="checkbox" id="estadistica-4" data-subject="estadistica" data-idx="4"><label for="estadistica-4">Si te toca esta, sube a prioridad alta (puesto 3 en el orden general).</label></li>
          </ul>

          <div class="yamil-note warn">Primero averigua en tu programa/syllabus cuál de las dos te toca — de eso depende si esta materia va de tercera en prioridad o de última.</div>
        </div>
      </div>
    </div>

    <!-- EDO -->
    <div class="subject" style="border-left-color:#7C8A55;">
      <div class="subject-head" onclick="toggleSubject(this)">
        <div class="subject-head-left">
          <span class="subject-num">04</span>
          <h3>Ecuaciones Diferenciales</h3>
          <span class="subject-stars" style="color:#7C8A55;">★★★★☆</span>
          <span class="head-bar-track"><span class="head-bar-fill" data-head-bar="edo" style="width:0%; background:#7C8A55;"></span></span>
        </div>
        <svg class="chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>
      </div>
      <div class="subject-body">
        <div class="subject-body-inner">
          <p class="why-box">Vienes con ventaja de Cálculo Integral, y según la experiencia real, es una materia "sencilla" — más aún si te toca con el profesor Palomino.</p>

          <div class="col-heading">Base necesaria (repasar primero) <span class="subject-progress" data-progress-label="edo">0/7</span></div>
          <ul class="topics" data-subject="edo">
            <li class="topic-row"><input type="checkbox" id="edo-0" data-subject="edo" data-idx="0"><label for="edo-0">Derivadas: producto, cociente, cadena, trigonométricas, exponenciales, logaritmos.</label></li>
            <li class="topic-row"><input type="checkbox" id="edo-1" data-subject="edo" data-idx="1"><label for="edo-1">Integrales: sustitución, por partes, fracciones parciales.</label></li>
            <li class="topic-row"><input type="checkbox" id="edo-2" data-subject="edo" data-idx="2"><label for="edo-2">Álgebra: despejes, factorización, fracciones — un signo mal puesto arruina la solución completa.</label></li>
          </ul>

          <div class="col-heading">Contenido en orden</div>
          <ul class="topics" data-subject="edo">
            <li class="topic-row"><input type="checkbox" id="edo-3" data-subject="edo" data-idx="3"><label for="edo-3">Variables separables</label></li>
            <li class="topic-row"><input type="checkbox" id="edo-4" data-subject="edo" data-idx="4"><label for="edo-4">Ecuaciones lineales</label></li>
            <li class="topic-row"><input type="checkbox" id="edo-5" data-subject="edo" data-idx="5"><label for="edo-5">Ecuaciones exactas</label></li>
            <li class="topic-row"><input type="checkbox" id="edo-6" data-subject="edo" data-idx="6"><label for="edo-6">Ecuaciones homogéneas</label></li>
          </ul>

          <div class="col-heading">Recursos</div>
          <div class="resource-row"><span class="tag">VIDEOS</span><span>El Profe Alex (YouTube) — según la experiencia real, sus videos "sirven muchísimo" para toda la materia.</span></div>

          <div class="col-heading">Plan de estudio</div>
          <p class="plan-line">2-3 horas semanales. No hace falta dominar todo antes de empezar — con llegar con base sólida el semestre se vuelve mucho más llevadero.</p>
        </div>
      </div>
    </div>

    <!-- SISTEMAS DIGITALES -->
    <div class="subject" style="border-left-color:#B98A25;">
      <div class="subject-head" onclick="toggleSubject(this)">
        <div class="subject-head-left">
          <span class="subject-num">05</span>
          <h3>Sistemas Digitales I</h3>
          <span class="subject-stars" style="color:#B98A25;">★★★★☆</span>
          <span class="head-bar-track"><span class="head-bar-fill" data-head-bar="sistemas" style="width:0%; background:var(--amber);"></span></span>
        </div>
        <svg class="chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>
      </div>
      <div class="subject-body">
        <div class="subject-body-inner">
          <p class="why-box">Vienes con cierta ventaja por programación y algo de electrónica. Pero es la materia más dispersa de las cinco: no hay un único libro guía, hay muchas bases sueltas.</p>

          <div class="col-heading">Temas en orden <span class="subject-progress" data-progress-label="sistemas">0/5</span></div>
          <ul class="topics" data-subject="sistemas">
            <li class="topic-row"><input type="checkbox" id="sistemas-0" data-subject="sistemas" data-idx="0"><label for="sistemas-0">Sistemas numéricos: decimal, binario, octal, hexadecimal — aprende a convertir entre todos.</label></li>
            <li class="topic-row"><input type="checkbox" id="sistemas-1" data-subject="sistemas" data-idx="1"><label for="sistemas-1">Álgebra de Boole: AND, OR, NOT, NAND, NOR, XOR.</label></li>
            <li class="topic-row"><input type="checkbox" id="sistemas-2" data-subject="sistemas" data-idx="2"><label for="sistemas-2">Tablas de verdad — muchas, hasta que sean automáticas.</label></li>
            <li class="topic-row"><input type="checkbox" id="sistemas-3" data-subject="sistemas" data-idx="3"><label for="sistemas-3">Mapas de Karnaugh — para simplificar circuitos.</label></li>
            <li class="topic-row"><input type="checkbox" id="sistemas-4" data-subject="sistemas" data-idx="4"><label for="sistemas-4">Circuitos combinacionales: multiplexores, demultiplexores, codificadores, decodificadores.</label></li>
          </ul>

          <div class="col-heading">Recursos</div>
          <div class="resource-row"><span class="tag">YOUTUBE</span><span>Unicrom · Ingeniería Electrónica · Neso Academy.</span></div>

          <div class="col-heading">Plan de estudio</div>
          <p class="plan-line">2 horas semanales.</p>

          <div class="yamil-note warn">En este curso sí se rescatan cosas de Circuitos I, pero acá hay muchas bases y no es tan lineal con un libro en específico — no busques "el" libro guía como en las otras materias.</div>
        </div>
      </div>
    </div>
  </section>

  <section class="schedule" id="cronograma">
    <div class="eyebrow">Semana tipo</div>
    <h2 style="font-size:26px; margin-top:6px;">Cronograma de vacaciones</h2>
    <p style="color:var(--ink-soft); font-size:15px; max-width:600px; margin-top:8px;">Ajustado al orden de prioridad real. Si tu Estadística es la básica, mueve ese bloque del miércoles hacia Ecuaciones o un repaso libre.</p>

    <div class="schedule-grid">
      <div class="day-col"><div class="day-name">Lun</div><div class="cell circ">Circuitos · 2h</div></div>
      <div class="day-col"><div class="day-name">Mar</div><div class="cell fis">Física · 2h</div></div>
      <div class="day-col"><div class="day-name">Mié</div><div class="cell est">Estadística* · 2h</div></div>
      <div class="day-col"><div class="day-name">Jue</div><div class="cell circ">Circuitos · 2h</div></div>
      <div class="day-col"><div class="day-name">Vie</div><div class="cell sis">Sistemas · 2h</div></div>
      <div class="day-col"><div class="day-name">Sáb</div><div class="cell fis">Física (ejerc.) · 1-2h</div><div class="cell edo" style="margin-top:6px;">Ecuaciones · 2h</div></div>
    </div>
    <div class="legend">
      <span><i style="background:var(--copper-bright)"></i>Circuitos I</span>
      <span><i style="background:var(--teal)"></i>Física</span>
      <span><i style="background:#5B6B8C"></i>Estadística</span>
      <span><i style="background:#7C8A55"></i>Ecuaciones Dif.</span>
      <span><i style="background:var(--amber)"></i>Sistemas Digit.</span>
    </div>
    <p style="font-size:12.5px; color:var(--ink-soft); margin-top:10px;">*Bloque condicional — solo si tu Estadística es la Inferencial. Si es la básica, cámbialo por repaso libre o refuerzo de Circuitos.</p>

    <div class="distribution">
      <div class="col-heading">Distribución sugerida del tiempo total</div>
      <div class="bar-row"><span class="bar-label">Circuitos I</span><div class="bar-track"><div class="bar-fill" style="width:40%; background:var(--copper-bright);"></div></div><span class="bar-pct">40%</span></div>
      <div class="bar-row"><span class="bar-label">Física</span><div class="bar-track"><div class="bar-fill" style="width:30%; background:var(--teal);"></div></div><span class="bar-pct">30%</span></div>
      <div class="bar-row"><span class="bar-label">Estadística / EDO</span><div class="bar-track"><div class="bar-fill" style="width:20%; background:#5B6B8C;"></div></div><span class="bar-pct">20%</span></div>
      <div class="bar-row"><span class="bar-label">Sistemas Digit.</span><div class="bar-track"><div class="bar-fill" style="width:10%; background:var(--amber);"></div></div><span class="bar-pct">10%</span></div>
    </div>
  </section>

  <section class="golden">
    <div class="chip">
      <span class="kicker">La clave de oro</span>
      <h2>No memorices fórmulas como recetas de cocina</h2>
      <p>Antes de pasar a la siguiente fórmula, pregúntate siempre:</p>
      <ul>
        <li>¿Qué significa físicamente esta fórmula?</li>
        <li>¿De dónde sale?</li>
        <li>¿Cuándo puedo usarla?</li>
        <li>¿Qué pasa si una variable aumenta o disminuye?</li>
      </ul>
      <p style="margin-top:16px;">Cuando respondes esas preguntas dejas de "hacer ejercicios" y empiezas a entender ingeniería — y esa diferencia se nota muchísimo cuando llegan los parciales difíciles.</p>
    </div>
  </section>

  <footer>
    <p>RUTA CONSTRUIDA A PARTIR DE DOS FUENTES · CRUZADA Y VERIFICADA CON EXPERIENCIA REAL DE CURSO</p>
  </footer>

</div>

<script>
  // ========== TOGGLE SUBJECTS ==========
  function toggleSubject(headEl){
    const card = headEl.parentElement;
    card.classList.toggle('open');
    updateSubjectStorage();
  }

  // ========== SUBJECTS CONFIG ==========
  const SUBJECTS = [
    {key:'circuitos', name:'Circuitos I', topics:7, color:'#9C5A28', weeklyTarget:4},
    {key:'fisica', name:'Física', topics:9, color:'#1F7A72', weeklyTarget:3},
    {key:'estadistica', name:'Estadística', topics:5, color:'#5B6B8C', weeklyTarget:2},
    {key:'edo', name:'Ecuaciones Dif.', topics:7, color:'#7C8A55', weeklyTarget:2.5},
    {key:'sistemas', name:'Sistemas Digit.', topics:5, color:'#B98A25', weeklyTarget:2}
  ];
  const TOTAL_TOPICS = SUBJECTS.reduce((a,s)=>a+s.topics,0);

  // ========== STATE & STORAGE ==========
  let state = { progress:{}, hours:{}, semesterDate:'', expandedSubjects:{} };
  SUBJECTS.forEach(s=>{ state.progress[s.key]=[]; state.hours[s.key]=0; });

  function loadState(){
    try{
      const saved = localStorage.getItem('study-data');
      if(saved){
        const parsed = JSON.parse(saved);
        state = Object.assign(state, parsed);
        SUBJECTS.forEach(s=>{
          if(!state.progress[s.key]) state.progress[s.key]=[];
          if(state.hours[s.key]===undefined) state.hours[s.key]=0;
        });
      }
    }catch(e){ 
      console.error('Error cargando datos:', e);
    }
    render();
  }

  function saveState(){
    try{
      localStorage.setItem('study-data', JSON.stringify(state));
    }catch(e){ 
      console.error('Error guardando datos:', e);
    }
  }

  // ========== RENDER FUNCTION ==========
  function render(){
    // ===== Render checkboxes =====
    document.querySelectorAll('.topic-row input[type=checkbox]').forEach(cb=>{
      const subj = cb.dataset.subject, idx = parseInt(cb.dataset.idx,10);
      const checked = !!state.progress[subj][idx];
      cb.checked = checked;
      cb.closest('.topic-row').classList.toggle('checked', checked);
    });

    // ===== Render progress labels & header bars =====
    let totalDone = 0;
    SUBJECTS.forEach(s=>{
      const done = state.progress[s.key].filter(Boolean).length;
      totalDone += done;
      document.querySelectorAll(`[data-progress-label="${s.key}"]`).forEach(el=>{
        el.textContent = `${done}/${s.topics}`;
      });
      document.querySelectorAll(`[data-head-bar="${s.key}"]`).forEach(el=>{
        el.style.width = (done/s.topics*100)+'%';
      });
    });
    
    // ===== Update overall progress =====
    const progressPct = totalDone/TOTAL_TOPICS*100;
    document.getElementById('overallFill').style.width = progressPct+'%';
    document.getElementById('overallPct').textContent = `${totalDone}/${TOTAL_TOPICS} temas completados (${Math.round(progressPct)}%)`;

    // ===== Render hours panel =====
    const hoursList = document.getElementById('hoursList');
    hoursList.innerHTML = '';
    let totalHours = 0;
    SUBJECTS.forEach(s=>{
      const total = state.hours[s.key] || 0;
      totalHours += total;
      const target = s.weeklyTarget * 4; // ~4 semanas vacaciones
      const pct = Math.min(100, (total/target)*100);
      const row = document.createElement('div');
      row.className = 'hours-item';
      const targetDisplay = target > 0 ? `/${target}h` : '';
      row.innerHTML = `
        <span class="h-name">${s.name}</span>
        <div class="h-track"><div class="h-fill" style="width:${pct}%; background:${s.color};"></div></div>
        <span class="h-total">${total}h${targetDisplay}</span>
        <div class="h-btns">
          <button data-add="0.5" data-key="${s.key}" title="Agregar 30 minutos">+0.5h</button>
          <button data-add="1" data-key="${s.key}" title="Agregar 1 hora">+1h</button>
          <button class="reset" data-reset="${s.key}" title="Reiniciar horas">↺</button>
        </div>`;
      hoursList.appendChild(row);
    });
    
    // ===== Add event listeners to hours buttons =====
    hoursList.querySelectorAll('[data-add]').forEach(btn=>{
      btn.addEventListener('click', ()=>{
        const key = btn.dataset.key;
        state.hours[key] = Math.round(((state.hours[key]||0) + parseFloat(btn.dataset.add))*10)/10;
        saveState(); 
        render();
      });
    });
    
    hoursList.querySelectorAll('[data-reset]').forEach(btn=>{
      btn.addEventListener('click', ()=>{
        if(confirm(`¿Reiniciar horas de ${SUBJECTS.find(s=>s.key===btn.dataset.reset)?.name}?`)){
          const key = btn.dataset.reset;
          state.hours[key] = 0;
          saveState(); 
          render();
        }
      });
    });

    // ===== Update countdown & date input =====
    const dateInput = document.getElementById('semDate');
    if(state.semesterDate) dateInput.value = state.semesterDate;
    updateCountdown();
    
    // ===== Restore expanded subjects =====
    document.querySelectorAll('.subject').forEach((card, idx)=>{
      const key = SUBJECTS[idx]?.key;
      if(state.expandedSubjects[key]){
        card.classList.add('open');
      }
    });
  }

  // ========== COUNTDOWN TIMER ==========
  function updateCountdown(){
    const numEl = document.getElementById('countdownNum');
    const labelEl = document.getElementById('countdownLabel');
    
    if(!state.semesterDate){
      numEl.textContent = '—';
      labelEl.textContent = 'configura la fecha de inicio';
      return;
    }
    
    const today = new Date(); 
    today.setHours(0,0,0,0);
    const target = new Date(state.semesterDate + 'T00:00:00');
    const diffDays = Math.ceil((target - today) / (1000*60*60*24));
    
    if(diffDays > 0){
      numEl.textContent = diffDays;
      numEl.style.color = diffDays < 7 ? '#B5652D' : 'var(--copper-bright)';
      labelEl.textContent = diffDays === 1 ? 'día para el semestre' : 'días para el semestre';
    } else if(diffDays === 0){
      numEl.textContent = '¡HOY!';
      numEl.style.color = '#B98A25';
      labelEl.textContent = '¡Empieza el semestre!';
    } else {
      numEl.textContent = '0';
      numEl.style.color = '#a05';
      labelEl.textContent = 'el semestre ya comenzó';
    }
  }

  function updateSubjectStorage(){
    document.querySelectorAll('.subject').forEach((card, idx)=>{
      const key = SUBJECTS[idx]?.key;
      if(key) state.expandedSubjects[key] = card.classList.contains('open');
    });
    saveState();
  }

  // ========== EVENT LISTENERS ==========
  document.addEventListener('change', (e)=>{
    // Handle topic checkboxes
    if(e.target.matches('.topic-row input[type=checkbox]')){
      const subj = e.target.dataset.subject, idx = parseInt(e.target.dataset.idx,10);
      state.progress[subj][idx] = e.target.checked;
      saveState(); 
      render();
    }
    
    // Handle semester date input
    if(e.target.id === 'semDate'){
      state.semesterDate = e.target.value;
      saveState(); 
      updateCountdown();
    }
  });

  // Real-time countdown updates
  setInterval(updateCountdown, 60000); // Update every minute

  // Keyboard shortcuts
  document.addEventListener('keydown', (e)=>{
    if(e.ctrlKey && e.key === 's'){
      e.preventDefault();
      alert('✓ Datos guardados automáticamente en tu navegador');
    }
  });

  // ========== INITIALIZATION ==========
  window.addEventListener('load', loadState);
  
  // Auto-save on page unload
  window.addEventListener('beforeunload', saveState);

  // Warn if data exists
  window.addEventListener('load', ()=>{
    const saved = localStorage.getItem('study-data');
    if(saved){
      const data = JSON.parse(saved);
      if(data.progress && Object.values(data.progress).some(arr => arr.some(Boolean))){
        console.log('✓ Datos guardados encontrados — continuando tu progreso');
      }
    }
  });
</script>

</body>
</html>
