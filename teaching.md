---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,600;1,400&family=DM+Sans:opsz,wght@9..40,300;9..40,400;9..40,500&display=swap" rel="stylesheet">

<style>
.teach-page {
  font-family: 'DM Sans', -apple-system, sans-serif !important;
  max-width: 920px;
  padding: 0.5rem 0 3rem;
  color: #1a1a18 !important;
}

.teach-page p,
.teach-page h1, .teach-page h2, .teach-page h3,
.teach-page ul, .teach-page li {
  margin: 0 !important;
  padding: 0 !important;
}

/* ── Section label ── */
.teach-section-label {
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
.teach-section-label::after {
  content: '' !important;
  flex: 1 !important;
  height: 1px !important;
  background: #D3D1C7 !important;
}

/* ── University card ── */
.uni-card {
  border: 1px solid #D3D1C7 !important;
  border-radius: 16px !important;
  overflow: hidden !important;
  margin-bottom: 1.2rem !important;
  background: #fff !important;
  transition: border-color 0.2s ease, box-shadow 0.2s ease !important;
  width: 100% !important;
}
.uni-card:hover {
  border-color: #aaa !important;
  box-shadow: 0 4px 20px rgba(0,0,0,0.06) !important;
}

/* ── Card header ── */
.uni-header {
  display: flex !important;
  align-items: center !important;
  gap: 14px !important;
  padding: 1.15rem 1.5rem !important;
  border-bottom: 1px solid #EDECE8 !important;
}

.uni-logo {
  width: 42px !important;
  height: 42px !important;
  min-width: 42px !important;
  border-radius: 10px !important;
  display: flex !important;
  align-items: center !important;
  justify-content: center !important;
  flex-shrink: 0 !important;
}
.uni-logo svg {
  width: 20px !important;
  height: 20px !important;
  fill: none !important;
  stroke-width: 1.7 !important;
  stroke-linecap: round !important;
  stroke-linejoin: round !important;
}

.uni-logo-paris   { background: #EDE9FE !important; }
.uni-logo-paris svg { stroke: #4C35B4 !important; }

.uni-logo-poitiers { background: #FAEEDA !important; }
.uni-logo-poitiers svg { stroke: #7A4A0A !important; }

.uni-logo-clermont { background: #E1F5EE !important; }
.uni-logo-clermont svg { stroke: #0F6E56 !important; }

.uni-header-text { flex: 1 !important; }

.uni-name {
  font-family: 'Lora', Georgia, serif !important;
  font-size: 15.5px !important;
  font-weight: 600 !important;
  color: #1a1a18 !important;
  line-height: 1.35 !important;
  margin: 0 !important;
}
.uni-location {
  font-size: 11.5px !important;
  color: #888780 !important;
  margin: 2px 0 0 !important;
  display: flex !important;
  align-items: center !important;
  gap: 4px !important;
}
.uni-location svg {
  width: 11px !important;
  height: 11px !important;
  stroke: #aaa !important;
  fill: none !important;
  stroke-width: 2 !important;
  stroke-linecap: round !important;
  stroke-linejoin: round !important;
  flex-shrink: 0 !important;
}

/* ── Card body: timeline rows ── */
.uni-body {
  padding: 0.2rem 0 !important;
}

.teach-row {
  display: grid !important;
  grid-template-columns: 190px minmax(0,1fr) !important;
  gap: 0 !important;
  border-bottom: 1px solid #F2F1ED !important;
}
.teach-row:last-child {
  border-bottom: none !important;
}

/* Left: period + role */
.teach-period-col {
  padding: 1rem 1.2rem 1rem 1.5rem !important;
  border-right: 1px solid #F2F1ED !important;
  display: flex !important;
  flex-direction: column !important;
  justify-content: center !important;
  gap: 5px !important;
  background: #FAFAF8 !important;
}

.teach-period {
  font-size: 12px !important;
  font-weight: 500 !important;
  color: #1a1a18 !important;
  margin: 0 !important;
  line-height: 1.4 !important;
}

.teach-role {
  font-size: 11px !important;
  color: #888780 !important;
  margin: 0 !important;
  line-height: 1.4 !important;
}

/* Right: course list */
.teach-courses-col {
  padding: 1rem 1.5rem !important;
  display: flex !important;
  flex-wrap: wrap !important;
  gap: 7px !important;
  align-items: center !important;
  align-content: center !important;
}

.course-tag {
  font-size: 11.5px !important;
  font-weight: 400 !important;
  color: #3a3a38 !important;
  background: #F4F3EF !important;
  border: 1px solid #E0DED8 !important;
  border-radius: 6px !important;
  padding: 4px 10px !important;
  display: inline-flex !important;
  align-items: center !important;
  gap: 5px !important;
  line-height: 1.4 !important;
  white-space: nowrap !important;
}
.course-tag svg {
  width: 11px !important;
  height: 11px !important;
  stroke: #aaa !important;
  fill: none !important;
  stroke-width: 2 !important;
  stroke-linecap: round !important;
  stroke-linejoin: round !important;
  flex-shrink: 0 !important;
}

/* Level badge next to role */
.level-badge {
  font-size: 10px !important;
  font-weight: 500 !important;
  padding: 2px 7px !important;
  border-radius: 4px !important;
  line-height: 1.5 !important;
  display: inline-block !important;
}
.level-ug   { background: #E6F1FB !important; color: #0C447C !important; }
.level-ma   { background: #EAF3DE !important; color: #27500A !important; }
.level-both { background: #FAEEDA !important; color: #633806 !important; }

/* ── Responsive ── */
@media (max-width: 680px) {
  .teach-row {
    grid-template-columns: 1fr !important;
  }
  .teach-period-col {
    border-right: none !important;
    border-bottom: 1px solid #F2F1ED !important;
    flex-direction: row !important;
    align-items: center !important;
    justify-content: space-between !important;
    flex-wrap: wrap !important;
    gap: 6px !important;
  }
  .teach-courses-col {
    padding-top: 0.8rem !important;
    padding-bottom: 1rem !important;
  }
  .course-tag { white-space: normal !important; }
}
</style>

<div class="teach-page">

<p class="teach-section-label">Teaching experience</p>

<!-- ══════════ Paris I Panthéon-Sorbonne ══════════ -->
<div class="uni-card">
  <div class="uni-header">
    <div class="uni-logo uni-logo-paris">
      <svg viewBox="0 0 24 24"><path d="M22 10v6M2 10l10-5 10 5"/><path d="M6 12v5c3 3 9 3 12 0v-5"/></svg>
    </div>
    <div class="uni-header-text">
      <p class="uni-name">University of Paris I, Panthéon-Sorbonne</p>
      <p class="uni-location">
        <svg viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>
        Paris, France
      </p>
    </div>
  </div>
  <div class="uni-body">
    <div class="teach-row">
      <div class="teach-period-col">
        <p class="teach-period">2025 – 2026</p>
        <p class="teach-role">Teaching Assistant – ATER &nbsp;<span class="level-badge level-ug">Undergraduate</span></p>
      </div>
      <div class="teach-courses-col">
        <span class="course-tag"><svg viewBox="0 0 24 24"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>Macroeconomics</span>
        <span class="course-tag"><svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><path d="M12 8v4l3 3"/></svg>Monetary Instruments</span>
      </div>
    </div>
    <div class="teach-row">
      <div class="teach-period-col">
        <p class="teach-period">2022 – present</p>
        <p class="teach-role">Teaching Assistant &nbsp;<span class="level-badge level-ug">Undergraduate</span></p>
      </div>
      <div class="teach-courses-col">
        <span class="course-tag"><svg viewBox="0 0 24 24"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/></svg>History of Economics</span>
      </div>
    </div>
  </div>
</div>

<!-- ══════════ University of Poitiers ══════════ -->
<div class="uni-card">
  <div class="uni-header">
    <div class="uni-logo uni-logo-poitiers">
      <svg viewBox="0 0 24 24"><path d="M22 10v6M2 10l10-5 10 5"/><path d="M6 12v5c3 3 9 3 12 0v-5"/></svg>
    </div>
    <div class="uni-header-text">
      <p class="uni-name">University of Poitiers</p>
      <p class="uni-location">
        <svg viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>
        Poitiers, France
      </p>
    </div>
  </div>
  <div class="uni-body">
    <div class="teach-row">
      <div class="teach-period-col">
        <p class="teach-period">2024 – 2025</p>
        <p class="teach-role">Teaching Assistant – ATER &nbsp;<span class="level-badge level-both">UG &amp; Masters</span></p>
      </div>
      <div class="teach-courses-col">
        <span class="course-tag"><svg viewBox="0 0 24 24"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>Macroeconomics</span>
        <span class="course-tag"><svg viewBox="0 0 24 24"><path d="M18 20V10M12 20V4M6 20v-6"/></svg>Microeconomics</span>
        <span class="course-tag"><svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/></svg>Economic Analysis</span>
      </div>
    </div>
  </div>
</div>

<!-- ══════════ Clermont Auvergne ══════════ -->
<div class="uni-card">
  <div class="uni-header">
    <div class="uni-logo uni-logo-clermont">
      <svg viewBox="0 0 24 24"><path d="M22 10v6M2 10l10-5 10 5"/><path d="M6 12v5c3 3 9 3 12 0v-5"/></svg>
    </div>
    <div class="uni-header-text">
      <p class="uni-name">Clermont Auvergne University</p>
      <p class="uni-location">
        <svg viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>
        Clermont-Ferrand, France
      </p>
    </div>
  </div>
  <div class="uni-body">
    <div class="teach-row">
      <div class="teach-period-col">
        <p class="teach-period">2020 – 2022</p>
        <p class="teach-role">Teaching Assistant &nbsp;<span class="level-badge level-ug">Undergraduate</span></p>
      </div>
      <div class="teach-courses-col">
        <span class="course-tag"><svg viewBox="0 0 24 24"><path d="M4 7h16M4 12h10M4 17h13"/></svg>Mathematics &amp; Statistics</span>
      </div>
    </div>
  </div>
</div>

</div>
