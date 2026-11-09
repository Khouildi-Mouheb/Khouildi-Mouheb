<svg xmlns="http://www.w3.org/2000/svg" xml:space="preserve" width="1200" height="300" viewBox="0 0 1200 300" role="img" aria-label="Mouheb Khouildi — terminal banner">
  <style>
    .mono { font-family: "JetBrains Mono", "Fira Code", Consolas, "Courier New", monospace; }
    .prompt { fill: #3fb950; }
    .path { fill: #58a6ff; }
    .cmd { fill: #e6edf3; }
    .dim { fill: #7d8590; }
    .name { fill: #e6edf3; font-weight: 700; }
    .accent { fill: #f0883e; }
    .line1 { clip-path: url(#reveal1); }
    .line2 { opacity: 0; animation: fade 0.4s ease forwards 2.2s; }
    .line3 { opacity: 0; animation: fade 0.4s ease forwards 2.7s; }
    .line4 { opacity: 0; animation: fade 0.4s ease forwards 3.2s; }
    .cursor { animation: blink 1s steps(1) infinite; }
    @keyframes fade { to { opacity: 1; } }
    @keyframes blink { 50% { opacity: 0; } }
    @keyframes type { from { width: 0; } to { width: 760px; } }
    #revealRect { animation: type 2s steps(46) forwards; }
  </style>

  <defs>
    <clipPath id="reveal1"><rect id="revealRect" x="40" y="70" width="0" height="40"/></clipPath>
    <linearGradient id="glow" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0" stop-color="#3fb950" stop-opacity="0.15"/>
      <stop offset="1" stop-color="#58a6ff" stop-opacity="0"/>
    </linearGradient>
  </defs>

  <!-- window -->
  <rect x="0.5" y="0.5" width="1199" height="299" rx="14" fill="#0d1117" stroke="#30363d"/>
  <rect x="0.5" y="0.5" width="1199" height="40" rx="14" fill="#161b22"/>
  <rect x="0.5" y="26" width="1199" height="15" fill="#161b22"/>
  <circle cx="26" cy="21" r="6" fill="#ff5f56"/>
  <circle cx="46" cy="21" r="6" fill="#ffbd2e"/>
  <circle cx="66" cy="21" r="6" fill="#27c93f"/>
  <text x="600" y="26" text-anchor="middle" class="mono dim" font-size="13">mouheb@enit: ~ — bash</text>

  <!-- line 1: typed command -->
  <g class="line1 mono" font-size="22">
    <text x="40" y="97"><tspan class="prompt">mouheb@enit</tspan><tspan class="dim">:</tspan><tspan class="path">~</tspan><tspan class="dim">$ </tspan><tspan class="cmd">./boot --ai --systems --security</tspan></text>
  </g>

  <!-- output -->
  <rect class="line2" x="40" y="122" width="700" height="62" fill="url(#glow)"/>
  <text class="line2 mono name" x="56" y="168" font-size="44">Mouheb Khouildi</text>
  <text class="line3 mono" x="56" y="210" font-size="19"><tspan class="dim">[</tspan><tspan class="prompt"> OK </tspan><tspan class="dim">]</tspan><tspan class="cmd"> Computer Engineering student @ ENIT, Tunis</tspan></text>
  <text class="line4 mono" x="56" y="242" font-size="19"><tspan class="dim">[</tspan><tspan class="prompt"> OK </tspan><tspan class="dim">]</tspan><tspan class="cmd"> Building AI agents, RAG systems &amp; reliable backends</tspan></text>

  <!-- final prompt with blinking cursor -->
  <text class="line4 mono" x="40" y="280" font-size="18"><tspan class="prompt">mouheb@enit</tspan><tspan class="dim">:</tspan><tspan class="path">~</tspan><tspan class="dim">$ </tspan></text>
  <rect class="line4 cursor" x="208" y="265" width="11" height="20" fill="#e6edf3"/>

  <!-- side decoration: tiny status panel -->
  <g class="line3 mono" font-size="14">
    <rect x="860" y="78" width="300" height="190" rx="10" fill="#161b22" stroke="#30363d"/>
    <text x="880" y="106" class="dim">$ uptime</text>
    <text x="880" y="132" class="cmd">load: <tspan class="accent">coffee</tspan>, <tspan class="accent">code</tspan>, <tspan class="accent">ship</tspan></text>
    <text x="880" y="166" class="dim">$ cat location</text>
    <text x="880" y="192" class="cmd">Bizerte, Tunisia</text>
    <text x="880" y="226" class="dim">$ cat status</text>
    <text x="880" y="252" class="prompt">● open to PFE &amp; internships</text>
  </g>
</svg>