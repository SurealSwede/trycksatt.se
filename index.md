---
layout: default
title: Sprinklerteknik & hydrauliska beräkningar
---

<section class="hero">
  <div class="container">
    <div class="hero-inner">
      <div class="hero-text">
        <span class="hero-eyebrow">Andreas Surell · Sprinklerteknik</span>
        <h1 class="hero-title">
          Hydraulik för<br>
          <em>sprinklersystem</em>
        </h1>
        <p class="hero-lead">
          Tekniska artiklar, normer och verktyg för sprinklerprojektörer. 
          Grundat i SBF 120 och EN 12845 — skrivet av en praktiker.
        </p>
        <div class="hero-actions">
          <a href="/artiklar/" class="btn btn-primary">Läs artiklar</a>
          <a href="/verktyg/" class="btn btn-secondary">Öppna verktyg</a>
        </div>
      </div>
      <div class="hero-visual">
        <div class="hero-diagram">
          <div>
            <div class="diagram-label">Hazen-Williams</div>
            <div class="diagram-formula">
              P<sub>f</sub> = <span>6.05×10⁵</span> × Q<sup>1.85</sup>
            </div>
          </div>
          <div class="diagram-bars">
            <div class="diagram-bar"></div>
            <div class="diagram-bar"></div>
            <div class="diagram-bar"></div>
            <div class="diagram-bar"></div>
            <div class="diagram-bar"></div>
            <div class="diagram-bar"></div>
          </div>
          <div class="diagram-stat">
            <div>
              <div class="diagram-stat-num">72 m²</div>
              <div class="diagram-stat-unit">Verkningsyta OH1</div>
            </div>
            <div style="text-align:right">
              <div class="diagram-stat-num">5.0</div>
              <div class="diagram-stat-unit">mm/min</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section-artiklar">
  <div class="container">
    <div class="section-header">
      <h2 class="section-title">Senaste artiklar</h2>
      <div class="section-line"></div>
      <a href="/artiklar/" class="section-link">Alla artiklar →</a>
    </div>
    <div class="artiklar-grid">
      {% for post in site.posts limit:3 %}
      <a href="{{ post.url | relative_url }}" class="artikel-card">
        {% if post.kategori %}<span class="artikel-kategori">{{ post.kategori }}</span>{% endif %}
        <h3 class="artikel-title">{{ post.title }}</h3>
        {% if post.ingress %}<p class="artikel-ingress">{{ post.ingress }}</p>{% endif %}
        <div class="artikel-meta">
          <span class="artikel-datum">{{ post.date | date: "%-d %b %Y" }}</span>
          <span class="artikel-arrow">→</span>
        </div>
      </a>
      {% endfor %}
    </div>
  </div>
</section>

<section class="section-verktyg">
  <div class="container">
    <div class="section-header">
      <h2 class="section-title">Hydraulikverktyg</h2>
      <div class="section-line"></div>
    </div>
    <a href="https://surealswede.github.io/Sprinkler-calcs-/" target="_blank" rel="noopener" class="verktyg-card">
      <div>
        <div class="verktyg-badge">● Live-verktyg</div>
        <h3 class="verktyg-title">Hydrauliskt beräkningsverktyg</h3>
        <p class="verktyg-desc">
          Beräkna tryckfall, flödeshastighet och sprinklerhuvudstryck direkt i webbläsaren. 
          Rördata hämtas live från Google Sheets. Byggt för SBF 120 och EN 12845.
        </p>
        <div class="verktyg-tags">
          <span class="verktyg-tag">Hazen-Williams</span>
          <span class="verktyg-tag">SBF 120</span>
          <span class="verktyg-tag">EN 12845</span>
          <span class="verktyg-tag">Tryckfall</span>
          <span class="verktyg-tag">Q = k√p</span>
        </div>
      </div>
      <div>
        <span class="btn btn-primary">Öppna verktyget →</span>
      </div>
    </a>
  </div>
</section>

<section class="section-om-strip">
  <div class="container">
    <div class="om-strip-inner">
      <div class="om-avatar">A</div>
      <div class="om-text">
        <p>
          <strong>Andreas Surell</strong> är brandskyddsingenjör med specialisering inom sprinklerteknik. 
          Trycksatt.se är ett kunskapsprojekt — ingen reklam, inga konsulttjänster, bara teknik.
        </p>
      </div>
      <div class="om-cta">
        <a href="/om/" class="btn btn-secondary">Om Andreas →</a>
      </div>
    </div>
  </div>
</section>
