---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

<style>
.rx { margin: 1.4em 0 0; }
.rx-vis { margin: 0 0 2.6em; }
.rx-vis-frame {
  position: relative;
  aspect-ratio: 16 / 9;
  border-radius: 10px;
  overflow: hidden;
  background: #14181b center / cover no-repeat;
}
.rx-vis-video { width: 100%; height: 100%; object-fit: cover; display: block; }
.rx-vis-cap {
  font-size: .8rem;
  line-height: 1.55;
  color: var(--global-text-color-light);
  margin: .75em 0 0;
  max-width: 46em;
}
.rx-vis-cap b { color: var(--global-text-color); font-weight: 600; }
/* The still carries the panel whenever the clip does not play: before the
   first frame decodes, if the file 404s, and under reduced motion. */
@media (prefers-reduced-motion: reduce) {
  .rx-vis-video { display: none; }
}
.rx-lead {
  font-size: 1.3rem;
  line-height: 1.62;
  font-weight: 400;
  letter-spacing: -.003em;
  color: var(--global-text-color);
  max-width: 40em;
  margin: 0 0 1.9em;
}
.rx-more {
  font-size: 1.05rem;
  line-height: 1.6;
  color: var(--global-text-color);
  margin: 0 0 .9em;
}
.rx-strands {
  list-style: none;
  padding: 0;
  margin: 0;
  max-width: 42em;
}
.rx-strands li {
  position: relative;
  padding: 0 0 0 1.15em;
  margin: 0 0 .6em;
  font-size: 1.05rem;
  line-height: 1.6;
  color: var(--global-text-color);
}
.rx-strands li::before {
  content: "";
  position: absolute;
  left: 0;
  top: .68em;
  width: 6px;
  height: 2px;
  background: var(--global-link-color);
}
@media (max-width: 560px) {
  .rx-lead { font-size: 1.16rem; margin-bottom: 1.6em; }
  .rx-more, .rx-strands li { font-size: 1rem; }
}
</style>

<div class="rx">
<figure class="rx-vis">
<div class="rx-vis-frame" style="background-image: url('/images/icon-ham-globes-poster.jpg');">
<video class="rx-vis-video" autoplay muted loop playsinline preload="metadata" poster="/images/icon-ham-globes-poster.jpg">
<source src="/images/icon-ham-globes.mp4" type="video/mp4">
</video>
</div>
<figcaption class="rx-vis-cap"><b>Aerosols, clouds and precipitation in a global ICON-HAM simulation, 1999&ndash;2010.</b> Aerosol optical depth at 550&nbsp;nm split by species (left), total cloud cover (centre) and precipitation rate (right).</figcaption>
</figure>
<p class="rx-lead">I work with global climate models to study the processes that shape clouds &mdash; in particular the role of ice-nucleating particles in mixed-phase clouds.</p>
<p class="rx-more">My broader interests include:</p>
<ul class="rx-strands">
<li>High-resolution and large-eddy simulation approaches to convective processes</li>
<li>Chemical processes in aerosols, and atmospheric gas-to-particle conversion</li>
<li>Vegetation&rsquo;s influence on climate through aerosol&ndash;cloud interactions</li>
</ul>
</div>
