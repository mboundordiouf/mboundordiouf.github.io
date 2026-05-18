---
permalink: /codes/
title: "Apps & Visualisations"
author_profile: true
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,600;1,400&family=DM+Sans:opsz,wght@9..40,300;9..40,400;9..40,500&display=swap" rel="stylesheet">

<style>
.app-page {
  font-family: 'DM Sans', -apple-system, sans-serif !important;
  max-width: 920px;
  padding: 0.5rem 0 3rem;
  color: #1a1a18 !important;
}

.app-page p,
.app-page h1, .app-page h2, .app-page h3 {
  margin: 0 !important;
  padding: 0 !important;
}

.app-page a {
  text-decoration: none !important;
  border-bottom: none !important;
  box-shadow: none !important;
}

/* ── Section label ── */
.app-section-label {
  font-size: 10.5px !important;
  font-weight: 500 !important;
  letter-spacing: 2px !important;
  text-transform: uppercase !important;
  color: #888780 !important;
  margin: 0 0 1.4rem !important;
  display: flex !important;
  align-items: center !important;
  gap: 10px !important;
  line-height: 1 !important;
}
.app-section-label::after {
  content: '' !important;
  flex: 1 !important;
  height: 1px !important;
  background: #D3D1C7 !important;
}

/* ── App card ── */
.app-card {
  border: 1px solid #D3D1C7 !important;
  border-radius: 16px !important;
  overflow: hidden !important;
  margin-bottom: 1.4rem !important;
  background: #fff !important;
  transition: border-color 0.2s ease, box-shadow 0.2s ease !important;
  width: 100% !important;
}
.app-card:hover {
  border-color: #aaa !important;
  box-shadow: 0 4px 20px rgba(0,0,0,0.07) !important;
}

/* ── Card header banner ── */
.app-header {
  display: flex !important;
  align-items: center !important;
  gap: 16px !important;
  padding: 1.3rem 1.5rem !important;
  border-bottom: 1px solid #EDECE8 !important;
}

.app-icon {
  width: 48px !important;
  height: 48px !important;
  min-width: 48px !important;
  border-radius: 12px !important;
  display: flex !important;
  align-items: center !important;
  justify-content: center !important;
  flex-shrink: 0 !important;
}
.app-icon svg {
  width: 24px !important;
  height: 24px !important;
  stroke-width: 1.6 !important;
  stroke-linecap: round !important;
  stroke-linejoin: round !important;
  fill: none !important;
}

.app-icon-minerals {
  background: #E6F1FB !important;
}
.app-icon-minerals svg { stroke: #185FA5 !important; }

.app-icon-forest {
  background: #EAF3DE !important;
}
.app-icon-forest svg { stroke: #3B6D11 !important; }

.app-header-text { flex: 1 !important; }

.app-title {
  font-family: 'Lora', Georgia, serif !important;
  font-size: 16px !important;
  font-weight: 600 !important;
  color: #1a1a18 !important;
  line-height: 1.4 !important;
  margin: 0 !important;
}

.app-subtitle {
  font-size: 12px !important;
  color: #888780 !important;
  margin: 3px 0 0 !important;
  line-height: 1.4 !important;
}

/* ── Card body ── */
.app-body {
  display: grid !important;
  grid-template-columns: minmax(0,1fr) 220px !important;
  gap: 0 !important;
}

.app-desc-col {
  padding: 1.3rem 1.5rem !important;
  display: flex !important;
  flex-direction: column !important;
  gap: 14px !important;
  border-right: 1px solid #EDECE8 !important;
}

.app-desc-text {
  font-size: 13px !important;
  color: #5F5E5A !important;
  line-height: 1.68 !important;
  margin: 0 !important;
}

/* ── Feature tags ── */
.app-features {
  display: flex !important;
  flex-wrap: wrap !important;
  gap: 6px !important;
}
.app-tag {
  font-size: 10.5px !important;
  font-weight: 400 !important;
  color: #5F5E5A !important;
  background: #F7F6F2 !important;
  border: 1px solid #E0DED8 !important;
  border-radius: 5px !important;
  padding: 3px 8px !important;
  display: inline-flex !important;
  align-items: center !important;
  gap: 4px !important;
  line-height: 1.5 !important;
}
.app-tag svg {
  width: 10px !important;
  height: 10px !important;
  stroke: #888780 !important;
  fill: none !important;
  stroke-width: 2 !important;
  stroke-linecap: round !important;
  stroke-linejoin: round !important;
  flex-shrink: 0 !important;
}

/* ── Right panel — launch ── */
.app-launch-col {
  padding: 1.3rem 1.4rem !important;
  display: flex !important;
  flex-direction: column !important;
  align-items: center !important;
  justify-content: center !important;
  gap: 14px !important;
  background: #FAFAF8 !important;
  text-align: center !important;
}

.app-launch-icon {
  width: 56px !important;
  height: 56px !important;
  border-radius: 50% !important;
  background: #fff !important;
  border: 1px solid #E0DED8 !important;
  display: flex !important;
  align-items: center !important;
  justify-content: center !important;
}
.app-launch-icon svg {
  width: 22px !important;
  height: 22px !important;
  fill: none !important;
  stroke-width: 1.7 !important;
  stroke-linecap: round !important;
  stroke-linejoin: round !important;
}

.app-launch-note {
  font-size: 11px !important;
  color: #aaa !important;
  line-height: 1.5 !important;
  margin: 0 !important;
}

.app-launch-btn {
  display: inline-flex !important;
  align-items: center !important;
  gap: 6px !important;
  padding: 9px 18px !important;
  border-radius: 8px !important;
  font-family: 'DM Sans', sans-serif !important;
  font-size: 12.5px !important;
  font-weight: 500 !important;
  text-decoration: none !important;
  border: none !important;
  cursor: pointer !important;
  transition: opacity 0.15s, transform 0.15s !important;
  line-height: 1 !important;
}
.app-launch-btn:hover {
  opacity: 0.85 !important;
  transform: translateY(-1px) !important;
  text-decoration: none !important;
}
.app-launch-btn svg {
  width: 13px !important;
  height: 13px !important;
  stroke: currentColor !important;
  fill: none !important;
  stroke-width: 2.2 !important;
  stroke-linecap: round !important;
  stroke-linejoin: round !important;
}

.btn-minerals {
  background: #185FA5 !important;
  color: #fff !important;
}
.btn-forest {
  background: #3B6D11 !important;
  color: #fff !important;
}

/* ── Responsive ── */
@media (max-width: 680px) {
  .app-body {
    grid-template-columns: 1fr !important;
  }
  .app-desc-col {
    border-right: none !important;
    border-bottom: 1px solid #EDECE8 !important;
  }
  .app-launch-col {
    padding: 1.2rem !important;
  }
}
</style>

<div class="app-page">

<p class="app-section-label">Interactive applications</p>

<!-- ── App 1 : Critical Minerals ── -->
<div class="app-card">
  <div class="app-header">
    <div class="app-icon app-icon-minerals">
      <svg viewBox="0 0 24 24"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87L18.18 21 12 17.77 5.82 21 7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
    </div>
    <div class="app-header-text">
      <p class="app-title">Critical Minerals &amp; Energy Transition</p>
      <p class="app-subtitle">Global supply chains · Mineral dependency · Transition pathways</p>
    </div>
  </div>
  <div class="app-body">
    <div class="app-desc-col">
      <p class="app-desc-text">
        An interactive Shiny dashboard exploring the role of critical minerals in the global energy transition.
        Navigate mineral supply chains, production geographies, and demand projections across countries and sectors.
        Visualise which economies are most exposed to mineral dependency and how transition scenarios reshape resource flows.
      </p>
      <div class="app-features">
        <span class="app-tag"><svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><line x1="2" y1="12" x2="22" y2="12"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>Global coverage</span>
        <span class="app-tag"><svg viewBox="0 0 24 24"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>32 minerals tracked</span>
        <span class="app-tag"><svg viewBox="0 0 24 24"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18M9 21V9"/></svg>Interactive maps</span>
        <span class="app-tag"><svg viewBox="0 0 24 24"><path d="M18 20V10M12 20V4M6 20v-6"/></svg>Scenario explorer</span>
      </div>
    </div>
    <div class="app-launch-col">
      <div class="app-launch-icon">
        <svg viewBox="0 0 24 24" style="stroke:#185FA5"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>
      </div>
      <p class="app-launch-note">Hosted on shinyapps.io<br>Allow ~10 sec to load</p>
      <a href="https://diouf.shinyapps.io/Mboundor-Critical-Minerals-World-App/" target="_blank" rel="noopener" class="app-launch-btn btn-minerals">
        <svg viewBox="0 0 24 24"><polygon points="5 3 19 12 5 21 5 3"/></svg>
        Launch app
      </a>
    </div>
  </div>
</div>

<!-- ── App 2 : Mining & Deforestation ── -->
<div class="app-card">
  <div class="app-header">
    <div class="app-icon app-icon-forest">
      <svg viewBox="0 0 24 24"><path d="M17 8C8 10 5.9 16.17 3.82 22"/><path d="M10.17 10.95C8.07 11.91 6.5 14.06 5.44 16.51"/><path d="M22 4c-3.5 0-6 1.5-7.5 4.5"/><path d="M13.1 15.5C12.37 17.07 11.86 18.96 12 22"/></svg>
    </div>
    <div class="app-header-text">
      <p class="app-title">Mining &amp; Deforestation in Sub-Saharan Africa</p>
      <p class="app-subtitle">Forest cover · Mine proximity · Environmental footprint</p>
    </div>
  </div>
  <div class="app-body">
    <div class="app-desc-col">
      <p class="app-desc-text">
        A companion dashboard to the paper <em>Under the Canopy</em>. Explore the spatial relationship between
        mining activity and forest loss across Sub-Saharan Africa from 2001 to 2018.
        Visualise deforestation rates at cell and buffer-zone levels, compare mineral types and mine sizes,
        and examine indirect effects extending up to 80 km from mining sites.
      </p>
      <div class="app-features">
        <span class="app-tag"><svg viewBox="0 0 24 24"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/></svg>45 SSA countries</span>
        <span class="app-tag"><svg viewBox="0 0 24 24"><circle cx="12" cy="10" r="3"/><path d="M12 21.7C17.3 17 20 13 20 10a8 8 0 1 0-16 0c0 3 2.7 6.9 8 11.7z"/></svg>Georeferenced data</span>
        <span class="app-tag"><svg viewBox="0 0 24 24"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18M9 21V9"/></svg>14 minerals</span>
        <span class="app-tag"><svg viewBox="0 0 24 24"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>Buffer analysis</span>
      </div>
    </div>
    <div class="app-launch-col">
      <div class="app-launch-icon">
        <svg viewBox="0 0 24 24" style="stroke:#3B6D11"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>
      </div>
      <p class="app-launch-note">Hosted on shinyapps.io<br>Allow ~10 sec to load</p>
      <a href="https://diouf.shinyapps.io/MiningDeforest_ShinyApp/" target="_blank" rel="noopener" class="app-launch-btn btn-forest">
        <svg viewBox="0 0 24 24"><polygon points="5 3 19 12 5 21 5 3"/></svg>
        Launch app
      </a>
    </div>
  </div>
</div>

</div>
