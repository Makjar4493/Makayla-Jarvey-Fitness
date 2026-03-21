
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Makayla Jarvey | Personal Trainer</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet"/>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

```
:root {
  --cream: #f5f0e8;
  --warm-white: #faf8f4;
  --sand: #e8dfc8;
  --terracotta: #c2714f;
  --terra-light: #d98a68;
  --dark: #1e1a16;
  --mid: #5c4f40;
  --light-text: #9c8b78;
}

html { scroll-behavior: smooth; }

body {
  background-color: var(--warm-white);
  color: var(--dark);
  font-family: 'DM Sans', sans-serif;
  font-weight: 300;
  overflow-x: hidden;
}

/* ── HERO ── */
.hero {
  min-height: 100vh;
  display: grid;
  grid-template-columns: 1fr 1fr;
  position: relative;
  overflow: hidden;
}

.hero-left {
  background-color: var(--dark);
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 80px 60px;
  position: relative;
  z-index: 1;
}

.hero-left::after {
  content: '';
  position: absolute;
  right: -40px;
  top: 0;
  bottom: 0;
  width: 80px;
  background: var(--dark);
  clip-path: polygon(0 0, 0% 100%, 100% 50%);
  z-index: 2;
}

.eyebrow {
  font-family: 'DM Sans', sans-serif;
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: var(--terracotta);
  margin-bottom: 28px;
  opacity: 0;
  animation: fadeUp 0.7s ease forwards 0.2s;
}

.hero-name {
  font-family: 'Playfair Display', serif;
  font-size: clamp(48px, 6vw, 78px);
  line-height: 1.05;
  color: var(--cream);
  margin-bottom: 24px;
  opacity: 0;
  animation: fadeUp 0.7s ease forwards 0.4s;
}

.hero-name em {
  font-style: italic;
  color: var(--terra-light);
}

.hero-tagline {
  font-size: 16px;
  line-height: 1.7;
  color: #a89880;
  max-width: 340px;
  margin-bottom: 48px;
  opacity: 0;
  animation: fadeUp 0.7s ease forwards 0.6s;
}

.hero-cta {
  display: inline-block;
  background: var(--terracotta);
  color: #fff;
  text-decoration: none;
  font-size: 13px;
  font-weight: 500;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  padding: 16px 36px;
  transition: background 0.25s;
  opacity: 0;
  animation: fadeUp 0.7s ease forwards 0.8s;
  align-self: flex-start;
}

.hero-cta:hover { background: var(--terra-light); }

.hero-right {
  background: var(--sand);
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  overflow: hidden;
}

.hero-graphic {
  width: 100%;
  height: 100%;
  position: absolute;
  inset: 0;
}

.initials-ring {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

.initials {
  font-family: 'Playfair Display', serif;
  font-size: 140px;
  font-weight: 700;
  color: rgba(194, 113, 79, 0.15);
  line-height: 1;
  letter-spacing: -4px;
  user-select: none;
}

.circle-deco {
  position: absolute;
  border-radius: 50%;
  border: 1px solid rgba(194,113,79,0.3);
}
.circle-deco.c1 { width: 340px; height: 340px; top: 50%; left: 50%; transform: translate(-50%,-50%); }
.circle-deco.c2 { width: 260px; height: 260px; top: 50%; left: 50%; transform: translate(-50%,-50%); border-style: dashed; }
.circle-deco.c3 { width: 460px; height: 460px; top: 50%; left: 50%; transform: translate(-50%,-50%); opacity: 0.4; }

.badge {
  position: absolute;
  bottom: 60px;
  right: 60px;
  background: var(--terracotta);
  color: #fff;
  width: 110px;
  height: 110px;
  border-radius: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  line-height: 1.2;
  opacity: 0;
  animation: fadeUp 0.7s ease forwards 1s;
}

.badge-num {
  font-family: 'Playfair Display', serif;
  font-size: 32px;
  font-weight: 700;
}

.badge-label {
  font-size: 10px;
  font-weight: 500;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

/* ── ABOUT ── */
.about {
  background: var(--cream);
  padding: 100px 60px;
  display: grid;
  grid-template-columns: 1fr 1.4fr;
  gap: 80px;
  align-items: center;
}

.section-label {
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: var(--terracotta);
  margin-bottom: 20px;
}

.section-title {
  font-family: 'Playfair Display', serif;
  font-size: clamp(32px, 3.5vw, 48px);
  line-height: 1.2;
  color: var(--dark);
  margin-bottom: 28px;
}

.section-title em { font-style: italic; color: var(--terracotta); }

.about-text {
  font-size: 16px;
  line-height: 1.85;
  color: var(--mid);
  margin-bottom: 20px;
}

.about-stats {
  display: flex;
  gap: 40px;
  margin-top: 48px;
  padding-top: 40px;
  border-top: 1px solid var(--sand);
}

.stat-num {
  font-family: 'Playfair Display', serif;
  font-size: 42px;
  color: var(--terracotta);
  line-height: 1;
}

.stat-label {
  font-size: 12px;
  font-weight: 500;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--light-text);
  margin-top: 6px;
}

.about-image-side {
  position: relative;
}

.cert-card {
  background: var(--dark);
  color: var(--cream);
  padding: 48px 44px;
  position: relative;
  overflow: hidden;
}

.cert-card::before {
  content: '';
  position: absolute;
  top: -40px;
  right: -40px;
  width: 160px;
  height: 160px;
  border-radius: 50%;
  background: rgba(194,113,79,0.12);
}

.cert-card-label {
  font-size: 10px;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: var(--terracotta);
  margin-bottom: 16px;
}

.cert-name {
  font-family: 'Playfair Display', serif;
  font-size: 28px;
  margin-bottom: 8px;
}

.cert-sub {
  font-size: 13px;
  color: #a89880;
  line-height: 1.6;
}

.location-tag {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  margin-top: 32px;
  padding: 10px 18px;
  border: 1px solid rgba(255,255,255,0.12);
  font-size: 12px;
  color: #a89880;
  letter-spacing: 0.05em;
}

.dot { width: 6px; height: 6px; border-radius: 50%; background: var(--terracotta); flex-shrink: 0; }

/* ── SPECIALTIES ── */
.specialties {
  background: var(--warm-white);
  padding: 100px 60px;
}

.specialties-header {
  text-align: center;
  margin-bottom: 64px;
}

.cards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2px;
}

.card {
  background: var(--cream);
  padding: 48px 40px;
  position: relative;
  overflow: hidden;
  transition: background 0.3s;
}

.card:hover { background: var(--sand); }

.card-icon {
  font-size: 36px;
  margin-bottom: 24px;
  display: block;
}

.card-title {
  font-family: 'Playfair Display', serif;
  font-size: 22px;
  margin-bottom: 14px;
  color: var(--dark);
}

.card-desc {
  font-size: 14px;
  line-height: 1.75;
  color: var(--mid);
}

.card-num {
  position: absolute;
  top: 24px;
  right: 28px;
  font-family: 'Playfair Display', serif;
  font-size: 56px;
  font-weight: 700;
  color: rgba(194,113,79,0.08);
  line-height: 1;
  user-select: none;
}

/* ── CONTACT ── */
.contact {
  background: var(--dark);
  padding: 100px 60px;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 80px;
  align-items: center;
}

.contact-title {
  font-family: 'Playfair Display', serif;
  font-size: clamp(36px, 4vw, 56px);
  color: var(--cream);
  line-height: 1.15;
  margin-bottom: 20px;
}

.contact-title em { font-style: italic; color: var(--terra-light); }

.contact-sub {
  font-size: 15px;
  color: #a89880;
  line-height: 1.75;
}

.contact-items {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.contact-item {
  display: flex;
  align-items: center;
  gap: 20px;
  padding: 24px 28px;
  border: 1px solid rgba(255,255,255,0.08);
  text-decoration: none;
  color: var(--cream);
  transition: border-color 0.25s, background 0.25s;
}

.contact-item:hover {
  border-color: var(--terracotta);
  background: rgba(194,113,79,0.06);
}

.contact-icon {
  width: 44px;
  height: 44px;
  border-radius: 50%;
  background: rgba(194,113,79,0.15);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 18px;
  flex-shrink: 0;
}

.contact-item-label {
  font-size: 10px;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--terracotta);
  margin-bottom: 4px;
}

.contact-item-val {
  font-size: 14px;
  color: #d0c4b4;
}

/* ── FOOTER ── */
footer {
  background: #13100c;
  padding: 28px 60px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.footer-name {
  font-family: 'Playfair Display', serif;
  font-size: 18px;
  color: var(--cream);
}

.footer-copy {
  font-size: 12px;
  color: #6b5e50;
}

/* ── ANIMATIONS ── */
@keyframes fadeUp {
  from { opacity: 0; transform: translateY(24px); }
  to   { opacity: 1; transform: translateY(0); }
}

/* ── RESPONSIVE ── */
@media (max-width: 768px) {
  .hero { grid-template-columns: 1fr; min-height: auto; }
  .hero-left { padding: 60px 32px; }
  .hero-left::after { display: none; }
  .hero-right { min-height: 300px; }
  .about { grid-template-columns: 1fr; padding: 64px 32px; gap: 48px; }
  .specialties { padding: 64px 32px; }
  .cards { grid-template-columns: 1fr; }
  .contact { grid-template-columns: 1fr; padding: 64px 32px; gap: 48px; }
  footer { flex-direction: column; gap: 8px; padding: 24px 32px; text-align: center; }
  .about-stats { gap: 24px; }
}
```

  </style>
</head>
<body>

  <!-- HERO -->

  <section class="hero">
    <div class="hero-left">
      <p class="eyebrow">NASM Certified Personal Trainer</p>
      <h1 class="hero-name">Makayla<br><em>Jarvey</em></h1>
      <p class="hero-tagline">Helping busy moms move, lift, and feel strong & empowered on their schedule, in their space.</p>
      <a href="mailto:Makaylajarvey@u.boisestate.edu" class="hero-cta">Work with me</a>
    </div>
    <div class="hero-right">
      <div class="circle-deco c3"></div>
      <div class="circle-deco c1"></div>
      <div class="circle-deco c2"></div>
      <div class="initials-ring">
        <div class="initials">MJ</div>
      </div>
      <div class="badge">
        <span class="badge-num">3</span>
        <span class="badge-label">Years Training</span>
      </div>
    </div>
  </section>

  <!-- ABOUT -->

  <section class="about">
    <div>
      <p class="section-label">About Me</p>
      <h2 class="section-title">Fitness that fits <em>your life</em></h2>
      <p class="about-text">I'm a NASM-certified personal trainer based in Meridian, Idaho, specializing in online and home-based coaching. My clients are busy moms who want real results without having to rearrange their whole day around a gym.</p>
      <p class="about-text">Whether you're brand new to lifting or want to kick your cardio up a notch, I build programs around what actually works for your body and your schedule.</p>
      <div class="about-stats">
        <div>
          <div class="stat-num">3+</div>
          <div class="stat-label">Years Experience</div>
        </div>
        <div>
          <div class="stat-num">100%</div>
          <div class="stat-label">Online & Home-Based</div>
        </div>
        <div>
          <div class="stat-num">1:1</div>
          <div class="stat-label">Personalized Coaching</div>
        </div>
      </div>
    </div>
    <div class="about-image-side">
      <div class="cert-card">
        <p class="cert-card-label">Certification</p>
        <p class="cert-name">NASM Certified<br>Personal Trainer</p>
        <p class="cert-sub">National Academy of Sports Medicine<br>Active & Practicing — Online + Home Gym</p>
        <div class="location-tag">
          <span class="dot"></span>
          Meridian, Idaho · Available Nationwide Online
        </div>
      </div>
    </div>
  </section>

  <!-- SPECIALTIES -->

  <section class="specialties">
    <div class="specialties-header">
      <p class="section-label">What I Offer</p>
      <h2 class="section-title">Training built <em>for you</em></h2>
    </div>
    <div class="cards">
      <div class="card">
        <span class="card-num">01</span>
        <span class="card-icon">🏋️‍♀️</span>
        <h3 class="card-title">Strength & Lifting</h3>
        <p class="card-desc">Progressive strength programs designed to build confidence and capability — no barbell experience required. We start where you are.</p>
      </div>
      <div class="card">
        <span class="card-num">02</span>
        <span class="card-icon">🔥</span>
        <h3 class="card-title">HIIT & Cardio</h3>
        <p class="card-desc">High-energy cardio sessions that get results in less time. Perfect for moms who need maximum impact in a short window.</p>
      </div>
      <div class="card">
        <span class="card-num">03</span>
        <span class="card-icon">📱</span>
        <h3 class="card-title">Online Coaching</h3>
        <p class="card-desc">Fully remote, fully personalized. Train at home, at the park, wherever life takes you — I'll be with you every step of the way.</p>
      </div>
    </div>
  </section>

  <!-- CONTACT -->

  <section class="contact">
    <div>
      <h2 class="contact-title">Ready to get <em>started?</em></h2>
      <p class="contact-sub">Sessions are booked directly through me — no third-party apps. Just reach out and we'll find a time that works for your life.</p>
    </div>
    <div class="contact-items">
      <a href="mailto:Makaylajarvey@u.boisestate.edu" class="contact-item">
        <div class="contact-icon">✉️</div>
        <div>
          <div class="contact-item-label">Email</div>
          <div class="contact-item-val">Makaylajarvey@u.boisestate.edu</div>
        </div>
      </a>
      <div class="contact-item">
        <div class="contact-icon">📍</div>
        <div>
          <div class="contact-item-label">Location</div>
          <div class="contact-item-val">Meridian, Idaho · Online Nationwide</div>
        </div>
      </div>
      <div class="contact-item">
        <div class="contact-icon">📅</div>
        <div>
          <div class="contact-item-label">Booking</div>
          <div class="contact-item-val">Reach out via email to schedule</div>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->

  <footer>
    <span class="footer-name">Makayla Jarvey</span>
    <span class="footer-copy">NASM Certified Personal Trainer · Meridian, Idaho</span>
  </footer>

</body>
</html>
