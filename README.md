<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Nurse Etiks Health Hub — Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <meta name="description" content="Nurse Etiks Health Hub — Professional nursing portfolio and health services." />
  <style>
    :root{
      --accent: #0066cc;
      --dark: #0f1724;
      --muted: #6b7280;
      --card: #ffffff;
      --glass: rgba(255,255,255,0.06);
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      background:linear-gradient(180deg,#f7fbff 0%, #f3f8ff 40%);
      color:var(--dark);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
    }

    header{display:flex;align-items:center;justify-content:space-between;padding:20px 32px;background:transparent}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:52px;height:52px;border-radius:10px;background:var(--accent);display:flex;align-items:center;justify-content:center;color:white;font-weight:700;box-shadow:0 6px 18px rgba(2,6,23,0.08)}
    nav{display:flex;gap:18px;align-items:center}
    nav a{color:var(--dark);text-decoration:none;font-weight:600}

    .container{max-width:1100px;margin:0 auto;padding:32px}

    .hero{display:grid;grid-template-columns:1fr 420px;gap:32px;align-items:center;padding:36px 0}
    .hero-card{background:linear-gradient(180deg, rgba(255,255,255,0.9), rgba(255,255,255,0.84));padding:34px;border-radius:14px;box-shadow:0 10px 30px rgba(16,24,40,0.06)}
    h1{margin:0;font-size:34px;line-height:1.05}
    p.lead{color:var(--muted);margin-top:12px}
    .cta{margin-top:20px;display:flex;gap:12px}
    .btn{padding:12px 18px;border-radius:10px;border:0;cursor:pointer;font-weight:700}
    .btn-primary{background:var(--accent);color:white}
    .btn-ghost{background:transparent;border:2px solid rgba(2,6,23,0.06)}

    .profile{background:linear-gradient(180deg,#fff,#fbfdff);padding:22px;border-radius:12px;text-align:center}
    .profile img{width:100%;height:260px;object-fit:cover;border-radius:10px}
    .profile h3{margin:12px 0 6px}
    .tags{display:flex;flex-wrap:wrap;gap:8px;justify-content:center;margin-top:12px}
    .tag{padding:6px 10px;border-radius:999px;background:var(--glass);font-size:13px;color:var(--muted)}

    /* Services / cards */
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:28px}
    .card{background:white;padding:18px;border-radius:12px;box-shadow:0 8px 20px rgba(16,24,40,0.04)}
    .card h4{margin:8px 0 6px}
    .card p{color:var(--muted);font-size:14px}

    /* Portfolio */
    .portfolio{margin-top:36px}
    .projects{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    .project{border-radius:10px;overflow:hidden;background:linear-gradient(180deg,#fff,#fbfdff);box-shadow:0 8px 18px rgba(16,24,40,0.04)}
    .project img{width:100%;height:160px;object-fit:cover;display:block}
    .project .meta{padding:12px}

    /* Contact */
    .contact{margin-top:36px;background:linear-gradient(180deg,#fff,#fbfdff);padding:20px;border-radius:12px}
    form{display:grid;grid-template-columns:1fr 1fr;gap:12px}
    form input, form textarea{padding:10px;border-radius:8px;border:1px solid #e6eef8}
    form textarea{grid-column:1/3;min-height:110px}
    form button{grid-column:1/3}

    footer{margin-top:36px;padding:24px 0;text-align:center;color:var(--muted);font-size:13px}

    /* Responsive */
    @media (max-width:1000px){
      .hero{grid-template-columns:1fr}
      .grid{grid-template-columns:repeat(2,1fr)}
      .projects{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:640px){
      header{padding:14px}
      .brand .name{display:none}
      .grid{grid-template-columns:1fr}
      .projects{grid-template-columns:1fr}
      form{grid-template-columns:1fr}
    }

    /* small helpers */
    .muted{color:var(--muted)}
    .pill{display:inline-block;padding:6px 10px;border-radius:999px;background:rgba(0,0,0,0.04);font-weight:700}
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <div class="logo">NE</div>
      <div>
        <div style="font-weight:800">Nurse Etiks</div>
        <div class="muted" style="font-size:13px">Health Hub</div>
      </div>
    </div>
    <nav>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main class="container">
    <section class="hero">
      <div class="hero-card">
        <h1>Nurse Etiks Health Hub</h1>
        <p class="lead">Professional nursing care, community health education, and bespoke patient advocacy. Building healthier lives with empathy, evidence, and excellence.</p>
        <div class="cta">
          <button class="btn btn-primary" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Book a consultation</button>
          <a href="#portfolio" class="btn btn-ghost">View work</a>
        </div>

        <div id="about" style="margin-top:26px">
          <h3>Who I am</h3>
          <p class="muted">I am a registered nurse with experience in community health, maternal-child care, and patient education. I combine clinical best practices with culturally-sensitive care.</p>
        </div>

        <div id="services" class="grid">
          <div class="card">
            <h4>Community Outreach</h4>
            <p>Workshops, school health programs and vaccination advocacy tailored to local communities.</p>
          </div>
          <div class="card">
            <h4>Patient Education</h4>
            <p>One-on-one counselling and easy-to-follow educational resources for chronic disease and postnatal care.</p>
          </div>
          <div class="card">
            <h4>Home Visits</h4>
            <p>Compassionate post-discharge and palliative care at home with practical clinical support.</p>
          </div>
        </div>

      </div>

      <aside class="profile">
        <img src="https://images.unsplash.com/photo-1584438786874-9d6f1a8c6a8e?q=80&w=900&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="Nurse portrait"/>
        <h3>Nurse Etiks</h3>
        <div class="muted">Registered Nurse • Community Health Advocate</div>
        <div class="tags">
          <span class="tag">BSc Nursing</span>
          <span class="tag">Community Health</span>
          <span class="tag">CPR/First Aid</span>
        </div>
        <div style="margin-top:14px"> <span class="pill">Open for projects</span></div>
      </aside>
    </section>

    <section id="portfolio" class="portfolio">
      <div style="display:flex;align-items:center;justify-content:space-between">
        <h2>Selected Work</h2>
        <div class="muted">Recent community & clinical projects</div>
      </div>
      <div class="projects">
        <article class="project">
          <img src="https://images.unsplash.com/photo-1582719478250-8f7f3c1e1f3b?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="project 1">
          <div class="meta">
            <strong>Postnatal Workshop — Community Hall</strong>
            <div class="muted">Education on breastfeeding, newborn care and maternal well-being.</div>
          </div>
        </article>

        <article class="project">
          <img src="https://images.unsplash.com/photo-1581574314298-4b6f69b0e5c4?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="project 2">
          <div class="meta">
            <strong>Vaccination Drive</strong>
            <div class="muted">Organised and led an outreach vaccination day reaching 300+ children.</div>
          </div>
        </article>

        <article class="project">
          <img src="https://images.unsplash.com/photo-1542736667-069246bdbc3d?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="project 3">
          <div class="meta">
            <strong>Home Follow-up Program</strong>
            <div class="muted">Post-discharge nursing visits reduced readmission rates for elderly patients.</div>
          </div>
        </article>
      </div>
    </section>

    <section id="contact" class="contact">
      <h2>Contact & Booking</h2>
      <p class="muted">Send a message to request a consultation, workshop or home visit. You can also reach me directly at:<br><strong>Email:</strong> Emmanueletikerentse8@gmail.com<br><strong>Phone:</strong> 09135126835</p>
      <form onsubmit="event.preventDefault();alert('Thanks! This demo form is not connected to a server. Replace with your backend or Formspree.');">
        <input type="text" placeholder="Your name" />
        <input type="email" placeholder="Email address" />
        <input type="text" placeholder="Phone (optional)" />
        <input type="text" placeholder="Service of interest (e.g., Home visit, Workshop)" />
        <textarea placeholder="Describe your request"></textarea>
        <button class="btn btn-primary">Send message</button>
      </form>
    </section>

    <footer>
      © <span id="year"></span> Nurse Etiks Health Hub — Built with care.
    </footer>
  </main>

  <script>
    document.getElementById('year').innerText = new Date().getFullYear();
  </script>
</body>
</html>
