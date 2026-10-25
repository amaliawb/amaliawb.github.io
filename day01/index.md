
---
layout: default
title: About Me
---

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@500;600;700&display=swap');

:root {
  --forest: #23483b;
  --sage: #dce8dc;
  --cream: #faf9f5;
  --ink: #29352f;
  --muted: #69776d;
  --accent: #4f8582;
}

.about-page {
  max-width: 1000px;
  margin: 0 auto;
  padding: 30px 22px 70px;
  color: var(--ink);
  font-family: 'DM Sans', sans-serif;
  line-height: 1.8;
}

.about-page * {
  box-sizing: border-box;
}

.about-page h1,
.about-page h2,
.about-page h3 {
  font-family: 'Playfair Display', Georgia, serif;
  color: var(--forest);
  line-height: 1.25;
}

.about-page h1 {
  font-size: clamp(2.5rem, 6vw, 4.1rem);
  margin: 12px 0 18px;
  letter-spacing: -1.5px;
}

.about-page h2 {
  font-size: 2rem;
  margin: 0 0 18px;
}

.about-page p {
  color: var(--muted);
}

.about-page a {
  color: var(--forest);
  text-decoration-thickness: 1px;
  text-underline-offset: 4px;
}

.about-page a:hover {
  color: var(--accent);
}

.hero {
  display: grid;
  grid-template-columns: 1.4fr 0.8fr;
  align-items: center;
  gap: 45px;
  padding: 35px 0 60px;
}

.eyebrow {
  display: inline-block;
  color: var(--forest);
  background: var(--sage);
  border-radius: 30px;
  padding: 5px 14px;
  font-size: 0.8rem;
  font-weight: 700;
  letter-spacing: 1px;
  text-transform: uppercase;
}

.hero .intro {
  font-size: 1.1rem;
  max-width: 550px;
}

.hero .subtitle {
  color: var(--accent);
  font-weight: 600;
  font-size: 1.05rem;
}

.profile-photo {
  width: 100%;
  max-width: 340px;
  aspect-ratio: 4 / 5;
  object-fit: cover;
  border-radius: 18px;
  display: block;
  margin: 0 auto;
  background: var(--sage);
  box-shadow: 15px 15px 0 var(--sage);
}

.buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 25px;
}

.button {
  display: inline-block;
  padding: 10px 19px;
  border: 1px solid var(--forest);
  border-radius: 8px;
  text-decoration: none !important;
  font-weight: 600;
  transition: transform 0.2s, background 0.2s;
}

.button:hover {
  transform: translateY(-2px);
}

.button.primary {
  color: white !important;
  background: var(--forest);
}

.button.secondary {
  background: transparent;
}

.section {
  padding: 45px 0;
  border-top: 1px solid #e4e8e0;
}

.section-label {
  color: var(--accent) !important;
  font-size: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 2px;
  font-weight: 700;
  margin-bottom: 10px;
}

.cards {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 18px;
  margin-top: 25px;
}

.info-card {
  background: var(--cream);
  border: 1px solid #e5e9e1;
  border-radius: 14px;
  padding: 23px;
}

.info-card .icon {
  font-size: 1.7rem;
}

.info-card h3 {
  font-size: 1.25rem;
  margin: 12px 0 8px;
}

.info-card p {
  font-size: 0.95rem;
  margin-bottom: 0;
}

.timeline {
  border-left: 2px solid var(--sage);
  padding-left: 25px;
  margin: 25px 0 0 8px;
}

.timeline-item {
  position: relative;
  padding: 0 0 27px;
}

.timeline-item:last-child {
  padding-bottom: 0;
}

.timeline-item::before {
  content: '';
  position: absolute;
  left: -32px;
  top: 9px;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: var(--accent);
  border: 3px solid white;
  box-shadow: 0 0 0 1px var(--accent);
}

.timeline-item h3 {
  font-size: 1.2rem;
  margin: 0 0 4px;
}

.timeline-item p {
  margin: 0;
}

.quote {
  background: var(--sage);
  border-radius: 16px;
  padding: 30px;
  margin: 10px 0 40px;
}

.quote p {
  color: var(--forest);
  font-family: 'Playfair Display', Georgia, serif;
  font-size: 1.35rem;
  margin: 0;
}

.footer {
  text-align: center;
  border-top: 1px solid #e4e8e0;
  padding-top: 30px;
}

.footer p {
  font-size: 0.9rem;
}

@media (max-width: 700px) {
  .about-page {
    padding: 15px 8px 45px;
  }

  .hero {
    grid-template-columns: 1fr;
    gap: 30px;
    padding-top: 20px;
  }

  .hero-copy {
    order: 1;
  }

  .hero-image {
    order: 0;
    max-width: 300px;
  }

  .cards {
    grid-template-columns: 1fr;
  }

  .section {
    padding: 35px 0;
  }
}
</style>

<div class="about-page">

  <section class="hero">
    <div class="hero-copy">
      <span class="eyebrow">About me</span>
      <h1>Hi, I'm Amalia<span style="color: var(--accent);">.</span> 👋</h1>
      <p class="subtitle">Life Sciences MSc Student · Weizmann Institute of Science</p>

      <p class="intro">
        I'm a biology student with a growing interest in computational
        approaches to understanding life. I'm fascinated by the complexity
        of cells, the interactions between molecules, and the ways research
        can help us uncover how biological systems work.
      </p>

      <div class="buttons">
        <a class="button primary"
           href="https://github.com/amaliawb"
           target="_blank" rel="noopener noreferrer">
          Explore my GitHub ↗
        </a>
        <a class="button secondary" href="#background">
          My background ↓
        </a>
      </div>
    </div>

    <div class="hero-image">
      <img class="profile-photo"
           src="{{ '/Python.jpg' | relative_url }}"
           alt="Python programming">
    </div>
  </section>

  <section class="section">
    <p class="section-label">What drives me</p>
    <h2>A little about my interests</h2>

    <div class="cards">
      <div class="info-card">
        <span class="icon">🧬</span>
        <h3>Molecular biology</h3>
        <p>
          I'm fascinated by how cells work, how molecules interact,
          and how tiny processes shape living systems.
        </p>
      </div>

      <div class="info-card">
        <span class="icon">📚</span>
        <h3>Books & reading</h3>
        <p>
          I enjoy reading, discovering new ideas, and learning
          about the world from different perspectives.
        </p>
      </div>

      <div class="info-card">
        <span class="icon">🌊</span>
        <h3>The beach & ocean</h3>
        <p>
          I love going to the beach, enjoying the sea, the sound
          of the waves, and spending time by the water.
        </p>
      </div>
    </div>
  </section>

  <section class="section" id="background">
    <p class="section-label">My journey</p>
    <h2>Education & research</h2>

    <div class="timeline">
      <div class="timeline-item">
        <h3>MSc in Life Sciences</h3>
        <p>
          <strong>Weizmann Institute of Science</strong><br>
          Continuing my scientific journey and developing my research skills.
        </p>
      </div>

      <div class="timeline-item">
        <h3>BSc in Life Sciences</h3>
        <p>
          <strong>The Hebrew University of Jerusalem</strong><br>
          Building a foundation in biology and exploring the molecular
          basis of cellular processes.
        </p>
      </div>

      <div class="timeline-item">
        <h3>Undergraduate research</h3>
        <p>
          Investigated interactions between chaperones and their cofactors
          in yeast, exploring molecular relationships that contribute
          to cellular function.
        </p>
      </div>
    </div>
  </section>

  <section class="quote">
    <p>
      "The most interesting questions often emerge when we look at
      familiar biological systems from a new perspective."
    </p>
  </section>

  <section class="section">
    <p class="section-label">Currently exploring</p>
    <h2>Biology meets code 💻</h2>
    <p>
      I'm building my computational skills alongside my background
      in biology. I'm currently taking a Python with AI course to
      learn how programming can help me explore data, solve problems,
      and approach scientific questions in new ways.
    </p>
    <p>
      This website is where I'll publish my Python assignments,
      projects, and things I learn along the way.
    </p>
  </section>

  <section class="footer">
    <h2>Let's connect!</h2>
    <p>Find me on GitHub.</p>

    <div class="buttons" style="justify-content: center;">
      <a class="button primary"
         href="https://github.com/amaliawb"
         target="_blank" rel="noopener noreferrer">
        GitHub profile ↗
      </a>
    </div>

    <p style="margin-top: 30px;">
      Made with curiosity and a love for science 🧬
    </p>
  </section>

</div>
