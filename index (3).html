<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GYVA Eco Estate | Barefoot Luxury & Private Lodges · Coto Brus, Costa Rica</title>
<meta name="description" content="GYVA Eco Estate — Refugio privado en el sur de Coto Brus, Puntarenas. Cabañas de madera, senderos llenos de naturaleza, gastronomía farm-to-table y fogatas bajo las estrellas.">
<meta property="og:title" content="GYVA Eco Estate | Barefoot Luxury & Private Lodges">
<meta property="og:description" content="Refugio privado en el corazón de la montaña. Coto Brus, Costa Rica.">
<meta property="og:type" content="website">

<script src="https://cdn.tailwindcss.com"></script>
<script>
tailwind.config = {
  theme: { extend: {
    colors: {
      brand: {
        forest: '#1A3A2E', deep: '#122A21', mid: '#22493A',
        sage: '#6B7F6A', sand: '#DCDCD0', cream: '#F4F1EA',
        wood: '#6B4D30', gold: '#C8A145', goldlight: '#E0C27A', golddark: '#9A7B2A'
      }
    },
    fontFamily: {
      serif: ['Cormorant Garamond', 'Georgia', 'serif'],
      sans: ['Plus Jakarta Sans', 'sans-serif']
    }
  }}
}
</script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<style>
  body{font-family:'Plus Jakarta Sans',sans-serif;background:#122A21;color:#F4F1EA}
  h1,h2,h3,h4,.font-serif{font-family:'Cormorant Garamond','Georgia',serif}
  section[id]{scroll-margin-top:92px}

  .gold-text{background:linear-gradient(120deg,#EBD9AC 0%,#C8A145 48%,#9A7B2A 100%);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
  .gold-btn{background:linear-gradient(135deg,#D9BA68 0%,#C8A145 55%,#A98432 100%);transition:all .3s ease}
  .gold-btn:hover{box-shadow:0 12px 34px rgba(200,161,69,.35);transform:translateY(-1px)}

  ::-webkit-scrollbar{width:9px}
  ::-webkit-scrollbar-track{background:#122A21}
  ::-webkit-scrollbar-thumb{background:#1A3A2E;border-radius:4px;border:1px solid rgba(200,161,69,.35)}

  .reveal{opacity:0;transform:translateY(26px);transition:.8s cubic-bezier(.2,.7,.2,1)}
  .reveal.visible{opacity:1;transform:none}

  input[type="date"]::-webkit-calendar-picker-indicator{filter:invert(72%) sepia(60%) saturate(400%) hue-rotate(-15deg);cursor:pointer}

  /* ---------- Mapa 3D Realista ---------- */
  #stage3d{perspective:1500px;perspective-origin:50% 45%;touch-action:none;
    background:radial-gradient(circle at 50% 40%,#1B382A 0%,#0A1912 80%)}
  #plane3d{transform-style:preserve-3d;will-change:transform;transition:transform .08s linear}
  #plane3d svg{pointer-events:none;user-select:none}
  #mapFrame{height:100%;aspect-ratio:1/1;max-width:100%;position:absolute;inset:0;margin:auto}

  .spot{position:absolute;left:var(--x);top:var(--y);transform:translate(-50%,-50%);
    display:flex;flex-direction:column;align-items:center;gap:7px;background:none;border:0;cursor:pointer;z-index:5}
  .spot-dot{width:16px;height:16px;border-radius:9999px;background:#C8A145;position:relative;
    box-shadow:0 0 0 5px rgba(200,161,69,.3),0 0 18px rgba(200,161,69,1)}
  .spot-dot::after{content:'';position:absolute;inset:-6px;border-radius:9999px;
    border:1px solid rgba(200,161,69,.7);animation:pulse 2.4s infinite ease-out}
  @keyframes pulse{0%{transform:scale(.7);opacity:.9}100%{transform:scale(2.2);opacity:0}}
  .spot-label{white-space:nowrap;font-size:10px;letter-spacing:.14em;text-transform:uppercase;font-weight:600;
    color:#F0E6CD;background:rgba(18,42,33,.92);border:1px solid rgba(200,161,69,.6);
    padding:4px 10px;border-radius:9999px;box-shadow:0 6px 18px rgba(0,0,0,.5);
    transform:rotateZ(calc(-1 * var(--rot,0deg))) rotateX(calc(-1 * var(--tilt,0deg)));
    transition:opacity .25s,background .25s,color .25s}
  .spot:hover .spot-label,.spot.active .spot-label{background:#C8A145;color:#122A21;border-color:#C8A145}
  .spot.active .spot-dot{background:#fff;box-shadow:0 0 0 6px rgba(200,161,69,.5),0 0 24px #fff}
  #plane3d.labels-off .spot-label{opacity:0;pointer-events:none}

  .ctrl-btn{display:inline-flex;align-items:center;justify-content:center;gap:.4rem;height:38px;padding:0 14px;
    border-radius:12px;background:#fff;border:1px solid rgba(26,58,46,.18);color:#1A3A2E;
    font-size:12px;font-weight:600;letter-spacing:.08em;transition:.2s}
  .ctrl-btn:hover,.ctrl-btn.active{background:#1A3A2E;color:#C8A145;border-color:#1A3A2E}
  input[type=range]{accent-color:#1A3A2E}
  .legend-chip{transition:.2s;cursor:pointer}
  .legend-chip:hover,.legend-chip.active{background:#1A3A2E;color:#C8A145;border-color:#1A3A2E}
</style>
</head>
<body class="antialiased selection:bg-brand-gold selection:text-brand-forest">

<!-- ============ HEADER ============ -->
<header class="fixed top-0 left-0 w-full z-50 bg-brand-deep/90 backdrop-blur-md border-b border-brand-gold/20">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-[92px] flex items-center justify-between">
    <a href="#inicio" class="flex items-center gap-3 group">
      <svg viewBox="0 0 64 80" class="w-8 h-11 text-brand-gold group-hover:scale-105 transition-transform" fill="none" aria-hidden="true">
        <path d="M32 6C46 20 56 33 56 47c0 15-11 27-24 27S8 62 8 47C8 33 18 20 32 6Z" stroke="currentColor" stroke-width="2.4"/>
        <path d="M32 66V34" stroke="currentColor" stroke-width="2.4" stroke-linecap="round"/>
        <path d="M32 50c-8-1-13-6-14-15 8 1 13 6 14 15Z" fill="currentColor"/>
        <path d="M32 42c8-1 13-6 14-15-8 1-13 6-14 15Z" fill="currentColor"/>
      </svg>
      <div class="flex flex-col leading-none">
        <span class="font-serif text-[26px] font-semibold tracking-[0.28em] text-brand-cream">GYVA</span>
        <span class="text-[8.5px] tracking-[0.42em] text-brand-gold uppercase mt-1">Eco Estate</span>
      </div>
    </a>

    <nav class="hidden lg:flex items-center space-x-8 text-[13px] font-medium tracking-wide">
      <a href="#inicio" class="text-brand-cream/80 hover:text-brand-gold transition">Inicio</a>
      <a href="#mapa3d" class="text-brand-cream/80 hover:text-brand-gold transition">Mapa 3D</a>
      <a href="#ubicacion" class="text-brand-cream/80 hover:text-brand-gold transition">Ruta</a>
      <a href="#tarifas" class="text-brand-cream/80 hover:text-brand-gold transition">Tarifas</a>
      <a href="#experiencia" class="text-brand-cream/80 hover:text-brand-gold transition">Experiencia</a>
    </nav>

    <a href="#reserva" class="hidden md:inline-flex gold-btn text-brand-deep font-semibold px-6 py-3 rounded-full text-[13px] items-center gap-2 tracking-wide">
      <i class="fa-regular fa-calendar-check text-xs"></i> Reservar estancia
    </a>

    <button id="mobile-menu-btn" class="lg:hidden text-brand-gold p-2" aria-label="Menú">
      <i class="fa-solid fa-bars text-2xl"></i>
    </button>
  </div>

  <div id="mobile-menu" class="hidden lg:hidden bg-brand-forest border-b border-brand-gold/20 px-4 pt-2 pb-6 space-y-1 text-sm">
    <a href="#inicio" class="block py-3 border-b border-white/10">Inicio</a>
    <a href="#mapa3d" class="block py-3 border-b border-white/10">Mapa 3D</a>
    <a href="#ubicacion" class="block py-3 border-b border-white/10">Ubicación y Ruta</a>
    <a href="#tarifas" class="block py-3 border-b border-white/10">Tarifas y Paquetes</a>
    <a href="#experiencia" class="block py-3 border-b border-white/10">La Experiencia</a>
    <a href="#reserva" class="block gold-btn text-center text-brand-deep font-semibold py-3 rounded-xl mt-4">Reservar ahora</a>
  </div>
</header>

<main class="pt-[92px]">

<!-- ============ HERO ============ -->
<section id="inicio" class="relative min-h-[92vh] flex items-center justify-center overflow-hidden py-20 px-4">
  <div class="absolute inset-0 z-0">
    <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?auto=format&fit=crop&q=80&w=2000"
         alt="Bosque tropical de montaña en Costa Rica"
         class="w-full h-full object-cover opacity-40">
    <div class="absolute inset-0 bg-gradient-to-t from-brand-deep via-brand-deep/80 to-brand-deep/30"></div>
  </div>

  <div class="relative z-10 max-w-4xl mx-auto text-center space-y-8 reveal">
    <div class="inline-flex items-center gap-2 px-5 py-2 rounded-full border border-brand-gold/40 bg-brand-forest/50 text-brand-gold text-[10px] font-semibold uppercase tracking-[0.28em]">
      <i class="fa-solid fa-tree"></i> Coto Brus · Puntarenas · Costa Rica
    </div>

    <h1 class="text-[42px] sm:text-6xl lg:text-[76px] font-light leading-[1.02] text-white">
      Refugio privado en el<br class="hidden sm:block">
      <span class="gold-text italic font-normal">sur de Costa Rica</span>
    </h1>

    <p class="text-base sm:text-lg text-brand-cream/75 max-w-2xl mx-auto font-light leading-relaxed">
      Cabañas de madera, senderos llenos de naturaleza y gastronomía de la huerta a la mesa.
      Un santuario de bienestar entre las montañas del sur de Costa Rica.
    </p>

    <p class="text-[10px] tracking-[0.45em] uppercase text-brand-gold/80">Barefoot Luxury &amp; Private Lodges</p>

    <div class="flex flex-col sm:flex-row justify-center gap-4 pt-2">
      <a href="#reserva" class="gold-btn text-brand-deep font-bold px-9 py-4 rounded-full flex items-center justify-center gap-3 text-sm tracking-wide">
        Planificar tu visita <i class="fa-solid fa-arrow-right text-xs"></i>
      </a>
      <a href="#mapa3d" class="bg-white/5 hover:bg-white/10 border border-brand-gold/35 px-9 py-4 rounded-full flex items-center justify-center gap-2 text-sm tracking-wide transition backdrop-blur-sm">
        <i class="fa-solid fa-cube text-brand-gold"></i> Explorar el mapa 3D
      </a>
    </div>

    <div class="grid grid-cols-2 md:grid-cols-4 gap-4 pt-12 border-t border-brand-gold/20 max-w-3xl mx-auto">
      <div><p class="font-serif text-2xl text-brand-gold">05</p><p class="text-[10px] uppercase tracking-[0.22em] text-brand-cream/60">Cabañas privadas</p></div>
      <div><p class="font-serif text-2xl text-brand-gold">3,5 he</p><p class="text-[10px] uppercase tracking-[0.22em] text-brand-cream/60">Bosque protegido</p></div>
      <div><p class="font-serif text-2xl text-brand-gold">827 m</p><p class="text-[10px] uppercase tracking-[0.22em] text-brand-cream/60">Sobre el nivel del mar</p></div>
      <div><p id="hero-time" class="font-serif text-2xl text-brand-gold">≈ 5 h</p><p class="text-[10px] uppercase tracking-[0.22em] text-brand-cream/60">Desde el SJO</p></div>
    </div>
  </div>
</section>

<!-- ============ MAPA 3D REALISTA (SVG AVANZADO) ============ -->
<section id="mapa3d" class="py-20 px-4 sm:px-6 lg:px-8 bg-brand-sand text-brand-forest">
  <div class="max-w-7xl mx-auto space-y-8">

    <div class="text-center max-w-3xl mx-auto space-y-4 reveal">
      <span class="text-[10px] uppercase tracking-[0.35em] font-semibold text-brand-wood">Recorre la finca</span>
      <h2 class="text-3xl sm:text-5xl font-light text-brand-forest">Mapa interactivo <span class="italic text-brand-wood">3D</span></h2>
      <div class="w-20 h-px bg-brand-forest/40 mx-auto"></div>
      <p class="text-brand-forest/70 text-sm sm:text-base font-light">
        Arrastra para desplazarte, acerca con la rueda o los botones, ajusta la inclinación y explora las 5 cabañas y áreas con renderizado de iluminación realista.
      </p>
    </div>

    <!-- Controles -->
    <div class="flex flex-wrap items-center justify-between gap-3 bg-white/60 border border-brand-forest/15 rounded-2xl p-3 backdrop-blur reveal">
      <div class="flex items-center gap-2">
        <button onclick="zoomBy(0.85)" class="ctrl-btn" title="Alejar"><i class="fa-solid fa-minus"></i></button>
        <button onclick="zoomBy(1.18)" class="ctrl-btn" title="Acercar"><i class="fa-solid fa-plus"></i></button>
        <button onclick="resetView()" class="ctrl-btn text-[10px] uppercase tracking-[0.14em]"><i class="fa-solid fa-rotate-left text-[10px]"></i> Restablecer</button>
      </div>
      <div class="flex items-center gap-3 px-1">
        <label for="tiltRange" class="text-[10px] uppercase tracking-[0.18em] font-semibold text-brand-forest/70">Inclinación 3D</label>
        <input id="tiltRange" type="range" min="0" max="58" value="30" class="w-28 sm:w-40">
      </div>
      <div class="flex items-center gap-2">
        <button onclick="toggleLabels()" id="labelsBtn" class="ctrl-btn text-[10px] uppercase tracking-[0.14em]"><i class="fa-solid fa-tags text-[10px]"></i> Etiquetas</button>
      </div>
    </div>

    <!-- Escenario 3D -->
    <div id="stage3d" class="relative w-full aspect-[4/3] sm:aspect-[16/10] max-h-[520px] sm:max-h-[750px] rounded-3xl overflow-hidden border border-brand-forest/25 shadow-2xl cursor-grab select-none">

      <div id="plane3d" class="absolute inset-0 origin-center">
        <div id="mapFrame">

          <!-- MAPA ILUSTRADO HIPERREALISTA DE ALTA DEFINICIÓN (SVG CON SHADOWS Y GRADIENTES ORGÁNICOS) -->
          <svg viewBox="0 0 1000 1000" preserveAspectRatio="xMidYMid slice" class="w-full h-full rounded-2xl shadow-2xl">
            <defs>
              <linearGradient id="grassGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                <stop offset="0%" stop-color="#2D523A"/>
                <stop offset="40%" stop-color="#21402D"/>
                <stop offset="80%" stop-color="#183122"/>
                <stop offset="100%" stop-color="#0F2117"/>
              </linearGradient>

              <linearGradient id="roofWood" x1="0%" y1="0%" x2="100%" y2="100%">
                <stop offset="0%" stop-color="#543A24"/>
                <stop offset="50%" stop-color="#3B2818"/>
                <stop offset="100%" stop-color="#24180E"/>
              </linearGradient>

              <radialGradient id="glowWarm" cx="50%" cy="50%" r="50%">
                <stop offset="0%" stop-color="#FFEBB3" stop-opacity="0.85"/>
                <stop offset="35%" stop-color="#F2C45A" stop-opacity="0.45"/>
                <stop offset="70%" stop-color="#C8A145" stop-opacity="0.15"/>
                <stop offset="100%" stop-color="#C8A145" stop-opacity="0"/>
              </radialGradient>

              <radialGradient id="fireReal" cx="50%" cy="50%" r="50%">
                <stop offset="0%" stop-color="#FFF2A3" stop-opacity="1"/>
                <stop offset="30%" stop-color="#FF9900" stop-opacity="0.85"/>
                <stop offset="60%" stop-color="#FF3300" stop-opacity="0.5"/>
                <stop offset="100%" stop-color="#D92600" stop-opacity="0"/>
              </radialGradient>

              <radialGradient id="treeShadow" cx="50%" cy="50%" r="50%">
                <stop offset="0%" stop-color="#000" stop-opacity="0.7"/>
                <stop offset="100%" stop-color="#000" stop-opacity="0"/>
              </radialGradient>

              <filter id="realShadow" x="-30%" y="-30%" width="160%" height="160%">
                <feDropShadow dx="2" dy="16" stdDeviation="10" flood-color="#050C08" flood-opacity="0.85"/>
              </filter>
            </defs>

            <!-- Terreno y Vegetación Base -->
            <rect width="1000" height="1000" fill="url(#grassGrad)"/>

            <!-- Masa Boscosa Perimetral Tupida -->
            <g fill="#10241A" opacity="0.85">
              <circle cx="80" cy="120" r="180"/> <circle cx="50" cy="400" r="160"/>
              <circle cx="90" cy="750" r="190"/> <circle cx="920" cy="100" r="170"/>
              <circle cx="950" cy="450" r="180"/> <circle cx="910" cy="850" r="200"/>
              <circle cx="500" cy="20" r="120"/>
            </g>

            <!-- Capa de copas de árboles con sombras 3D -->
            <g filter="url(#realShadow)">
              <!-- Arboles zona izquierda -->
              <circle cx="140" cy="220" r="45" fill="#1C3829"/> <circle cx="110" cy="520" r="50" fill="#183124"/>
              <circle cx="160" cy="820" r="55" fill="#14281D"/>
              <!-- Arboles zona derecha -->
              <circle cx="860" cy="200" r="48" fill="#1C3829"/> <circle cx="890" cy="580" r="52" fill="#183124"/>
              <circle cx="840" cy="890" r="60" fill="#14281D"/>
            </g>

            <!-- Carretera Exterior de Tierra y Piedra -->
            <path d="M 100 990 L 640 840 L 990 600" fill="none" stroke="#4D3B2A" stroke-width="48" stroke-linecap="round"/>
            <path d="M 100 990 L 640 840 L 990 600" fill="none" stroke="#69533D" stroke-width="36" stroke-linecap="round"/>

            <!-- Cerca de Madera que rodea la finca privada -->
            <path d="M 280 160 Q 480 50 740 60 Q 720 370 650 580 L 620 900 L 400 930 L 80 920 Q 230 520 280 160 Z"
                  fill="#1D3B2A" stroke="#7A5E3C" stroke-width="7" stroke-dasharray="16 12" filter="url(#realShadow)"/>

            <!-- Senderos de Piedra Orgánicos entre áreas -->
            <path d="M 390 840 Q 420 740 470 650 Q 520 540 480 470 Q 440 400 520 320 Q 580 260 620 160 Q 520 120 330 150"
                  fill="none" stroke="#D1C29B" stroke-width="14" stroke-dasharray="10 14" stroke-linecap="round" opacity="0.85"/>
            <path d="M 480 470 L 600 450" fill="none" stroke="#D1C29B" stroke-width="12" stroke-dasharray="8 12" opacity="0.85"/>
            <path d="M 520 320 L 420 250" fill="none" stroke="#D1C29B" stroke-width="12" stroke-dasharray="8 12" opacity="0.85"/>

            <!-- 1. TARIMA DE YOGA (Arriba Izquierda) -->
            <g id="svg-yoga" filter="url(#realShadow)">
              <ellipse cx="330" cy="165" rx="52" ry="20" fill="url(#treeShadow)"/>
              <circle cx="330" cy="150" r="50" fill="#422D1B" stroke="#694B2E" stroke-width="6"/>
              <circle cx="330" cy="150" r="42" fill="#694B2E" stroke="#C8A145" stroke-width="2"/>
              <circle cx="330" cy="150" r="26" fill="none" stroke="#FFE5A3" stroke-width="2" stroke-dasharray="8 5"/>
              <!-- Faroles de luz cálida -->
              <circle cx="288" cy="130" r="5" fill="#FFEBB3"/> <circle cx="372" cy="130" r="5" fill="#FFEBB3"/>
              <circle cx="372" cy="170" r="5" fill="#FFEBB3"/> <circle cx="288" cy="170" r="5" fill="#FFEBB3"/>
            </g>

            <!-- 2. LAS 5 CABAÑAS DE HOSPEDAJE (Estructuras 3D con Ventanales Iluminados) -->
            <!-- Cabaña 1 (Arriba Derecha) -->
            <g id="svg-cabana1" filter="url(#realShadow)">
              <circle cx="640" cy="120" r="65" fill="url(#glowWarm)"/>
              <rect x="595" y="90" width="90" height="55" rx="6" fill="url(#roofWood)" stroke="#523924" stroke-width="3"/>
              <polygon points="585,90 640,50 695,90" fill="#193626" stroke="#2B543E" stroke-width="3"/>
              <rect x="612" y="105" width="22" height="24" rx="2" fill="#FFE5A3"/>
              <rect x="646" y="105" width="22" height="24" rx="2" fill="#FFE5A3"/>
            </g>

            <!-- Cabaña 2 (Centro Arriba) -->
            <g id="svg-cabana2" filter="url(#realShadow)">
              <circle cx="450" cy="240" r="65" fill="url(#glowWarm)"/>
              <rect x="405" y="210" width="90" height="55" rx="6" fill="url(#roofWood)" stroke="#523924" stroke-width="3"/>
              <polygon points="395,210 450,170 505,210" fill="#193626" stroke="#2B543E" stroke-width="3"/>
              <rect x="422" y="225" width="22" height="24" rx="2" fill="#FFE5A3"/>
              <rect x="456" y="225" width="22" height="24" rx="2" fill="#FFE5A3"/>
            </g>

            <!-- Cabaña 3 (Centro Derecha) -->
            <g id="svg-cabana3" filter="url(#realShadow)">
              <circle cx="620" cy="310" r="65" fill="url(#glowWarm)"/>
              <rect x="575" y="280" width="90" height="55" rx="6" fill="url(#roofWood)" stroke="#523924" stroke-width="3"/>
              <polygon points="565,280 620,240 675,280" fill="#193626" stroke="#2B543E" stroke-width="3"/>
              <rect x="592" y="295" width="22" height="24" rx="2" fill="#FFE5A3"/>
              <rect x="626" y="295" width="22" height="24" rx="2" fill="#FFE5A3"/>
            </g>

            <!-- Cabaña 4 (Centro Medio) -->
            <g id="svg-cabana4" filter="url(#realShadow)">
              <circle cx="480" cy="380" r="65" fill="url(#glowWarm)"/>
              <rect x="435" y="350" width="90" height="55" rx="6" fill="url(#roofWood)" stroke="#523924" stroke-width="3"/>
              <polygon points="425,350 480,310 535,350" fill="#193626" stroke="#2B543E" stroke-width="3"/>
              <rect x="452" y="365" width="22" height="24" rx="2" fill="#FFE5A3"/>
              <rect x="486" y="365" width="22" height="24" rx="2" fill="#FFE5A3"/>
            </g>

            <!-- Cabaña 5 (Centro Abajo) -->
            <g id="svg-cabana5" filter="url(#realShadow)">
              <circle cx="470" cy="530" r="65" fill="url(#glowWarm)"/>
              <rect x="425" y="500" width="90" height="55" rx="6" fill="url(#roofWood)" stroke="#523924" stroke-width="3"/>
              <polygon points="415,500 470,460 525,500" fill="#193626" stroke="#2B543E" stroke-width="3"/>
              <rect x="442" y="515" width="22" height="24" rx="2" fill="#FFE5A3"/>
              <rect x="476" y="515" width="22" height="24" rx="2" fill="#FFE5A3"/>
            </g>

            <!-- 3. FOGATA COMUNAL (Efecto de Fuego Realista) -->
            <g id="svg-fogata" filter="url(#realShadow)">
              <circle cx="610" cy="450" r="75" fill="url(#fireReal)"/>
              <circle cx="610" cy="450" r="32" fill="#241B13" stroke="#6B5743" stroke-width="7"/>
              <circle cx="610" cy="450" r="14" fill="#FFF2A3"/>
              <!-- Asientos de madera alrededor -->
              <rect x="560" y="442" width="18" height="16" rx="4" fill="#422D1B"/>
              <rect x="642" y="442" width="18" height="16" rx="4" fill="#422D1B"/>
              <rect x="602" y="400" width="16" height="18" rx="4" fill="#422D1B"/>
              <rect x="602" y="482" width="16" height="18" rx="4" fill="#422D1B"/>
            </g>

            <!-- 4. EDIFICIO CENTRAL (Complejo con Restaurante, Recepción y Minimercado) -->
            <g id="svg-central" filter="url(#realShadow)">
              <circle cx="430" cy="700" r="140" fill="url(#glowWarm)"/>
              <rect x="300" y="650" width="260" height="100" rx="10" fill="url(#roofWood)" stroke="#523924" stroke-width="4"/>
              <polygon points="280,650 430,570 580,660" fill="#173625" stroke="#2B543E" stroke-width="4"/>
              <!-- Grandes Ventanales con luz cálida interior -->
              <rect x="320" y="675" width="45" height="55" rx="4" fill="#FFE5A3"/>
              <rect x="375" y="675" width="45" height="55" rx="4" fill="#FFE5A3"/>
              <rect x="440" y="675" width="45" height="55" rx="4" fill="#FFE5A3"/>
              <rect x="495" y="675" width="45" height="55" rx="4" fill="#FFE5A3"/>
            </g>

            <!-- 5. ESTACIONAMIENTO (Zona de Acceso) -->
            <g id="svg-parqueo" filter="url(#realShadow)">
              <rect x="170" y="730" width="160" height="100" rx="14" fill="#18241F" stroke="#334A40" stroke-width="3"/>
              <rect x="190" y="748" width="30" height="60" rx="6" fill="#364F47" stroke="#52756A" stroke-width="2"/>
              <rect x="235" y="748" width="30" height="60" rx="6" fill="#4B4E54" stroke="#71757E" stroke-width="2"/>
              <rect x="280" y="748" width="30" height="60" rx="6" fill="#25323D" stroke="#3F5363" stroke-width="2"/>
            </g>

            <!-- 6. CASETILLA DE GUARDIA Y ENTRADA PRINCIPAL -->
            <g id="svg-caseta" filter="url(#realShadow)">
              <circle cx="480" cy="850" r="40" fill="url(#glowWarm)"/>
              <rect x="450" y="825" width="60" height="45" rx="6" fill="url(#roofWood)" stroke="#523924" stroke-width="3"/>
              <polygon points="440,825 480,795 520,825" fill="#173625" stroke="#2B543E" stroke-width="3"/>
              <rect x="468" y="838" width="24" height="22" fill="#FFE5A3"/>
              <!-- Portón de Seguridad -->
              <rect x="400" y="885" width="160" height="14" rx="4" fill="#7A5E3C" stroke="#422D1B" stroke-width="3"/>
            </g>

          </svg>

          <!-- Hotspots interactivos alineados a las posiciones exactas -->
        </div>
      </div>

      <div id="mapHint" class="absolute top-4 left-1/2 -translate-x-1/2 z-20 pointer-events-none bg-brand-deep/80 backdrop-blur border border-brand-gold/40 text-brand-cream text-[10px] uppercase tracking-[0.22em] px-4 py-2 rounded-full transition-opacity duration-500">
        <i class="fa-solid fa-hand-pointer text-brand-gold mr-1"></i> Arrastra para explorar
      </div>

      <div id="spotPanel" class="hidden absolute z-30 left-4 right-4 bottom-4 sm:left-6 sm:bottom-6 sm:right-auto sm:max-w-sm bg-brand-deep/95 backdrop-blur border border-brand-gold/40 rounded-2xl p-5 text-brand-cream shadow-2xl">
        <button onclick="closeSpot()" class="absolute top-3 right-3 text-brand-gold/60 hover:text-brand-gold" aria-label="Cerrar">
          <i class="fa-solid fa-xmark"></i>
        </button>
        <div class="flex items-center gap-3 mb-2 pr-6">
          <span id="spotIcon" class="w-10 h-10 shrink-0 rounded-full bg-brand-gold/15 border border-brand-gold/50 text-brand-gold flex items-center justify-center">
            <i class="fa-solid fa-leaf"></i>
          </span>
          <div>
            <p id="spotTag" class="text-[9px] uppercase tracking-[0.24em] text-brand-gold/80"></p>
            <h4 id="spotTitle" class="font-serif text-xl text-white leading-tight"></h4>
          </div>
        </div>
        <p id="spotDesc" class="text-xs text-brand-cream/80 leading-relaxed"></p>
      </div>
    </div>

    <div id="legend" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-3 reveal"></div>

    <div class="flex flex-col sm:flex-row items-center justify-between gap-3 bg-white/50 border border-brand-forest/15 rounded-2xl p-4 text-[11px] text-brand-forest/65 font-light">
      <p><i class="fa-solid fa-circle-info text-brand-wood mr-1"></i> Render Vectorial 3D de alta definición de las 5 cabañas y áreas de GYVA Eco Estate.</p>
      <span class="text-brand-forest/40">Plano interactivo · Coto Brus</span>
    </div>
  </div>
</section>

<!-- ============ UBICACIÓN Y RUTA ============ -->
<section id="ubicacion" class="py-20 px-4 sm:px-6 lg:px-8 bg-brand-deep border-y border-brand-gold/10">
  <div class="max-w-7xl mx-auto space-y-12">

    <div class="text-center max-w-3xl mx-auto space-y-4 reveal">
      <span class="text-[10px] uppercase tracking-[0.35em] font-semibold text-brand-gold">Cómo llegar a GYVA</span>
      <h2 class="text-3xl sm:text-5xl font-light text-white">Ubicación y ruta guiada</h2>
      <div class="w-20 h-px bg-brand-gold/60 mx-auto"></div>
      <p class="text-brand-cream/70 text-sm sm:text-base font-light">Ruta recomendada desde el Aeropuerto Juan Santamaría (SJO) por la Interamericana Sur hasta Coto Brus.</p>
    </div>

    <div class="grid grid-cols-1 lg:grid-cols-3 gap-8 items-start">

      <div class="bg-brand-forest/60 p-6 rounded-2xl border border-brand-gold/20 space-y-4 shadow-xl reveal">
        <h3 class="font-serif text-xl text-brand-gold"><i class="fa-solid fa-route mr-2"></i>Resumen del trayecto</h3>

        <div class="flex gap-3 p-3 rounded-xl bg-brand-deep/60 border border-white/10 text-sm">
          <i class="fa-solid fa-plane-departure text-brand-gold mt-1"></i>
          <div>
            <p class="text-[10px] text-brand-gold/80 uppercase tracking-widest">Origen</p>
            <p class="font-semibold">Aeropuerto Juan Santamaría (SJO)</p>
            <p class="text-xs text-brand-cream/50">XQXW+73 Río Segundo, Alajuela</p>
            <p class="text-[10px] text-brand-cream/40 font-mono mt-0.5">9.9984, -84.2046</p>
          </div>
        </div>

        <div class="flex gap-3 p-3 rounded-xl bg-brand-deep/60 border border-brand-gold/40 text-sm">
          <i class="fa-solid fa-campground text-brand-gold mt-1"></i>
          <div>
            <p class="text-[10px] text-brand-gold/80 uppercase tracking-widest">Destino</p>
            <p class="font-semibold">GYVA Eco Estate</p>
            <p class="text-xs text-brand-cream/50">R2X5+JC Coto Brus, Puntarenas</p>
            <p class="text-[10px] text-brand-cream/40 font-mono mt-0.5">8.8491, -82.9914</p>
          </div>
        </div>

        <div class="grid grid-cols-2 gap-3">
          <div class="bg-brand-deep/60 p-3 rounded-xl border border-white/10 text-center">
            <i class="fa-solid fa-road text-brand-gold text-xs"></i>
            <span class="block text-[10px] text-brand-cream/60 uppercase tracking-widest mt-1">Distancia</span>
            <span id="route-km" class="font-serif text-lg">≈ 265 km</span>
          </div>
          <div class="bg-brand-deep/60 p-3 rounded-xl border border-white/10 text-center">
            <i class="fa-solid fa-clock text-brand-gold text-xs"></i>
            <span class="block text-[10px] text-brand-cream/60 uppercase tracking-widest mt-1">Tiempo</span>
            <span id="route-time" class="font-serif text-lg">≈ 5 h</span>
          </div>
        </div>

        <div class="grid grid-cols-2 gap-2 pt-1">
          <button onclick="showFullRouteView()" class="bg-brand-gold text-brand-deep font-semibold text-[11px] py-2.5 rounded-lg tracking-wide"><i class="fa-solid fa-map-location-dot mr-1"></i> Ruta completa</button>
          <button onclick="showEstateOnlyView()" class="bg-brand-deep border border-brand-gold/30 text-[11px] py-2.5 rounded-lg hover:text-brand-gold transition tracking-wide"><i class="fa-solid fa-location-pin mr-1"></i> Solo la finca</button>
        </div>

        <div class="grid grid-cols-2 gap-2">
          <a href="https://www.google.com/maps/dir/?api=1&origin=9.9984,-84.2046&destination=8.8491,-82.9914" target="_blank" rel="noopener" class="text-center bg-white/95 text-brand-forest text-[11px] font-bold py-2.5 rounded-lg hover:bg-white transition"><i class="fa-brands fa-google mr-1"></i> Google Maps</a>
          <a href="https://waze.com/ul?ll=8.8491,-82.9914&navigate=yes" target="_blank" rel="noopener" class="text-center bg-[#33ccff] text-black text-[11px] font-bold py-2.5 rounded-lg hover:brightness-105 transition"><i class="fa-brands fa-waze mr-1"></i> Abrir Waze</a>
        </div>

        <div class="bg-brand-deep/50 p-4 rounded-xl border border-white/10 text-xs space-y-2">
          <p class="font-bold text-brand-gold"><i class="fa-solid fa-car mr-1"></i> Consejos</p>
          <ul class="list-disc list-inside text-brand-cream/70 space-y-1">
            <li>Se recomienda vehículo 4x4 o SUV alto.</li>
            <li>Última gasolinera: San Vito de Coto Brus.</li>
            <li>Descarga el mapa: hay tramos sin señal.</li>
          </ul>
        </div>
      </div>

      <div class="lg:col-span-2 space-y-3 reveal">
        <div class="w-full h-[420px] sm:h-[560px] rounded-2xl overflow-hidden border border-brand-gold/30 shadow-2xl">
          <div id="map" class="w-full h-full z-0"></div>
        </div>
        <div class="flex flex-wrap justify-between text-[11px] text-brand-cream/60 px-2">
          <span><i class="fa-solid fa-circle text-emerald-500 text-[9px]"></i> Punto A: SJO</span>
          <span><i class="fa-solid fa-circle text-brand-gold text-[9px]"></i> Punto B: GYVA Eco Estate</span>
          <span class="text-brand-gold"><i class="fa-solid fa-compass"></i> Ruta real por carretera</span>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- ============ TARIFAS ============ -->
<section id="tarifas" class="py-20 px-4 sm:px-6 lg:px-8 bg-brand-sand text-brand-forest">
  <div class="max-w-7xl mx-auto space-y-12">

    <div class="text-center max-w-3xl mx-auto space-y-4 reveal">
      <span class="text-[10px] uppercase tracking-[0.35em] font-semibold text-brand-wood">Nuestras propuestas</span>
      <h2 class="text-3xl sm:text-5xl font-light text-brand-forest">Tarifas y paquetes</h2>
      <div class="w-20 h-px bg-brand-forest/40 mx-auto"></div>
      <p class="text-brand-forest/70 text-sm font-light">Precios por noche. Mínimo 2 noches en fines de semana y temporada alta.</p>
    </div>

    <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">

      <div class="bg-brand-cream rounded-3xl p-7 sm:p-9 border border-brand-forest/15 flex flex-col justify-between reveal">
        <div class="space-y-6">
          <div class="flex justify-between items-start">
            <div>
              <span class="text-[10px] font-semibold text-brand-wood uppercase tracking-[0.28em]">Opción 1</span>
              <h3 class="text-3xl font-normal text-brand-forest mt-1">Paquete Esencial</h3>
              <p class="text-xs text-brand-wood/80 italic">Self-Guided &amp; Libertad</p>
            </div>
            <div class="w-12 h-12 rounded-2xl bg-brand-forest/5 border border-brand-forest/15 flex items-center justify-center text-brand-wood text-xl">
              <i class="fa-solid fa-compass-drafting"></i>
            </div>
          </div>

          <p class="text-sm text-brand-forest/75 font-light">Para explorar a tu propio ritmo, con total confort y privacidad.</p>

          <ul class="space-y-2.5 text-sm text-brand-forest/85 border-y border-brand-forest/15 py-4">
            <li><i class="fa-solid fa-check text-brand-wood mr-2 text-xs"></i>Cabaña de madera sostenible</li>
            <li><i class="fa-solid fa-check text-brand-wood mr-2 text-xs"></i>Acceso ilimitado a los senderos privados</li>
            <li><i class="fa-solid fa-check text-brand-wood mr-2 text-xs"></i>Fogata comunal nocturna</li>
            <li><i class="fa-solid fa-check text-brand-wood mr-2 text-xs"></i>Desayuno artesanal diario</li>
          </ul>

          <div class="grid sm:grid-cols-2 gap-3">
            <div class="bg-white/70 p-4 rounded-xl border border-brand-forest/15">
              <span class="text-[11px] uppercase tracking-widest text-brand-forest/60">Cabaña de pareja</span>
              <div class="text-xl font-semibold text-brand-forest mt-1">$450 – $600 <span class="text-[10px] font-normal text-brand-wood">USD</span></div>
              <span class="text-[10px] text-brand-forest/50 block">~₡203,000 – ₡271,000 CRC</span>
            </div>
            <div class="bg-white/70 p-4 rounded-xl border border-brand-forest/15">
              <span class="text-[11px] uppercase tracking-widest text-brand-forest/60">Cabaña familiar</span>
              <div class="text-xl font-semibold text-brand-forest mt-1">$750 – $950 <span class="text-[10px] font-normal text-brand-wood">USD</span></div>
              <span class="text-[10px] text-brand-forest/50 block">~₡339,000 – ₡429,000 CRC</span>
            </div>
          </div>
        </div>

        <button onclick="selectPackageInForm('esencial')" class="mt-7 w-full border border-brand-forest/25 text-brand-forest font-semibold py-3.5 rounded-xl hover:bg-brand-forest hover:text-brand-gold transition text-sm tracking-wide">
          Seleccionar Esencial <i class="fa-solid fa-chevron-right text-[10px] ml-1"></i>
        </button>
      </div>

      <div class="bg-brand-forest text-brand-cream rounded-3xl p-7 sm:p-9 border-2 border-brand-gold flex flex-col justify-between relative shadow-2xl reveal">
        <div class="absolute top-0 right-0 bg-brand-gold text-brand-deep text-[9px] font-bold uppercase tracking-[0.22em] px-4 py-1.5 rounded-bl-xl">Recomendado</div>

        <div class="space-y-6">
          <div class="flex justify-between items-start">
            <div>
              <span class="text-[10px] font-semibold text-brand-gold uppercase tracking-[0.28em]">Opción 2</span>
              <h3 class="text-3xl font-normal text-white mt-1">Experiencia de la Casa</h3>
              <p class="text-xs text-brand-gold/90 italic">All-Inclusive Wellness &amp; Gourmet</p>
            </div>
            <div class="w-12 h-12 rounded-2xl bg-brand-gold/15 border border-brand-gold/60 flex items-center justify-center text-brand-gold text-xl">
              <i class="fa-solid fa-crown"></i>
            </div>
          </div>

          <p class="text-sm text-brand-cream/75 font-light">La vivencia inmersiva definitiva: cuidado personalizado, gastronomía orgánica y bienestar integral.</p>

          <ul class="space-y-2.5 text-sm text-brand-cream/90 border-y border-brand-gold/25 py-4">
            <li><i class="fa-solid fa-star text-brand-gold mr-2 text-xs"></i>Todas las comidas diarias <em>Farm-to-Table</em></li>
            <li><i class="fa-solid fa-star text-brand-gold mr-2 text-xs"></i>Guía naturalista privado: una caminata por los senderos llenos de naturaleza</li>
            <li><i class="fa-solid fa-star text-brand-gold mr-2 text-xs"></i>Instructor exclusivo de yoga y meditación</li>
            <li><i class="fa-solid fa-star text-brand-gold mr-2 text-xs"></i>Fogata privada con maridaje de vinos y tabla gourmet</li>
          </ul>

          <div class="grid sm:grid-cols-2 gap-3">
            <div class="bg-white/5 p-4 rounded-xl border border-brand-gold/35">
              <span class="text-[11px] uppercase tracking-widest text-brand-cream/55">Cabaña de pareja</span>
              <div class="text-xl font-semibold text-white mt-1">$850 – $1,100 <span class="text-[10px] font-normal text-brand-gold">USD</span></div>
              <span class="text-[10px] text-brand-gold/70 block">~₡384,000 – ₡497,000 CRC</span>
            </div>
            <div class="bg-white/5 p-4 rounded-xl border border-brand-gold/35">
              <span class="text-[11px] uppercase tracking-widest text-brand-cream/55">Cabaña familiar</span>
              <div class="text-xl font-semibold text-white mt-1">$1,300 – $1,700 <span class="text-[10px] font-normal text-brand-gold">USD</span></div>
              <span class="text-[10px] text-brand-gold/70 block">~₡587,000 – ₡768,000 CRC</span>
            </div>
          </div>
        </div>

        <button onclick="selectPackageInForm('experiencia')" class="mt-7 w-full gold-btn text-brand-deep font-bold py-3.5 rounded-xl shadow-lg text-sm tracking-wide">
          Seleccionar Experiencia <i class="fa-solid fa-chevron-right text-[10px] ml-1"></i>
        </button>
      </div>

    </div>
  </div>
</section>

<!-- ============ EXPERIENCIA (CON IMAGEN DE CABAÑA INTEGRADA) ============ -->
<section id="experiencia" class="py-20 px-4 sm:px-6 lg:px-8 bg-brand-deep border-t border-brand-gold/10">
  <div class="max-w-7xl mx-auto space-y-12">

    <div class="text-center max-w-3xl mx-auto space-y-4 reveal">
      <span class="text-[10px] uppercase tracking-[0.35em] font-semibold text-brand-gold">Atmósfera única</span>
      <h2 class="text-3xl sm:text-5xl font-light text-white">Esencia de montaña</h2>
      <div class="w-20 h-px bg-brand-gold/60 mx-auto"></div>
    </div>

    <div class="grid md:grid-cols-3 gap-6">

      <!-- TARJETA 1: CABAÑA DE MADERA CON IMAGEN DE CABAÑA DE HOSPITALIDAD REAL -->
      <article class="bg-brand-forest/50 rounded-2xl overflow-hidden border border-brand-gold/15 group reveal shadow-xl">
        <div class="h-60 overflow-hidden relative">
          <img src="https://images.unsplash.com/photo-1587061949409-02df41d5e562?auto=format&fit=crop&q=80&w=1000"
               alt="Cabaña privada de madera en el bosque de GYVA Eco Estate" loading="lazy"
               class="w-full h-full object-cover group-hover:scale-105 transition duration-700">
          <div class="absolute inset-0 bg-gradient-to-t from-brand-forest via-transparent to-transparent opacity-60"></div>
          <span class="absolute bottom-3 left-4 text-[10px] uppercase tracking-widest text-brand-gold font-semibold bg-brand-deep/80 px-2.5 py-1 rounded-full border border-brand-gold/30">
            <i class="fa-solid fa-house-chimney mr-1"></i> Cabaña de hospedaje
          </span>
        </div>
        <div class="p-6">
          <h3 class="text-xl text-white font-serif">Arquitectura de madera sostenible</h3>
          <p class="text-xs text-brand-cream/65 mt-2 leading-relaxed font-light">Maderas nobles locales, ventanales panorámicos hacia el dosel del bosque y acabados artesanales de lujo para una reconexión total.</p>
        </div>
      </article>

      <!-- TARJETA 2: FOGATAS -->
      <article class="bg-brand-forest/50 rounded-2xl overflow-hidden border border-brand-gold/15 group reveal shadow-xl">
        <div class="h-60 overflow-hidden relative">
          <img src="https://images.unsplash.com/photo-1478131143081-80f7f84ca84d?auto=format&fit=crop&q=80&w=900"
               alt="Fogata nocturna en el bosque" loading="lazy"
               class="w-full h-full object-cover group-hover:scale-105 transition duration-700">
          <div class="absolute inset-0 bg-gradient-to-t from-brand-forest via-transparent to-transparent opacity-60"></div>
        </div>
        <div class="p-6">
          <h3 class="text-xl text-white font-serif">Fogatas nocturnas &amp; maridaje</h3>
          <p class="text-xs text-brand-cream/65 mt-2 leading-relaxed font-light">Cielo estrellado sin contaminación lumínica, vinos selectos y charcutería gourmet alrededor del fuego comunal.</p>
        </div>
      </article>

      <!-- TARJETA 3: SENDEROS -->
      <article class="bg-brand-forest/50 rounded-2xl overflow-hidden border border-brand-gold/15 group reveal shadow-xl">
        <div class="h-60 overflow-hidden relative">
          <img src="https://images.unsplash.com/photo-1518495973542-4542c06a5843?auto=format&fit=crop&q=80&w=900"
               alt="Sendero natural entre árboles verdes" loading="lazy"
               class="w-full h-full object-cover group-hover:scale-105 transition duration-700">
          <div class="absolute inset-0 bg-gradient-to-t from-brand-forest via-transparent to-transparent opacity-60"></div>
        </div>
        <div class="p-6">
          <h3 class="text-xl text-white font-serif">Senderos privados</h3>
          <p class="text-xs text-brand-cream/65 mt-2 leading-relaxed font-light">Una caminata por los senderos llenos de naturaleza: flora endémica de Coto Brus, avistamiento de aves y silencio profundo.</p>
        </div>
      </article>

    </div>

    <div class="grid grid-cols-2 md:grid-cols-5 gap-4 pt-10 border-t border-brand-gold/15 reveal">
      <div class="text-center"><i class="fa-solid fa-seedling text-brand-gold text-lg"></i><p class="text-[10px] uppercase tracking-[0.25em] text-brand-cream/60 mt-2">Sostenible</p></div>
      <div class="text-center"><i class="fa-regular fa-gem text-brand-gold text-lg"></i><p class="text-[10px] uppercase tracking-[0.25em] text-brand-cream/60 mt-2">Exclusivo</p></div>
      <div class="text-center"><i class="fa-solid fa-mountain text-brand-gold text-lg"></i><p class="text-[10px] uppercase tracking-[0.25em] text-brand-cream/60 mt-2">Conectado</p></div>
      <div class="text-center"><i class="fa-solid fa-leaf text-brand-gold text-lg"></i><p class="text-[10px] uppercase tracking-[0.25em] text-brand-cream/60 mt-2">Natural</p></div>
      <div class="text-center"><i class="fa-regular fa-sun text-brand-gold text-lg"></i><p class="text-[10px] uppercase tracking-[0.25em] text-brand-cream/60 mt-2">Auténtico</p></div>
    </div>
  </div>
</section>

<!-- ============ RESERVA ============ -->
<section id="reserva" class="py-20 px-4 sm:px-6 lg:px-8 bg-brand-sand text-brand-forest">
  <div class="max-w-4xl mx-auto space-y-10">

    <div class="text-center space-y-4 reveal">
      <span class="text-[10px] uppercase tracking-[0.35em] font-semibold text-brand-wood">Reserva directa</span>
      <h2 class="text-3xl sm:text-5xl font-light text-brand-forest">Solicitud de reserva</h2>
      <div class="w-20 h-px bg-brand-forest/40 mx-auto"></div>
      <p class="text-brand-forest/70 text-sm font-light">Calcula tu estancia y verifica disponibilidad.</p>
    </div>

    <form id="booking-form" onsubmit="handleFormSubmit(event)" class="bg-white/70 rounded-3xl p-6 sm:p-10 border border-brand-forest/20 shadow-xl space-y-6 reveal">
      <div class="grid md:grid-cols-2 gap-5">
        <div>
          <label class="text-[10px] font-semibold uppercase text-brand-wood tracking-[0.2em]">Nombre completo *</label>
          <input id="guest-name" required placeholder="Ej: María Rodríguez" class="mt-2 w-full bg-white border border-brand-forest/20 rounded-xl px-4 py-3 text-sm text-brand-forest placeholder:text-brand-forest/35 focus:border-brand-wood focus:outline-none">
        </div>
        <div>
          <label class="text-[10px] font-semibold uppercase text-brand-wood tracking-[0.2em]">Correo electrónico *</label>
          <input id="guest-email" type="email" required placeholder="tu@email.com" class="mt-2 w-full bg-white border border-brand-forest/20 rounded-xl px-4 py-3 text-sm text-brand-forest placeholder:text-brand-forest/35 focus:border-brand-wood focus:outline-none">
        </div>
        <div>
          <label class="text-[10px] font-semibold uppercase text-brand-wood tracking-[0.2em]">Check-in *</label>
          <input id="checkin-date" type="date" required onchange="calculateTotal()" class="mt-2 w-full bg-white border border-brand-forest/20 rounded-xl px-4 py-3 text-sm text-brand-forest focus:border-brand-wood focus:outline-none">
        </div>
        <div>
          <label class="text-[10px] font-semibold uppercase text-brand-wood tracking-[0.2em]">Check-out *</label>
          <input id="checkout-date" type="date" required onchange="calculateTotal()" class="mt-2 w-full bg-white border border-brand-forest/20 rounded-xl px-4 py-3 text-sm text-brand-forest focus:border-brand-wood focus:outline-none">
        </div>
        <div>
          <label class="text-[10px] font-semibold uppercase text-brand-wood tracking-[0.2em]">Paquete *</label>
          <select id="package-select" onchange="calculateTotal()" class="mt-2 w-full bg-white border border-brand-forest/20 rounded-xl px-4 py-3 text-sm text-brand-forest focus:border-brand-wood focus:outline-none">
            <option value="esencial">Paquete Esencial</option>
            <option value="experiencia">Experiencia de la Casa</option>
          </select>
        </div>
        <div>
          <label class="text-[10px] font-semibold uppercase text-brand-wood tracking-[0.2em]">Cabaña *</label>
          <select id="cabin-select" onchange="calculateTotal()" class="mt-2 w-full bg-white border border-brand-forest/20 rounded-xl px-4 py-3 text-sm text-brand-forest focus:border-brand-wood focus:outline-none">
            <option value="pareja">Pareja (2 personas)</option>
            <option value="familiar">Familiar (5 personas)</option>
          </select>
        </div>
      </div>

      <div>
        <label class="text-[10px] font-semibold uppercase text-brand-wood tracking-[0.2em]">Peticiones especiales</label>
        <textarea id="guest-notes" rows="3" placeholder="Alergias, transporte, celebraciones..." class="mt-2 w-full bg-white border border-brand-forest/20 rounded-xl p-4 text-sm text-brand-forest placeholder:text-brand-forest/35 focus:border-brand-wood focus:outline-none"></textarea>
      </div>

      <div class="bg-brand-forest text-brand-cream p-6 rounded-2xl border border-brand-gold/40">
        <div class="flex flex-col sm:flex-row justify-between gap-2 border-b border-white/15 pb-4">
          <div>
            <span class="text-[10px] text-brand-gold uppercase tracking-[0.22em] font-semibold">Resumen estimado</span>
            <p id="summary-nights-text" class="text-sm text-brand-cream/85">Selecciona las fechas</p>
            <p id="error-msg" class="text-[11px] text-red-300 hidden mt-1">La salida debe ser posterior a la entrada.</p>
          </div>
          <div class="sm:text-right text-[11px]">
            <span class="text-brand-cream/50 block">Tipo de cambio referencia</span>
            <span class="font-semibold text-brand-gold">1 USD = ₡452</span>
          </div>
        </div>
        <div class="flex flex-col sm:flex-row justify-between gap-4 pt-4">
          <div>
            <p class="text-[10px] uppercase tracking-[0.2em] text-brand-cream/60">Por noche</p>
            <p id="price-per-night" class="text-lg font-medium">$450 – $600 USD</p>
          </div>
          <div class="sm:text-right">
            <p class="text-[10px] text-brand-gold uppercase tracking-[0.22em] font-bold">Total estancia</p>
            <div id="total-usd" class="text-3xl font-serif font-semibold text-brand-gold">$0 USD</div>
            <div id="total-crc" class="text-[11px] text-brand-cream/60 font-mono">~₡0 CRC</div>
          </div>
        </div>
      </div>

      <p class="text-[11px] text-brand-forest/55 font-light">Cancelación gratuita hasta 15 días antes. Se requiere 50% de anticipo para confirmar.</p>

      <button class="w-full gold-btn text-brand-deep font-bold py-4 rounded-xl text-sm tracking-wide">
        <i class="fa-solid fa-paper-plane mr-2"></i>Confirmar solicitud de reserva
      </button>
    </form>
  </div>
</section>

</main>

<!-- ============ FOOTER ============ -->
<footer class="bg-brand-deep border-t border-brand-gold/20 py-14 px-4 sm:px-6 lg:px-8 text-brand-cream/70">
  <div class="max-w-7xl mx-auto grid md:grid-cols-4 gap-8">
    <div class="md:col-span-2">
      <div class="flex items-center gap-3">
        <svg viewBox="0 0 64 80" class="w-7 h-10 text-brand-gold" fill="none" aria-hidden="true">
          <path d="M32 6C46 20 56 33 56 47c0 15-11 27-24 27S8 62 8 47C8 33 18 20 32 6Z" stroke="currentColor" stroke-width="2.4"/>
          <path d="M32 66V34" stroke="currentColor" stroke-width="2.4" stroke-linecap="round"/>
          <path d="M32 50c-8-1-13-6-14-15 8 1 13 6 14 15Z" fill="currentColor"/>
          <path d="M32 42c8-1 13-6 14-15-8 1-13 6-14 15Z" fill="currentColor"/>
        </svg>
        <div>
          <p class="font-serif text-2xl tracking-[0.25em] text-brand-cream">GYVA</p>
          <p class="text-[8px] tracking-[0.42em] text-brand-gold uppercase">Eco Estate</p>
        </div>
      </div>
      <p class="text-[10px] tracking-[0.3em] uppercase text-brand-gold/60 mt-4">Barefoot Luxury &amp; Private Lodges</p>
      <p class="text-xs mt-4 max-w-md font-light leading-relaxed">Santuario privado de hospedaje, conservación y bienestar en Coto Brus, Puntarenas. Un refugio para desconectar del mundo y reconectar con la naturaleza.</p>
    </div>

    <div class="text-xs">
      <h4 class="font-serif text-base text-brand-gold mb-3">Ubicación</h4>
      <p class="font-light"><i class="fa-solid fa-location-dot text-brand-gold mr-2"></i>R2X5+JC · Coto Brus<br><span class="ml-5">Puntarenas, Costa Rica</span></p>
      <p class="font-mono text-[10px] text-brand-cream/40 ml-5 mt-1">8.8491, -82.9914</p>
    </div>

    <div class="text-xs">
      <h4 class="font-serif text-base text-brand-gold mb-3">Contacto</h4>
      <p class="font-light"><i class="fa-solid fa-envelope text-brand-gold mr-2"></i>reservas@gyvaecoestate.com</p>
      <p class="font-light mt-2"><i class="fa-solid fa-phone text-brand-gold mr-2"></i>+506 8312-3456</p>
      <p class="font-light mt-2"><i class="fa-brands fa-instagram text-brand-gold mr-2"></i>@gyva.ecoestate</p>
    </div>
  </div>

  <div class="max-w-7xl mx-auto pt-8 mt-8 border-t border-white/10 flex flex-col sm:flex-row justify-between text-[10px] text-brand-cream/40 gap-3">
    <p>© 2026 GYVA Eco Estate. Todos los derechos reservados.</p>
    <p><i class="fa-solid fa-leaf text-brand-gold mr-1"></i> Compromiso de conservación ecológica</p>
  </div>
</footer>

<!-- ============ MODAL ============ -->
<div id="booking-modal" class="fixed inset-0 z-[100] bg-black/75 backdrop-blur-md hidden items-center justify-center p-4">
  <div class="bg-brand-forest border border-brand-gold/50 rounded-3xl max-w-lg w-full p-8 text-center space-y-5 text-brand-cream">
    <div class="w-16 h-16 rounded-full bg-brand-gold/15 border border-brand-gold text-brand-gold flex items-center justify-center text-3xl mx-auto">
      <i class="fa-solid fa-check"></i>
    </div>
    <h3 class="font-serif text-2xl text-white">¡Solicitud recibida!</h3>
    <p class="text-xs text-brand-cream/80 font-light">Gracias <span id="modal-guest-name" class="font-semibold text-brand-gold"></span>, hemos procesado tu solicitud en GYVA Eco Estate.</p>

    <div class="bg-brand-deep/80 p-4 rounded-xl border border-brand-gold/25 text-left text-xs space-y-2">
      <div class="flex justify-between border-b border-white/10 pb-1.5"><span class="text-brand-cream/55">Paquete</span><span id="modal-package" class="font-semibold"></span></div>
      <div class="flex justify-between border-b border-white/10 pb-1.5"><span class="text-brand-cream/55">Cabaña</span><span id="modal-cabin" class="font-semibold"></span></div>
      <div class="flex justify-between border-b border-white/10 pb-1.5"><span class="text-brand-cream/55">Fechas</span><span id="modal-dates" class="font-semibold"></span></div>
      <div class="flex justify-between pt-1"><span class="text-brand-gold font-bold">Total estimado</span><span id="modal-total" class="font-bold text-brand-gold"></span></div>
    </div>

    <p class="text-[11px] text-brand-cream/50 font-light">Un concierge te contactará por correo para confirmar disponibilidad y detalles de pago.</p>

    <div class="grid grid-cols-2 gap-3">
      <button onclick="closeModal()" class="border border-brand-gold/40 py-3 rounded-xl font-semibold text-sm hover:bg-white/5 transition">Cerrar</button>
      <button onclick="sendWhatsApp()" class="gold-btn text-brand-deep py-3 rounded-xl font-bold text-sm"><i class="fa-brands fa-whatsapp mr-1"></i> WhatsApp</button>
    </div>
  </div>
</div>

<script>
const WHATSAPP_NUMBER = '50683123456';
const sjoCoords  = [9.9984, -84.2046];
const gyvaCoords = [8.8491, -82.9914];

const PRICING = {
  esencial: {
    pareja:   { min: 450,  max: 600,  crcMin: 203000, crcMax: 271000 },
    familiar: { min: 750,  max: 950,  crcMin: 339000, crcMax: 429000 }
  },
  experiencia: {
    pareja:   { min: 850,  max: 1100, crcMin: 384000, crcMax: 497000 },
    familiar: { min: 1300, max: 1700, crcMin: 587000, crcMax: 768000 }
  }
};

const SPOTS = {
  yoga:    { title:'Tarima de Yoga',       tag:'Bienestar', icon:'fa-spa',           desc:'Plataforma circular de madera elevada entre los árboles. Sesiones privadas de yoga y meditación al amanecer.' },
  cabanas: { title:'Cabañas de Hospedaje', tag:'05 Lodges Privados', icon:'fa-house-chimney', desc:'Cinco cabañas de madera con terrazas panorámicas y ventanales orientados a la naturaleza.' },
  fogata:  { title:'Fogata Comunal',       tag:'Noches',    icon:'fa-fire',          desc:'El punto de encuentro de la finca. Fuego, vino, charcutería y cielos estrellados sin contaminación lumínica.' },
  central: { title:'Edificio Central',     tag:'Recepción · Restaurante · Minimercado', icon:'fa-utensils', desc:'El corazón de GYVA: recepción, restaurante farm-to-table y minimercado con productos locales.' },
  parqueo: { title:'Estacionamiento',      tag:'Acceso',    icon:'fa-car',           desc:'Parqueo privado, iluminado y dentro del perímetro de la finca. A pocos pasos del edificio central.' },
  caseta:  { title:'Casetilla de Guardia', tag:'Seguridad', icon:'fa-shield-halved', desc:'Control de acceso 24/7 y seguridad privada. Ingreso único y monitoreado.' }
};

const SPOT_POS = {
  yoga:[33,15], cabanas:[56,29], fogata:[61,45],
  central:[43,70], parqueo:[25,78], caseta:[48,85]
};

const stage = document.getElementById('stage3d');
const plane = document.getElementById('plane3d');
let px = 0, py = 0, zoom = 1, tilt = 30, rot = 0;
let dragging = false, startX = 0, startY = 0, baseX = 0, baseY = 0;

function applyTransform(){
  plane.style.transform = `translate3d(${px}px, ${py}px, 0) rotateX(${tilt}deg) rotateZ(${rot}deg) scale(${zoom})`;
  plane.style.setProperty('--tilt', tilt + 'deg');
  plane.style.setProperty('--rot', rot + 'deg');
}
const clamp = (v,a,b) => Math.min(Math.max(v,a), b);

function zoomBy(f){ zoom = clamp(zoom * f, 0.75, 3.2); applyTransform(); }

function resetView(){
  px = 0; py = 0; zoom = 1; tilt = 30; rot = 0;
  document.getElementById('tiltRange').value = 30;
  applyTransform();
  closeSpot();
}

function toggleLabels(){
  plane.classList.toggle('labels-off');
  document.getElementById('labelsBtn').classList.toggle('active');
}

function hideHint(){ const h = document.getElementById('mapHint'); if (h) h.style.opacity = '0'; }

function buildSpots(){
  const legend = document.getElementById('legend');
  Object.entries(SPOTS).forEach(([key, s]) => {
    const b = document.createElement('button');
    b.className = 'spot';
    b.dataset.spot = key;
    b.style.setProperty('--x', SPOT_POS[key][0] + '%');
    b.style.setProperty('--y', SPOT_POS[key][1] + '%');
    b.setAttribute('aria-label', s.title);
    b.innerHTML = `<span class="spot-dot"></span><span class="spot-label">${s.title}</span>`;
    b.addEventListener('click', ev => { ev.stopPropagation(); focusSpot(key); });
    document.getElementById('mapFrame').appendChild(b);

    const chip = document.createElement('button');
    chip.className = 'legend-chip bg-white/60 border border-brand-forest/15 rounded-xl px-3 py-2.5 text-left';
    chip.dataset.spot = key;
    chip.innerHTML = `<i class="fa-solid ${s.icon} text-brand-wood text-[11px] mr-1.5"></i><span class="text-[10px] uppercase tracking-[0.14em] font-semibold">${s.title}</span>`;
    chip.addEventListener('click', () => focusSpot(key));
    legend.appendChild(chip);
  });
}

function focusSpot(key){
  const [x,y] = SPOT_POS[key];
  const w = stage.clientWidth, h = stage.clientHeight;
  zoom = 1.75;
  px = -((x - 50) / 100) * w * zoom;
  py = -((y - 50) / 100) * h * zoom * 0.75;
  tilt = 22;
  document.getElementById('tiltRange').value = tilt;
  applyTransform();
  openSpot(key);
}

function openSpot(key){
  const s = SPOTS[key];
  document.getElementById('spotTag').textContent = s.tag;
  document.getElementById('spotTitle').textContent = s.title;
  document.getElementById('spotDesc').textContent = s.desc;
  document.getElementById('spotIcon').innerHTML = `<i class="fa-solid ${s.icon}"></i>`;
  document.getElementById('spotPanel').classList.remove('hidden');

  document.querySelectorAll('.spot').forEach(el => el.classList.toggle('active', el.dataset.spot === key));
  document.querySelectorAll('.legend-chip').forEach(el => el.classList.toggle('active', el.dataset.spot === key));

  const panel = document.getElementById('spotPanel');
  if (window.innerWidth >= 640){
    if (SPOT_POS[key][0] < 50){ panel.style.left = 'auto'; panel.style.right = '1.5rem'; }
    else { panel.style.right = 'auto'; panel.style.left = '1.5rem'; }
  }
}

function closeSpot(){
  document.getElementById('spotPanel').classList.add('hidden');
  document.querySelectorAll('.spot').forEach(el => el.classList.remove('active'));
  document.querySelectorAll('.legend-chip').forEach(el => el.classList.remove('active'));
}

stage.addEventListener('pointerdown', e => {
  if (e.target.closest('.spot') || e.target.closest('input') || e.target.closest('label')) return;
  dragging = true;
  startX = e.clientX; startY = e.clientY;
  baseX = px; baseY = py;
  stage.setPointerCapture(e.pointerId);
  stage.classList.add('cursor-grabbing');
  hideHint();
});
stage.addEventListener('pointermove', e => {
  if (!dragging) return;
  px = baseX + (e.clientX - startX);
  py = baseY + (e.clientY - startY);
  applyTransform();
});
['pointerup','pointercancel'].forEach(ev => stage.addEventListener(ev, () => {
  dragging = false;
  stage.classList.remove('cursor-grabbing');
}));

stage.addEventListener('wheel', e => {
  e.preventDefault();
  zoom = clamp(zoom * (e.deltaY < 0 ? 1.1 : 0.9), 0.75, 3.2);
  applyTransform();
  hideHint();
}, { passive:false });
stage.addEventListener('dblclick', e => {
  if (e.target.closest('.spot')) return;
  zoomBy(1.4);
});

document.getElementById('tiltRange').addEventListener('input', e => {
  tilt = Number(e.target.value);
  applyTransform();
});

let map, routePolyline, gyvaMarker;

function initMap(){
  map = L.map('map').setView([9.4, -83.6], 8);
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 18, attribution: '© OpenStreetMap'
  }).addTo(map);

  const goldIcon = L.divIcon({
    html:`<div style="background:#C8A145;width:22px;height:22px;border-radius:50%;border:3px solid #122A21;box-shadow:0 0 12px #C8A145"></div>`,
    iconSize:[22,22], iconAnchor:[11,11]
  });
  const greenIcon = L.divIcon({
    html:`<div style="background:#6B7F6A;width:18px;height:18px;border-radius:50%;border:3px solid #122A21"></div>`,
    iconSize:[18,18], iconAnchor:[9,9]
  });

  L.marker(sjoCoords, { icon: greenIcon }).addTo(map)
    .bindPopup('<b>Aeropuerto Juan Santamaría (SJO)</b><br>9.9984, -84.2046');
  gyvaMarker = L.marker(gyvaCoords, { icon: goldIcon }).addTo(map)
    .bindPopup('<b>GYVA Eco Estate</b><br>Coto Brus · 8.8491, -82.9914').openPopup();

  routePolyline = L.polyline([
    sjoCoords,
    [9.9333, -84.0833], [9.8644, -83.9194], [9.5667, -83.7500],
    [9.3736, -83.7036], [9.1700, -83.3300], [8.9561, -83.4356],
    [8.9614, -83.1903], [8.8264, -82.9706], gyvaCoords
  ], { color:'#C8A145', weight:4, opacity:.9, dashArray:'8,8' }).addTo(map);

  map.fitBounds(routePolyline.getBounds(), { padding:[40,40] });
  cargarRutaReal();
}

async function cargarRutaReal(){
  const url = `https://router.project-osrm.org/route/v1/driving/` +
              `${sjoCoords[1]},${sjoCoords[0]};${gyvaCoords[1]},${gyvaCoords[0]}` +
              `?overview=full&geometries=geojson`;
  try{
    const res = await fetch(url);
    if (!res.ok) throw new Error('OSRM');
    const data = await res.json();
    const ruta = data.routes && data.routes[0];
    if (!ruta) throw new Error('sin ruta');

    routePolyline.setLatLngs(ruta.geometry.coordinates.map(([lon, lat]) => [lat, lon]));
    routePolyline.setStyle({ dashArray: null, weight: 5, opacity: .95 });
    map.fitBounds(routePolyline.getBounds(), { padding: [40,40] });

    const km = Math.round(ruta.distance / 1000);
    const mins = Math.round(ruta.duration / 60);
    const hh = Math.floor(mins / 60);
    const mm = String(mins % 60).padStart(2, '0');

    document.getElementById('route-km').textContent = `~${km} km`;
    document.getElementById('route-time').textContent = `${hh}h ${mm} min`;
    document.getElementById('hero-time').textContent = `${hh}h ${mm}`;
  }catch(e){}
}

function showFullRouteView(){ map.fitBounds(routePolyline.getBounds(), { padding:[40,40] }); }
function showEstateOnlyView(){ map.setView(gyvaCoords, 13); gyvaMarker.openPopup(); }

function toLocalDate(d){
  return new Date(d.getTime() - d.getTimezoneOffset()*60000).toISOString().split('T')[0];
}
function setDates(){
  const t = new Date();
  const o = new Date(); o.setDate(t.getDate() + 2);
  const ci = document.getElementById('checkin-date');
  const co = document.getElementById('checkout-date');
  ci.min = toLocalDate(t); co.min = toLocalDate(t);
  ci.value = toLocalDate(t);
  co.value = toLocalDate(o);
}

function selectPackageInForm(v){
  document.getElementById('package-select').value = v;
  calculateTotal();
  document.getElementById('reserva').scrollIntoView({ behavior:'smooth' });
}

function calculateTotal(){
  const ciVal = document.getElementById('checkin-date').value;
  const coVal = document.getElementById('checkout-date').value;
  const ci = new Date(ciVal), co = new Date(coVal);
  const pkg = document.getElementById('package-select').value;
  const cab = document.getElementById('cabin-select').value;
  const err = document.getElementById('error-msg');

  if (!ciVal || !coVal || co <= ci){
    err.classList.remove('hidden');
    document.getElementById('summary-nights-text').textContent = 'Revisa las fechas de tu estancia';
    document.getElementById('total-usd').textContent = '$0 USD';
    document.getElementById('total-crc').textContent = '~₡0 CRC';
    return;
  }
  err.classList.add('hidden');

  const nights = Math.ceil((co - ci) / 86400000);
  const d = PRICING[pkg][cab];
  const pkgLabel = pkg === 'esencial' ? 'Esencial' : 'Experiencia';
  const cabLabel = cab === 'pareja' ? 'Pareja' : 'Familiar';

  document.getElementById('summary-nights-text').textContent =
    `${nights} noche${nights>1?'s':''} · ${pkgLabel} · Cabaña ${cabLabel}`;
  document.getElementById('price-per-night').textContent =
    `$${d.min.toLocaleString()} – $${d.max.toLocaleString()} USD / noche`;
  document.getElementById('total-usd').textContent =
    `$${(d.min*nights).toLocaleString()} – $${(d.max*nights).toLocaleString()} USD`;
  document.getElementById('total-crc').textContent =
    `~₡${(d.crcMin*nights).toLocaleString()} – ₡${(d.crcMax*nights).toLocaleString()} CRC`;
}

let lastBooking = {};

function handleFormSubmit(e){
  e.preventDefault();
  if (!document.getElementById('error-msg').classList.contains('hidden')){
    alert('Revisa las fechas: la salida debe ser posterior a la entrada.');
    return;
  }

  const ps = document.getElementById('package-select');
  const cs = document.getElementById('cabin-select');

  lastBooking = {
    name:  document.getElementById('guest-name').value,
    email: document.getElementById('guest-email').value,
    pkg:   ps.options[ps.selectedIndex].text,
    cab:   cs.options[cs.selectedIndex].text,
    ci:    document.getElementById('checkin-date').value,
    co:    document.getElementById('checkout-date').value,
    total: document.getElementById('total-usd').textContent,
    notes: document.getElementById('guest-notes').value
  };

  document.getElementById('modal-guest-name').textContent = lastBooking.name;
  document.getElementById('modal-package').textContent    = lastBooking.pkg;
  document.getElementById('modal-cabin').textContent      = lastBooking.cab;
  document.getElementById('modal-dates').textContent      = `${lastBooking.ci} al ${lastBooking.co}`;
  document.getElementById('modal-total').textContent      = lastBooking.total;

  const m = document.getElementById('booking-modal');
  m.classList.remove('hidden');
  m.classList.add('flex');
}

function closeModal(){
  const m = document.getElementById('booking-modal');
  m.classList.add('hidden');
  m.classList.remove('flex');
}
document.addEventListener('keydown', e => { if (e.key === 'Escape') closeModal(); });
document.getElementById('booking-modal').addEventListener('click', e => {
  if (e.target.id === 'booking-modal') closeModal();
});

function sendWhatsApp(){
  const t = `Hola GYVA Eco Estate 🌿%0A%0ANombre: ${lastBooking.name}%0AInterés: ${lastBooking.pkg} · ${lastBooking.cab}%0AFechas: ${lastBooking.ci} al ${lastBooking.co}%0ATotal estimado: ${lastBooking.total}%0ANotas: ${lastBooking.notes || '—'}`;
  window.open(`https://wa.me/${WHATSAPP_NUMBER}?text=${t}`, '_blank');
}

function setupMenu(){
  const b = document.getElementById('mobile-menu-btn');
  const m = document.getElementById('mobile-menu');
  b.addEventListener('click', () => m.classList.toggle('hidden'));
  m.querySelectorAll('a').forEach(a => a.addEventListener('click', () => m.classList.add('hidden')));
}

function setupReveal(){
  const io = new IntersectionObserver(entries => {
    entries.forEach(en => { if (en.isIntersecting) en.target.classList.add('visible'); });
  }, { threshold:.12 });
  document.querySelectorAll('.reveal').forEach(el => io.observe(el));
}

window.addEventListener('load', () => {
  buildSpots();
  applyTransform();
  initMap();
  setupMenu();
  setupReveal();
  setDates();
  calculateTotal();
});
</script>
</body>
</html>
