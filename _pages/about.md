---
permalink: /
title: "About Me"
author_profile: true
cover:
  video: cover-clouds.mp4
  poster: cover-clouds-poster.jpg
redirect_from: 
  - /about/
  - /about.html
---

<section class="content-box" markdown="1">

I am a postdoctoral scientist in the [Atmospheric Physics group](https://iac.ethz.ch/group/atmospheric-physics.html) of Prof. Ulrike Lohmann at ETH Zurich, where I am investigating the role of ice-nucleating particles in mixed-phase clouds using global climate models.

I completed my PhD at the [Max Planck Institute for Chemistry](https://www.mpic.de/2285/en) and the [Institute for Atmospheric Physics](https://www.blogs.uni-mainz.de/fb08-ipa-en/), Johannes Gutenberg University Mainz. Under the supervision of Prof. Jos Lelieveld and Prof. Holger Tost, my doctoral research focused on vegetation–climate interactions, specifically the role of biogenic volatile organic compound emissions in the Earth system.

Before my PhD, I completed a fellowship in Earth Observation at the [European Space Agency (ESA)](https://www.esa.int/) in Frascati, Italy. I hold a BSc in Physics & Mathematics and an MSc in Geosciences from the [University of Malta](https://www.um.edu.mt/).

</section>



<style>
.ri {
  --ri-card-bg: #fff;
  --ri-chip-bg: #eceff1;
  --ri-accent: #2a7793;
}
html[data-theme="dark"] .ri {
  --ri-card-bg: rgba(255, 255, 255, .045);
  --ri-chip-bg: rgba(255, 255, 255, .08);
  --ri-accent: #5cc6e4;
}
.ri-lead {
  font-size: 1.04rem;
  line-height: 1.62;
  color: var(--global-text-color);
  max-width: 46em;
  margin: 0 0 1.5em;
}
.ri-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 12px;
  margin: 0 0 1.9em;
}
.ri-card {
  border: 1px solid var(--global-border-color);
  border-radius: 11px;
  background: var(--ri-card-bg);
  padding: 16px 17px 17px;
  transition: border-color .15s ease;
}
.ri-card:hover { border-color: var(--ri-accent); }
.ri-icon {
  display: block;
  font-size: .95rem;
  color: var(--ri-accent);
  margin: 0 0 10px;
}
.ri-title {
  font-size: .97rem;
  font-weight: 700;
  line-height: 1.3;
  letter-spacing: -.008em;
  color: var(--global-text-color);
  margin: 0 0 6px;
}
.ri-desc {
  font-size: .85rem;
  line-height: 1.55;
  color: var(--global-text-color-light);
  margin: 0;
}
.ri-kicker {
  display: flex;
  align-items: center;
  gap: .85em;
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  font-size: .68rem;
  font-weight: 700;
  letter-spacing: .14em;
  text-transform: uppercase;
  color: var(--global-text-color-light);
  margin: 0 0 .95em;
}
.ri-kicker::after {
  content: "";
  flex: 1;
  height: 1px;
  background: var(--global-border-color);
}
.ri-chips {
  display: flex;
  flex-wrap: wrap;
  gap: 7px;
  list-style: none;
  margin: 0;
  padding: 0;
}
.ri-chips li {
  font-size: .8rem;
  line-height: 1.2;
  color: var(--global-text-color-light);
  background: var(--ri-chip-bg);
  border-radius: 999px;
  padding: 6px 12px;
}
@media (prefers-reduced-motion: reduce) {
  .ri-card { transition: none; }
}

.obs {
  --obs-card-bg: #fff;
  --obs-metric-bg: #eceff1;
  --obs-accent: #2a7793;
  --obs-green: #2e7d5b;
  --obs-warm: #d97706;
  --obs-purple: #7c3aed;
}
html[data-theme="dark"] .obs {
  --obs-card-bg: rgba(255, 255, 255, .045);
  --obs-metric-bg: rgba(255, 255, 255, .08);
  --obs-accent: #5cc6e4;
  --obs-green: #48b98a;
  --obs-warm: #f59e0b;
  --obs-purple: #a78bfa;
}
.obs-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 14px;
  margin: 0 0 1em;
}
.obs-card {
  border: 1px solid var(--global-border-color);
  border-radius: 11px;
  background: var(--obs-card-bg);
  padding: 18px;
  transition: border-color .15s ease;
  display: flex;
  flex-direction: column;
}
.obs-card:hover { border-color: var(--obs-accent); }
.obs-top {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 12px;
}
.obs-title {
  font-size: 1rem;
  font-weight: 700;
  line-height: 1.3;
  margin: 0 0 4px;
}
.obs-sub {
  font-size: 0.78rem;
  color: var(--global-text-color-light);
  margin: 0;
}
.obs-badge {
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  font-size: 0.65rem;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  padding: 3px 8px;
  border-radius: 5px;
  background: var(--obs-metric-bg);
  color: var(--global-text-color-light);
  display: inline-flex;
  align-items: center;
  gap: 5px;
  white-space: nowrap;
}
.obs-badge.is-live {
  color: var(--obs-green);
  background: rgba(46, 125, 91, 0.12);
}
html[data-theme="dark"] .obs-badge.is-live {
  background: rgba(72, 185, 138, 0.16);
}
.obs-pulse {
  width: 7px;
  height: 7px;
  border-radius: 50%;
  background: var(--obs-green);
  display: inline-block;
}
.obs-metrics {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 6px;
  margin: 10px 0 12px;
  padding: 10px 12px;
  background: var(--obs-metric-bg);
  border-radius: 8px;
}
.obs-m-item {
  display: flex;
  flex-direction: column;
}
.obs-m-lbl {
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  font-size: 0.62rem;
  text-transform: uppercase;
  color: var(--global-text-color-light);
  margin-bottom: 2px;
}
.obs-m-val {
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  font-size: 1.05rem;
  font-weight: 700;
  line-height: 1.2;
}
.obs-m-unit {
  font-size: 0.68rem;
  font-weight: 400;
  color: var(--global-text-color-light);
}
.obs-bortle {
  margin: 8px 0 14px;
  padding-top: 10px;
  border-top: 1px dashed var(--global-border-color);
}
.obs-bortle-top {
  display: flex;
  justify-content: space-between;
  font-size: 0.7rem;
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  color: var(--global-text-color-light);
  margin-bottom: 5px;
}
.obs-bortle-bar {
  height: 8px;
  border-radius: 4px;
  background: linear-gradient(to right, #eab308 0%, #ca8a04 25%, #475569 50%, #1e293b 75%, #020617 100%);
  position: relative;
}
.obs-bortle-pip {
  position: absolute;
  top: -2px;
  left: 75%;
  width: 5px;
  height: 12px;
  border-radius: 2px;
  background: #fff;
  box-shadow: 0 0 4px rgba(255,255,255,0.8);
  transition: left 0.3s ease;
}
.obs-img-preview {
  position: relative;
  aspect-ratio: 16 / 9;
  border-radius: 8px;
  overflow: hidden;
  margin: 10px 0 12px;
  border: 1px solid var(--global-border-color);
  background: #111418;
}
.obs-img-preview img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}
.obs-img-tag {
  position: absolute;
  bottom: 6px;
  left: 8px;
  background: rgba(0,0,0,0.72);
  color: #fff;
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  font-size: 0.65rem;
  padding: 2px 7px;
  border-radius: 4px;
}
.obs-link {
  font-size: 0.85rem;
  font-weight: 600;
  margin-top: auto;
  display: inline-flex;
  align-items: center;
  gap: 5px;
}
@media (prefers-reduced-motion: reduce) {
  .obs-card { transition: none; }
}
</style>

<section class="content-box">

<h2>Research</h2>

<div class="ri">

<p class="ri-lead">My work sits at the intersection of atmospheric physics and chemistry, climate science and Earth-system modelling &mdash; with a particular interest in the processes that shape clouds, and the part they play in the climate system.</p>

<div class="ri-grid">

<div class="ri-card">
<i class="fas fa-earth-europe ri-icon" aria-hidden="true"></i>
<h3 class="ri-title">Earth-system modelling</h3>
<p class="ri-desc">Coupled global models, used to follow how a change in one part of the system propagates through the rest.</p>
</div>

<div class="ri-card">
<i class="fas fa-cloud ri-icon" aria-hidden="true"></i>
<h3 class="ri-title">Aerosol&ndash;cloud interactions</h3>
<p class="ri-desc">How particles seed droplets and ice crystals &mdash; still the largest single uncertainty in the climate forcing record.</p>
</div>

<div class="ri-card">
<i class="fas fa-snowflake ri-icon" aria-hidden="true"></i>
<h3 class="ri-title">Cloud physics</h3>
<p class="ri-desc">The microphysics inside a cloud: nucleation, growth, freezing, and the step from droplet to precipitation.</p>
</div>

<div class="ri-card">
<i class="fas fa-sun ri-icon" aria-hidden="true"></i>
<h3 class="ri-title">Aerosol&ndash;climate interactions</h3>
<p class="ri-desc">The response of the climate system to aerosol, from direct scattering of sunlight through to circulation change.</p>
</div>

<div class="ri-card">
<i class="fas fa-leaf ri-icon" aria-hidden="true"></i>
<h3 class="ri-title">Vegetation&ndash;atmosphere interactions</h3>
<p class="ri-desc">Biogenic volatile organic compounds, and the chemistry that couples the land biosphere to aerosol and cloud.</p>
</div>

<div class="ri-card">
<i class="fas fa-cloud-bolt ri-icon" aria-hidden="true"></i>
<h3 class="ri-title">Convection</h3>
<p class="ri-desc">How convection organises, carries moisture and aerosol upward, and drives extreme rainfall.</p>
</div>

</div>

<p class="ri-kicker">Also</p>

<ul class="ri-chips">
<li>Earth observation</li>
<li>Satellite remote sensing</li>
<li>Shipping emissions</li>
<li>Light pollution</li>
</ul>

</div>

</section>

<section class="content-box">

<h2>Malta Atmospheric Observatory</h2>

<div class="obs">

<p class="ri-lead">Autonomous environmental observing stations and numerical weather prediction pipelines operating continuously in the Maltese Islands.</p>

<div class="obs-grid">

<!-- Card 1: Live Sensors -->
<div class="obs-card">
  <div class="obs-top">
    <div>
      <h3 class="obs-title">Malta Live Sensors</h3>
      <p class="obs-sub">Station: Mqabba &middot; Froggit WH3000, Airly, Unihedron SQM</p>
    </div>
    <span class="obs-badge is-live"><span class="obs-pulse"></span> LIVE</span>
  </div>

  <div class="obs-metrics">
    <div class="obs-m-item">
      <span class="obs-m-lbl">Temp</span>
      <span class="obs-m-val" style="color: var(--obs-warm);" id="obs-temp">26.9<span class="obs-m-unit">°C</span></span>
    </div>
    <div class="obs-m-item">
      <span class="obs-m-lbl">Humidity</span>
      <span class="obs-m-val" style="color: var(--obs-accent);" id="obs-rh">89<span class="obs-m-unit">%</span></span>
    </div>
    <div class="obs-m-item">
      <span class="obs-m-lbl">PM2.5</span>
      <span class="obs-m-val" style="color: var(--obs-green);" id="obs-pm25">3.0<span class="obs-m-unit">µg</span></span>
    </div>
    <div class="obs-m-item">
      <span class="obs-m-lbl">Sky</span>
      <span class="obs-m-val" style="color: var(--obs-purple);" id="obs-sky">16.4<span class="obs-m-unit">mpsas</span></span>
    </div>
  </div>

  <div class="obs-bortle">
    <div class="obs-bortle-top">
      <span>Night Sky Brightness (SQM)</span>
      <span>Dark Sky Indicator</span>
    </div>
    <div class="obs-bortle-bar">
      <div class="obs-bortle-pip" id="obs-bortle-pip" title="SQM reading position"></div>
    </div>
  </div>

  <a href="/environmental-monitoring/" class="obs-link">Open Live Dashboard &rarr;</a>
</div>

<!-- Card 2: Weather Forecast -->
<div class="obs-card">
  <div class="obs-top">
    <div>
      <h3 class="obs-title">Weather Forecasts</h3>
      <p class="obs-sub">Central Med &middot; ECMWF IFS 0.25° + DWD ICON-EU 0.0625°</p>
    </div>
    <span class="obs-badge">00z / 12z</span>
  </div>

  <div class="obs-img-preview">
    <img src="/images/S2-L-pressure.png" alt="Synoptic chart preview" loading="lazy">
    <span class="obs-img-tag">500 hPa Height Anomaly &middot; Central Med</span>
  </div>

  <p class="ri-desc" style="margin-bottom: 14px;">Pre-rendered synoptic maps, high-resolution meteograms, and MTG satellite loops updated twice daily.</p>

  <a href="/forecast/" class="obs-link">View Synoptic Weather Charts &rarr;</a>
</div>

</div>
</div>

<script>
/* Safe from Jekyll HTML compressor: only block comments used here */
(function() {
  var LOCAL_URL = "/data/current.json";
  var REMOTE_URL = "https://raw.githubusercontent.com/ryanvella9/ryanvella9.github.io/data/current.json";

  function update(d) {
    if (!d) return;
    if (d.weather && d.weather.temp != null) {
      var t = document.getElementById("obs-temp");
      if (t) t.innerHTML = Number(d.weather.temp).toFixed(1) + '<span class="obs-m-unit">°C</span>';
    }
    if (d.weather && d.weather.rh != null) {
      var r = document.getElementById("obs-rh");
      if (r) r.innerHTML = Math.round(d.weather.rh) + '<span class="obs-m-unit">%</span>';
    }
    if (d.air && d.air.pm25 != null) {
      var p = document.getElementById("obs-pm25");
      if (p) p.innerHTML = Number(d.air.pm25).toFixed(1) + '<span class="obs-m-unit">µg</span>';
    }
    if (d.sky && d.sky.mag != null) {
      var s = document.getElementById("obs-sky");
      if (s) s.innerHTML = Number(d.sky.mag).toFixed(1) + '<span class="obs-m-unit">mpsas</span>';
      var pip = document.getElementById("obs-bortle-pip");
      if (pip) {
        var mag = Number(d.sky.mag);
        var pct = Math.max(0, Math.min(100, ((mag - 15.0) / (21.8 - 15.0)) * 100));
        pip.style.left = pct.toFixed(1) + "%";
      }
    }
  }

  fetch(LOCAL_URL)
    .then(function(res) { if (!res.ok) throw new Error(); return res.json(); })
    .then(update)
    .catch(function() {
      fetch(REMOTE_URL)
        .then(function(res) { return res.json(); })
        .then(update)
        .catch(function() {});
    });
})();
</script>

</section>

<section class="content-box" markdown="1">

## Beyond Research

I co-founded and managed the environmental NGO Għaqda Siġar Maltin in Malta, dedicating several years to promoting ecological sustainability. I am passionate about trees, birds, and the natural environment. I enjoy working with satellite data and also operate several personal environmental sensors in Malta. As part of my conservation work, I help to raise awareness about light pollution and advocate for the preservation of Malta’s remaining Dark Sky Heritage Areas. Beyond these projects, I enjoy biking, hiking, and capturing the beauty of nature through photography.

</section>

<p style="margin: 2em 0 1.2em;">
  <a href="/files/rv_cv.pdf" class="btn btn--primary" download style="display: inline-flex; align-items: center; gap: 8px; padding: 10px 18px; border-radius: 6px; font-weight: 600; text-decoration: none;">
    <i class="fas fa-file-arrow-down" aria-hidden="true"></i> Download Curriculum Vitae (PDF)
  </a>
</p>

<div style="text-align: right; font-style: italic;">
Last updated on 30 August 2026
</div>
