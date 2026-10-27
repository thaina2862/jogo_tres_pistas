<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jogo das Três Pistas - Operação Honda & Bulgarelli</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  
  <style>
    /* FONTES DO JOGO E DO CARRO */
    @import url('https://fonts.googleapis.com/css2?family=Bungee&family=Poppins:wght@300;400;600;700;800;900&family=Chakra+Petch:ital,wght@0,600;0,700;1,700&family=Inter:wght@400;600;800&display=swap');
    
    @font-face {
      font-family: 'Ultimatum Heavy Italic';
      src: local('Ultimatum Heavy Italic'), local('Ultimatum-Heavy-Italic');
      font-weight: 900;
      font-style: italic;
      font-display: swap;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: radial-gradient(circle at top, #1a0304 0%, #080102 100%);
      color: #ffffff;
      min-height: 100vh;
      overflow-x: hidden;
      user-select: none;
      -webkit-user-select: none;
    }

    .font-game {
      font-family: 'Ultimatum Heavy Italic', 'Poppins', sans-serif;
      font-weight: 900;
      font-style: italic;
      letter-spacing: 3px;
      text-transform: uppercase;
    }

    .racing-font {
      font-family: 'Chakra Petch', sans-serif;
    }

    /* ESTILIZAÇÃO RETRO COMIC NEON PARA TITULOS */
    .retro-comic-neon-fire {
      font-family: 'Bungee', 'Ultimatum Heavy Italic', cursive, sans-serif;
      font-style: italic;
      text-transform: uppercase;
      display: inline-block;
      
      background: linear-gradient(
        0deg,
        #ff0000 0%,
        #ff5500 25%,
        #ffaa00 50%,
        #ffff00 75%,
        #ffffff 100%
      );
      background-size: 100% 200%;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: fireGlowPulse 2s ease-in-out infinite alternate;

      filter: drop-shadow(0 0 8px #ff4500) 
              drop-shadow(0 0 18px #ff6c00) 
              drop-shadow(0 0 30px #ff0000);
      -webkit-text-stroke: 1.8px #ff8c00;
    }

    @keyframes fireGlowPulse {
      0% {
        background-position: 0% 0%;
        filter: drop-shadow(0 0 6px #ff4500) drop-shadow(0 0 15px #ff6c00) drop-shadow(0 0 25px #ff0000);
      }
      100% {
        background-position: 0% 100%;
        filter: drop-shadow(0 0 12px #ff6c00) drop-shadow(0 0 25px #ff4500) drop-shadow(0 0 40px #ff2200);
      }
    }

    .glass-card {
      background: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(12px);
      border: 1px solid rgba(255, 255, 255, 0.12);
    }
    .honda-red { background-color: #cc0000; }
    .honda-red-hover:hover { background-color: #a80000; }

    /* ESTILOS DO HONDA CIVIC TYPE-R (CAPA) */
    #screenCover {
        background: #07090e;
    }

    .stage-wrapper {
        perspective: 800px;
        perspective-origin: 50% 55%;
        transform-style: preserve-3d;
    }

    .shake-screen {
        animation: cameraShake 0.06s infinite alternate;
    }

    @keyframes cameraShake {
        0% { transform: translate(1.5px, 1.5px) rotate(0.1deg); }
        100% { transform: translate(-1.5px, -1.5px) rotate(-0.1deg); }
    }

    .road-perspective {
        position: absolute;
        bottom: 0;
        left: 50%;
        width: 120vw;
        height: 55vh;
        transform: translateX(-50%) rotateX(75deg);
        transform-origin: bottom center;
        background: radial-gradient(circle at 50% 0%, #1c222e 0%, #0d1017 80%, #050608 100%);
        box-shadow: 0 -10px 40px rgba(0, 0, 0, 0.95);
        overflow: hidden;
    }

    .road-grid {
        position: absolute;
        inset: 0;
        background-image: 
            linear-gradient(to right, rgba(255, 255, 255, 0.05) 1px, transparent 1px),
            linear-gradient(to bottom, rgba(255, 0, 0, 0.1) 1px, transparent 1px);
        background-size: 80px 40px;
    }

    .road-stripes {
        position: absolute;
        top: 0;
        bottom: 0;
        left: 50%;
        width: 8px;
        transform: translateX(-50%);
        background: repeating-linear-gradient(to bottom, #ffea00, #ffea00 35px, transparent 35px, transparent 70px);
        opacity: 0.6;
    }

    .road-stripes.speeding {
        animation: roadSpeed 0.12s linear infinite;
    }

    @keyframes roadSpeed {
        from { background-position-y: 0px; }
        to { background-position-y: 70px; }
    }

    .idle-vibe {
        animation: engineIdle 0.12s infinite alternate ease-in-out;
    }

    @keyframes engineIdle {
        0% { transform: translateY(0px) rotate(0deg); }
        100% { transform: translateY(-2px) rotate(0.08deg); }
    }

    .car-assembly {
        transform-style: preserve-3d;
        transition: transform 0.25s cubic-bezier(0.2, 0.8, 0.2, 1);
    }

    .launching {
        animation: launchDrive 1.35s cubic-bezier(0.65, 0.02, 0.2, 1) forwards !important;
    }

    @keyframes launchDrive {
        0% { transform: translate3d(0, 0, 0) scale(1) rotateX(0deg); opacity: 1; }
        18% { transform: translate3d(0, 15px, -60px) scale(0.94) rotateX(-2deg); opacity: 1; }
        35% { transform: translate3d(0, -6px, 100px) scale(1.3) rotateX(2deg); opacity: 1; }
        75% { transform: translate3d(0, -20px, 600px) scale(4.8) rotateX(5deg); opacity: 0.95; }
        100% { transform: translate3d(0, -50px, 1200px) scale(9.5) rotateX(8deg); opacity: 0; filter: blur(5px); }
    }

    .car-shadow {
        transition: transform 1.3s cubic-bezier(0.65, 0.02, 0.2, 1), opacity 1.1s ease;
    }
    .car-assembly.launching ~ .car-shadow {
        transform: translateX(-50%) scale(0.1);
        opacity: 0;
    }

    .drl-glow { filter: drop-shadow(0 0 10px rgba(180, 230, 255, 0.9)) drop-shadow(0 0 25px rgba(0, 160, 255, 0.7)); }
    .fog-glow { box-shadow: 0 0 14px #ffffff, 0 0 25px rgba(255, 255, 255, 0.8); }

    .start-button-ring {
        background: radial-gradient(circle, #555 0%, #222 60%, #111 100%);
        border: 3px solid #8e959e;
        box-shadow: 0 0 20px rgba(0,0,0,0.8), inset 0 2px 4px rgba(255,255,255,0.4);
    }
    .start-button-core {
        background: radial-gradient(circle at 35% 35%, #ff3b30 0%, #b80d0d 65%, #7a0000 100%);
        box-shadow: 0 4px 15px rgba(230, 0, 0, 0.6), inset 0 2px 5px rgba(255, 255, 255, 0.5);
        transition: all 0.15s ease;
    }
    .start-button-core:active {
        transform: scale(0.94);
        box-shadow: 0 1px 6px rgba(255, 0, 0, 0.8), inset 0 2px 8px rgba(0,0,0,0.6);
    }
    .start-button-core.running {
        background: radial-gradient(circle at 35% 35%, #ff2020 0%, #cf0000 70%, #990000 100%);
        box-shadow: 0 0 25px rgba(255, 30, 30, 0.9), inset 0 2px 5px rgba(255, 255, 255, 0.6);
    }

    .launch-flash {
        position: absolute;
        inset: 0;
        background: radial-gradient(circle, rgba(255,255,255,0.8) 0%, rgba(255,0,0,0.3) 45%, transparent 75%);
        pointer-events: none;
        opacity: 0;
        z-index: 50;
        transition: opacity 0.1s ease;
    }
    .launch-flash.active { opacity: 1; }

    /* ANIMAÇÃO DA MOTO MOTO ESPORTIVA 3D */
    @keyframes bikeDriveCustom {
      0% { left: -300px; opacity: 0; }
      10% { opacity: 1; }
      90% { opacity: 1; }
      100% { left: calc(100% + 100px); opacity: 0; }
    }

    .animate-bike-custom { animation: bikeDriveCustom 1.8s linear forwards; }

    .racetrack-container {
      background: #1c1c1e;
      border-top: 6px solid #e11d48;
      border-bottom: 6px solid #e11d48;
      box-shadow: inset 0 0 20px rgba(0,0,0,0.9);
    }
    .curb-pattern {
      background: repeating-linear-gradient( 90deg, #ffffff, #ffffff 20px, #cc0000 20px, #cc0000 40px );
    }
    .chequered-flag {
      background-image: repeating-linear-gradient(45deg, #000 25%, transparent 25%, transparent 75%, #000 75%, #000), 
                        repeating-linear-gradient(45deg, #000 25%, #fff 25%, #fff 75%, #000 75%, #000);
      background-position: 0 0, 10px 10px;
      background-size: 20px 20px;
    }

    .modal-backdrop { background: rgba(0, 0, 0, 0.85); backdrop-filter: blur(6px); }
  </style>
</head>
<body class="flex flex-col justify-between min-h-screen text-slate-100">

  <!-- BARRA DE NAVEGAÇÃO SUPERIOR -->
  <header id="appHeader" class="hidden sticky top-0 z-30 glass-card border-b border-red-900/40 px-4 py-3 shadow-xl">
    <div class="max-w-5xl mx-auto flex flex-wrap justify-between items-center gap-2">
      <div class="flex items-center space-x-3">
        <i class="fa-solid fa-motorcycle text-2xl text-red-500"></i>
        <div>
          <span class="font-bold text-sm tracking-wider uppercase text-red-500 block">Operação Honda</span>
          <span class="text-xs text-slate-400">Bulgarelli Advogados</span>
        </div>
      </div>
      <div id="userInfoHeader" class="text-xs sm:text-sm bg-black/40 px-3 py-1.5 rounded-full border border-red-500/30 flex items-center gap-2">
        <i class="fa-solid fa-user-check text-green-400"></i>
        <span id="headerPlayerName" class="font-semibold text-white">---</span>
        <span class="text-slate-500">|</span>
        <span id="headerPlayerMatricula" class="text-slate-300">---</span>
        <span class="text-slate-500">|</span>
        <span id="headerPlayerScore" class="font-bold text-yellow-400">0 pts</span>
      </div>
      <div class="flex items-center gap-2">
        <button onclick="logoutSession()" class="px-2.5 py-1.5 bg-black/50 hover:bg-black/80 text-xs font-semibold rounded-lg border border-slate-700 transition flex items-center gap-1">
          <i class="fa-solid fa-right-from-bracket text-slate-400"></i> Sair
        </button>
        <button onclick="goToCover()" class="px-3 py-1.5 bg-red-900/60 hover:bg-red-800 text-xs font-semibold rounded-lg border border-red-500/50 transition flex items-center gap-1.5">
          <i class="fa-solid fa-house text-red-300"></i> Voltar à Capa Inicial
        </button>
      </div>
    </div>
  </header>

  <!-- TELA 1: CAPA INICIAL COM HONDA CIVIC TYPE-R 3D -->
  <section id="screenCover" class="flex-1 flex flex-col justify-between items-center w-full relative overflow-hidden">
    
    <div id="flashOverlay" class="launch-flash"></div>

    <div class="w-full flex flex-col items-center z-20 pt-6 px-4 gap-6">
        <div class="w-full max-w-4xl flex flex-wrap items-center justify-between gap-4">
            <div class="flex items-center gap-3">
                <div class="w-10 h-7 bg-[#b20000] border border-gray-200 rounded flex items-center justify-center font-bold text-white shadow-md text-xs tracking-wider">
                    CIVIC
                </div>
                <div>
                    <h1 class="text-lg md:text-xl font-black italic tracking-wide racing-font flex items-center gap-2 leading-none">
                        HONDA <span class="text-red-500 font-extrabold">TYPE-R</span>
                    </h1>
                    <p class="text-[10px] md:text-xs text-gray-400 font-mono tracking-widest uppercase">2.0L VTEC TURBO // 315 HP</p>
                </div>
            </div>

            <div class="flex items-center gap-4 bg-gray-900/80 backdrop-blur border border-gray-800 rounded-full px-4 py-1.5 text-xs font-mono">
                <div class="flex items-center gap-1.5">
                    <span id="engineStatusDot" class="w-2.5 h-2.5 rounded-full bg-red-600 animate-pulse"></span>
                    <span id="engineStatusText" class="text-gray-300 font-semibold tracking-wider">ENGINE IDLE</span>
                </div>
                <div class="h-3 w-px bg-gray-700"></div>
                <div class="text-red-400 font-bold w-16 text-right" id="rpmGauge">850 RPM</div>
            </div>
        </div>

        <div class="text-center mt-2">
            <h1 class="text-4xl sm:text-6xl md:text-7xl font-black mb-3 tracking-wider leading-tight">
                <span class="retro-comic-neon-fire">JOGO DAS TRÊS PISTAS</span>
            </h1>
            <p class="text-slate-300 text-sm sm:text-base bg-black/40 inline-block px-4 py-1.5 rounded-full border border-slate-700/50">
                Treinamento de Negociação e Recuperação de Crédito — <span class="text-red-400 font-semibold">Honda &amp; Bulgarelli</span>
            </p>
        </div>
    </div>

    <main id="sceneWrapper" class="stage-wrapper relative w-full max-w-4xl flex-1 flex items-center justify-center overflow-visible min-h-[360px]">
        <div class="road-perspective pointer-events-none">
            <div class="road-grid"></div>
            <div id="roadStripes" class="road-stripes"></div>
        </div>

        <div id="lightBeams" class="absolute bottom-28 w-[420px] h-48 pointer-events-none opacity-40 transition-opacity duration-300 flex justify-between px-6 z-0">
            <div class="w-36 h-full bg-gradient-to-t from-transparent via-cyan-400/20 to-blue-200/50 rounded-full blur-xl transform -rotate-6"></div>
            <div class="w-36 h-full bg-gradient-to-t from-transparent via-cyan-400/20 to-blue-200/50 rounded-full blur-xl transform rotate-6"></div>
        </div>

        <div id="carShadow" class="car-shadow absolute bottom-24 w-[380px] h-6 bg-black/85 rounded-full blur-md z-0"></div>

        <div id="carRoot" class="car-assembly idle-vibe relative w-[390px] h-[210px] z-10 flex flex-col items-center justify-end">
            
            <div class="absolute -top-3 w-[310px] flex flex-col items-center z-0">
                <div class="w-full h-4 bg-gradient-to-r from-[#181818] via-[#2a2a2a] to-[#181818] rounded-t-md shadow-lg border-b border-black flex justify-between px-1 items-center">
                    <div class="w-2.5 h-6 bg-[#0e0e0e] rounded-sm transform -rotate-6 border border-zinc-700"></div>
                    <div class="w-48 h-1.5 bg-[#141414] rounded-full mx-auto"></div>
                    <div class="w-2.5 h-6 bg-[#0e0e0e] rounded-sm transform rotate-6 border border-zinc-700"></div>
                </div>
                <div class="w-[210px] flex justify-between px-6">
                    <div class="w-3 h-8 bg-gradient-to-b from-[#1c1c1c] to-[#0c0c0c] rounded-b-sm border-x border-zinc-800"></div>
                    <div class="w-3 h-8 bg-gradient-to-b from-[#1c1c1c] to-[#0c0c0c] rounded-b-sm border-x border-zinc-800"></div>
                </div>
            </div>

            <div class="relative w-[280px] h-[82px] flex items-center justify-center z-10">
                <div class="absolute -left-6 top-10 flex items-center">
                    <div class="w-8 h-5 bg-[#111] rounded-l-full border border-zinc-800 shadow-md transform -rotate-3 relative overflow-hidden flex items-center justify-end pr-1">
                        <div class="w-1.5 h-3.5 bg-sky-200/40 rounded-sm"></div>
                        <div class="absolute top-0 left-0 w-full h-1.5 bg-[#c70000]"></div>
                    </div>
                    <div class="w-3 h-1.5 bg-[#0a0a0a]"></div>
                </div>
                <div class="absolute -right-6 top-10 flex items-center">
                    <div class="w-3 h-1.5 bg-[#0a0a0a]"></div>
                    <div class="w-8 h-5 bg-[#111] rounded-r-full border border-zinc-800 shadow-md transform rotate-3 relative overflow-hidden flex items-center justify-start pl-1">
                        <div class="w-1.5 h-3.5 bg-sky-200/40 rounded-sm"></div>
                        <div class="absolute top-0 right-0 w-full h-1.5 bg-[#c70000]"></div>
                    </div>
                </div>
                <div class="w-[220px] h-[78px] bg-gradient-to-b from-[#1a1a1a] via-[#101318] to-[#08090c] rounded-t-[55px] p-2 border-t-2 border-zinc-600/30 relative shadow-2xl flex flex-col items-center">
                    <div class="w-[196px] h-[64px] bg-gradient-to-b from-[#16212e] via-[#0c131c] to-[#05080c] rounded-t-[44px] relative overflow-hidden border border-white/10 shadow-inner">
                        <div class="absolute bottom-1 w-full flex justify-between px-9 opacity-40">
                            <div class="w-6 h-7 bg-red-700 rounded-t-md border border-red-500"></div>
                            <div class="w-6 h-7 bg-red-700 rounded-t-md border border-red-500"></div>
                        </div>
                        <div class="absolute top-1 left-1/2 -translate-x-1/2 w-6 h-2 bg-neutral-900 border border-zinc-700 rounded-sm"></div>
                        <div class="absolute -top-4 left-4 w-10 h-28 bg-white/15 transform rotate-35 pointer-events-none blur-[0.5px]"></div>
                        <div class="absolute -top-4 right-10 w-4 h-28 bg-white/10 transform rotate-35 pointer-events-none"></div>
                        <div class="absolute inset-y-0 left-0 w-3 bg-gradient-to-r from-black/80 to-transparent"></div>
                        <div class="absolute inset-y-0 right-0 w-3 bg-gradient-to-l from-black/80 to-transparent"></div>
                    </div>
                </div>
            </div>

            <div class="relative w-[360px] z-20 flex flex-col items-center -mt-1">
                <div class="relative w-full h-[62px] bg-gradient-to-b from-[#b80000] via-[#c70000] to-[#990000] rounded-t-2xl shadow-xl border-t border-red-400/50 flex flex-col items-center">
                    <div class="w-[260px] h-full flex justify-between items-center px-4 relative">
                        <div class="w-1.5 h-10 bg-black/20 rounded-full blur-[0.5px] transform -rotate-12"></div>
                        <div class="w-20 h-3.5 bg-[#121212] border border-zinc-800 rounded-t-sm shadow-inner flex items-center justify-center -mt-3">
                            <div class="w-16 h-1 bg-[#222] rounded-sm"></div>
                        </div>
                        <div class="w-1.5 h-10 bg-black/20 rounded-full blur-[0.5px] transform rotate-12"></div>
                    </div>
                    <div class="absolute bottom-0 w-full h-[32px] bg-gradient-to-b from-[#181818] via-[#101010] to-[#080808] border-t-2 border-zinc-700 flex items-center justify-between px-3 z-30 shadow-md">
                        <div class="relative w-[76px] h-[22px] bg-[#0c1017] rounded-bl-lg overflow-hidden border-t border-l border-zinc-500 transform -rotate-3 flex items-center px-1 shadow-[0_0_12px_rgba(0,180,255,0.4)]">
                            <div class="absolute top-0.5 right-0 w-full h-[3px] bg-white drl-glow"></div>
                            <div class="flex items-center gap-1.5 z-10 pl-1">
                                <div class="w-3.5 h-3 bg-white rounded-sm shadow-[0_0_8px_#ffffff]"></div>
                                <div class="w-3.5 h-3 bg-white rounded-sm shadow-[0_0_8px_#ffffff]"></div>
                                <div class="w-3.5 h-3 bg-cyan-200 rounded-sm shadow-[0_0_8px_#38bdf8]"></div>
                            </div>
                            <div class="absolute bottom-0 left-0 w-3 h-1 bg-amber-400"></div>
                        </div>
                        <div class="flex-1 h-full flex items-center justify-center px-2">
                            <div class="relative w-full h-[26px] bg-[#0d0d0d] rounded flex items-center justify-center border-b border-red-700/60">
                                <div class="absolute inset-0 opacity-40 bg-[radial-gradient(#333_1px,transparent_1px)] [background-size:4px_4px]"></div>
                                <div class="relative w-8 h-6 bg-[#b00000] border-2 border-[#e6e6e6] rounded-[4px] flex items-center justify-center shadow-[0_0_8px_rgba(200,0,0,0.8)] z-20">
                                    <svg viewBox="0 0 24 20" class="w-5 h-4 fill-white drop-shadow">
                                        <path d="M3 2h3.2l2.3 12.5h1.2L12 9.5l2.3 5h1.2L17.8 2H21l-3 16h-4.2l-1.8-4.5-1.8 4.5H6.2L3 2z"/>
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div class="relative w-[76px] h-[22px] bg-[#0c1017] rounded-br-lg overflow-hidden border-t border-r border-zinc-500 transform rotate-3 flex items-center justify-end px-1 shadow-[0_0_12px_rgba(0,180,255,0.4)]">
                            <div class="absolute top-0.5 left-0 w-full h-[3px] bg-white drl-glow"></div>
                            <div class="flex items-center gap-1.5 z-10 pr-1">
                                <div class="w-3.5 h-3 bg-cyan-200 rounded-sm shadow-[0_0_8px_#38bdf8]"></div>
                                <div class="w-3.5 h-3 bg-white rounded-sm shadow-[0_0_8px_#ffffff]"></div>
                                <div class="w-3.5 h-3 bg-white rounded-sm shadow-[0_0_8px_#ffffff]"></div>
                            </div>
                            <div class="absolute bottom-0 right-0 w-3 h-1 bg-amber-400"></div>
                        </div>
                    </div>
                </div>
                <div class="w-full h-[62px] bg-gradient-to-b from-[#8f0000] via-[#750000] to-[#590000] rounded-b-xl border-t border-black/40 relative flex items-center justify-between px-3 shadow-2xl">
                    <div class="w-14 h-11 bg-[#101010] rounded-md border border-zinc-800 relative overflow-hidden flex flex-col justify-end p-1 shadow-inner">
                        <div class="w-3 h-3 bg-white rounded-full fog-glow mb-0.5 ml-1"></div>
                        <div class="w-full h-1.5 bg-red-600/80 rounded-sm"></div>
                    </div>
                    <div class="w-[188px] h-11 bg-[#0b0c0e] rounded-md border border-zinc-800 relative flex flex-col justify-between p-1 shadow-inner">
                        <div class="w-full h-1.5 bg-[#1f242d] rounded-sm opacity-60"></div>
                        <div class="w-full h-4 bg-gradient-to-r from-zinc-800 via-zinc-400 to-zinc-800 opacity-25 rounded-xs"></div>
                        <div class="w-full h-[3px] bg-[#ff1a1a] rounded-full shadow-[0_0_6px_#ff0000]"></div>
                    </div>
                    <div class="w-14 h-11 bg-[#101010] rounded-md border border-zinc-800 relative overflow-hidden flex flex-col justify-end items-end p-1 shadow-inner">
                        <div class="w-3 h-3 bg-white rounded-full fog-glow mb-0.5 mr-1"></div>
                        <div class="w-full h-1.5 bg-red-600/80 rounded-sm"></div>
                    </div>
                    <div class="absolute -bottom-2 inset-x-0 h-3 bg-[#0a0a0a] rounded-b-md border-t border-zinc-700 flex justify-between px-1">
                        <div class="w-5 h-4 bg-black rounded-tl-sm border-l border-zinc-600 -mt-1"></div>
                        <div class="w-5 h-4 bg-black rounded-tr-sm border-r border-zinc-600 -mt-1"></div>
                    </div>
                </div>
                <div class="absolute -bottom-4 w-[372px] flex justify-between px-1 -z-10">
                    <div class="w-10 h-16 bg-[#121316] rounded-md border-2 border-zinc-800 shadow-2xl flex flex-col items-center justify-center transform -rotate-1">
                        <div class="w-5 h-8 border border-zinc-600/50 rounded-sm bg-gradient-to-b from-[#222] to-[#111] flex items-center justify-center">
                            <div class="w-2.5 h-2.5 bg-red-600 rounded-full"></div>
                        </div>
                    </div>
                    <div class="w-10 h-16 bg-[#121316] rounded-md border-2 border-zinc-800 shadow-2xl flex flex-col items-center justify-center transform rotate-1">
                        <div class="w-5 h-8 border border-zinc-600/50 rounded-sm bg-gradient-to-b from-[#222] to-[#111] flex items-center justify-center">
                            <div class="w-2.5 h-2.5 bg-red-600 rounded-full"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <!-- CONSOLE ENGINE START -->
    <footer class="w-full max-w-xl flex flex-col items-center gap-3 z-30 pb-10 mt-auto">
        <div class="flex items-center gap-6">
            <div class="hidden sm:flex flex-col items-end text-right font-mono text-xs text-gray-400 w-36">
                <span class="text-zinc-500 uppercase tracking-wider">LAUNCH CONTROL</span>
                <span id="turboBoost" class="text-emerald-400 font-semibold">BOOST: 0.0 BAR</span>
            </div>

            <div class="start-button-ring p-1.5 rounded-full shadow-2xl">
                <button id="engineStartBtn" onclick="startCarAccelerationTransition()" class="start-button-core w-24 h-24 rounded-full flex flex-col items-center justify-center text-center cursor-pointer select-none active:scale-95 transition-transform" title="Iniciar Arrancada e Começar Jogo">
                    <span class="text-[10px] tracking-widest text-red-200 font-extrabold uppercase">Engine</span>
                    <span class="text-base font-black tracking-tight text-white uppercase drop-shadow leading-tight">START</span>
                    <span class="text-[9px] tracking-wider text-red-200 font-bold uppercase">STOP</span>
                    <span id="buttonLed" class="w-3 h-1 bg-white rounded-full mt-1 shadow-[0_0_6px_#ffffff]"></span>
                </button>
            </div>

            <div class="hidden sm:flex flex-col items-start text-left font-mono text-xs text-gray-400 w-36">
                <span class="text-zinc-500 uppercase tracking-wider">VTEC CAM PHASE</span>
                <span id="vtecState" class="text-gray-400 font-semibold">STAGE: IDLE</span>
            </div>
        </div>
    </footer>

  </section>

  <!-- TELA 2: IDENTIFICAÇÃO DO OPERADOR -->
  <section id="screenRegistration" class="hidden flex-1 flex flex-col justify-center items-center p-6">
    <div class="max-w-md w-full glass-card p-8 rounded-3xl border-red-600/30 shadow-2xl relative">
      <div class="absolute inset-0 bg-red-900/10 blur-xl -z-10 rounded-3xl"></div>
      <div class="text-center mb-6">
        <i class="fa-solid fa-id-card text-4xl text-red-500 mb-2"></i>
        <h2 class="text-2xl font-bold font-game">Identificação do Operador</h2>
        <p class="text-xs text-slate-400">Insira seus dados para registrar sua pontuação no ranking</p>
      </div>
      <form id="formRegistration" onsubmit="handleRegistrationSubmit(event)" class="space-y-4">
        <div>
          <label class="block text-xs font-semibold uppercase text-slate-300 mb-1">Nome e Sobrenome</label>
          <input type="text" id="inputName" required maxlength="40" placeholder="Ex: Carlos Silva" class="w-full px-4 py-3 bg-black/50 border border-slate-700 rounded-xl text-white focus:outline-none focus:border-red-500 transition">
        </div>
        <div>
          <label class="block text-xs font-semibold uppercase text-slate-300 mb-1">Matrícula</label>
          <input type="text" id="inputMatricula" required maxlength="20" placeholder="Ex: 84920" class="w-full px-4 py-3 bg-black/50 border border-slate-700 rounded-xl text-white focus:outline-none focus:border-red-500 transition">
        </div>
        <button type="submit" id="btnSubmitRegistration" class="w-full py-4 honda-red honda-red-hover text-white font-bold rounded-xl shadow-lg shadow-red-900/50 transition duration-300 flex items-center justify-center gap-2">
          <span class="font-game text-lg">CONFIRMAR E JOGAR</span>
          <i class="fa-solid fa-circle-check"></i>
        </button>
      </form>
    </div>
  </section>

  <!-- TELA 3: TRANSITION "VAMOS JOGAR!" (ESTILO RETRO-NEON DA CAPA) -->
  <section id="screenTransitionMoto" class="hidden fixed inset-0 z-50 bg-[#090203] flex flex-col justify-center items-center text-center overflow-hidden">
    <div class="relative z-10 px-4 mb-12">
      <h2 class="text-5xl sm:text-7xl md:text-8xl font-black tracking-widest uppercase retro-comic-neon-fire">
        VAMOS JOGAR!
      </h2>
    </div>

    <!-- PISTA DA MOTO ESPORTIVA HONDA 3D -->
    <div class="absolute bottom-16 w-full h-28 racetrack-container flex flex-col justify-between overflow-hidden">
      <div class="w-full h-3 curb-pattern"></div>
      <div class="relative flex-1 flex items-center overflow-hidden">
        <div class="w-full border-b-2 border-dashed border-slate-400/60"></div>
        <div class="absolute right-24 top-0 bottom-0 w-8 chequered-flag opacity-80 border-x border-white"></div>
        
        <!-- MOTO VETORIAL 3D DETALHADA -->
        <div class="absolute top-1/2 -translate-y-1/2 animate-bike-custom flex items-center">
          <svg class="w-44 h-28 sm:w-56 sm:h-36 drop-shadow-[0_10px_12px_rgba(0,0,0,0.95)]" viewBox="0 0 550 320" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="120" cy="200" r="54" fill="#111" stroke="#222" stroke-width="12"/>
            <circle cx="120" cy="200" r="38" fill="#d1d5db" stroke="#6b7280" stroke-width="4"/>
            <circle cx="120" cy="200" r="22" fill="#ef4444"/>
            <circle cx="410" cy="200" r="54" fill="#111" stroke="#222" stroke-width="12"/>
            <circle cx="410" cy="200" r="38" fill="#d1d5db" stroke="#6b7280" stroke-width="4"/>
            <circle cx="410" cy="200" r="22" fill="#ef4444"/>
            <path d="M400 170 L420 230" stroke="#000" stroke-width="8"/>
            <path d="M160 215 L240 215 L280 185" stroke="#4b5563" stroke-width="14" stroke-linecap="round"/>
            <path d="M220 210 L285 180" stroke="#f59e0b" stroke-width="8" stroke-linecap="round"/>
            <path d="M140 170 L220 120 L300 110 L370 140 L350 190 L240 190 Z" fill="#dc2626"/>
            <path d="M220 120 L320 110 L270 160 Z" fill="#ffffff"/>
            <path d="M120 140 L210 110 L160 160 Z" fill="#111827"/>
            <path d="M340 130 C360 100, 420 120, 430 160 C400 170, 360 170, 340 130 Z" fill="#b91c1c"/>
            <polygon points="360,115 410,125 390,145" fill="#38bdf8" opacity="0.8"/>
            <polygon points="410,145 435,150 420,165" fill="#ffffff"/>
            <circle cx="310" cy="65" r="22" fill="#111827" stroke="#dc2626" stroke-width="4"/>
            <path d="M315 55 Q330 65 325 75" stroke="#f59e0b" stroke-width="6" fill="none"/>
            <path d="M230 130 C240 80, 290 85, 310 90 L270 135 Z" fill="#1f2937"/>
            <path d="M290 90 L350 110 L330 130" stroke="#dc2626" stroke-width="12" stroke-linecap="round" fill="none"/>
          </svg>
        </div>
      </div>
      <div class="w-full h-3 curb-pattern"></div>
    </div>
  </section>

  <!-- TELA 4: SELEÇÃO DE NÍVEIS E RANKING -->
  <section id="screenLevels" class="hidden flex-1 max-w-5xl w-full mx-auto p-4 sm:p-6 space-y-8">
    <div class="glass-card p-4 rounded-2xl border-red-500/30 flex flex-wrap justify-between items-center gap-4">
      <div>
        <span class="text-xs text-slate-400 uppercase font-semibold block">Operador Conectado</span>
        <h3 class="text-lg font-bold text-white flex items-center gap-2">
          <i class="fa-solid fa-user-circle text-red-500"></i>
          <span id="displayPlayerName">---</span> 
          <span class="text-xs font-normal text-slate-400">(Matrícula: <span id="displayPlayerMatricula">---</span>)</span>
        </h3>
      </div>
      <div class="flex items-center gap-3">
        <div class="text-right bg-black/40 px-4 py-1.5 rounded-xl border border-yellow-500/30">
          <span class="text-[10px] text-slate-400 uppercase block">Pontuação Total</span>
          <span id="displayPlayerScore" class="text-lg font-black text-yellow-400">0 pts</span>
        </div>
        <button onclick="goToCover()" class="px-3 py-2 bg-red-900/60 hover:bg-red-800 text-xs font-semibold rounded-xl border border-red-500/40 transition flex items-center gap-1.5">
          <i class="fa-solid fa-house text-red-300"></i> Capa Inicial
        </button>
      </div>
    </div>

    <!-- Grid de Níveis (Totalmente Desbloqueados) -->
    <div>
      <div class="flex justify-between items-center mb-4">
        <h2 class="text-xl font-bold font-game flex items-center gap-2">
          <i class="fa-solid fa-layer-group text-red-500"></i> Níveis de Desafio
        </h2>
      </div>
      <div id="levelsGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4"></div>
    </div>

    <!-- Tabela de Ranking da Operação -->
    <div class="glass-card p-6 rounded-2xl border-red-500/20">
      <div class="flex flex-wrap justify-between items-center gap-2 mb-4">
        <h2 class="text-xl font-bold flex items-center gap-2 font-game tracking-wide text-yellow-400">
          <i class="fa-solid fa-ranking-star"></i> Ranking da Operação
        </h2>
        <span id="dbStatusBadge" class="text-xs px-2.5 py-1 rounded-full bg-slate-800 text-slate-400 border border-slate-700 flex items-center gap-1.5">
          <i class="fa-solid fa-circle-check text-green-400"></i> Ranking Ativo
        </span>
      </div>
      <div class="overflow-x-auto">
        <table class="w-full text-left text-sm">
          <thead>
            <tr class="border-b border-slate-700 text-slate-400 text-xs uppercase">
              <th class="p-3">Posição</th>
              <th class="p-3">Operador</th>
              <th class="p-3">Matrícula</th>
              <th class="p-3">Progresso</th>
              <th class="p-3 text-right">Pontos</th>
            </tr>
          </thead>
          <tbody id="rankingTableBody">
            <tr>
              <td colspan="5" class="p-4 text-center text-slate-500 italic">Carregando classificação...</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </section>

  <!-- TELA 5: EXECUÇÃO DO JOGO -->
  <section id="screenGame" class="hidden flex-1 max-w-3xl w-full mx-auto p-4 sm:p-6 flex flex-col justify-center">
    <div class="glass-card p-6 sm:p-8 rounded-3xl border-red-500/30 space-y-6 relative">
      <div class="absolute inset-0 bg-red-900/5 blur-xl -z-10 rounded-3xl"></div>
      <div class="flex justify-between items-center border-b border-slate-700/60 pb-4">
        <div>
          <span id="gameLevelTitle" class="text-xs font-bold text-red-400 uppercase tracking-widest block font-game">Nível 1</span>
          <div class="flex items-center gap-2 mt-0.5">
            <h2 id="gameRoundTitle" class="text-lg font-bold font-game">Rodada 1 de 3</h2>
            <span id="roundStatusBadge" class="hidden text-[10px] bg-yellow-500/20 text-yellow-300 border border-yellow-500/40 px-2 py-0.5 rounded-full font-semibold">Já Concluída</span>
          </div>
        </div>
        <div class="text-right">
          <span class="text-xs text-slate-400 block">Sua Pontuação</span>
          <span id="gameScoreDisplay" class="text-2xl font-black text-yellow-400">0 pts</span>
        </div>
      </div>

      <div id="cluesContainer" class="space-y-3"></div>

      <form id="formAnswer" onsubmit="handleAnswerSubmit(event)" class="space-y-3 pt-2">
        <label class="block text-xs font-semibold uppercase text-slate-300">Sua Resposta para a Pista Ativa:</label>
        <div class="flex gap-2">
          <input type="text" id="inputAnswer" autocomplete="off" required placeholder="Digite a resposta..." class="flex-1 px-4 py-3 bg-black/60 border border-slate-700 rounded-xl text-white focus:outline-none focus:border-red-500 transition">
          <button type="submit" class="px-6 py-3 honda-red honda-red-hover text-white font-bold rounded-xl transition flex items-center gap-2">
            <span>ENVIAR</span> <i class="fa-solid fa-paper-plane"></i>
          </button>
        </div>
      </form>

      <div class="pt-2 text-center">
        <button onclick="showLevelsScreen()" class="text-xs text-slate-400 hover:text-white transition underline">
          <i class="fa-solid fa-arrow-left"></i> Voltar à Seleção de Níveis
        </button>
      </div>
    </div>
  </section>

  <!-- MODAL CENTRALIZADO -->
  <div id="modalOverlay" class="hidden fixed inset-0 z-50 modal-backdrop flex justify-center items-center p-4">
    <div id="modalCard" class="max-w-md w-full glass-card p-6 sm:p-8 rounded-3xl border text-center shadow-2xl transform transition-all duration-200 scale-95 opacity-0">
      <div id="modalIconContainer" class="mb-4"></div>
      <h3 id="modalTitle" class="text-2xl font-bold mb-2 font-game">---</h3>
      <p id="modalMessage" class="text-sm text-slate-300 mb-6">---</p>
      <button id="modalButton" onclick="closeModal()" class="w-full py-3 font-bold rounded-xl text-white transition">CONTINUAR</button>
    </div>
  </div>

  <footer class="py-4 text-center text-xs text-slate-500 border-t border-slate-800/60 mt-auto">
    <p>Treinamento Operacional Honda &amp; Bulgarelli Advogados — © 2026</p>
  </footer>

  <!-- SCRIPT UNIFICADO -->
  <script>
    let audioCtx = null;

    function initAudio() {
        try {
            if (!audioCtx) {
                const AudioContextClass = window.AudioContext || window.webkitAudioContext;
                if (AudioContextClass) audioCtx = new AudioContextClass();
            }
            if (audioCtx && audioCtx.state === 'suspended') {
                audioCtx.resume();
            }
        } catch (e) {
            console.warn("Web Audio API não suportada ou bloqueada pelo navegador.");
        }
    }

    function playEngineLaunchAudio() {
        if (!audioCtx) return;
        try {
            const now = audioCtx.currentTime;
            const oscFundamental = audioCtx.createOscillator();
            const oscHarmonic = audioCtx.createOscillator();
            const gainNode = audioCtx.createGain();
            const filterNode = audioCtx.createBiquadFilter();

            oscFundamental.type = 'sawtooth';
            oscHarmonic.type = 'triangle';

            filterNode.type = 'lowpass';
            filterNode.frequency.setValueAtTime(450, now);
            filterNode.frequency.exponentialRampToValueAtTime(3200, now + 0.8);
            filterNode.Q.setValueAtTime(4, now);

            oscFundamental.frequency.setValueAtTime(75, now);
            oscFundamental.frequency.linearRampToValueAtTime(140, now + 0.25);
            oscFundamental.frequency.exponentialRampToValueAtTime(560, now + 1.05);

            oscHarmonic.frequency.setValueAtTime(150, now);
            oscHarmonic.frequency.linearRampToValueAtTime(280, now + 0.25);
            oscHarmonic.frequency.exponentialRampToValueAtTime(1120, now + 1.05);

            gainNode.gain.setValueAtTime(0.08, now);
            gainNode.gain.linearRampToValueAtTime(0.35, now + 0.3);
            gainNode.gain.linearRampToValueAtTime(0.6, now + 0.9);
            gainNode.gain.exponentialRampToValueAtTime(0.001, now + 1.4);

            oscFundamental.connect(filterNode);
            oscHarmonic.connect(filterNode);
            filterNode.connect(gainNode);
            gainNode.connect(audioCtx.destination);

            oscFundamental.start(now);
            oscHarmonic.start(now);
            oscFundamental.stop(now + 1.45);
            oscHarmonic.stop(now + 1.45);
        } catch(e){}
    }

    let isLaunching = false;

    window.startCarAccelerationTransition = function() {
        if (isLaunching) return;
        isLaunching = true;

        const carRoot = document.getElementById('carRoot');
        const startBtn = document.getElementById('engineStartBtn');
        const buttonLed = document.getElementById('buttonLed');
        const engineStatusText = document.getElementById('engineStatusText');
        const engineStatusDot = document.getElementById('engineStatusDot');
        const rpmGauge = document.getElementById('rpmGauge');
        const turboBoost = document.getElementById('turboBoost');
        const vtecState = document.getElementById('vtecState');
        const sceneWrapper = document.getElementById('sceneWrapper');
        const roadStripes = document.getElementById('roadStripes');
        const flashOverlay = document.getElementById('flashOverlay');

        initAudio();
        playEngineLaunchAudio();

        startBtn.classList.add('running');
        buttonLed.className = 'w-3 h-1 bg-green-400 rounded-full mt-1 shadow-[0_0_8px_#4ade80]';
        engineStatusText.innerText = 'VTEC ENGAGED';
        engineStatusDot.className = 'w-2.5 h-2.5 rounded-full bg-emerald-400 animate-ping';
        vtecState.innerText = 'STAGE: HIGH CAM 7000+';
        vtecState.className = 'text-red-400 font-bold';

        let currentRpm = 850;
        const rpmInterval = setInterval(() => {
            if (currentRpm < 7800) {
                currentRpm += 380;
                rpmGauge.innerText = `${currentRpm} RPM`;
                turboBoost.innerText = `BOOST: ${(Math.min(1.8, (currentRpm / 4500) * 1.6)).toFixed(1)} BAR`;
            }
        }, 40);

        roadStripes.classList.add('speeding');
        sceneWrapper.classList.add('shake-screen');
        carRoot.classList.remove('idle-vibe');
        carRoot.classList.add('launching');

        setTimeout(() => { flashOverlay.classList.add('active'); }, 900);
        setTimeout(() => { flashOverlay.classList.remove('active'); }, 1250);

        setTimeout(() => {
            clearInterval(rpmInterval);
            document.getElementById("screenCover").classList.add("hidden");
            
            // Se já houver sessão ativa, vai direto para os níveis
            if (currentPlayer.matricula) {
                showLevelsScreen();
            } else {
                goToRegistration();
            }
            
            carRoot.classList.remove('launching');
            sceneWrapper.classList.remove('shake-screen');
            roadStripes.classList.remove('speeding');
            carRoot.classList.add('idle-vibe');
            startBtn.classList.remove('running');
            buttonLed.className = 'w-3 h-1 bg-white rounded-full mt-1 shadow-[0_0_6px_#ffffff]';
            engineStatusText.innerText = 'ENGINE IDLE';
            engineStatusDot.className = 'w-2.5 h-2.5 rounded-full bg-red-600 animate-pulse';
            rpmGauge.innerText = '850 RPM';
            turboBoost.innerText = 'BOOST: 0.0 BAR';
            vtecState.innerText = 'STAGE: IDLE';
            vtecState.className = 'text-gray-400 font-semibold';
            isLaunching = false;
        }, 1350); 
    };

    /* DADOS DOS NÍVEIS (SEM BLOQUEIO DE DATA) */
    const gameLevels = [
      {
        id: 1,
        title: "Nível 1: Fase de Teste (Treinamento Livre)",
        rounds: [
          {
            id: "1-1",
            answer: "SAFRA DIARIA",
            clues: [
              { points: 10, text: "Dica 1: Segmento operacional focado nos contratos com menor tempo de inadimplência." },
              { points: 9, text: "Dica 2: Atende clientes com atrasos iniciais de 11 a 15 dias (e atualizados de 16 a 30 dias)." },
              { points: 8, text: "Dica 3: Foco em reabilitar o acesso do cliente às plataformas digitais de pagamento." }
            ],
            explanation: "Safra Diária é a faixa inicial de cobrança operacional para atrasos recentes."
          },
          {
            id: "1-2",
            answer: "CONFIRMACAO POSITIVA",
            clues: [
              { points: 10, text: "Dica 1: Procedimento obrigatório de monitoria de qualidade antes de passar dados do débito." },
              { points: 9, text: "Dica 2: Exige solicitar o nome completo mais os 3 primeiros dígitos do CPF do cliente." },
              { points: 8, text: "Dica 3: Pode ser feita também confirmando marca, modelo e ano do veículo se houver recusa do CPF." }
            ],
            explanation: "A confirmação positiva garante a segurança das informações e evita quebra de sigilo."
          },
          {
            id: "1-3",
            answer: "ATENDIMENTO HUMANIZADO",
            clues: [
              { points: 10, text: "Dica 1: Prática de comunicação focada na escuta ativa e empatia durante o contato." },
              { points: 9, text: "Dica 2: Saber se colocar no lugar do cliente, entendendo o imprevisto financeiro." },
              { points: 8, text: "Dica 3: Cativa o cliente para um atendimento diferenciado em vez de apenas impor cobrança." }
            ],
            explanation: "Atendimento Humanizado busca criar relacionamento e resolver a inadimplência com empatia."
          }
        ]
      },
      {
        id: 2,
        title: "Nível 2: Procedimentos & Validação",
        rounds: [
          {
            id: "2-1",
            answer: "OCORRENCIA 2600",
            clues: [
              { points: 10, text: "Dica 1: Status acionado em sistema quando o cliente pagou por engano uma parcela futura." },
              { points: 9, text: "Dica 2: Exige do operador a inclusão do texto 'Cliente solicita realocação da parcela nº...'." },
              { points: 8, text: "Dica 3: É puxada diariamente às 17h pelo Backoffice para envio ao banco via planilha." }
            ],
            explanation: "A ocorrência 2600 é utilizada para solicitar o processo de realocação de parcela paga incorretamente."
          },
          {
            id: "2-2",
            answer: "BOLETO COMPLEMENTAR",
            clues: [
              { points: 10, text: "Dica 1: Emitido pela Honda quando o valor pago na parcela errada é menor que o valor correto." },
              { points: 9, text: "Dica 2: Necessário para cobrir a diferença financeira no processo de realocação." },
              { points: 8, text: "Dica 3: É gerado atualizando os juros até a sua nova data de vencimento." }
            ],
            explanation: "Se o valor pago na parcela de destino for insuficiente, a Honda gera um boleto complementar."
          },
          {
            id: "2-3",
            answer: "OCORRENCIA 2601",
            clues: [
              { points: 10, text: "Dica 1: Solicitação obrigatória direcionada ao setor Jurídico em contratos ajuizados." },
              { points: 9, text: "Dica 2: Exige informar Tipo de Acordo (Atualização ou Quitação), Parcelas, Vencimento e UF." },
              { points: 8, text: "Dica 3: Usada para obter autorização e formalização de propostas em ações judiciais." }
            ],
            explanation: "A Ocorrência 2601 é indispensável para solicitar autorização do Jurídico antes de fechar acordo ajuizado."
          }
        ]
      },
      {
        id: 3,
        title: "Nível 3: Argumentação & Objeções",
        rounds: [
          {
            id: "3-1",
            answer: "BOLETIM DE OCORRENCIA",
            clues: [
              { points: 10, text: "Dica 1: Documento indispensável a ser solicitado ao cliente em casos de veículo roubado ou furtado." },
              { points: 9, text: "Dica 2: Encaminhado ao banco para análise de tentativa de concessão de desconto." },
              { points: 8, text: "Dica 3: Não isenta o cliente do débito, mantendo os juros diários até a regularização." }
            ],
            explanation: "Em casos de roubo do veículo, solicita-se o B.O. para tentar condições especiais com o Banco."
          },
          {
            id: "3-2",
            answer: "EXECUCAO DE BENS",
            clues: [
              { points: 10, text: "Dica 1: Medida judicial cabível quando a garantia (veículo) é perdida, roubada ou não localizada." },
              { points: 9, text: "Dica 2: O Banco pode ingressar contra o titular do contrato para reaver o prejuízo." },
              { points: 8, text: "Dica 3: Pode resultar na penhora de patrimônio ou bloqueio de contas bancárias do cliente." }
            ],
            explanation: "Quando a garantia se perde, o Banco pode mover ação de execução de bens e bloqueio de contas."
          },
          {
            id: "3-3",
            answer: "CESSAO DE DIREITOS",
            clues: [
              { points: 10, text: "Dica 1: Procedimento indicado quando o titular falece ou transfere o financiamento a terceiros." },
              { points: 9, text: "Dica 2: Realizado diretamente na Honda para alterar formalmente a titularidade do contrato." },
              { points: 8, text: "Dica 3: Exige a prévia regularização do débito em atraso pelo herdeiro ou interessado." }
            ],
            explanation: "A Cessão de Direitos transfere o contrato para o nome do herdeiro/terceiro após quitar os débitos."
          }
        ]
      },
      {
        id: 4,
        title: "Nível 4: Negociação & Jurídico",
        rounds: [
          {
            id: "4-1",
            answer: "ENTREGA AMIGAVEL",
            clues: [
              { points: 10, text: "Dica 1: Procedimento obrigatório de oferta para contratos que possuem mais de 50% em aberto." },
              { points: 9, text: "Dica 2: Devolução voluntária do veículo quando o cliente não tem mais condições de pagar." },
              { points: 8, text: "Dica 3: Evita a inclusão de custas extras de busca e apreensão como guincho e pátio." }
            ],
            explanation: "A Entrega Amigável deve ser oferecida a clientes sem condições financeiras de manter as parcelas."
          },
          {
            id: "4-2",
            answer: "BANCO HONDA",
            clues: [
              { points: 10, text: "Dica 1: Razão Social obrigatória a ser informada no script antifraude do fechamento." },
              { points: 9, text: "Dica 2: Deve constar como beneficiário do boleto sob o CNPJ 03.634.220/0001-65." },
              { points: 8, text: "Dica 3: O código de barras emitido para este credor sempre se inicia com os dígitos 237." }
            ],
            explanation: "No Fechamento Antifraude, confirma-se o beneficiário Banco Honda, CNPJ e início de código 237."
          },
          {
            id: "4-3",
            answer: "CUSTAS PROCESSUAIS",
            clues: [
              { points: 10, text: "Dica 1: Valores incorporados à dívida quando o contrato entra em vias de ajuizamento." },
              { points: 9, text: "Dica 2: Inclui a cobrança do valor mínimo de 1% do valor da causa no agravamento." },
              { points: 8, text: "Dica 3: Seu pagamento juntamente com o atraso é obrigatório para paralisar a ação." }
            ],
            explanation: "Ao ser ajuizado, somam-se custas processuais ao débito que devem ser pagas para suspender a ação."
          }
        ]
      },
      {
        id: 5,
        title: "Nível 5: Casos Especiais & Regras SPF",
        rounds: [
          {
            id: "5-1",
            answer: "SEGURO PROTECAO FINANCEIRA",
            clues: [
              { points: 10, text: "Dica 1: Benefício verificado na tela de início (F1) em casos de desemprego ou óbito." },
              { points: 9, text: "Dica 2: Pode cobrir até 6 parcelas do contrato no caso de demissão involuntária." },
              { points: 8, text: "Dica 3: Em caso de falecimento do titular, a seguradora pode quitar o saldo devedor." }
            ],
            explanation: "O Seguro Proteção Financeira (SPF) garante a quitação de parcelas ou do saldo em imprevistos."
          },
          {
            id: "5-2",
            answer: "QUEBRA DE SIGILO",
            clues: [
              { points: 10, text: "Dica 1: Considerada uma Não Conformidade Grave (NCG) na monitoria de qualidade." },
              { points: 9, text: "Dica 2: Ocorre ao informar dados da dívida antes de validar a confirmação positiva." },
              { points: 8, text: "Dica 3: Passar informações do contrato para terceiros não autorizados sem validação de dados." }
            ],
            explanation: "Passar dados do contrato sem a confirmação positiva do cliente caracteriza Quebra de Sigilo."
          },
          {
            id: "5-3",
            answer: "RESTRICAO SPC SERASA",
            clues: [
              { points: 10, text: "Dica 1: Consequência de inadimplência informada na argumentação de cobrança." },
              { points: 9, text: "Dica 2: O envio para a negativação no SPC ocorre aos 21 dias de atraso." },
              { points: 8, text: "Dica 3: Ao atingir 31 dias de atraso, o CPF do cliente é encaminhado ao SERASA." }
            ],
            explanation: "A inclusão de restrição de crédito é direcionada ao SPC com 21 dias e ao SERASA aos 31 dias."
          }
        ]
      }
    ];

    let currentPlayer = { name: "", matricula: "", score: 0, completedRounds: 0, completedRoundIds: [], updatedAt: 0 };
    let currentRoundState = { levelId: null, roundIndex: 0, clueIndex: 0, roundData: null };
    let localRanking = JSON.parse(localStorage.getItem("honda_ranking") || "[]");

    // CARREGAR SESSÃO PERSISTENTE SE EXISTIR
    window.addEventListener("DOMContentLoaded", () => {
      const savedSession = sessionStorage.getItem("honda_active_session");
      if (savedSession) {
        try {
          const parsed = JSON.parse(savedSession);
          if (parsed.matricula) {
            currentPlayer = parsed;
            const updatedRanking = localRanking.find(p => p.matricula === currentPlayer.matricula);
            if (updatedRanking) {
              currentPlayer.score = updatedRanking.score;
              currentPlayer.completedRoundIds = updatedRanking.completedRoundIds || [];
            }
          }
        } catch(e){}
      }
    });

    function sanitizeMatricula(str) {
      return String(str).replace(/[^a-zA-Z0-9_\.-]/g, "").trim().toUpperCase();
    }

    function escapeHTML(str) {
      return String(str || "").replace(/[&<>"']/g, m => ({
        "&": "&amp;", "<": "&lt;", ">": "&gt;", '"': "&quot;", "'": "&#39;"
      }[m]));
    }

    function normalizeString(str) {
      return String(str || "")
        .toLowerCase()
        .normalize("NFD")
        .replace(/[\u0300-\u036f]/g, "")
        .replace(/[^a-z0-9]/g, "");
    }

    window.goToCover = function() {
      document.getElementById("screenCover").classList.remove("hidden");
      document.getElementById("screenRegistration").classList.add("hidden");
      document.getElementById("screenTransitionMoto").classList.add("hidden");
      document.getElementById("screenLevels").classList.add("hidden");
      document.getElementById("screenGame").classList.add("hidden");
      document.getElementById("appHeader").classList.add("hidden");
    };

    window.goToRegistration = function() {
      document.getElementById("screenCover").classList.add("hidden");
      document.getElementById("screenTransitionMoto").classList.add("hidden");
      document.getElementById("screenRegistration").classList.remove("hidden");
      document.getElementById("screenLevels").classList.add("hidden");
      document.getElementById("screenGame").classList.add("hidden");
    };

    window.logoutSession = function() {
      sessionStorage.removeItem("honda_active_session");
      currentPlayer = { name: "", matricula: "", score: 0, completedRounds: 0, completedRoundIds: [], updatedAt: 0 };
      goToRegistration();
    };

    window.handleRegistrationSubmit = function(e) {
      e.preventDefault();
      const name = document.getElementById("inputName").value.trim();
      const rawMatricula = document.getElementById("inputMatricula").value;
      const matricula = sanitizeMatricula(rawMatricula);

      if (!name || !matricula) {
        alert("Por favor, preencha nome e matrícula corretamente.");
        return;
      }

      currentPlayer.name = name;
      currentPlayer.matricula = matricula;

      const saved = localRanking.find(p => p.matricula === matricula);
      if (saved) {
        currentPlayer.score = saved.score || 0;
        currentPlayer.completedRoundIds = saved.completedRoundIds || [];
      }

      sessionStorage.setItem("honda_active_session", JSON.stringify(currentPlayer));

      document.getElementById("screenRegistration").classList.add("hidden");
      const transMoto = document.getElementById("screenTransitionMoto");
      transMoto.classList.remove("hidden");

      setTimeout(() => {
        transMoto.classList.add("hidden");
        showLevelsScreen();
      }, 1800);
    };

    function showLevelsScreen() {
      document.getElementById("screenCover").classList.add("hidden");
      document.getElementById("screenRegistration").classList.add("hidden");
      document.getElementById("screenTransitionMoto").classList.add("hidden");
      document.getElementById("screenGame").classList.add("hidden");
      document.getElementById("screenLevels").classList.remove("hidden");
      document.getElementById("appHeader").classList.remove("hidden");

      document.getElementById("headerPlayerName").innerText = currentPlayer.name;
      document.getElementById("headerPlayerMatricula").innerText = currentPlayer.matricula;
      document.getElementById("headerPlayerScore").innerText = `${currentPlayer.score} pts`;

      document.getElementById("displayPlayerName").innerText = currentPlayer.name;
      document.getElementById("displayPlayerMatricula").innerText = currentPlayer.matricula;
      document.getElementById("displayPlayerScore").innerText = `${currentPlayer.score} pts`;

      renderLevelsGrid();
      renderRankingTable(localRanking);
    }

    function renderLevelsGrid() {
      const grid = document.getElementById("levelsGrid");
      grid.innerHTML = "";

      gameLevels.forEach(lvl => {
        const totalRounds = lvl.rounds.length;
        const doneRounds = lvl.rounds.filter(r => currentPlayer.completedRoundIds.includes(r.id)).length;

        const card = document.createElement("div");
        card.className = "glass-card p-5 rounded-2xl border border-red-500/40 hover:border-red-500 transition duration-300 flex flex-col justify-between";

        const statusTag = `<span class="text-[10px] px-2 py-0.5 rounded-full bg-green-950 text-green-300 border border-green-500/40 font-bold">Disponível</span>`;

        card.innerHTML = `
          <div>
            <div class="flex justify-between items-start mb-2">
              <h3 class="font-bold text-base text-white">${escapeHTML(lvl.title)}</h3>
              ${statusTag}
            </div>
            <p class="text-xs text-slate-400 mb-4">${doneRounds}/${totalRounds} rodadas concluídas</p>
          </div>
          <button onclick="startLevel(${lvl.id})" 
            class="w-full py-2.5 rounded-xl font-bold text-xs flex items-center justify-center gap-2 transition honda-red honda-red-hover text-white shadow-md shadow-red-900/40">
            <span>INICIAR DESAFIO</span>
            <i class="fa-solid fa-play"></i>
          </button>
        `;
        grid.appendChild(card);
      });
    }

    window.startLevel = function(levelId) {
      const lvl = gameLevels.find(l => l.id === levelId);
      if (!lvl) return;

      currentRoundState = { levelId: levelId, roundIndex: 0, clueIndex: 0, roundData: lvl.rounds[0] };
      setupRoundDisplay();

      document.getElementById("screenLevels").classList.add("hidden");
      document.getElementById("screenGame").classList.remove("hidden");
    };

    function setupRoundDisplay() {
      const lvl = gameLevels.find(l => l.id === currentRoundState.levelId);
      const round = lvl.rounds[currentRoundState.roundIndex];
      currentRoundState.roundData = round;
      currentRoundState.clueIndex = 0;

      document.getElementById("gameLevelTitle").innerText = lvl.title;
      document.getElementById("gameRoundTitle").innerText = `Rodada ${currentRoundState.roundIndex + 1} de ${lvl.rounds.length}`;
      document.getElementById("gameScoreDisplay").innerText = `${currentPlayer.score} pts`;

      const badge = document.getElementById("roundStatusBadge");
      if (currentPlayer.completedRoundIds.includes(round.id)) {
        badge.classList.remove("hidden");
      } else {
        badge.classList.add("hidden");
      }

      document.getElementById("inputAnswer").value = "";
      renderClues();
      setTimeout(() => document.getElementById("inputAnswer").focus(), 100);
    }

    function renderClues() {
      const container = document.getElementById("cluesContainer");
      container.innerHTML = "";

      const round = currentRoundState.roundData;
      for (let i = 0; i <= currentRoundState.clueIndex; i++) {
        const clue = round.clues[i];
        const clueDiv = document.createElement("div");
        clueDiv.className = "glass-card p-4 rounded-xl border border-red-500/30 flex items-start gap-3";
        clueDiv.innerHTML = `
          <div class="bg-red-600/30 text-yellow-400 font-bold px-2.5 py-1 rounded-lg text-xs border border-red-500/40 whitespace-nowrap">
            ${clue.points} Pts
          </div>
          <p class="text-xs sm:text-sm text-slate-200 leading-relaxed">${escapeHTML(clue.text)}</p>
        `;
        container.appendChild(clueDiv);
      }
    }

    window.handleAnswerSubmit = function(e) {
      e.preventDefault();
      const input = document.getElementById("inputAnswer");
      const userAns = normalizeString(input.value);
      const expectedAns = normalizeString(currentRoundState.roundData.answer);

      if (userAns === expectedAns) {
        const round = currentRoundState.roundData;
        const pointsEarned = round.clues[currentRoundState.clueIndex].points;

        if (!currentPlayer.completedRoundIds.includes(round.id)) {
          currentPlayer.score += pointsEarned;
          currentPlayer.completedRoundIds.push(round.id);
          currentPlayer.updatedAt = Date.now();
          savePlayerToRanking();
        }

        showModal(
          `<i class="fa-solid fa-circle-check text-5xl text-green-400"></i>`,
          "Resposta Correta!",
          `Você acertou e acumulou +${pointsEarned} pontos!<br><br><span class="text-slate-400 text-xs">${round.explanation}</span>`,
          "PRÓXIMA RODADA",
          () => advanceGame()
        );
      } else {
        if (currentRoundState.clueIndex < 2) {
          currentRoundState.clueIndex++;
          renderClues();
          input.value = "";
          showModal(
            `<i class="fa-solid fa-circle-xmark text-5xl text-yellow-400"></i>`,
            "Ainda não é isso!",
            "Sua resposta está incorreta. Liberamos a próxima pista valendo menos pontos para você tentar novamente!",
            "TENTAR NOVAMENTE",
            () => setTimeout(() => document.getElementById("inputAnswer").focus(), 100)
          );
        } else {
          showModal(
            `<i class="fa-solid fa-face-frown text-5xl text-red-500"></i>`,
            "Fim das Pistas!",
            `Não foi desta vez. A resposta correta era: <strong class="text-yellow-400">${currentRoundState.roundData.answer}</strong>.<br><br><span class="text-slate-400 text-xs">${currentRoundState.roundData.explanation}</span>`,
            "CONTINUAR",
            () => advanceGame()
          );
        }
      }
    };

    function savePlayerToRanking() {
      const index = localRanking.findIndex(p => p.matricula === currentPlayer.matricula);
      const playerData = {
        name: currentPlayer.name,
        matricula: currentPlayer.matricula,
        score: currentPlayer.score,
        completedRounds: currentPlayer.completedRoundIds.length,
        completedRoundIds: currentPlayer.completedRoundIds,
        updatedAt: currentPlayer.updatedAt
      };

      if (index >= 0) {
        localRanking[index] = playerData;
      } else {
        localRanking.push(playerData);
      }

      localRanking.sort((a, b) => {
        if (b.score !== a.score) return b.score - a.score;
        if (b.completedRounds !== a.completedRounds) return b.completedRounds - a.completedRounds;
        return a.updatedAt - b.updatedAt;
      });

      localStorage.setItem("honda_ranking", JSON.stringify(localRanking));
      sessionStorage.setItem("honda_active_session", JSON.stringify(currentPlayer));
    }

    function advanceGame() {
      const lvl = gameLevels.find(l => l.id === currentRoundState.levelId);
      if (currentRoundState.roundIndex < lvl.rounds.length - 1) {
        currentRoundState.roundIndex++;
        setupRoundDisplay();
      } else {
        showModal(
          `<i class="fa-solid fa-trophy text-6xl text-yellow-400"></i>`,
          "Nível Concluído!",
          `Parabéns! Você completou todas as rodadas deste nível.<br>Sua pontuação atual é: <strong class="text-yellow-400">${currentPlayer.score} pts</strong>.`,
          "VOLTAR AO MENU",
          () => showLevelsScreen()
        );
      }
    }

    function showModal(iconHTML, title, message, btnText, callback) {
      document.getElementById("modalIconContainer").innerHTML = iconHTML;
      document.getElementById("modalTitle").innerHTML = title;
      document.getElementById("modalMessage").innerHTML = message;

      const btn = document.getElementById("modalButton");
      btn.innerHTML = btnText || "CONTINUAR";
      btn.className = "w-full py-3 font-bold rounded-xl text-white transition honda-red honda-red-hover shadow-lg shadow-red-900/50";

      window.modalCallback = callback;

      const overlay = document.getElementById("modalOverlay");
      const card = document.getElementById("modalCard");

      overlay.classList.remove("hidden");
      setTimeout(() => {
        card.classList.remove("scale-95", "opacity-0");
        card.classList.add("scale-100", "opacity-100");
      }, 10);
    }

    window.closeModal = function() {
      const overlay = document.getElementById("modalOverlay");
      const card = document.getElementById("modalCard");

      card.classList.remove("scale-100", "opacity-100");
      card.classList.add("scale-95", "opacity-0");

      setTimeout(() => {
        overlay.classList.add("hidden");
        if (window.modalCallback) {
          const cb = window.modalCallback;
          window.modalCallback = null;
          cb();
        }
      }, 200);
    };

    function renderRankingTable(rankingArray) {
      const tbody = document.getElementById("rankingTableBody");
      if (!tbody) return;
      tbody.innerHTML = "";

      if (rankingArray.length === 0) {
        tbody.innerHTML = `<tr><td colspan="5" class="p-4 text-center text-slate-500 italic">Nenhum operador registrado ainda. Seja o primeiro!</td></tr>`;
        return;
      }

      rankingArray.forEach((item, idx) => {
        const isCurrent = item.matricula === currentPlayer.matricula;
        let medal = `<span class="text-slate-400 font-semibold">#${idx + 1}</span>`;
        if (idx === 0) medal = `🥇 <span class="text-yellow-400 font-bold">1º</span>`;
        if (idx === 1) medal = `🥈 <span class="text-slate-300 font-bold">2º</span>`;
        if (idx === 2) medal = `🥉 <span class="text-amber-600 font-bold">3º</span>`;

        const tr = document.createElement("tr");
        tr.className = `border-b border-slate-800/80 transition ${isCurrent ? "bg-red-950/40 font-semibold text-white" : "hover:bg-white/5 text-slate-300"}`;
        tr.innerHTML = `
          <td class="p-3">${medal}</td>
          <td class="p-3 flex items-center gap-2">
            <i class="fa-solid fa-user text-xs ${isCurrent ? "text-red-400" : "text-slate-500"}"></i>
            <span>${escapeHTML(item.name)}</span>
            ${isCurrent ? '<span class="text-[10px] bg-red-600 text-white px-1.5 py-0.5 rounded uppercase">Você</span>' : ""}
          </td>
          <td class="p-3 text-slate-400">${escapeHTML(item.matricula)}</td>
          <td class="p-3 text-slate-400">${item.completedRounds}/15 rodadas</td>
          <td class="p-3 text-right font-bold text-yellow-400">${item.score} pts</td>
        `;
        tbody.appendChild(tr);
      });
    }
  </script>
</body>
</html>
