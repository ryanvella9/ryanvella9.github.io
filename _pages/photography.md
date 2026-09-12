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

/* Step buttons, so the lightbox is somewhere to browse from rather than a
   one-shot view that has to be closed and reopened for every photograph.
   Deliberately sitting over the image rather than outside it: at 94vh tall
   there is no reliable margin to put them in, and a faint scrim keeps them
   legible over a bright frame as easily as over a dark one. */
.ph-nav {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  width: 52px;
  height: 76px;
  font-size: 2.2rem;
  line-height: 1;
  color: #fff;
  background: rgba(8, 10, 12, .38);
  border: 0;
  border-radius: 6px;
  cursor: pointer;
  opacity: .6;
}
.ph-nav:hover, .ph-nav:focus-visible { opacity: 1; background: rgba(8, 10, 12, .62); }
.ph-prev { left: 10px; }
.ph-next { right: 10px; }
/* Which of thirteen you are looking at. Without it, wrapping from the last
   photograph to the first reads as the gallery having glitched rather than as
   having come full circle. */
.ph-count {
  position: absolute;
  left: 50%;
  bottom: 10px;
  transform: translateX(-50%);
  font-size: .85rem;
  letter-spacing: .04em;
  color: #fff;
  opacity: .68;
  font-variant-numeric: tabular-nums;
  pointer-events: none;
}
@media (max-width: 480px) {
  /* Smaller, because on a phone the swipe is the primary control and these
     become the fallback — but still past the 44 px minimum tap target. */
  .ph-nav { width: 44px; height: 64px; font-size: 1.7rem; }
}
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
<button type="button" class="ph-nav ph-prev" aria-label="Previous photograph">&#8249;</button>
<img src="" alt="">
<button type="button" class="ph-nav ph-next" aria-label="Next photograph">&#8250;</button>
<span class="ph-count" aria-live="polite"></span>
</div>

<script>
/* The site's HTML compressor collapses this block onto a single line, so only
   block comments are safe here: a double-slash comment would swallow the whole
   rest of the script and break it. */
(function () {
  var box = document.querySelector(".ph-lb");
  var full = box.querySelector("img");
  var closeBtn = box.querySelector(".ph-close");
  var prevBtn = box.querySelector(".ph-prev");
  var nextBtn = box.querySelector(".ph-next");
  var count = box.querySelector(".ph-count");
  var items = Array.prototype.slice.call(document.querySelectorAll(".ph-item"));
  /* Which photograph is open, or -1 for none. Replaces the old `opener`
     reference: the index answers both "what do I show next" and "what do I
     hand focus back to", where a bare element answered only the second. */
  var at = -1;

  /* Fetch the neighbours as soon as one is shown, so stepping is a swap of an
     already-decoded image rather than a fresh download with a blank frame in
     the middle of it. The grid holds the same files, but those are lazy and a
     photograph further down the page may never have been fetched at all. */
  function preload(i) {
    var img = items[i] && items[i].querySelector("img");
    if (img) { new Image().src = img.src; }
  }

  function show(i) {
    /* Wraps in both directions, so the end of the gallery is not a dead end.
       The counter below is what keeps that from reading as a glitch. */
    at = (i + items.length) % items.length;
    var thumb = items[at].querySelector("img");
    full.src = thumb.src;
    full.alt = thumb.alt;
    count.textContent = (at + 1) + " / " + items.length;
    preload((at + 1) % items.length);
    preload((at - 1 + items.length) % items.length);
  }

  function open(i) {
    show(i);
    box.classList.add("is-open");
    document.body.classList.add("ph-locked");
    closeBtn.focus();
  }

  function close() {
    box.classList.remove("is-open");
    document.body.classList.remove("ph-locked");
    /* Drop the source so a large image is not held in memory while closed. */
    full.src = "";
    /* Back to whichever thumbnail was last shown rather than the one that was
       first clicked — after stepping through six photographs, returning focus
       to the sixth is what puts the keyboard where the eye already is. */
    if (at >= 0) { items[at].focus(); at = -1; }
  }

  items.forEach(function (btn, i) {
    btn.addEventListener("click", function () { open(i); });
  });

  closeBtn.addEventListener("click", close);
  prevBtn.addEventListener("click", function () { show(at - 1); });
  nextBtn.addEventListener("click", function () { show(at + 1); });

  /* Only the backdrop dismisses. This used to test against the photo alone,
     which was right when the photo was the only thing on the backdrop; the
     step buttons sit on it too, so a click on one would have closed the
     lightbox instead of advancing it. Testing for the backdrop itself is the
     form that stays correct as controls are added. */
  box.addEventListener("click", function (e) { if (e.target === box) close(); });

  document.addEventListener("keydown", function (e) {
    if (!box.classList.contains("is-open")) { return; }
    if (e.key === "Escape") { close(); }
    else if (e.key === "ArrowRight") { e.preventDefault(); show(at + 1); }
    else if (e.key === "ArrowLeft") { e.preventDefault(); show(at - 1); }
  });

  /* Swipe, so a phone can flick through without aiming at a 44 px arrow.
     Threshold in pixels rather than a fraction of the width: it is guarding
     against a shaky tap, which is the same few pixels on any screen. */
  var x0 = null;
  box.addEventListener("touchstart", function (e) {
    x0 = e.changedTouches[0].clientX;
  }, { passive: true });
  box.addEventListener("touchend", function (e) {
    if (x0 === null) { return; }
    var dx = e.changedTouches[0].clientX - x0;
    x0 = null;
    if (Math.abs(dx) > 45) { show(dx < 0 ? at + 1 : at - 1); }
  });

  /* A gallery of one has nothing to step through, and arrows that wrap to the
     same photograph would look broken. */
  if (items.length < 2) {
    prevBtn.hidden = nextBtn.hidden = count.hidden = true;
  }
})();
</script>
