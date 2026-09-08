---
layout: archive
title: "Photography"
permalink: /photography/
author_profile: true
---

<style>
.ph-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 18px;
  margin: 1.4em 0 0;
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
<button type="button" class="ph-item" aria-label="Enlarge: dragonfly resting on a bramble stem">
<img src="/images/photography/dsc05911.jpg" alt="A dragonfly resting on a bramble stem against a green background" width="2000" height="2000" loading="lazy">
</button>
<button type="button" class="ph-item" aria-label="Enlarge: cumulus clouds building over a lake">
<img src="/images/photography/img_5301.jpg" alt="Cumulus clouds building over a lake, seen from a wooded shoreline" width="2000" height="2000" loading="lazy">
</button>
</div>

<div class="ph-lb" role="dialog" aria-modal="true" aria-label="Enlarged photograph">
<button type="button" class="ph-close" aria-label="Close">&times;</button>
<img src="" alt="">
</div>

<script>
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
    // Drop the source so a large image is not held in memory while closed.
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
  // Clicking the photo itself should not dismiss, only the surrounding backdrop.
  box.addEventListener("click", function (e) { if (e.target !== full) close(); });
  document.addEventListener("keydown", function (e) {
    if (e.key === "Escape" && box.classList.contains("is-open")) close();
  });
})();
</script>
