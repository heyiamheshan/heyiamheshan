<svg width="900" height="280" viewBox="0 0 900 280" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Background gradient -->
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0A0F1E;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#0D1B3E;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#0A0F1E;stop-opacity:1" />
    </linearGradient>

    <!-- Blue glow gradient -->
    <radialGradient id="glowLeft" cx="20%" cy="50%" r="40%">
      <stop offset="0%" style="stop-color:#1A56DB;stop-opacity:0.25" />
      <stop offset="100%" style="stop-color:#1A56DB;stop-opacity:0" />
    </radialGradient>
    <radialGradient id="glowRight" cx="80%" cy="50%" r="35%">
      <stop offset="0%" style="stop-color:#0EA5E9;stop-opacity:0.15" />
      <stop offset="100%" style="stop-color:#0EA5E9;stop-opacity:0" />
    </radialGradient>

    <!-- Animated glow pulse -->
    <radialGradient id="pulseGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" style="stop-color:#1A56DB;stop-opacity:0.08" />
      <stop offset="100%" style="stop-color:#1A56DB;stop-opacity:0" />
    </radialGradient>

    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="strongGlow">
      <feGaussianBlur stdDeviation="5" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="textGlow">
      <feGaussianBlur stdDeviation="8" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <clipPath id="svgClip">
      <rect width="900" height="280" rx="16"/>
    </clipPath>
  </defs>

  <g clip-path="url(#svgClip)">
    <!-- Base background -->
    <rect width="900" height="280" fill="url(#bgGrad)"/>

    <!-- Ambient glow layers -->
    <rect width="900" height="280" fill="url(#glowLeft)"/>
    <rect width="900" height="280" fill="url(#glowRight)"/>

    <!-- Animated center pulse -->
    <rect width="900" height="280" fill="url(#pulseGlow)">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="4s" repeatCount="indefinite"/>
    </rect>

    <!-- Grid lines - horizontal -->
    <g opacity="0.07" stroke="#4A9EFF" stroke-width="0.5">
      <line x1="0" y1="35" x2="900" y2="35"/>
      <line x1="0" y1="70" x2="900" y2="70"/>
      <line x1="0" y1="105" x2="900" y2="105"/>
      <line x1="0" y1="140" x2="900" y2="140"/>
      <line x1="0" y1="175" x2="900" y2="175"/>
      <line x1="0" y1="210" x2="900" y2="210"/>
      <line x1="0" y1="245" x2="900" y2="245"/>
    </g>
    <!-- Grid lines - vertical -->
    <g opacity="0.07" stroke="#4A9EFF" stroke-width="0.5">
      <line x1="90" y1="0" x2="90" y2="280"/>
      <line x1="180" y1="0" x2="180" y2="280"/>
      <line x1="270" y1="0" x2="270" y2="280"/>
      <line x1="360" y1="0" x2="360" y2="280"/>
      <line x1="450" y1="0" x2="450" y2="280"/>
      <line x1="540" y1="0" x2="540" y2="280"/>
      <line x1="630" y1="0" x2="630" y2="280"/>
      <line x1="720" y1="0" x2="720" y2="280"/>
      <line x1="810" y1="0" x2="810" y2="280"/>
    </g>

    <!-- Neural network nodes - LEFT SIDE -->
    <!-- Layer 1 nodes -->
    <circle cx="80" cy="80" r="5" fill="#1A56DB" filter="url(#glow)" opacity="0.9">
      <animate attributeName="r" values="5;7;5" dur="2.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.9;1;0.9" dur="2.5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="80" cy="140" r="5" fill="#1A56DB" filter="url(#glow)" opacity="0.9">
      <animate attributeName="r" values="5;7;5" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.9;1;0.9" dur="3s" repeatCount="indefinite"/>
    </circle>
    <circle cx="80" cy="200" r="5" fill="#1A56DB" filter="url(#glow)" opacity="0.9">
      <animate attributeName="r" values="5;7;5" dur="2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.9;1;0.9" dur="2s" repeatCount="indefinite"/>
    </circle>

    <!-- Layer 2 nodes -->
    <circle cx="155" cy="60" r="5" fill="#0EA5E9" filter="url(#glow)" opacity="0.85">
      <animate attributeName="r" values="5;6.5;5" dur="2.2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="155" cy="110" r="5" fill="#0EA5E9" filter="url(#glow)" opacity="0.85">
      <animate attributeName="r" values="5;6.5;5" dur="2.8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="155" cy="160" r="5" fill="#0EA5E9" filter="url(#glow)" opacity="0.85">
      <animate attributeName="r" values="5;6.5;5" dur="3.2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="155" cy="210" r="5" fill="#0EA5E9" filter="url(#glow)" opacity="0.85">
      <animate attributeName="r" values="5;6.5;5" dur="2.6s" repeatCount="indefinite"/>
    </circle>

    <!-- Layer 3 nodes -->
    <circle cx="230" cy="80" r="5" fill="#1A56DB" filter="url(#glow)" opacity="0.9">
      <animate attributeName="r" values="5;7;5" dur="1.8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="230" cy="140" r="5" fill="#1A56DB" filter="url(#glow)" opacity="0.9">
      <animate attributeName="r" values="5;7;5" dur="2.4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="230" cy="200" r="5" fill="#1A56DB" filter="url(#glow)" opacity="0.9">
      <animate attributeName="r" values="5;7;5" dur="3s" repeatCount="indefinite"/>
    </circle>

    <!-- Neural network connections - L1 to L2 -->
    <g stroke="#1A56DB" stroke-width="0.8" opacity="0.3">
      <line x1="80" y1="80" x2="155" y2="60"><animate attributeName="opacity" values="0.3;0.7;0.3" dur="2s" repeatCount="indefinite"/></line>
      <line x1="80" y1="80" x2="155" y2="110"><animate attributeName="opacity" values="0.3;0.6;0.3" dur="2.5s" repeatCount="indefinite"/></line>
      <line x1="80" y1="80" x2="155" y2="160"><animate attributeName="opacity" values="0.2;0.5;0.2" dur="3s" repeatCount="indefinite"/></line>
      <line x1="80" y1="140" x2="155" y2="60"><animate attributeName="opacity" values="0.2;0.5;0.2" dur="2.2s" repeatCount="indefinite"/></line>
      <line x1="80" y1="140" x2="155" y2="110"><animate attributeName="opacity" values="0.3;0.7;0.3" dur="1.8s" repeatCount="indefinite"/></line>
      <line x1="80" y1="140" x2="155" y2="160"><animate attributeName="opacity" values="0.3;0.6;0.3" dur="2.7s" repeatCount="indefinite"/></line>
      <line x1="80" y1="140" x2="155" y2="210"><animate attributeName="opacity" values="0.2;0.5;0.2" dur="3.1s" repeatCount="indefinite"/></line>
      <line x1="80" y1="200" x2="155" y2="160"><animate attributeName="opacity" values="0.3;0.6;0.3" dur="2.3s" repeatCount="indefinite"/></line>
      <line x1="80" y1="200" x2="155" y2="210"><animate attributeName="opacity" values="0.3;0.7;0.3" dur="2s" repeatCount="indefinite"/></line>
    </g>
    <!-- L2 to L3 -->
    <g stroke="#0EA5E9" stroke-width="0.8" opacity="0.3">
      <line x1="155" y1="60" x2="230" y2="80"><animate attributeName="opacity" values="0.3;0.7;0.3" dur="2.4s" repeatCount="indefinite"/></line>
      <line x1="155" y1="60" x2="230" y2="140"><animate attributeName="opacity" values="0.2;0.5;0.2" dur="2.9s" repeatCount="indefinite"/></line>
      <line x1="155" y1="110" x2="230" y2="80"><animate attributeName="opacity" values="0.3;0.6;0.3" dur="2.1s" repeatCount="indefinite"/></line>
      <line x1="155" y1="110" x2="230" y2="140"><animate attributeName="opacity" values="0.3;0.7;0.3" dur="2.6s" repeatCount="indefinite"/></line>
      <line x1="155" y1="160" x2="230" y2="140"><animate attributeName="opacity" values="0.3;0.6;0.3" dur="1.9s" repeatCount="indefinite"/></line>
      <line x1="155" y1="160" x2="230" y2="200"><animate attributeName="opacity" values="0.3;0.7;0.3" dur="2.3s" repeatCount="indefinite"/></line>
      <line x1="155" y1="210" x2="230" y2="140"><animate attributeName="opacity" values="0.2;0.5;0.2" dur="3s" repeatCount="indefinite"/></line>
      <line x1="155" y1="210" x2="230" y2="200"><animate attributeName="opacity" values="0.3;0.6;0.3" dur="2.5s" repeatCount="indefinite"/></line>
    </g>

    <!-- Floating particles - RIGHT SIDE -->
    <g filter="url(#glow)">
      <circle cx="720" cy="50" r="2" fill="#4A9EFF" opacity="0.7">
        <animate attributeName="cy" values="50;30;50" dur="4s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.7;0.2;0.7" dur="4s" repeatCount="indefinite"/>
      </circle>
      <circle cx="760" cy="90" r="1.5" fill="#0EA5E9" opacity="0.6">
        <animate attributeName="cy" values="90;70;90" dur="3.5s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.6;0.1;0.6" dur="3.5s" repeatCount="indefinite"/>
      </circle>
      <circle cx="800" cy="140" r="2.5" fill="#1A56DB" opacity="0.8">
        <animate attributeName="cy" values="140;115;140" dur="5s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.8;0.3;0.8" dur="5s" repeatCount="indefinite"/>
      </circle>
      <circle cx="840" cy="80" r="2" fill="#4A9EFF" opacity="0.6">
        <animate attributeName="cy" values="80;60;80" dur="3.8s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.6;0.1;0.6" dur="3.8s" repeatCount="indefinite"/>
      </circle>
      <circle cx="870" cy="190" r="1.5" fill="#0EA5E9" opacity="0.7">
        <animate attributeName="cy" values="190;170;190" dur="4.5s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.7;0.2;0.7" dur="4.5s" repeatCount="indefinite"/>
      </circle>
      <circle cx="740" cy="210" r="2" fill="#1A56DB" opacity="0.5">
        <animate attributeName="cy" values="210;190;210" dur="3.2s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.5;0.1;0.5" dur="3.2s" repeatCount="indefinite"/>
      </circle>
      <circle cx="690" cy="160" r="1.5" fill="#4A9EFF" opacity="0.6">
        <animate attributeName="cy" values="160;145;160" dur="4.2s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.6;0.2;0.6" dur="4.2s" repeatCount="indefinite"/>
      </circle>
      <circle cx="820" cy="230" r="2" fill="#0EA5E9" opacity="0.5">
        <animate attributeName="cy" values="230;210;230" dur="3.6s" repeatCount="indefinite"/>
        <animate attributeName="opacity" values="0.5;0.1;0.5" dur="3.6s" repeatCount="indefinite"/>
      </circle>
    </g>

    <!-- Scanning line animation -->
    <rect x="0" y="0" width="900" height="2" fill="url(#glowLeft)" opacity="0.4">
      <animate attributeName="y" values="-2;282;-2" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.4;0" dur="6s" repeatCount="indefinite"/>
    </rect>

    <!-- Divider line between neural net and text -->
    <line x1="270" y1="30" x2="270" y2="250" stroke="#1A56DB" stroke-width="0.5" opacity="0.3"/>

    <!-- ── MAIN TEXT CONTENT ── -->

    <!-- Name -->
    <text x="450" y="95" font-family="'Courier New', Courier, monospace" font-size="36" font-weight="bold"
          fill="#FFFFFF" text-anchor="middle" filter="url(#textGlow)" letter-spacing="2">
      Heshan Pramuditha
      <animate attributeName="opacity" values="0;1" dur="1.2s" fill="freeze"/>
    </text>
    <text x="450" y="133" font-family="'Courier New', Courier, monospace" font-size="36" font-weight="bold"
          fill="#FFFFFF" text-anchor="middle" filter="url(#textGlow)" letter-spacing="2">
      Dharmasena
      <animate attributeName="opacity" values="0;1" dur="1.5s" fill="freeze"/>
    </text>

    <!-- Animated blue underline -->
    <rect x="310" y="142" width="0" height="2" fill="#1A56DB" rx="1" filter="url(#glow)">
      <animate attributeName="width" values="0;280" dur="1.8s" fill="freeze" begin="0.5s"/>
    </rect>

    <!-- Role badge -->
    <rect x="320" y="158" width="260" height="28" rx="14" fill="#1A56DB" opacity="0.15" stroke="#1A56DB" stroke-width="0.8" stroke-opacity="0.5">
      <animate attributeName="opacity" values="0;0.15" dur="2s" fill="freeze"/>
    </rect>
    <text x="450" y="177" font-family="'Courier New', Courier, monospace" font-size="13"
          fill="#4A9EFF" text-anchor="middle" letter-spacing="1.5">
      AI &amp; ML DEVELOPER
      <animate attributeName="opacity" values="0;1" dur="2s" fill="freeze"/>
    </text>

    <!-- University -->
    <text x="450" y="208" font-family="'Courier New', Courier, monospace" font-size="12"
          fill="#94A3B8" text-anchor="middle" letter-spacing="0.5">
      University of Kelaniya · Sri Lanka
      <animate attributeName="opacity" values="0;1" dur="2.2s" fill="freeze"/>
    </text>

    <!-- Tags row -->
    <!-- Tag 1: Computer Vision -->
    <rect x="315" y="220" width="115" height="22" rx="4" fill="#0D1B3E" stroke="#1A56DB" stroke-width="0.6" stroke-opacity="0.6">
      <animate attributeName="opacity" values="0;1" dur="2.5s" fill="freeze"/>
    </rect>
    <text x="372" y="235" font-family="'Courier New', Courier, monospace" font-size="10"
          fill="#4A9EFF" text-anchor="middle" letter-spacing="0.5">
      Computer Vision
      <animate attributeName="opacity" values="0;1" dur="2.5s" fill="freeze"/>
    </text>

    <!-- Tag 2: RAG Systems -->
    <rect x="438" y="220" width="90" height="22" rx="4" fill="#0D1B3E" stroke="#0EA5E9" stroke-width="0.6" stroke-opacity="0.6">
      <animate attributeName="opacity" values="0;1" dur="2.7s" fill="freeze"/>
    </rect>
    <text x="483" y="235" font-family="'Courier New', Courier, monospace" font-size="10"
          fill="#0EA5E9" text-anchor="middle" letter-spacing="0.5">
      RAG Systems
      <animate attributeName="opacity" values="0;1" dur="2.7s" fill="freeze"/>
    </text>

    <!-- Tag 3: LLMs -->
    <rect x="536" y="220" width="50" height="22" rx="4" fill="#0D1B3E" stroke="#4A9EFF" stroke-width="0.6" stroke-opacity="0.6">
      <animate attributeName="opacity" values="0;1" dur="2.9s" fill="freeze"/>
    </rect>
    <text x="561" y="235" font-family="'Courier New', Courier, monospace" font-size="10"
          fill="#4A9EFF" text-anchor="middle" letter-spacing="0.5">
      LLMs
      <animate attributeName="opacity" values="0;1" dur="2.9s" fill="freeze"/>
    </text>

    <!-- Bottom status bar -->
    <rect x="0" y="263" width="900" height="17" fill="#0D1B3E" opacity="0.6"/>
    <circle cx="18" cy="271" r="4" fill="#1A56DB" filter="url(#glow)">
      <animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/>
    </circle>
    <text x="30" y="275" font-family="'Courier New', Courier, monospace" font-size="9"
          fill="#4A9EFF" letter-spacing="1">
      OPEN TO INTERNSHIPS · AI/ML ENGINEERING · DATA SCIENCE
    </text>
    <text x="870" y="275" font-family="'Courier New', Courier, monospace" font-size="9"
          fill="#1A56DB" text-anchor="end" letter-spacing="0.5" opacity="0.8">
      🇱🇰 SRI LANKA
    </text>

    <!-- Corner accent dots -->
    <circle cx="12" cy="12" r="3" fill="#1A56DB" opacity="0.6" filter="url(#glow)"/>
    <circle cx="888" cy="12" r="3" fill="#1A56DB" opacity="0.6" filter="url(#glow)"/>
    <circle cx="12" cy="255" r="3" fill="#1A56DB" opacity="0.6" filter="url(#glow)"/>
    <circle cx="888" cy="255" r="3" fill="#1A56DB" opacity="0.6" filter="url(#glow)"/>

    <!-- Border -->
    <rect width="900" height="280" rx="16" fill="none" stroke="#1A56DB" stroke-width="1" opacity="0.25"/>
  </g>
</svg>
