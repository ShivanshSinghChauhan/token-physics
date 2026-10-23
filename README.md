# TokenPhysics: Interactive Tokenomics & Vesting Physics Deck

> **Real-time 2D rigid-body simulation of token emissions, constant-product AMM slippage, and liquidity drain for Web3 founders, launchpads, and crypto VCs.**

[![Live Demo](https://img.shields.io/badge/Demo-Live%20on%20GitHub%20Pages-2563eb?style=for-the-badge&logo=github)](https://shivanshsinghchauhan.github.io/token-physics/)
[![License: MIT](https://img.shields.io/badge/License-MIT-emerald?style=for-the-badge)](LICENSE)
[![Zero Build](https://img.shields.io/badge/Build-Zero%20Config%20(Pure%20HTML5)-amber?style=for-the-badge)](index.html)

---

## 🌐 Overview

Instead of static, opaque spreadsheets, **TokenPhysics** visualizes token cohorts (*Seed, Team, Staking, Public Float*) as physical rigid bodies inside a calibrated reservoir chamber. 

Adjusting vesting cliffs, emission curves, and market liquidity parameters dynamically releases tokens through an aperture valve into a simulated AMM sink—visually and mathematically demonstrating liquidity drain, sell pressure stress, and price impact.

---

## ⚡ Key Capabilities

### 1. 2D Physics Reservoir Simulation (Matter.js)
- **Cohort-Coded Physical Bodies**: Real-time simulation of tokens with proportional radius, mass, and restitution.
- **Dynamic Aperture Drain Valve**: Calibrated valve gates physically rotate and open proportional to monthly unlock intensity.
- **Interactive Chamber Controls**: Drag and throw orbs with mouse physics, trigger an **"Agitate Chamber"** impulse, or initiate an **"Emergency Valve Flush"**.
- **AMM Sink Absorption**: Falling tokens trigger immediate market absorption effects, updating instantaneous slippage in real time.

### 2. Quantitative Financial Engine & Defensible AMM Modeling
- **Constant-Product Market Impact**:
  $$\Delta P / P = \frac{\Delta x}{x + \Delta x}$$
  Calculates single-month price impact against automated market maker liquidity depth.
- **Investor Paper Multiple**: Automatically tracks Seed round entry valuation vs. listing price to compute live paper ROI multiples (e.g., $10.0\times$).
- **Institutional Health Score (0–100)**: Composite rating factoring in initial float percentage, peak depth multiples, and price impact risk.
- **Required Daily Organic Volume**: Computes the daily trading volume required to absorb unlock sell pressure without exceeding a 2% price decline.

### 3. Real-World Presets for Institutional Pitching
- **Arbitrum-style Ecosystem Drip**: Long cliffs, extended 4-year linear drip, low initial sell pressure.
- **Balanced VC L1**: 12-month seed/team cliffs, 3-year team vesting, 40% rewards, healthy float.
- **Predatory Low Float / High FDV**: Classic 2024 VC trap (5% float, massive month-6 cliff, red alert flag).
- **Fair Launch (35% Float)**: High initial float, minimal cliffs, organic price discovery.

### 4. Executive VC Due Diligence & PDF Export
- **Print / PDF Optimized Memo**: Generates an institutional-grade memorandum with KPI tiles, allocation matrices, AMM stress tests, milestone roadmap, and formal sign-off blocks.
- **48-Month Granular Ledger**: Full numerical schedule with one-click **"Download CSV for Excel"** export.
- **State-Preserving Shareable Links**: Encodes complete token models into base64 URL hashes for sharing with investors and launchpad partners.

---

## 🛠 Tech Stack

- **Styling**: Tailwind CSS (CDN) — Crisp FinTech light aesthetic.
- **Physics Engine**: Matter.js 0.19.0.
- **Charts**: Chart.js 4.4.1 (Stacked circulating area + monthly sell volume vs. daily absorption).
- **Audio Synthesizer**: Web Audio API (procedural coin and drainage feedback without audio file dependencies).
- **Typography**: Inter & JetBrains Mono.
- **Confetti**: Canvas-Confetti 1.6.0.

---

## 🚀 Running Locally

No `npm install`, build steps, or local dev servers required:

```bash
# Clone the repository
git clone https://github.com/ShivanshSinghChauhan/token-physics.git
cd token-physics

# Open in your browser
open index.html
```

---

## 📄 License

MIT License. Designed and maintained for Web3 founders, launchpads, and crypto researchers.
