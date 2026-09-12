---
layout: archive
title: "Photography"
permalink: /photography/
author_profile: true
---

<style>
/* Fixed-width columns rather than 1fr, so two photos stay thumbnail-sized
   instead of stretching to fill half the page each. */
.ph-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, 210px);
  justify-content: start;
  gap: 16px;
  margin: 1.4em 0 0;
}
@media (max-width: 480px) {
  .ph-grid { grid-template-columns: repeat(auto-fill, minmax(140px, 1fr)); }
}
.ph-item {
  display: block;
  padding: 0;
  border: 0;
  border-radius: 10px;
  overflow: hidden;
  background: #14181b;
  cursor: zoom-in;
  line-height: 0;
}
.ph-item img {
  width: 100%;
  height: auto;
  aspect-ratio: 1 / 1;
  object-fit: cover;
  display: block;
  transition: transform .35s ease, opacity .2s ease;
}
.ph-item:hover img,
.ph-item:focus-visible img { transform: scale(1.035); opacity: .93; }
.ph-item:focus-visible { outline: 2px solid var(--global-link-color); outline-offset: 3px; }

.ph-lb {
  position: fixed;
  inset: 0;
  z-index: 999;
  display: none;
  align-items: center;
  justify-content: center;
  padding: 3vmin;
  background: rgba(8, 10, 12, .93);
  /* The backdrop itself is the click target for dismissing the lightbox. */
  cursor: zoom-out;
}
.ph-lb.is-open { display: flex; }
.ph-lb img {
  max-width: 100%;
  max-height: 94vh;
  width: auto;
  height: auto;
  border-radius: 4px;
  cursor: default;
}
.ph-close {
  position: absolute;
  top: 12px;
  right: 16px;
  width: 44px;
  height: 44px;
  font-size: 1.9rem;
  line-height: 1;
  color: #fff;
  background: none;
  border: 0;
  border-radius: 6px;
  cursor: pointer;
  opacity: .75;
}
.ph-close:hover, .ph-close:focus-visible { opacity: 1; }
body.ph-locked { overflow: hidden; }
@media (prefers-reduced-motion: reduce) {
  .ph-item img { transition: none; }
  .ph-item:hover img, .ph-item:focus-visible img { transform: none; }
}
</style>

<div class="ph-grid">
<button type="button" class="ph-item" aria-label="Enlarge: the Milky Way over Death Valley">
<img src="/images/photography/final_milkyway_plus_background.jpg" alt="The Milky Way rising over a dark ridge in Death Valley, California" width="1344" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: dragonfly resting on a bramble stem">
<img src="/images/photography/dsc05911.jpg" alt="A dragonfly resting on a bramble stem against a green background" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: cumulus clouds building over a lake">
<img src="/images/photography/img_5301.jpg" alt="Cumulus clouds building over a lake, seen from a wooded shoreline" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: a cumulus tower over a desert plateau">
<img src="/images/photography/dsc07713.jpg" alt="A tall cumulus cloud building over a desert plateau, with red rock and distant mesas below" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: golden larches on a snow-dusted alpine slope">
<img src="/images/photography/img_7682.jpg" alt="Larches in golden autumn colour on a snow-dusted alpine slope, below a waterfall and grey peaks" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: fireworks over a city waterfront at dusk">
<img src="/images/photography/dsc06772.jpg" alt="Fireworks bursting in gold, red and green over a city waterfront at dusk" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: aerial view of a sandy bay and anchored boats">
<img src="/images/photography/dsc02491.jpg" alt="An aerial view of a sandy bay, boats anchored over turquoise shallows that deepen to open blue" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: a narrow beach seen from directly above">
<img src="/images/photography/40eb74f8-e7b8-40fc-8dc1-c8dfe2b2fb91.jpg" alt="A narrow sandy beach between scrubland and clear green shallows, seen from directly above" width="1875" height="1875" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: boats moored over turquoise shallows">
<img src="/images/photography/dji_0808.jpg" alt="Small boats and a swimming pontoon moored over bright turquoise shallows, seen from directly above" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: a narrow inlet between limestone cliffs">
<img src="/images/photography/a65aa8a8-8e55-4215-a6c2-bcde96cee74d.jpg" alt="A narrow inlet of deep blue water between pale limestone cliffs, seen from directly above" width="1875" height="1875" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: a red and white husky">
<img src="/images/photography/dsc09492.jpg" alt="A red and white husky panting, photographed close up at an outdoor gathering" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: fossil scallop shells in limestone">
<img src="/images/photography/img_0440.jpg" alt="Fossilised scallop shells embedded in weathered pale limestone" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: the Statue of Liberty against a pale sky">
<img src="/images/photography/dsc05668.jpg" alt="The Statue of Liberty on its stone pedestal against a pale blue sky" width="2000" height="2000" loading="lazy">
</button>
</div>

<div class="ph-lb" role="dialog" aria-modal="true" aria-label="Enlarged photograph">
<button type="button" class="ph-close" aria-label="Close">&times;</button>
<img src="" alt="">
</div>

<script>
/* The site's HTML compressor collapses this block onto a single line, so only
   block comments are safe here: a double-slash comment would swallow the whole
   rest of the script and break it. */
(function () {
  var box = document.querySelector(".ph-lb");
  var full = box.querySelector("img");
  var closeBtn = box.querySelector(".ph-close");
  var opener = null;

  function open(thumb) {
    full.src = thumb.src;
    full.alt = thumb.alt;
    box.classList.add("is-open");
    document.body.classList.add("ph-locked");
    closeBtn.focus();
  }

  function close() {
    box.classList.remove("is-open");
    document.body.classList.remove("ph-locked");
    /* Drop the source so a large image is not held in memory while closed. */
    full.src = "";
    if (opener) { opener.focus(); opener = null; }
  }

  document.querySelectorAll(".ph-item").forEach(function (btn) {
    btn.addEventListener("click", function () {
      opener = btn;
      open(btn.querySelector("img"));
    });
  });

  closeBtn.addEventListener("click", close);
  /* Clicking the photo itself should not dismiss, only the surrounding backdrop. */
  box.addEventListener("click", function (e) { if (e.target !== full) close(); });
  document.addEventListener("keydown", function (e) {
    if (e.key === "Escape" && box.classList.contains("is-open")) close();
  });
})();
</script>
