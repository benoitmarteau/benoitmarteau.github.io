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
        4th-year <strong>Ph.D. student</strong> in <strong>Electrical &amp; Computer Engineering</strong> at <strong>Georgia Tech</strong>,
        working at the intersection of <strong>Biomedical AI</strong>, <strong>XR</strong>, and <strong>trustworthy data</strong>.
      </p>
    </div>
    <div class="hero-image">
      <!-- Replace assets/img/profile.jpg with your own photo using the same filename -->
      <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Profile photo of Benoit L. Marteau">
    </div>
  </div>

  <!-- Social Links and Resume Download moved to hero section -->
  <div class="container">
    <ul class="hero-social-links">
      {% for item in site.data.social %}
        <li class="social-link-item">
          <a href="{{ item.url }}" target="_blank" rel="noopener noreferrer">
            <i class="{{ item.icon }}" aria-hidden="true"></i>
            <span class="social-name">{{ item.name }}</span>
          </a>
        </li>
      {% endfor %}
      <li class="social-link-item">
        <a href="{{ '/assets/Resume_Marteau_Benoit_2025_01_25.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer" class="resume-download">
          <i class="fa fa-file-pdf-o" aria-hidden="true"></i>
          <span class="social-name">Resume (PDF)</span>
        </a>
      </li>
    </ul>
  </div>
</section>

<section id="about" class="section section-alt">
  <div class="container">
    <h2>About</h2>
    <p>
      I am a 4<sup>th</sup>-year <strong>Ph.D. student</strong> in <strong>Electrical &amp; Computer Engineering</strong> at <strong>Georgia Tech</strong> and a member of the
      <strong>Bio-MIBLab</strong>, advised by <strong>Dr. May D. Wang</strong>. I completed a <strong>Diplôme d'Ingénieur</strong> from <strong>Arts et Métiers ParisTech</strong> in 2020
      and an <strong>M.S. in Electrical &amp; Computer Engineering</strong> at Georgia Tech in 2019 (recipient of the <strong>ECE-Coulter Shenzhen M.S. Fellowship</strong>) before continuing into my doctoral studies.
    </p>
    <p>
      My research focuses on <strong>Artificial Intelligence (AI) Implementation Science</strong> within healthcare, <strong>medical data harmonization</strong>, <strong>eXtended Reality (XR)</strong>,
      <strong>digital signal processing</strong>, and <strong>clinical decision support systems</strong>. I have expertise in developing AI-based clinical systems using
      <strong>Generative AI</strong> for medical imaging, <strong>multimodal data harmonization</strong>,
      and <strong>Digital Twin (DT)</strong> technologies for healthcare applications.
    </p>
    <p>
      As <strong>Lab Manager</strong>, I manage a laboratory with over 50 graduate and undergraduate students, coordinate lab computational infrastructure including Azure cloud environments. I also co-led the
      organization of a symposium on Safe, Trustworthy, Actionable, and Responsible AI in healthcare.
    </p>
    <p>
      I successfully completed the <strong>TI:GER (Technology Innovation: Generating Economic Results) Program</strong>, a 3-semester entrepreneurship program at Georgia Tech,
      where I explored translating research into impactful technologies. During this program, I shadowed GATE Space startup and performed regulatory framework analysis.
    </p>
    <p>
      In my free time, I enjoy <strong>astrophysics</strong>, <strong>aerospace</strong>, <strong>model trains</strong>, <strong>space exploration</strong>, and playing <strong>piano</strong>.
      I am fluent in both <strong>English</strong> and <strong>French</strong> (native).
    </p>
  </div>
</section>

<section id="interests" class="section">
  <div class="container">
    <h2>Interests</h2>
    <div class="chips">
      <span class="chip">AI Implementation Science</span>
      <span class="chip">XR/Digital Twins</span>
      <span class="chip">Medical Data Harmonization</span>
      <span class="chip">Computer Vision</span>
      <span class="chip">Biomedical AI</span>
      <span class="chip">Generative Models (GANs, Diffusion)</span>
      <span class="chip">Clinical Decision Support</span>
      <span class="chip">Trustworthy AI</span>
      <span class="chip">Astrophysics</span>
      <span class="chip">Aerospace</span>
      <span class="chip">Model Trains</span>
      <span class="chip">Piano</span>
    </div>
  </div>
</section>

<section id="publications" class="section section-alt">
  <div class="container">
    <h2>Publications</h2>

    {% if site.data.publications and site.data.publications | size > 0 %}
      {% assign current_year = "" %}
      {% for pub in site.data.publications %}
        {% assign pub_year = pub.year | default: "Unknown" | append: "" %}
        {% if pub_year != current_year %}
          {% if current_year != "" %}
            </ul>
          {% endif %}
          <h3 class="publication-year-header">{{ pub_year }}</h3>
          <ul class="publication-list">
          {% assign current_year = pub_year %}
        {% endif %}
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
          </div>
        </li>
      {% endfor %}
      </ul>
    {% else %}
      <p>No publications listed yet. Coming soon. I will add my publications here.</p>
    {% endif %}
  </div>
</section>

