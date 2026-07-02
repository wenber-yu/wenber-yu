<div align="center">

<!-- POLISH POSTER STYLE BANNER -->
<svg viewBox="0 0 900 420" xmlns="http://www.w3.org/2000/svg" style="max-width:100%;">
  <defs>
    <!-- Noise texture -->
    <filter id="noise">
      <feTurbulence type="fractalNoise" baseFrequency="0.65" numOctaves="3" stitchTiles="stitch"/>
      <feColorMatrix type="saturate" values="0"/>
      <feBlend in="SourceGraphic" mode="multiply" result="noisy"/>
    </filter>
    <!-- Rough edge displacement -->
    <filter id="rough">
      <feTurbulence type="turbulence" baseFrequency="0.04" numOctaves="4" result="t"/>
      <feDisplacementMap in="SourceGraphic" in2="t" scale="6" xChannelSelector="R" yChannelSelector="G"/>
    </filter>
    <!-- Gradient: crimson to black -->
    <linearGradient id="crimson" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#8B1A1A"/>
      <stop offset="100%" stop-color="#1a0a0a"/>
    </linearGradient>
    <!-- Gradient: gold accent -->
    <linearGradient id="gold" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#D4A853"/>
      <stop offset="100%" stop-color="#8B6914"/>
    </linearGradient>
    <!-- Gradient: slate -->
    <linearGradient id="slate" x1="0" y1="1" x2="1" y2="0">
      <stop offset="0%" stop-color="#2C3E50"/>
      <stop offset="100%" stop-color="#1a252f"/>
    </linearGradient>
    <!-- Gradient: muted teal -->
    <linearGradient id="teal" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#2A6B6B"/>
      <stop offset="100%" stop-color="#1a4040"/>
    </linearGradient>
    <!-- Noise overlay -->
    <filter id="grain">
      <feTurbulence type="fractalNoise" baseFrequency="0.8" numOctaves="3" result="n"/>
      <feColorMatrix in="n" type="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 0.08 0" result="g"/>
      <feBlend in="SourceGraphic" in2="g" mode="multiply"/>
    </filter>
  </defs>

  <!-- Background: aged paper -->
  <rect width="900" height="420" fill="#F0E6D3"/>

  <!-- Background texture layers -->
  <rect width="900" height="420" fill="#E8DCC8" filter="url(#grain)"/>

  <!-- Large abstract semicircle (crimson) - Polish poster "face" motif -->
  <ellipse cx="200" cy="280" rx="260" ry="180" fill="url(#crimson)" filter="url(#rough)" opacity="0.92"/>

  <!-- Slate geometric slash across -->
  <polygon points="420,80 520,420 650,420 500,80" fill="url(#slate)" filter="url(#rough)" opacity="0.88"/>

  <!-- Gold diagonal accent line -->
  <line x1="340" y1="0" x2="580" y2="420" stroke="url(#gold)" stroke-width="3" opacity="0.6"/>

  <!-- Small circle (moon/motif) -->
  <circle cx="700" cy="100" r="28" fill="#D4A853" opacity="0.35"/>

  <!-- Abstract floating rectangle - teal -->
  <rect x="620" y="280" width="80" height="120" fill="url(#teal)" filter="url(#rough)" opacity="0.7" transform="rotate(-12, 660, 340)"/>

  <!-- Small crimson square -->
  <rect x="720" y="190" width="35" height="35" fill="#8B1A1A" opacity="0.5" transform="rotate(25, 737, 207)"/>

  <!-- Horizontal rule accent line -->
  <line x1="60" y1="375" x2="840" y2="375" stroke="#2C3E50" stroke-width="1.5" opacity="0.3"/>

  <!-- TYPOGRAPHY: W I L B U R (Polish poster style, uneven spacing) -->
  <text x="440" y="105" font-family="Georgia, 'Times New Roman', serif" font-size="72" font-weight="bold" fill="#2C3E50" letter-spacing="18" text-anchor="middle" opacity="0.9">W I L B U R</text>

  <!-- Subtitle: staggered, poster style -->
  <text x="445" y="148" font-family="'Courier New', monospace" font-size="13" fill="#6B5B4A" letter-spacing="8" text-anchor="middle" opacity="0.7">D E V E L O P E R</text>

  <!-- Small anchored type at bottom-left -->
  <text x="75" y="398" font-family="'Courier New', monospace" font-size="11" fill="#8B6B5A" letter-spacing="4" opacity="0.6">PHP · TYPESCRIPT · ENCRYPTION</text>

  <!-- Bottom-right: stylized hand-drawn cross/plus -->
  <g transform="translate(815, 388)" opacity="0.3">
    <line x1="-8" y1="0" x2="8" y2="0" stroke="#2C3E50" stroke-width="2"/>
    <line x1="0" y1="-8" x2="0" y2="8" stroke="#2C3E50" stroke-width="2"/>
  </g>

  <!-- Polish poster signature mark - abstract eye shape -->
  <ellipse cx="160" cy="240" rx="45" ry="22" fill="none" stroke="#D4A853" stroke-width="2.5" opacity="0.5" transform="rotate(-8, 160, 240)"/>
  <circle cx="160" cy="240" r="6" fill="#D4A853" opacity="0.6"/>

  <!-- Scattered dots - film grain aesthetic -->
  <circle cx="80" cy="130" r="2" fill="#2C3E50" opacity="0.25"/>
  <circle cx="380" cy="75" r="1.5" fill="#2C3E50" opacity="0.2"/>
  <circle cx="560" cy="300" r="2" fill="#2C3E50" opacity="0.15"/>
  <circle cx="730" cy="350" r="1.5" fill="#2C3E50" opacity="0.2"/>
  <circle cx="850" cy="180" r="2" fill="#2C3E50" opacity="0.15"/>
</svg>

<br><br>

<!-- CINE-STYLE QUOTE -->
<p>
  <i>"Code is not written. It is <strong>haunted</strong> into existence."</i>
</p>

</div>

---

### ◈  ABOUT

Building things in the dark hours. Backend architecture, cryptographic protocols, and the spaces between.

| night | language | mood |
|:---:|:---:|:---:|
| ![](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white) | ![](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white) | ![](https://img.shields.io/badge/Hyperf-00BFFF?style=for-the-badge) |
| ![](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white) | ![](https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white) | ![](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white) |
| ![](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white) | ![](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white) | ![](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) |

---

### ◈  FEATURED

<br>

<div align="center">

**req-res-crypto**

*An anonymous AEAD encryption protocol for HTTP*

<table>
<tr>
<td align="center" width="25%">
  <a href="https://github.com/wilbur-yu/req-res-crypto-core"><b>core</b></a><br>
  <sub>PHP · zero deps</sub>
</td>
<td align="center" width="25%">
  <a href="https://github.com/wilbur-yu/req-res-crypto-hyperf"><b>hyperf</b></a><br>
  <sub>PSR-15 middleware</sub>
</td>
<td align="center" width="25%">
  <a href="https://github.com/wilbur-yu/req-res-crypto-laravel"><b>laravel</b></a><br>
  <sub>middleware · facade</sub>
</td>
<td align="center" width="25%">
  <a href="https://github.com/wilbur-yu/req-res-crypto-js"><b>js</b></a><br>
  <sub>browser client</sub>
</td>
</tr>
</table>

> X25519 ECDH + XChaCha20-Poly1305 — ephemeral keys, forward secrecy, ~0.05ms per request

</div>

---

<div align="center">

| | |
|:---:|:---:|
| [wenber.club](https://wenber.club) | [packagist](https://packagist.org/packages/wenbo/) |

<img src="https://github-readme-stats.vercel.app/api?username=wilbur-yu&show_icons=true&hide_border=true&bg_color=F0E6D3&title_color=2C3E50&text_color=5C4A3A&icon_color=8B1A1A&include_all_commits=true&count_private=true" height="150" />

<br>

<sub>— fin —</sub>

</div>
