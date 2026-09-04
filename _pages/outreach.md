---
layout: archive
title: "Outreach"
permalink: /outreach/
author_profile: true
---

<style>
.ot {
  margin: 1.4em 0 0;
  --ot-write: #2e7d5b;   --ot-write-bg: #e4f1ea;
  --ot-quote: #2a7793;   --ot-quote-bg: #e0eef4;
  --ot-tv: #a4671a;      --ot-tv-bg: #f6ecdb;
  --ot-talk: #6b5aa6;    --ot-talk-bg: #ece9f5;
  --ot-hover: #f2f5f6;
  --ot-chip-bg: #eceff1;
}
html[data-theme="dark"] .ot {
  --ot-write: #6fce9f;   --ot-write-bg: rgba(111, 206, 159, .15);
  --ot-quote: #5cc6e4;   --ot-quote-bg: rgba(92, 198, 228, .15);
  --ot-tv: #e0a765;      --ot-tv-bg: rgba(224, 167, 101, .16);
  --ot-talk: #b3a6e8;    --ot-talk-bg: rgba(179, 166, 232, .16);
  --ot-hover: rgba(255, 255, 255, .06);
  --ot-chip-bg: rgba(255, 255, 255, .08);
}
.ot-kicker {
  display: flex;
  align-items: center;
  gap: .85em;
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  font-size: .72rem;
  font-weight: 700;
  letter-spacing: .14em;
  text-transform: uppercase;
  color: var(--global-text-color-light);
  margin: 0 0 1.1em;
}
.ot-kicker::after {
  content: "";
  flex: 1;
  height: 1px;
  background: var(--global-border-color);
}
.ot-kicker-arc { margin-top: 2.6em; }
.ot-badge {
  display: inline-block;
  font-family: ui-monospace, Menlo, Consolas, monospace;
  font-size: .6rem;
  font-weight: 700;
  letter-spacing: .07em;
  text-transform: uppercase;
  padding: 3px 7px;
  border-radius: 5px;
  margin-left: 7px;
  vertical-align: 2px;
  white-space: nowrap;
}
.ot-badge.is-write { color: var(--ot-write); background: var(--ot-write-bg); }
.ot-badge.is-quote { color: var(--ot-quote); background: var(--ot-quote-bg); }
.ot-badge.is-tv { color: var(--ot-tv); background: var(--ot-tv-bg); }
.ot-badge.is-talk { color: var(--ot-talk); background: var(--ot-talk-bg); }
.ot-badge.is-lang,
.ot-badge.is-event { color: var(--global-text-color-light); background: var(--ot-chip-bg); }
.ot-card {
  display: grid;
  grid-template-columns: minmax(0, .92fr) minmax(0, 1.18fr);
  border: 1px solid var(--global-border-color);
  border-radius: 13px;
  overflow: hidden;
  margin: 0 0 12px;
  background: var(--ot-hover);
  transition: border-color .15s ease;
}
.ot-card:hover { border-color: var(--global-link-color); }
.ot-card-img { position: relative; min-height: 210px; background: #000; }
.ot-card-img img { width: 100%; height: 100%; object-fit: cover; object-position: left center; display: block; }
.ot-card-body {
  padding: 22px 24px 24px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.ot-card-kick {
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  font-size: .64rem;
  font-weight: 700;
  letter-spacing: .12em;
  text-transform: uppercase;
  color: var(--global-link-color);
  margin: 0 0 9px;
}
.ot-card-title {
  font-size: 1.34rem;
  font-weight: 700;
  line-height: 1.26;
  letter-spacing: -.012em;
  margin: 0 0 9px;
}
.ot-card-title a { color: var(--global-text-color); text-decoration: none; transition: color .15s ease; }
.ot-card:hover .ot-card-title a { color: var(--global-link-color); }
.ot-card-title a:focus-visible { outline: 2px solid var(--global-link-color); outline-offset: 3px; border-radius: 3px; }
.ot-card-dek {
  font-size: .95rem;
  line-height: 1.58;
  color: var(--global-text-color);
  margin: 0 0 12px;
}
.ot-card-meta {
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  font-size: .69rem;
  color: var(--global-text-color-light);
}
.ot-pair {
  display: flex;
  gap: 10px;
  align-items: flex-start;
  font-size: .87rem;
  line-height: 1.55;
  color: var(--global-text-color-light);
  background: var(--ot-hover);
  border-left: 2px solid var(--global-link-color);
  border-radius: 0 8px 8px 0;
  padding: 12px 16px;
  margin: 0;
}
.ot-pair b { color: var(--global-text-color); font-weight: 600; }
.ot-pair a { color: var(--global-link-color); text-decoration: none; }
.ot-pair a:hover { text-decoration: underline; }
.ot-item {
  display: grid;
  grid-template-columns: 108px 1fr;
  gap: 18px;
  padding: 16px 12px;
  border-top: 1px solid var(--global-border-color);
  border-left: 2px solid transparent;
  border-radius: 8px;
  transition: background .15s ease, border-color .15s ease;
}
.ot-item:hover { background: var(--ot-hover); border-left-color: var(--global-link-color); }
.ot-meta {
  font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace;
  font-size: .7rem;
  line-height: 1.55;
  color: var(--global-text-color-light);
  font-variant-numeric: tabular-nums;
  padding-top: 2px;
}
.ot-meta b { display: block; color: var(--global-text-color); font-weight: 700; }
.ot-title { font-size: .99rem; font-weight: 700; line-height: 1.4; margin: 0 0 4px; }
.ot-title a { color: var(--global-text-color); text-decoration: none; transition: color .15s ease; }
.ot-item:hover .ot-title a { color: var(--global-link-color); }
.ot-title a:focus-visible { outline: 2px solid var(--global-link-color); outline-offset: 3px; border-radius: 3px; }
.ot-desc {
  font-size: .87rem;
  line-height: 1.55;
  color: var(--global-text-color-light);
  margin: 0;
  max-width: 44em;
}
.ot-video {
  position: relative;
  width: 100%;
  max-width: 520px;
  aspect-ratio: 16 / 9;
  margin: 13px 0 0;
  border-radius: 10px;
  overflow: hidden;
  background: #000;
}
.ot-video iframe { width: 100%; height: 100%; border: 0; display: block; }
.ot-play {
  display: block;
  width: 100%;
  height: 100%;
  padding: 0;
  border: 0;
  background: none;
  cursor: pointer;
}
.ot-play img { width: 100%; height: 100%; object-fit: cover; display: block; }
.ot-play::after {
  content: "";
  position: absolute;
  top: 50%;
  left: 50%;
  width: 62px;
  height: 44px;
  transform: translate(-50%, -50%);
  border-radius: 11px;
  background: rgba(22, 22, 22, .78) url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%23fff'%3E%3Cpath d='M8 5v14l11-7z'/%3E%3C/svg%3E") center / 23px no-repeat;
  transition: background-color .15s ease, transform .15s ease;
}
.ot-play:hover::after { background-color: #cc0000; transform: translate(-50%, -50%) scale(1.06); }
.ot-play:focus-visible { outline: 2px solid var(--global-link-color); outline-offset: -2px; }
@media (max-width: 680px) {
  .ot-card { grid-template-columns: 1fr; }
  .ot-card-img { min-height: 170px; }
  .ot-card-body { padding: 18px 18px 20px; }
  .ot-card-title { font-size: 1.2rem; }
  .ot-item { grid-template-columns: 1fr; gap: 6px; padding: 15px 12px; }
  .ot-meta { padding-top: 0; }
  .ot-meta b { display: inline; margin-right: 8px; }
}
@media (prefers-reduced-motion: reduce) {
  .ot * { transition: none !important; }
}
</style>

<div class="ot">
<h2 class="ot-kicker">Latest</h2>
<div class="ot-card">
<div class="ot-card-img"><img src="https://cdn-attachments.timesofmalta.com/9e2c17a9b60b10ba9a334620c74abc8ef683f8e6-1787826572-4c5f8be7-1200x630.jpg" alt="Bathers on a crowded Maltese beach during the summer marine heatwave" loading="lazy" width="1200" height="630"></div>
<div class="ot-card-body">
<p class="ot-card-kick">Op-ed &middot; 30 August 2026</p>
<h3 class="ot-card-title"><a href="https://timesofmalta.com/article/warmer-seas-stronger-storms-science-says.1133290">Warmer seas, stronger storms: what the science actually says</a></h3>
<p class="ot-card-dek">Warmer seas do not predict the next storm &mdash; they raise the odds of stronger ones.</p>
<p class="ot-card-meta">Times of Malta &middot; with James Ciarl&ograve;</p>
</div>
</div>
<p class="ot-pair"><span aria-hidden="true">&#8627;</span><span>Written as a follow-up to <b>&ldquo;Why major autumn storms could be on the horizon&rdquo;</b> (21 August), in which I was <a href="https://timesofmalta.com/article/malta-unusually-warm-seas-fuel-stronger-autumn-storms-experts-say.1133005">interviewed by Matthew Bonanno</a> on the marine heatwave running about 3&deg;C above normal.</span></p>
<h2 class="ot-kicker ot-kicker-arc">Archive</h2>
<article class="ot-item">
<div class="ot-meta"><b>2026</b>21 August<br>Times of Malta</div>
<div class="ot-main">
<h3 class="ot-title"><a href="https://timesofmalta.com/article/malta-unusually-warm-seas-fuel-stronger-autumn-storms-experts-say.1133005">Why major autumn storms could be on the horizon</a><span class="ot-badge is-quote">Interview</span></h3>
<p class="ot-desc">&ldquo;What the warm sea guarantees is the fuel.&rdquo; Interviewed by Matthew Bonanno.</p>
</div>
</article>
<article class="ot-item">
<div class="ot-meta"><b>2026</b>20 January<br>TVM News</div>
<div class="ot-main">
<h3 class="ot-title"><a href="https://tvmnews.mt/news/nistennew-li-dawn-il-maltempati-jkunu-iktar-frekwenti-u-bsahhithom/">&ldquo;Nistennew li dawn il-maltempati jkunu iktar frekwenti u b&rsquo;saħħithom&rdquo;</a><span class="ot-badge is-tv">TV</span><span class="ot-badge is-lang">In Maltese</span></h3>
<p class="ot-desc">On the severity of Storm Harry, and why extreme weather in the central Mediterranean is expected to become more frequent and more intense.</p>
<div class="ot-video" data-yt="v4Tz5YdoFoQ" data-title="TVM News: Storm Harry and extreme weather">
<button type="button" class="ot-play" aria-label="Play the TVM News segment on Storm Harry"><img src="/images/outreach/storm-harry.jpg" alt="" loading="lazy" width="1280" height="720"></button>
</div>
</div>
</article>
<article class="ot-item">
<div class="ot-meta"><b>2025</b>27 July<br>Times of Malta</div>
<div class="ot-main">
<h3 class="ot-title"><a href="https://timesofmalta.com/article/maltese-atmospheric-climate-scientist-attends-lindau-meeting.1113716">Maltese atmospheric and climate scientist attends Lindau meeting</a><span class="ot-badge is-quote">Feature</span></h3>
<p class="ot-desc">The annual Lindau Nobel Laureate Meeting brings together Nobel Prize laureates and young scientists from around the world.</p>
</div>
</article>
<article class="ot-item">
<div class="ot-meta"><b>2024</b>15 August<br>TVM News</div>
<div class="ot-main">
<h3 class="ot-title"><a href="https://tvmnews.mt/news/l-gharajjex-jintensifikaw-fnofs-awwissu-meta-l-wicc-tal-bahar-jilhaq-it-30-grad/">&ldquo;L-għarajjex jintensifikaw f&rsquo;nofs Awwissu, meta l-wiċċ tal-baħar jilħaq it-30 grad&rdquo;</a><span class="ot-badge is-tv">TV</span><span class="ot-badge is-lang">In Maltese</span></h3>
<p class="ot-desc">How Malta&rsquo;s convective summer thunderstorms &mdash; locally known as <em>għarajjex</em> &mdash; form once the sea surface climbs past 30&deg;C.</p>
<div class="ot-video" data-yt="-i5lAr-bag4" data-title="TVM News: how summer għarajjex form">
<button type="button" class="ot-play" aria-label="Play the TVM News segment on summer thunderstorms"><img src="/images/outreach/gharajjex.jpg" alt="" loading="lazy" width="1280" height="720"></button>
</div>
</div>
</article>
<article class="ot-item">
<div class="ot-meta"><b>2020</b>26 November<br>Times of Malta</div>
<div class="ot-main">
<h3 class="ot-title"><a href="https://timesofmalta.com/article/shipping-industrys-heavy-toll-on-the-environment.834511">Shipping industry&rsquo;s heavy toll on the environment</a><span class="ot-badge is-write">Op-ed</span></h3>
<p class="ot-desc">Air pollution from ships is linked to some 40,000 premature deaths worldwide each year, and the industry accounts for around four per cent of anthropogenic greenhouse gas emissions.</p>
</div>
</article>
<h2 class="ot-kicker ot-kicker-arc">Talks &amp; festivals</h2>
<article class="ot-item">
<div class="ot-meta"><b>2026</b>August<br>Zurich</div>
<div class="ot-main">
<h3 class="ot-title"><a href="https://www.scientifica.ch/">Scientifica</a><span class="ot-badge is-event">Festival</span></h3>
<p class="ot-desc">The public science festival of ETH Zurich and the University of Zurich, held across the city over nine days.</p>
</div>
</article>
<article class="ot-item">
<div class="ot-meta"><b>2019</b>September<br>Valletta</div>
<div class="ot-main">
<h3 class="ot-title"><a href="https://www.scienceinthecity.org.mt/">Science in the City</a><span class="ot-badge is-event">Festival</span></h3>
<p class="ot-desc">Malta&rsquo;s national science and arts festival, which takes over the streets of Valletta each autumn.</p>
</div>
</article>
<article class="ot-item">
<div class="ot-meta"><b>2019</b>June<br>Malta</div>
<div class="ot-main">
<h3 class="ot-title">Light pollution in Malta<span class="ot-badge is-talk">Invited talk</span></h3>
<p class="ot-desc">Public talk given at the invitation of <a href="https://www.maltastro.org/">The Astronomical Society of Malta</a>.</p>
</div>
</article>
<article class="ot-item">
<div class="ot-meta"><b>2016</b>September<br>Valletta</div>
<div class="ot-main">
<h3 class="ot-title"><a href="https://www.scienceinthecity.org.mt/">Science in the City</a><span class="ot-badge is-event">Festival</span></h3>
<p class="ot-desc">Malta&rsquo;s national science and arts festival, which takes over the streets of Valletta each autumn.</p>
</div>
</article>
</div>

<script>
(function () {
  document.querySelectorAll(".ot-video").forEach(function (box) {
    box.addEventListener("click", function () {
      var frame = document.createElement("iframe");
      frame.src = "https://www.youtube-nocookie.com/embed/" + box.dataset.yt + "?autoplay=1&rel=0";
      frame.title = box.dataset.title || "Video";
      frame.allow = "accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture";
      frame.allowFullscreen = true;
      box.textContent = "";
      box.appendChild(frame);
    }, { once: true });
  });
})();
</script>
