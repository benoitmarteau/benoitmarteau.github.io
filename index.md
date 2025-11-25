---
layout: default
title: "Benoit L. Marteau"
---

<a id="top"></a>

<section class="hero">
  <div class="container hero-content">
    <div class="hero-text">
      <h1 class="hero-name">Benoit L. Marteau</h1>
      <p class="hero-tagline">
        4th-year Ph.D. student in Electrical &amp; Computer Engineering at Georgia Tech,
        working at the intersection of biomedical AI, XR, and trustworthy data.
      </p>
    </div>
    <div class="hero-image">
      <!-- Replace assets/img/profile.jpg with your own photo using the same filename -->
      <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Profile photo of Benoit L. Marteau">
    </div>
  </div>
</section>

<section id="about" class="section section-alt">
  <div class="container">
    <h2>About</h2>
    <p>
      I am a 4th-year Ph.D. student in Electrical &amp; Computer Engineering at Georgia Tech and a member of the
      Bio-MIBLab, advised by Dr. May D. Wang. I completed a Diplôme d’Ingénieur from Arts et Métiers ParisTech in 2019
      and an M.S. in Electrical &amp; Computer Engineering at Georgia Tech before continuing into my doctoral studies.
      My work focuses on biomedical AI and data-driven systems for healthcare.
    </p>
    <p>
      I have a strong interest in entrepreneurship and participated in the TI:GER program at Georgia Tech, where I
      explored how to translate research into impactful technologies and ventures.
    </p>
    <p>
      I enjoy exploring AI, XR, technology, computer vision, biomedical AI, data harmonization, and trustworthy AI and
      data systems &mdash; and I also love space and playing piano in my free time.
    </p>
  </div>
</section>

<section id="interests" class="section">
  <div class="container">
    <h2>Interests</h2>
    <div class="chips">
      <span class="chip">AI</span>
      <span class="chip">XR</span>
      <span class="chip">Technology</span>
      <span class="chip">Computer vision</span>
      <span class="chip">Biomedical AI</span>
      <span class="chip">Data harmonization</span>
      <span class="chip">Trustworthy AI and data</span>
      <span class="chip">Space</span>
      <span class="chip">Music (piano)</span>
    </div>
  </div>
</section>

<section id="publications" class="section section-alt">
  <div class="container">
    <h2>Publications</h2>

    {% if site.data.publications and site.data.publications | size > 0 %}
      <ul class="publication-list">
        {% for pub in site.data.publications %}
          <li class="publication-item">
            <div class="publication-title">
              {% if pub.link %}
                <a href="{{ pub.link }}" target="_blank" rel="noopener noreferrer">{{ pub.title }}</a>
              {% else %}
                {{ pub.title }}
              {% endif %}
            </div>
            <div class="publication-meta">
              {% if pub.authors %}<span class="pub-authors">{{ pub.authors }}</span>{% endif %}
              {% if pub.venue %}<span class="pub-venue">{{ pub.venue }}</span>{% endif %}
              {% if pub.year %}<span class="pub-year">{{ pub.year }}</span>{% endif %}
            </div>
          </li>
        {% endfor %}
      </ul>
    {% else %}
      <p>No publications listed yet. Coming soon. I will add my publications here.</p>
    {% endif %}
  </div>
</section>

<section id="links" class="section">
  <div class="container">
    <h2>Links &amp; Contact</h2>
    <p>You can find me on the following platforms:</p>
    <ul class="social-links">
      {% for item in site.data.social %}
        <li class="social-link-item">
          <a href="{{ item.url }}" target="_blank" rel="noopener noreferrer">
            <i class="{{ item.icon }}" aria-hidden="true"></i>
            <span class="social-name">{{ item.name }}</span>
          </a>
        </li>
      {% endfor %}
    </ul>
  </div>
</section>
