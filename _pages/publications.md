---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,600;1,400&family=DM+Sans:opsz,wght@9..40,300;9..40,400;9..40,500&display=swap" rel="stylesheet">

<style>
/* ── Scope everything under .pub-page to avoid theme conflicts ── */

.pub-page {
  font-family: 'DM Sans', -apple-system, sans-serif !important;
  max-width: 920px;
  padding: 0.5rem 0 3rem;
  color: #1a1a18 !important;
}

/* Reset inside scope — fight Minimal Mistakes defaults */
.pub-page p,
.pub-page h1, .pub-page h2, .pub-page h3,
.pub-page ul, .pub-page li {
  margin: 0 !important;
  padding: 0 !important;
}

.pub-page a {
  color: #185FA5 !important;
  text-decoration: none !important;
  border-bottom: none !important;
  box-shadow: none !important;
}
.pub-page a:hover {
  text-decoration: underline !important;
  color: #0c3d7a !important;
}

/* ── Section label ── */
.pub-section-label {
  font-size: 10.5px !important;
  font-weight: 500 !important;
  letter-spacing: 2px !important;
  text-transform: uppercase !important;
  color: #888780 !important;
  margin: 2.5rem 0 1.1rem !important;
  display: flex !important;
  align-items: center !important;
  gap: 10px !important;
  line-height: 1 !important;
}
.pub-section-label::after {
  content: '' !important;
  flex: 1 !important;
  height: 1px !important;
  background: #D3D1C7 !important;
}

/* ── Publication card ── */
.pub-card {
  display: grid !important;
  grid-template-columns: 210px minmax(0, 1fr) !important;
  border: 1px solid #D3D1C7 !important;
  border-radius: 14px !important;
  overflow: hidden !important;
  margin-bottom: 1.2rem !important;
  background: #fff !important;
  transition: border-color 0.2s ease, box-shadow 0.2s ease !important;
  width: 100% !important;
}
.pub-card:hover {
  border-color: #999 !important;
  box-shadow: 0 2px 14px rgba(0,0,0,0.07) !important;
}

/* ── Left column — image ── */
.pub-img-col {
  background: #F7F6F2 !important;
  border-right: 1px solid #D3D1C7 !important;
  padding: 1.2rem 1rem !important;
  display: flex !important;
  flex-direction: column !important;
  align-items: center !important;
  justify-content: center !important;
  gap: 10px !important;
  min-height: 210px !important;
}

/* CRITICAL — override theme's img { height: auto } */
.pub-page .pub-img-col img {
  width: 100% !important;
  height: 148px !important;
  max-height: 148px !important;
  min-height: 148px !important;
  object-fit: cover !important;
  border-radius: 8px !important;
  border: 1px solid #D3D1C7 !important;
  display: block !important;
  margin: 0 !important;
  padding: 0 !important;
  box-shadow: none !important;
}

.pub-page .pub-img-col.two-images img {
  height: 100px !important;
  max-height: 100px !important;
  min-height: 100px !important;
}

.pub-img-caption {
  font-size: 10px !important;
  color: #888780 !important;
  text-align: center !important;
  line-height: 1.45 !important;
  font-style: italic !important;
  margin: 0 !important;
}

/* ── Right column — content ── */
.pub-content-col {
  padding: 1.3rem 1.5rem !important;
  display: flex !important;
  flex-direction: column !important;
  gap: 9px !important;
}

/* ── Badges (prefixed pub-badge to avoid MM conflict) ── */
.pub-badges {
  display: flex !important;
  flex-wrap: wrap !important;
  gap: 5px !important;
}
.pub-badge {
  font-size: 10px !important;
  font-weight: 500 !important;
  letter-spacing: 0.4px !important;
  padding: 3px 9px !important;
  border-radius: 6px !important;
  line-height: 1.6 !important;
  display: inline-block !important;
}
.pub-badge-blue  { background: #E6F1FB !important; color: #0C447C !important; }
.pub-badge-green { background: #EAF3DE !important; color: #27500A !important; }
.pub-badge-amber { background: #FAEEDA !important; color: #633806 !important; }
.pub-badge-teal  { background: #E1F5EE !important; color: #085041 !important; }

/* ── Title ── */
.pub-title {
  font-family: 'Lora', Georgia, serif !important;
  font-size: 15.5px !important;
  font-weight: 600 !important;
  color: #1a1a18 !important;
  line-height: 1.48 !important;
  letter-spacing: -0.15px !important;
  margin: 0 !important;
}

/* ── Co-authors ── */
.pub-coauthors {
  font-size: 12px !important;
  color: #5F5E5A !important;
  line-height: 1.5 !important;
  margin: 0 !important;
}

/* ── Abstract ── */
.pub-abstract {
  font-size: 12.5px !important;
  color: #5F5E5A !important;
  line-height: 1.68 !important;
  flex: 1 !important;
  margin: 0 !important;
}
.pub-abstract.collapsed {
  display: -webkit-box !important;
  -webkit-line-clamp: 4 !important;
  -webkit-box-orient: vertical !important;
  overflow: hidden !important;
}

/* ── Toggle button ── */
.pub-toggle {
  background: none !important;
  border: none !important;
  cursor: pointer !important;
  font-family: 'DM Sans', sans-serif !important;
  font-size: 11.5px !important;
  font-weight: 500 !important;
  color: #185FA5 !important;
  padding: 0 !important;
  display: inline-flex !important;
  align-items: center !important;
  gap: 4px !important;
  transition: opacity 0.15s !important;
  align-self: flex-start !important;
  box-shadow: none !important;
  text-shadow: none !important;
  margin: 4px 0 0 !important;
}
.pub-toggle:hover { opacity: 0.7 !important; }
.pub-toggle svg {
  width: 13px !important;
  height: 13px !important;
  stroke: currentColor !important;
  fill: none !important;
  stroke-width: 2.2 !important;
  stroke-linecap: round !important;
  stroke-linejoin: round !important;
  transition: transform 0.2s !important;
  display: inline-block !important;
  vertical-align: middle !important;
}

/* ── Divider ── */
.pub-divider {
  height: 1px !important;
  background: #D3D1C7 !important;
  margin: 2.5rem 0 0 !important;
  border: none !important;
}

/* ── Work-in-progress cards ── */
.pub-wip-card {
  display: flex !important;
  align-items: center !important;
  gap: 14px !important;
  padding: 0.95rem 1.25rem !important;
  background: #fff !important;
  border: 1px solid #D3D1C7 !important;
  border-radius: 12px !important;
  margin-bottom: 0.75rem !important;
  transition: border-color 0.2s ease !important;
}
.pub-wip-card:hover { border-color: #B4B2A9 !important; }

.pub-wip-icon {
  width: 38px !important;
  height: 38px !important;
  min-width: 38px !important;
  border-radius: 50% !important;
  background: #F7F6F2 !important;
  border: 1px solid #D3D1C7 !important;
  display: flex !important;
  align-items: center !important;
  justify-content: center !important;
  flex-shrink: 0 !important;
}
.pub-wip-icon svg {
  width: 17px !important;
  height: 17px !important;
  stroke: #888780 !important;
  fill: none !important;
  stroke-width: 1.8 !important;
  stroke-linecap: round !important;
  stroke-linejoin: round !important;
}

.pub-wip-body { flex: 1 !important; }

.pub-wip-title {
  font-family: 'Lora', Georgia, serif !important;
  font-size: 13.5px !important;
  font-weight: 600 !important;
  color: #1a1a18 !important;
  line-height: 1.42 !important;
  margin: 0 !important;
}
.pub-wip-coauth {
  font-size: 11.5px !important;
  color: #888780 !important;
  margin: 3px 0 0 !important;
}

/* ── Responsive ── */
@media (max-width: 680px) {
  .pub-card {
    grid-template-columns: 1fr !important;
  }
  .pub-img-col {
    border-right: none !important;
    border-bottom: 1px solid #D3D1C7 !important;
    min-height: unset !important;
  }
  .pub-page .pub-img-col img {
    height: 180px !important;
    max-height: 180px !important;
    min-height: 180px !important;
  }
  .pub-wip-card {
    flex-wrap: wrap !important;
  }
}
</style>

<div class="pub-page">

<!-- ══════════════ ONGOING WORKS ══════════════ -->
<p class="pub-section-label">On-going works</p>

<!-- Paper 1 -->
<div class="pub-card"><div class="pub-img-col"><img src="/images/att_decay_by_distance.png" alt="Map: Malaria and Electricity Access at DHS cluster levels in SSA 1997-2021"><p class="pub-img-caption">Malaria &amp; Electricity Access<br>DHS clusters · SSA 1997–2021</p></div><div class="pub-content-col"><div class="pub-badges"><span class="pub-badge pub-badge-blue">On-going</span><span class="pub-badge pub-badge-teal">Solo-authored</span></div><p class="pub-title">Light and Disease: Mining-Electrification and Malaria in Africa</p><p class="pub-abstract collapsed" id="abs-1">I study the health externalities of industrial mining using 1.6 million grid-cell–year observations for 45 sub-Saharan African countries from 2000 to 2022. Exploiting staggered mine discoveries in a ring-based difference-in-differences design, I find that mining increases annual malaria incidence by 35 cases per 1,000 (+10.5% relative to baseline), prevalence by 6.2 percentage points (+21.4%), and mortality by 9.6 deaths per 100,000 (+9.3%) in a 5 km grid cell exposed to mining, with effects 3 to 4 times larger at 10–50 km than within 10 km of the mine. Cumulating over a 15-year horizon, these translate into a +158.2% increase in incidence, +140.1% in prevalence, and +320.6% in mortality relative to pre-treatment levels — the mortality burden accelerating as immunity erodes and health systems are strained. Deforestation is the dominant mechanism and fully explains the malaria premium of artisanal gold mining, whose effects are 4–8 times larger than those of formal operations. Mine-induced electrification attenuates but does not offset these impacts, and the net health costs fall disproportionately on poor households.</p><button class="pub-toggle" onclick="pubToggle('abs-1',this)" aria-expanded="false"><svg viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg> Read abstract</button></div></div>

<!-- Paper 2 -->
<div class="pub-card"><div class="pub-img-col two-images"><img src="/images/mining_electricty_ASS.png" alt="Discovery Mining and Population Access of Energy"><img src="/images/DISTANCE_generator_energy_access_ssa.png" alt="Energy Access from generator locations in SSA"><p class="pub-img-caption">Discovery Mining &amp; Energy Access · SSA</p></div><div class="pub-content-col"><div class="pub-badges"><span class="pub-badge pub-badge-green">Working Paper</span></div><p class="pub-title">Mining and Power: Darkness or Lighting for Africa?</p><p class="pub-coauthors">with <a href="https://search.asu.edu/profile/2183493" target="_blank" rel="noopener">Nathan Johnson</a> and <a href="https://scholar.google.com/citations?user=hrZlpwUAAAAJ&hl=en" target="_blank" rel="noopener">Tam Kemabonta</a> &nbsp;·&nbsp; <em>Available upon request</em></p><p class="pub-abstract collapsed" id="abs-2">This study investigates the effect of mining activities involving 32 minerals on energy access (created using population and night lights at 1×1 km resolution) in sub-Saharan Africa from 2000 to 2022. Using georeferenced data in cells of 0.5°×0.5°, we compare energy access in areas with active mines to those with inactive mines, defined as sites that were discovered but were never active, serving as our control group. Our results indicate no evidence of active mines on energy access when using inactive mines for comparison. However, when all areas without mines are considered as the control group, the impact of mining activities appears significant and positive. Regions mining energy-intensive minerals like uranium and cobalt have the lowest energy access, while those mining gold have higher access rates. Mining areas exhibit enclave characteristics, with positive spillover effects on nearby regions.</p><button class="pub-toggle" onclick="pubToggle('abs-2',this)" aria-expanded="false"><svg viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg> Read abstract</button></div></div>

<!-- Paper 3 -->
<div class="pub-card"><div class="pub-img-col"><img src="/images/africa_conflict_events_1997_2022ok.png" alt="Number of conflict events in Africa 1997-2022"><p class="pub-img-caption">Conflict events in Africa · 1997–2022</p></div><div class="pub-content-col"><div class="pub-badges"><span class="pub-badge pub-badge-green">Working Paper</span></div><p class="pub-title">The New Mining Rush: Mineral Discoveries and Social Conflicts in Africa</p><p class="pub-coauthors">with <a href="https://sites.google.com/site/soubeyranhomepage/" target="_blank" rel="noopener">Raphael Soubeyran</a> and <a href="https://sites.google.com/site/ahmtritah/" target="_blank" rel="noopener">Ahmed Tritah</a> &nbsp;·&nbsp; <em>Available upon request</em></p><p class="pub-abstract collapsed" id="abs-3">The global energy transition is crucial but presents social and political challenges, particularly in mineral-rich African countries. This study uses high-resolution data to explore the relationship between mining discoveries and conflict from 1997 to 2022. Using high-resolution remote sensing data combined with a dynamic panel and event-study approach, our findings indicate that conflict increases during exploration, primarily due to protests and riots over gold minerals. This escalation peaks during the Pre-Feasibility and Feasibility stages before continuing to rise after production starts. Conflict patterns vary by mine size, mineral type, and ownership. Mechanism analysis highlights local economic development and environmental degradation induced by mining, amplifying the risk of conflict and emphasizing the need for local engagement.</p><button class="pub-toggle" onclick="pubToggle('abs-3',this)" aria-expanded="false"><svg viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg> Read abstract</button></div></div>

<!-- Paper 4 -->
<div class="pub-card"><div class="pub-img-col"><img src="/images/RESULTdeforstation.jpg" alt="Deforestation rate before/after mining discovery"><p class="pub-img-caption">Deforestation rate before/after<br>mining discovery</p></div><div class="pub-content-col"><div class="pub-badges"><span class="pub-badge pub-badge-green">Working Paper</span></div><p class="pub-title">Under the Canopy: Mining and Deforestation in Sub-Saharan Africa</p><p class="pub-coauthors">with <a href="https://sites.google.com/site/rajachakir/home" target="_blank" rel="noopener">Raja Chakir</a> and <a href="https://sites.google.com/site/ahmtritah/" target="_blank" rel="noopener">Ahmed Tritah</a> &nbsp;·&nbsp; <em>Available upon request</em></p><p class="pub-abstract collapsed" id="abs-4">This study examines the impact of mining on deforestation in Sub-Saharan Africa (2001–2018). Using geospatial data on 14 minerals and a Two-Way Fixed Effects Difference-in-Differences approach, we find that mining significantly increases deforestation, with indirect effects exceeding direct ones and extending up to 80 km from mining sites. Causal mediation analysis identifies key mechanisms, including agriculture, urbanization, infrastructure, and conflict. Results remain robust to global mineral price fluctuations and vary by mine size, mineral type, and ownership structure. Our findings highlight the broad environmental footprint of mining and the need for sustainable policies.</p><button class="pub-toggle" onclick="pubToggle('abs-4',this)" aria-expanded="false"><svg viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg> Read abstract</button></div></div>

<!-- ══════════════ WORK IN PROGRESS ══════════════ -->
<div class="pub-divider"></div>
<p class="pub-section-label">Work in progress</p>

<div class="pub-wip-card"><div class="pub-wip-icon"><svg viewBox="0 0 24 24"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg></div><div class="pub-wip-body"><p class="pub-wip-title">Mining, Local Governance, and Urbanization in Sub-Saharan Africa</p><p class="pub-wip-coauth">with Rose Camille Vincent</p></div><span class="pub-badge pub-badge-amber">In progress</span></div>

<div class="pub-wip-card"><div class="pub-wip-icon"><svg viewBox="0 0 24 24"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg></div><div class="pub-wip-body"><p class="pub-wip-title">Natural Disasters Kill Natural Resources: Is Mining Investment for Energy Transition at Risk?</p></div><span class="pub-badge pub-badge-amber">In progress</span></div>

</div>

<script>
function pubToggle(id, btn) {
  var el = document.getElementById(id);
  var collapsed = el.classList.contains('collapsed');
  el.classList.toggle('collapsed', !collapsed);
  btn.setAttribute('aria-expanded', collapsed ? 'true' : 'false');
  btn.innerHTML = collapsed
    ? '<svg viewBox="0 0 24 24" style="width:13px;height:13px;stroke:currentColor;fill:none;stroke-width:2.2;stroke-linecap:round;stroke-linejoin:round;display:inline-block;vertical-align:middle;transform:rotate(180deg)"><polyline points="6 9 12 15 18 9"/></svg> Hide abstract'
    : '<svg viewBox="0 0 24 24" style="width:13px;height:13px;stroke:currentColor;fill:none;stroke-width:2.2;stroke-linecap:round;stroke-linejoin:round;display:inline-block;vertical-align:middle;"><polyline points="6 9 12 15 18 9"/></svg> Read abstract';
}
</script>
