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
        Last-year <strong>Ph.D. student</strong> in <strong>Electrical &amp; Computer Engineering</strong> at <strong>Georgia Tech</strong>,
        working at the intersection of <strong>Biomedical AI</strong>, <strong>XR</strong>, and <strong>Trustworthy AI &amp; Data</strong>.
      </p>
    </div>
    <div class="hero-image">
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
        <a href="{{ '/assets/Benoit_Marteau_Resume.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer" class="resume-download">
          <i class="fa fa-file-pdf-o" aria-hidden="true"></i>
          <span class="social-name">Resume (PDF)</span>
        </a>
      </li>
    </ul>
  </div>
</section>

<section id="awards" class="section section-alt">
  <div class="container">
    <h2>Awards &amp; Leadership</h2>
    <ul class="awards-list">
      <li><strong>STAR-AI Symposium 2026 Organizing Committee</strong> - Safe, Trustworthy, Actionable, and Responsible AI in Healthcare</li>
      <li><strong>NSF-Google-EMBS Award</strong> - IEEE BHI 2025</li>
      <li><strong>IEEE BHI 2025 Young Professionals Co-Chair</strong> - IEEE International Conference on Biomedical and Health Informatics</li>
      <li><strong>NSF Student Travel Award</strong> - IEEE BHI 2024</li>
      <li><strong>IEEE ICIR 2022 Best Paper Award</strong> - "IDTVR: A Novel Cloud Framework for an Interactive Digital Twin in Virtual Reality"</li>
      <li><strong>ECE-Coulter Shenzhen M.S. Fellowship</strong> - Georgia Tech (2019)</li>
      <li><strong>3rd Place, Dassault UAV Challenge (2017)</strong> - Team lead, Arts et Métiers ParisTech (first team to use deep learning in the competition)</li>
    </ul>
  </div>
</section>

<section id="about" class="section">
  <div class="container">
    <h2>About</h2>
    <p>
      I am a last-year <strong>Ph.D. student</strong> in <strong>Electrical &amp; Computer Engineering</strong> at <strong>Georgia Tech</strong> (expected <strong>2027</strong>),
      advised by <strong>Dr. May D. Wang</strong>. I have served as <strong>Lab Manager</strong> of the <strong>Bio-MIBLab</strong> for three years.
      I hold a <strong>Diplôme d'Ingénieur</strong> from <strong>Arts et Métiers ParisTech</strong> (2016–2020) and an <strong>M.S. in Electrical &amp; Computer Engineering</strong> from <strong>Georgia Tech</strong> (2019) through a double-diploma program.
      I interned at <strong>Cisco</strong> (2020) and worked as a <strong>Research Assistant</strong> in the <strong>Coskun Lab</strong> at Georgia Tech (2021), where I focused on single-cell imaging and AI-driven analysis, before joining Dr. Wang's lab to start my Ph.D. in 2022.
    </p>
    <p>
      My research centers on <strong>Trustworthy AI and Data</strong> in healthcare. I develop methods for <strong>healthcare data quality assessment and improvement</strong>,
      <strong>medical data standardization and harmonization</strong> (including <strong>FHIR</strong> and <strong>OMOP CDM v5.4</strong>), and <strong>agentic AI systems</strong> for multimodal clinical data.
      I also investigate <strong>eXtended Reality (XR)</strong> and <strong>brain digital twin</strong> technologies for clinical applications, as well as <strong>world models</strong> and <strong>representation learning</strong>.
    </p>
    <p>
      As Lab Manager, I oversee a laboratory of over <strong>50 graduate and undergraduate students</strong> and directly mentor <strong>12+ researchers</strong>.
      I coordinate lab computational infrastructure including <strong>Azure cloud environments</strong> and serve on the organizing committees for <strong>IEEE BHI 2025</strong> and the <strong>STAR-AI Symposium 2026</strong>.
    </p>
    <p>
      I have authored <strong>30+ peer-reviewed publications</strong> (9 first/co-first author) and developed <strong>XR applications</strong> using <strong>Unity</strong> with <strong>Meta SDK</strong> for brain visualization and rehabilitation research.
    </p>
    <p>
      I completed the <strong>TI:GER (Technology Innovation: Generating Economic Results) Program</strong>, a three-semester entrepreneurship program at Georgia Tech focused on translating research into impactful technologies.
    </p>
    <p>
      Outside of research, I am passionate about <strong>aerospace</strong>, <strong>robotics</strong>, and <strong>drones</strong>. I led the Arts et Métiers team at the <strong>2017 Dassault UAV Challenge</strong> (3rd place, first team to use deep learning in the competition).
      I also enjoy <strong>model trains</strong>, <strong>space exploration</strong>, and playing <strong>piano</strong>.
      I am fluent in both <strong>English</strong> and <strong>French</strong> (native).
    </p>
  </div>
</section>

<section id="skills" class="section section-alt">
  <div class="container">
    <h2>Technical Skills</h2>
    <div class="skills-grid">
      <div class="skill-category">
        <h3>Languages</h3>
        <div class="chips">
          <span class="chip">Python</span>
          <span class="chip">C#</span>
          <span class="chip">C++</span>
          <span class="chip">SQL</span>
        </div>
      </div>
      <div class="skill-category">
        <h3>AI/ML</h3>
        <div class="chips">
          <span class="chip">PyTorch</span>
          <span class="chip">TensorFlow</span>
          <span class="chip">Hugging Face</span>
          <span class="chip">LLMs</span>
          <span class="chip">Diffusion Models</span>
          <span class="chip">Computer Vision</span>
        </div>
      </div>
      <div class="skill-category">
        <h3>XR Development</h3>
        <div class="chips">
          <span class="chip">Unity</span>
          <span class="chip">Meta SDK</span>
        </div>
      </div>
      <div class="skill-category">
        <h3>Cloud &amp; Data</h3>
        <div class="chips">
          <span class="chip">Azure (IoT Hub, ML, Blob)</span>
          <span class="chip">MS Fabric</span>
          <span class="chip">Docker</span>
          <span class="chip">FHIR</span>
          <span class="chip">OMOP CDM</span>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="interests" class="section">
  <div class="container">
    <h2>Research Interests</h2>
    <div class="chips">
      <span class="chip">Trustworthy AI &amp; Data</span>
      <span class="chip">Healthcare Data Quality</span>
      <span class="chip">Medical Data Harmonization</span>
      <span class="chip">Agentic AI</span>
      <span class="chip">World Models &amp; JEPA</span>
      <span class="chip">Brain Digital Twins</span>
      <span class="chip">Extended Reality in Healthcare</span>
      <span class="chip">Clinical Decision Support</span>
      <span class="chip">Biomedical Imaging</span>
      <span class="chip">Representation Learning</span>
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
            {% if pub.link and pub.link != "" %}
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

