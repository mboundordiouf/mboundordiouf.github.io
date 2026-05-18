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
/* ── Reset & base ─────────────────────────────────────────── */
.pub-page *,
.pub-page *::before,
.pub-page *::after { box-sizing: border-box; margin: 0; padding: 0; }

.pub-page {
  font-family: 'DM Sans', -apple-system, sans-serif;
  max-width: 900px;
  padding: 0.5rem 0 3rem;
  color: #1a1a18;
}

/* ── Section label ─────────────────────────────────────────── */
.pub-section-label {
  font-size: 10.5px;
  font-weight: 500;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: #888780;
  margin: 2.5rem 0 1.1rem;
  display: flex;
  align-items: center;
  gap: 10px;
}
.pub-section-label::after {
  content: '';
  flex: 1;
  height: 0.5px;
  background: #D3D1C7;
}

/* ── Publication card ──────────────────────────────────────── */
.pub-card {
  display: grid;
  grid-template-columns: 210px minmax(0, 1fr);
  border: 0.5px solid #D3D1C7;
  border-radius: 14px;
  overflow: hidden;
  margin-bottom: 1.2rem;
  background: #fff;
  transition: border-color 0.2s ease, box-shadow 0.2s ease;
}
.pub-card:hover {
  border-color: #B4B2A9;
  box-shadow: 0 2px 16px rgba(0,0,0,0.06);
}

/* ── Left column — image ───────────────────────────────────── */
.pub-img-col {
  background: #F7F6F2;
  border-right: 0.5px solid #D3D1C7;
  padding: 1.2rem 1rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 10px;
  min-height: 210px;
}

.pub-img-col img {
  width: 100%;
  height: 148px;
  object-fit: cover;
  border-radius: 8px;
  border: 0.5px solid #D3D1C7;
  display: block;
}

.pub-img-caption {
  font-size: 10px;
  color: #888780;
  text-align: center;
  line-height: 1.45;
  font-style: italic;
}

/* Multiple images stacked */
.pub-img-col.two-images img {
  height: 104px;
}

/* ── Right column — content ────────────────────────────────── */
.pub-content-col {
  padding: 1.3rem 1.5rem;
  display: flex;
  flex-direction: column;
  gap: 9px;
}

/* ── Badges ────────────────────────────────────────────────── */
.pub-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 5px;
}
.badge {
  font-size: 10px;
  font-weight: 500;
  letter-spacing: 0.4px;
  padding: 3px 9px;
  border-radius: 6px;
  line-height: 1.6;
}
.badge-blue   { background: #E6F1FB; color: #0C447C; }
.badge-green  { background: #EAF3DE; color: #27500A; }
.badge-amber  { background: #FAEEDA; color: #633806; }
.badge-teal   { background: #E1F5EE; color: #085041; }

/* ── Title ─────────────────────────────────────────────────── */
.pub-title {
  font-family: 'Lora', Georgia, serif;
  font-size: 15.5px;
  font-weight: 600;
  color: #1a1a18;
  line-height: 1.48;
  letter-spacing: -0.15px;
}

/* ── Co-authors ─────────────────────────────────────────────── */
.pub-coauthors {
  font-size: 12px;
  color: #5F5E5A;
  line-height: 1.5;
}
.pub-coauthors a {
  color: #185FA5;
  text-decoration: none;
  font-weight: 400;
}
.pub-coauthors a:hover { text-decoration: underline; }

/* ── Abstract ───────────────────────────────────────────────── */
.pub-abstract {
  font-size: 12.5px;
  color: #5F5E5A;
  line-height: 1.68;
  flex: 1;
}
.pub-abstract.collapsed {
  display: -webkit-box;
  -webkit-line-clamp: 4;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

/* ── Toggle button ──────────────────────────────────────────── */
.pub-toggle {
  background: none;
  border: none;
  cursor: pointer;
  font-family: 'DM Sans', sans-serif;
  font-size: 11.5px;
  font-weight: 500;
  color: #185FA5;
  padding: 0;
  display: inline-flex;
  align-items: center;
  gap: 4px;
  transition: opacity 0.15s;
  align-self: flex-start;
}
.pub-toggle:hover { opacity: 0.7; }
.pub-toggle svg {
  width: 13px;
  height: 13px;
  stroke: currentColor;
  fill: none;
  stroke-width: 2.2;
  stroke-linecap: round;
  stroke-linejoin: round;
  transition: transform 0.2s;
}
.pub-toggle.open svg { transform: rotate(180deg); }

/* ── Divider ────────────────────────────────────────────────── */
.pub-divider {
  height: 0.5px;
  background: #D3D1C7;
  margin: 2.5rem 0 0;
}

/* ── Work-in-progress cards ─────────────────────────────────── */
.wip-card {
  display: flex;
  align-items: center;
  gap: 14px;
  padding: 0.95rem 1.25rem;
  background: #fff;
  border: 0.5px solid #D3D1C7;
  border-radius: 12px;
  margin-bottom: 0.75rem;
  transition: border-color 0.2s ease;
}
.wip-card:hover { border-color: #B4B2A9; }

.wip-icon {
  width: 38px;
  height: 38px;
  border-radius: 50%;
  background: #F7F6F2;
  border: 0.5px solid #D3D1C7;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}
.wip-icon svg {
  width: 17px;
  height: 17px;
  stroke: #888780;
  fill: none;
  stroke-width: 1.8;
  stroke-linecap: round;
  stroke-linejoin: round;
}

.wip-body { flex: 1; }
.wip-title {
  font-family: 'Lora', Georgia, serif;
  font-size: 13.5px;
  font-weight: 600;
  color: #1a1a18;
  line-height: 1.42;
}
.wip-coauth {
  font-size: 11.5px;
  color: #888780;
  margin-top: 3px;
}

/* ── Responsive ─────────────────────────────────────────────── */
@media (max-width: 680px) {
  .pub-card {
    grid-template-columns: 1fr;
  }
  .pub-img-col {
    border-right: none;
    border-bottom: 0.5px solid #D3D1C7;
    min-height: unset;
  }
  .pub-img-col img {
    height: 180px;
  }
  .wip-card {
    flex-wrap: wrap;
  }
}
</style>

<div class="pub-page">

  <!-- ─────────────────── ONGOING WORKS ─────────────────── -->
  <p class="pub-section-label">On-going works</p>

  <!-- Paper 1 -->
  <div class="pub-card">
    <div class="pub-img-col">
      <img src="/images/Malaria_Electricity.png" alt="Map: Malaria and Electricity Access at DHS cluster levels in SSA 1997-2021">
      <p class="pub-img-caption">Malaria &amp; Electricity Access<br>DHS clusters · SSA 1997–2021</p>
    </div>
    <div class="pub-content-col">
      <div class="pub-badges">
        <span class="badge badge-blue">On-going</span>
        <span class="badge badge-teal">Solo-authored</span>
      </div>
      <p class="pub-title">Light and Disease: Mining-Electrification and Malaria in Africa</p>
      <p class="pub-abstract collapsed" id="abs-1">
        I study the health externalities of industrial mining using 1.6 million grid-cell–year observations
        for 45 sub-Saharan African countries from 2000 to 2022. Exploiting staggered mine discoveries in a
        ring-based difference-in-differences design, I find that mining increases annual malaria incidence
        by 35 cases per 1,000 (+10.5% relative to baseline), prevalence by 6.2 percentage points (+21.4%),
        and mortality by 9.6 deaths per 100,000 (+9.3%) in a 5 km grid cell exposed to mining, with effects
        3 to 4 times larger at 10–50 km than within 10 km of the mine. Cumulating over a 15-year horizon,
        these translate into a +158.2% increase in incidence, +140.1% in prevalence, and +320.6% in
        mortality relative to pre-treatment levels — the mortality burden accelerating as immunity erodes
        and health systems are strained. Deforestation is the dominant mechanism and fully explains the
        malaria premium of artisanal gold mining, whose effects are 4–8 times larger than those of formal
        operations. Mine-induced electrification attenuates but does not offset these impacts, and the
        net health costs fall disproportionately on poor households, who bear most of the deforestation
        burden while richer households capture electrification gains.
      </p>
      <button class="pub-toggle" onclick="pubToggle('abs-1', this)" aria-expanded="false">
        <svg viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
        Read abstract
      </button>
    </div>
  </div>

  <!-- Paper 2 -->
  <div class="pub-card">
    <div class="pub-img-col two-images">
      <img src="/images/mining_electricty_ASS.png" alt="Discovery Mining (2001-2009) and Population Access of Energy (2000 and 2010)">
      <img src="/images/DISTANCE_generator_energy_access_ssa.png" alt="Energy Access from generator locations in SSA">
      <p class="pub-img-caption">Discovery Mining &amp; Energy Access · SSA</p>
    </div>
    <div class="pub-content-col">
      <div class="pub-badges">
        <span class="badge badge-green">Working Paper</span>
      </div>
      <p class="pub-title">Mining and Power: Darkness or Lighting for Africa?</p>
      <p class="pub-coauthors">
        with <a href="https://search.asu.edu/profile/2183493" target="_blank" rel="noopener">Nathan Johnson</a>
        and <a href="https://scholar.google.com/citations?user=hrZlpwUAAAAJ&hl=en" target="_blank" rel="noopener">Tam Kemabonta</a>
        &nbsp;·&nbsp; <em>Available upon request</em>
      </p>
      <p class="pub-abstract collapsed" id="abs-2">
        This study investigates the effect of mining activities involving 32 minerals on energy access
        (created using population and night lights at 1×1 km resolution) in sub-Saharan Africa from 2000 to 2022.
        Using georeferenced data in cells of 0.5°×0.5°, we compare energy access in areas with active mines
        to those with inactive mines, defined as sites that were discovered but were never active, serving as
        our control group. Our results indicate no evidence of active mines on energy access when using inactive
        mines for comparison. However, when all areas without mines are considered as the control group, the
        impact of mining activities appears significant and positive. Our findings show that regions mining
        energy-intensive minerals like uranium and cobalt have the lowest energy access. In contrast, those
        mining less intensive minerals such as gold have higher access rates. Interestingly, cells with Giant
        and SuperGiant mine sizes have relatively low energy access for local communities. Mining areas exhibit
        enclave characteristics, with positive spillover effects on nearby regions. Energy access is notably
        greater in mining locations near generators, power plants, large cities, ports, and key agricultural areas.
      </p>
      <button class="pub-toggle" onclick="pubToggle('abs-2', this)" aria-expanded="false">
        <svg viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
        Read abstract
      </button>
    </div>
  </div>

  <!-- Paper 3 -->
  <div class="pub-card">
    <div class="pub-img-col">
      <img src="/images/africa_conflict_events_1997_2022ok.png" alt="Number of conflict events in Africa 1997-2021">
      <p class="pub-img-caption">Conflict events in Africa · 1997–2022</p>
    </div>
    <div class="pub-content-col">
      <div class="pub-badges">
        <span class="badge badge-green">Working Paper</span>
      </div>
      <p class="pub-title">The New Mining Rush: Mineral Discoveries and Social Conflicts in Africa</p>
      <p class="pub-coauthors">
        with <a href="https://sites.google.com/site/soubeyranhomepage/" target="_blank" rel="noopener">Raphael Soubeyran</a>
        and <a href="https://sites.google.com/site/ahmtritah/" target="_blank" rel="noopener">Ahmed Tritah</a>
        &nbsp;·&nbsp; <em>Available upon request</em>
      </p>
      <p class="pub-abstract collapsed" id="abs-3">
        The global energy transition is crucial but presents social and political challenges, particularly
        in mineral-rich African countries. This study uses high-resolution data to explore the relationship
        between mining discoveries and conflict from 1997 to 2022. Using high-resolution remote sensing data
        combined with a dynamic panel and event-study approach, our findings indicate that conflict increases
        during exploration, primarily due to protests and riots over gold minerals. This escalation peaks
        during the Pre-Feasibility and Feasibility stages before continuing to rise after production starts.
        Conflict patterns vary by mine size, mineral type, and ownership. Mechanism analysis highlights local
        economic development (local economic activity, electricity access, urbanization, and migration) and
        environmental degradation (deforestation rate) induced by mining, amplifying the risk of conflict and
        emphasizing the need for local engagement. Results are consistent across varying specifications,
        including using mineral prices as a treatment variable and adopting a Synthetic Control
        Differences-in-Differences design.
      </p>
      <button class="pub-toggle" onclick="pubToggle('abs-3', this)" aria-expanded="false">
        <svg viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
        Read abstract
      </button>
    </div>
  </div>

  <!-- Paper 4 -->
  <div class="pub-card">
    <div class="pub-img-col">
      <img src="/images/RESULTdeforstation.jpg" alt="Deforestation rate before/after mining discovered at cell and buffer zone levels">
      <p class="pub-img-caption">Deforestation rate before/after<br>mining discovery</p>
    </div>
    <div class="pub-content-col">
      <div class="pub-badges">
        <span class="badge badge-green">Working Paper</span>
      </div>
      <p class="pub-title">Under the Canopy: Mining and Deforestation in Sub-Saharan Africa</p>
      <p class="pub-coauthors">
        with <a href="https://sites.google.com/site/rajachakir/home" target="_blank" rel="noopener">Raja Chakir</a>
        and <a href="https://sites.google.com/site/ahmtritah/" target="_blank" rel="noopener">Ahmed Tritah</a>
        &nbsp;·&nbsp; <em>Available upon request</em>
      </p>
      <p class="pub-abstract collapsed" id="abs-4">
        This study examines the impact of mining on deforestation in Sub-Saharan Africa (2001–2018).
        Using geospatial data on 14 minerals and a Two-Way Fixed Effects Difference-in-Differences
        approach, we find that mining significantly increases deforestation, with indirect effects
        exceeding direct ones and extending up to 80 km from mining sites. Causal mediation analysis
        identifies key mechanisms, including agriculture, urbanization, infrastructure, and conflict.
        Results remain robust to global mineral price fluctuations and vary by mine size, mineral type,
        and ownership structure. Our findings highlight the broad environmental footprint of mining
        and the need for sustainable policies.
      </p>
      <button class="pub-toggle" onclick="pubToggle('abs-4', this)" aria-expanded="false">
        <svg viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"/></svg>
        Read abstract
      </button>
    </div>
  </div>


  <!-- ─────────────────── WORK IN PROGRESS ─────────────────── -->
  <div class="pub-divider"></div>
  <p class="pub-section-label">Work in progress</p>

  <div class="wip-card">
    <div class="wip-icon">
      <svg viewBox="0 0 24 24"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg>
    </div>
    <div class="wip-body">
      <p class="wip-title">Mining, Local Governance, and Urbanization in Sub-Saharan Africa</p>
      <p class="wip-coauth">with Rose Camille Vincent</p>
    </div>
    <span class="badge badge-amber">In progress</span>
  </div>

  <div class="wip-card">
    <div class="wip-icon">
      <svg viewBox="0 0 24 24"><path d="M14.5 10c-.83 0-1.5-.67-1.5-1.5v-5c0-.83.67-1.5 1.5-1.5s1.5.67 1.5 1.5v5c0 .83-.67 1.5-1.5 1.5z"/><path d="M20.5 10H19V8.5c0-.83.67-1.5 1.5-1.5s1.5.67 1.5 1.5-.67 1.5-1.5 1.5z"/><path d="M9.5 14c.83 0 1.5.67 1.5 1.5v5c0 .83-.67 1.5-1.5 1.5S8 21.33 8 20.5v-5c0-.83.67-1.5 1.5-1.5z"/><path d="M3.5 14H5v1.5c0 .83-.67 1.5-1.5 1.5S2 16.33 2 15.5 2.67 14 3.5 14z"/><path d="M14 14.5c0-.83.67-1.5 1.5-1.5h5c.83 0 1.5.67 1.5 1.5s-.67 1.5-1.5 1.5h-5c-.83 0-1.5-.67-1.5-1.5z"/><path d="M15.5 19H14v1.5c0 .83.67 1.5 1.5 1.5s1.5-.67 1.5-1.5-.67-1.5-1.5-1.5z"/><path d="M10 9.5C10 8.67 9.33 8 8.5 8h-5C2.67 8 2 8.67 2 9.5S2.67 11 3.5 11h5c.83 0 1.5-.67 1.5-1.5z"/><path d="M8.5 5H10V3.5C10 2.67 9.33 2 8.5 2S7 2.67 7 3.5 7.67 5 8.5 5z"/></svg>
    </div>
    <div class="wip-body">
      <p class="wip-title">Natural Disasters Kill Natural Resources: Is Mining Investment for Energy Transition at Risk?</p>
    </div>
    <span class="badge badge-amber">In progress</span>
  </div>

</div>

<script>
function pubToggle(id, btn) {
  var el = document.getElementById(id);
  var isCollapsed = el.classList.contains('collapsed');
  el.classList.toggle('collapsed', !isCollapsed);
  btn.setAttribute('aria-expanded', isCollapsed ? 'true' : 'false');
  btn.classList.toggle('open', isCollapsed);
  btn.innerHTML = isCollapsed
    ? '<svg viewBox="0 0 24 24" style="width:13px;height:13px;stroke:currentColor;fill:none;stroke-width:2.2;stroke-linecap:round;stroke-linejoin:round;transform:rotate(180deg)"><polyline points="6 9 12 15 18 9"/></svg> Hide abstract'
    : '<svg viewBox="0 0 24 24" style="width:13px;height:13px;stroke:currentColor;fill:none;stroke-width:2.2;stroke-linecap:round;stroke-linejoin:round;"><polyline points="6 9 12 15 18 9"/></svg> Read abstract';
}
</script>
