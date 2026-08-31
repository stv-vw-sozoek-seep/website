---
editor_options:
  markdown:
    wrap: 72
---

<style>
:root {
  --stv-coral: #f64f60;
  --stv-coral-dark: #d93d4e;
  --stv-ink: #222126;
  --stv-muted: #66616b;
  --stv-paper: #fffafa;
  --stv-line: #eadfe1;
  --stv-shadow: 0 12px 32px rgba(55, 35, 40, 0.09);
}

html {
  scroll-behavior: smooth;
}

.topnav {
  align-items: center;
  background: rgba(255, 255, 255, 0.95);
  border: 1px solid var(--stv-line);
  border-radius: 14px;
  display: flex;
  flex-wrap: wrap;
  gap: 4px;
  margin-bottom: 28px;
  padding: 7px;
  position: sticky;
  top: 12px;
  z-index: 10;
}

.topnav a {
  border-radius: 9px;
  color: var(--stv-ink);
  font-size: 15px;
  font-weight: 600;
  padding: 9px 12px;
  text-decoration: none;
  transition: background 150ms ease, color 150ms ease;
}

.topnav a:hover,
.topnav a:focus {
  background: #fff0f2;
  color: var(--stv-coral-dark);
}

.topnav .instagram-nav {
  background: var(--stv-coral);
  color: white;
  margin-left: auto;
}

.topnav .instagram-nav:hover,
.topnav .instagram-nav:focus {
  background: var(--stv-coral-dark);
  color: white;
}

.topnav .menu-toggle {
  background: transparent;
  border: 0;
  border-radius: 9px;
  color: var(--stv-ink);
  cursor: pointer;
  display: none;
  font-size: 22px;
  margin-left: auto;
  padding: 5px 10px;
}

.hero-panel {
  background:
    radial-gradient(circle at 92% 12%, rgba(246, 79, 96, 0.22), transparent 34%),
    linear-gradient(135deg, #fff7f8 0%, #ffffff 75%);
  border: 1px solid var(--stv-line);
  border-radius: 22px;
  box-shadow: var(--stv-shadow);
  margin-bottom: 42px;
  overflow: hidden;
  padding: 44px 40px;
  position: relative;
}

.eyebrow {
  color: var(--stv-coral-dark);
  font-size: 13px;
  font-weight: 800;
  letter-spacing: 0.09em;
  margin: 0 0 12px;
  text-transform: uppercase;
}

.hero-panel h1 {
  color: var(--stv-ink);
  font-size: clamp(32px, 6vw, 52px);
  letter-spacing: -0.035em;
  line-height: 1.04;
  margin: 0 0 18px;
  max-width: 680px;
}

.hero-panel .lead {
  color: var(--stv-muted);
  font-size: 18px;
  line-height: 1.65;
  margin: 0;
  max-width: 680px;
}

.button-row {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 26px;
}

.stv-button {
  border: 1px solid var(--stv-coral);
  border-radius: 999px;
  display: inline-block;
  font-weight: 700;
  padding: 11px 18px;
  text-decoration: none;
  transition: transform 150ms ease, box-shadow 150ms ease;
}

.stv-button:hover,
.stv-button:focus {
  box-shadow: 0 7px 18px rgba(246, 79, 96, 0.2);
  transform: translateY(-1px);
}

.stv-button.primary {
  background: var(--stv-coral);
  color: white;
}

.stv-button.secondary {
  background: white;
  color: var(--stv-coral-dark);
}

.section-block {
  scroll-margin-top: 90px;
  margin: 52px 0;
}

.section-intro {
  color: var(--stv-muted);
  font-size: 17px;
  line-height: 1.7;
  max-width: 720px;
}

.card-grid {
  display: grid;
  gap: 16px;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  margin-top: 24px;
}

.info-card {
  background: white;
  border: 1px solid var(--stv-line);
  border-radius: 16px;
  padding: 22px;
}

.info-card h3 {
  color: var(--stv-ink);
  font-size: 19px;
  margin: 0 0 8px;
}

.info-card p {
  color: var(--stv-muted);
  line-height: 1.6;
  margin: 0;
}

.instagram-panel {
  align-items: center;
  background: var(--stv-ink);
  border-radius: 20px;
  color: white;
  display: grid;
  gap: 28px;
  grid-template-columns: 1fr auto;
  padding: 30px;
}

.instagram-panel h2 {
  color: white;
  margin: 5px 0 10px;
}

.instagram-panel p {
  color: #ded9df;
  line-height: 1.65;
  margin: 0;
}

.live-label {
  align-items: center;
  color: #ffb9c0;
  display: flex;
  font-size: 13px;
  font-weight: 800;
  gap: 8px;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.live-dot {
  animation: pulse 1.8s infinite;
  background: var(--stv-coral);
  border-radius: 50%;
  height: 9px;
  width: 9px;
}

@keyframes pulse {
  0%, 100% { box-shadow: 0 0 0 0 rgba(246, 79, 96, 0.5); }
  50% { box-shadow: 0 0 0 7px rgba(246, 79, 96, 0); }
}

.instagram-handle {
  background: var(--stv-coral);
  border-radius: 14px;
  color: white;
  display: inline-block;
  font-size: 17px;
  font-weight: 800;
  padding: 15px 19px;
  text-decoration: none;
  white-space: nowrap;
}

.instagram-handle:hover,
.instagram-handle:focus {
  background: white;
  color: var(--stv-coral-dark);
}

.resource-group {
  border-top: 1px solid var(--stv-line);
  padding: 22px 0 8px;
}

.resource-group h3 {
  margin-top: 0;
}

.link-list {
  display: grid;
  gap: 8px;
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.link-list a {
  background: var(--stv-paper);
  border-radius: 10px;
  color: var(--stv-ink);
  padding: 10px 12px;
  text-decoration: none;
}

.link-list a:hover,
.link-list a:focus {
  color: var(--stv-coral-dark);
}

details.archive {
  border: 1px solid var(--stv-line);
  border-radius: 14px;
  margin-top: 14px;
  padding: 14px 17px;
}

details.archive summary {
  color: var(--stv-ink);
  cursor: pointer;
  font-weight: 700;
}

details.archive ul {
  margin-bottom: 4px;
}

.contact-panel {
  background: var(--stv-paper);
  border-left: 4px solid var(--stv-coral);
  border-radius: 0 16px 16px 0;
  padding: 24px 26px;
}

.contact-panel p:last-child {
  margin-bottom: 0;
}

@media screen and (max-width: 720px) {
  .hero-panel {
    padding: 34px 24px;
  }

  .card-grid,
  .link-list,
  .instagram-panel {
    grid-template-columns: 1fr;
  }

  .instagram-handle {
    text-align: center;
  }

  .topnav {
    display: block;
  }

  .topnav .menu-toggle {
    display: block;
    float: right;
  }

  .topnav a {
    display: none;
    margin: 2px 0;
  }

  .topnav.responsive a {
    display: block;
  }

  .topnav.responsive .instagram-nav {
    margin-left: 0;
  }
}
</style>

<script>
function toggleNavigation() {
  var navigation = document.getElementById("site-navigation");
  navigation.classList.toggle("responsive");
}
</script>

<nav class="topnav" id="site-navigation" aria-label="Main navigation">
  <button class="menu-toggle" type="button" onclick="toggleNavigation()"
    aria-label="Open navigation">☰</button>
  <a href="#about">About us</a>
  <a href="#work">What we do</a>
  <a href="#guides">Guides</a>
  <a href="#resources">Resources</a>
  <a href="#contact">Contact</a>
  <a class="instagram-nav" href="https://www.instagram.com/vw.sozoek.seep/"
    target="_blank" rel="noopener">Instagram ↗</a>
</nav>

<div class="hero-panel" id="about">
  <p class="eyebrow">Your student representatives at WU Vienna</p>
  <h1>For Economics, Socioeconomics &amp; SEEP students.</h1>
  <p class="lead">
    We represent your interests, connect the community and help make your
    studies more accessible, inclusive and enjoyable. Come to a plenary,
    share an idea or simply get to know us.
  </p>
  <div class="button-row">
    <a class="stv-button primary" href="https://www.instagram.com/vw.sozoek.seep/"
      target="_blank" rel="noopener">See current updates on Instagram</a>
    <a class="stv-button secondary" href="mailto:stv-vwsozoekseep@wu.ac.at">
      Contact the STV</a>
  </div>
</div>

<section class="section-block" id="work">

## What we do

<p class="section-intro">
  Our work grows out of the questions, ideas and needs of students in the
  three master's programmes. These are some of the ways we support the
  community throughout the academic year.
</p>

<div class="card-grid">
  <div class="info-card">
    <h3>Student representation</h3>
    <p>We bring student perspectives into conversations with programme
    coordinators, departments and university bodies.</p>
  </div>
  <div class="info-card">
    <h3>Open plenaries</h3>
    <p>Our meetings are open to students who want to raise a concern,
    contribute an idea, help with a project or learn how the STV works.</p>
  </div>
  <div class="info-card">
    <h3>Study support</h3>
    <p>We share practical guides, answer questions and organise learning
    opportunities such as R tutorials and other skills-based workshops.</p>
  </div>
  <div class="info-card">
    <h3>Community &amp; connection</h3>
    <p>We create spaces to meet across programmes through semester gatherings,
    informal outings, parties and relaxed events in and around the common room.</p>
  </div>
  <div class="info-card">
    <h3>Inclusive spaces</h3>
    <p>We support initiatives that make university more welcoming, including
    safer learning environments and dedicated formats for FLINTA* students.</p>
  </div>
  <div class="info-card">
    <h3>Ideas from students</h3>
    <p>Have a workshop, event or advocacy idea? We can help develop it, connect
    you with others and explore how the STV can support it.</p>
  </div>
</div>
</section>

<section class="section-block" id="instagram">
  <div class="instagram-panel">
    <div>
      <div class="live-label"><span class="live-dot"></span> Live updates</div>
      <h2>Instagram is our noticeboard</h2>
      <p>Event announcements, plenary details, registrations and other
      time-sensitive information are published on Instagram. Follow the account
      to see the current feed and avoid relying on outdated dates here.</p>
    </div>
    <a class="instagram-handle" href="https://www.instagram.com/vw.sozoek.seep/"
      target="_blank" rel="noopener">@vw.sozoek.seep ↗</a>
  </div>
</section>

<section class="section-block" id="guides">

## Student guides

<p class="section-intro">
  Our guides collect practical information for choosing a programme, applying,
  writing a thesis and navigating everyday student life.
</p>

<div class="resource-group">
  <h3>Choosing a programme</h3>
  <div class="link-list">
    <a href="./guides/Guide_Econ_Introduction.pdf" target="_blank">Economics introduction ↗</a>
    <a href="./guides/Guide_SEEP_Introduction.pdf" target="_blank">SEEP introduction ↗</a>
    <a href="./guides/Guide_SozOek_Overview.pdf" target="_blank">Sozioökonomie introduction ↗</a>
    <a href="./guides/Guide_SozOek_Erfahrungsberichte1.pdf" target="_blank">Sozioökonomie experiences ↗</a>
  </div>
</div>

<div class="resource-group">
  <h3>Applications &amp; theses</h3>
  <div class="link-list">
    <a href="./guides/Guide_Econ_Application.pdf" target="_blank">Economics application ↗</a>
    <a href="./guides/Guide_SEEP_Application.pdf" target="_blank">SEEP application ↗</a>
    <a href="./guides/Guide_Econ_Master_Thesis.pdf" target="_blank">Economics master's thesis ↗</a>
    <a href="./guides/Guide_SEEP_Master_Thesis.pdf" target="_blank">SEEP master's thesis ↗</a>
  </div>
</div>

<div class="resource-group">
  <h3>General study support</h3>
  <div class="link-list">
    <a href="./guides/Guide_Semester_Abroad.pdf" target="_blank">Semester abroad ↗</a>
    <a href="./guides/Guide_Academic_Writing.pdf" target="_blank">Academic writing ↗</a>
    <a href="./guides/Guide_Residence_Permit.pdf" target="_blank">Residence permit ↗</a>
  </div>
</div>
</section>

<section class="section-block" id="resources">

## Community resources

<p class="section-intro">
  Explore publications and reports created by earlier student representatives
  and members of the Economics, Socioeconomics and SEEP community.
</p>

<details class="archive">
  <summary>Standpunkte magazine archive</summary>
  <ul>
    <li><a href="./standpunkte/Standpunkte_18.pdf">Let's talk about Economics — Issue 18</a></li>
    <li><a href="./standpunkte/Standpunkte_17_3_.pdf">Die Ökonomie als Wissenschaft — Issue 17</a></li>
    <li><a href="./standpunkte/Standpunkte16_Final1.pdf">Arbeitsverhältnisse — Issue 16</a></li>
    <li><a href="./standpunkte/Standpunkte15.pdf">Nachhaltigkeit — Issue 15</a></li>
    <li><a href="./standpunkte/Standpunkte_14-Aktuell.pdf">Die verlorene Ausgabe — Issue 14</a></li>
    <li><a href="./standpunkte/Standpunkte13_-_Volldampf_Voraus.pdf">Volldampf voraus! — Issue 13</a></li>
    <li><a href="./standpunkte/standpunkte12_05-2014.pdf">Mit vielen Brillen — Issue 12</a></li>
    <li><a href="./standpunkte/standpunkte11_11-2012.pdf">Was kostet die Welt? — Issue 11</a></li>
    <li><a href="./standpunkte/standpunkte10_02-2012.pdf">Spaziergang um den Tellerrand — Issue 10</a></li>
    <li><a href="./standpunkte/standpunkte9_10-2011.pdf">Backe, Backe Kuchen — Issue 9</a></li>
    <li><a href="./standpunkte/standpunkte8_03-2011.pdf">Schmerzfrei Wachsen — Issue 8</a></li>
    <li><a href="./standpunkte/standpunkte7_06-2010.pdf">Business Needs Banking — Issue 7</a></li>
    <li><a href="./standpunkte/standpunkte6-03-2010.pdf">Bachelor of Multiple Choice — Issue 6</a></li>
    <li><a href="./standpunkte/standpunkte5_01-2009.pdf">Der Turm stürzt ein! — Issue 5</a></li>
    <li><a href="./standpunkte/standpunkte4_06-2008.pdf">Eine Frage der Verteilung — Issue 4</a></li>
    <li><a href="./standpunkte/standpunkte3_03-2008.pdf">Wealth of Nations? — Issue 3</a></li>
    <li><a href="./standpunkte/standpunkte2_11-2007.pdf">Wohin geht die EU? — Issue 2</a></li>
    <li><a href="./standpunkte/standpunkte1_05-2007.pdf">Sind Österreichs Reiche zu arm? — Issue 1</a></li>
  </ul>
</details>

<details class="archive">
  <summary>Reports to the University Representation (ÖH)</summary>
  <ul>
    <li><a href="./uv/uv_bericht_ws_18_19.pdf">STV report — archive A</a></li>
    <li><a href="./uv/1UVWise1920.pdf">STV report — archive B</a></li>
    <li><a href="./uv/2UVWise1920.pdf">STV report — archive C</a></li>
  </ul>
</details>
</section>

<section class="section-block" id="contact">

## Talk to us

<div class="contact-panel">
  <p><strong>Email:</strong>
    <a href="mailto:stv-vwsozoekseep@wu.ac.at">stv-vwsozoekseep [at] wu.ac.at</a>
  </p>
  <p><strong>Instagram:</strong>
    <a href="https://www.instagram.com/vw.sozoek.seep/" target="_blank"
      rel="noopener">@vw.sozoek.seep</a>
  </p>
  <p><strong>On campus:</strong> You can also find us and many of our activities
    around the common room in building D4. Check Instagram for current access,
    meeting and event information.</p>
</div>
</section>
