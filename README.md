# Royal-Sister-Book-Cafe-
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Sip. Scribble. Share. — Café and Creative Space</title>
  <meta name="description" content="Where Milk nourishes the body, and Pen nourishes the soul." />

  <!-- Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">

  <style>
    :root{
      --cream: #F7F3EE;
      --latte: #E6D7C8;
      --slate: #3E4A53;
      --mocha: #6B4F3A;
      --accent: #C9A77A;
      --max-width: 1100px;
      --radius: 12px;
      --glass: rgba(255,255,255,0.6);
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: "Inter", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      color:var(--slate);
      background:linear-gradient(180deg,var(--cream),#fff);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
    }

    .container{
      max-width:var(--max-width);
      margin:0 auto;
      padding:28px;
    }

    /* Header */
    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:20px;
      padding:18px 0;
    }

    .logo{
      display:flex;
      align-items:center;
      gap:14px;
    }

    .logo-mark{
      width:48px;
      height:48px;
      border-radius:10px;
      background:linear-gradient(135deg,var(--latte),var(--mocha));
      display:flex;
      align-items:center;
      justify-content:center;
      color:white;
      font-weight:700;
      font-family:"Playfair Display", serif;
      box-shadow:0 6px 18px rgba(107,79,58,0.12);
    }

    .brand{
      display:flex;
      flex-direction:column;
      line-height:1;
    }

    .brand .title{
      font-family:"Playfair Display", serif;
      font-size:20px;
      color:var(--slate);
      letter-spacing:0.2px;
    }

    .brand .tag{
      font-size:11px;
      color:var(--mocha);
      text-transform:uppercase;
      letter-spacing:1px;
    }

    nav{
      display:flex;
      gap:18px;
      align-items:center;
    }

    nav a{
      color:var(--slate);
      text-decoration:none;
      font-weight:500;
      padding:8px 10px;
      border-radius:8px;
    }

    nav a:hover{background:var(--glass)}

    .btn{
      background:var(--slate);
      color:white;
      padding:10px 14px;
      border-radius:10px;
      font-weight:600;
      border:none;
      cursor:pointer;
    }

    /* Hero */
    .hero{
      display:grid;
      grid-template-columns:1fr 420px;
      gap:28px;
      align-items:center;
      margin-top:18px;
    }

    .hero-card{
      background:linear-gradient(180deg, rgba(255,255,255,0.8), rgba(255,255,255,0.6));
      border-radius:var(--radius);
      padding:28px;
      box-shadow:0 10px 30px rgba(62,74,83,0.06);
      backdrop-filter: blur(6px);
    }

    .hero h1{
      font-family:"Playfair Display", serif;
      font-size:36px;
      margin:0 0 12px 0;
      color:var(--slate);
    }

    .hero p.lead{
      margin:0 0 18px 0;
      color:#5b6a70;
      font-size:16px;
    }

    .hero .actions{display:flex;gap:12px}
    .btn-ghost{
      background:transparent;
      border:1px solid var(--slate);
      color:var(--slate);
      padding:10px 14px;
      border-radius:10px;
      cursor:pointer;
    }

    .hero-visual{
      border-radius:var(--radius);
      overflow:hidden;
      box-shadow:0 12px 40px rgba(107,79,58,0.08);
      height:100%;
      min-height:320px;
      background: url('assets/hero.jpg') center/cover no-repeat;
      display:flex;
      align-items:flex-end;
      padding:18px;
    }

    .hero-visual .note{
      background:linear-gradient(180deg, rgba(255,255,255,0.9), rgba(255,255,255,0.7));
      padding:12px 14px;
      border-radius:10px;
      font-size:14px;
      color:var(--slate);
      width:100%;
    }

    /* Two column features */
    .split{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:22px;
      margin:34px 0;
    }

    .card{
      background:white;
      border-radius:12px;
      padding:18px;
      box-shadow:0 8px 24px rgba(62,74,83,0.04);
      display:flex;
      gap:14px;
      align-items:flex-start;
    }

    .icon{
      width:64px;
      height:64px;
      border-radius:10px;
      background:var(--latte);
      display:flex;
      align-items:center;
      justify-content:center;
      color:var(--mocha);
      font-size:22px;
      font-weight:700;
      flex-shrink:0;
    }

    .card h3{margin:0 0 6px 0;font-size:18px;color:var(--slate)}
    .card p{margin:0;color:#5b6a70;font-size:14px}

    /* Gallery */
    .gallery{
      margin:28px 0;
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:12px;
    }

    .gallery .tile{
      background:#fff;
      border-radius:10px;
      overflow:hidden;
      min-height:120px;
      background-size:cover;
      background-position:center;
      box-shadow:0 8px 20px rgba(62,74,83,0.04);
    }

    /* Menu */
    .menu{
      margin:28px 0;
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:12px;
    }

    .menu .menu-card{
      background:linear-gradient(180deg,var(--cream),#fff);
      border-radius:10px;
      padding:16px;
      text-align:center;
      box-shadow:0 8px 20px rgba(62,74,83,0.04);
    }

    .menu .menu-card h4{margin:8px 0;color:var(--mocha)}
    .menu .menu-card p{margin:0;color:#5b6a70;font-size:13px}

    /* Visit */
    .visit{
      display:grid;
      grid-template-columns:1fr 360px;
      gap:18px;
      margin:28px 0 60px 0;
      align-items:start;
    }

    .map{
      border-radius:10px;
      overflow:hidden;
      min-height:240px;
      background:#e9e6e3;
      display:flex;
      align-items:center;
      justify-content:center;
      color:#8a7f76;
      font-weight:600;
    }

    .hours{
      background:white;
      border-radius:10px;
      padding:16px;
      box-shadow:0 8px 20px rgba(62,74,83,0.04);
    }

    .hours h4{margin:0 0 8px 0;color:var(--mocha)}
    .hours p{margin:6px 0;color:#5b6a70}

    /* Footer */
    footer{
      border-top:1px solid rgba(62,74,83,0.06);
      padding:22px 0;
      margin-top:40px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      gap:12px;
      flex-wrap:wrap;
    }

    .socials{display:flex;gap:10px}
    .socials a{
      display:inline-block;
      width:36px;
      height:36px;
      border-radius:8px;
      background:var(--latte);
      color:var(--mocha);
      display:flex;
      align-items:center;
      justify-content:center;
      text-decoration:none;
      font-weight:700;
    }

    /* Responsive */
    @media (max-width:980px){
      .hero{grid-template-columns:1fr}
      .visit{grid-template-columns:1fr}
      .gallery{grid-template-columns:repeat(2,1fr)}
      .menu{grid-template-columns:repeat(2,1fr)}
    }

    @media (max-width:640px){
      header{flex-direction:column;align-items:flex-start}
      nav{order:2;width:100%;display:flex;flex-wrap:wrap}
      .gallery{grid-template-columns:1fr}
      .menu{grid-template-columns:1fr}
    }

    /* Reservation modal */
    .modal-backdrop{
      position:fixed;
      inset:0;
      background:rgba(0,0,0,0.35);
      display:none;
      align-items:center;
      justify-content:center;
      z-index:60;
    }

    .modal{
      background:white;
      border-radius:12px;
      padding:20px;
      width:420px;
      max-width:92%;
      box-shadow:0 20px 60px rgba(62,74,83,0.2);
    }

    .modal h3{margin:0 0 8px 0}
    .modal form{display:grid;gap:10px}
    .modal input, .modal select{
      padding:10px;
      border-radius:8px;
      border:1px solid rgba(62,74,83,0.08);
      font-size:14px;
    }

    .close-btn{background:transparent;border:none;color:var(--slate);font-weight:700;cursor:pointer}
  </style>
</head>
<body>

  <div class="container">
    <header>
      <div class="logo">
        <div class="logo-mark">S</div>
        <div class="brand">
          <div class="title">Sip. Scribble. Share.</div>
          <div class="tag">Café & Creative Space</div>
        </div>
      </div>

      <nav>
        <a href="#home">Home</a>
        <a href="#our-story">Our Story</a>
        <a href="#menu">Menu</a>
        <a href="#creative-space">Creative Space</a>
        <a href="#visit">Visit Us</a>
        <button class="btn" id="reserveBtn">Reserve a Table</button>
      </nav>
    </header>

    <!-- Hero -->
    <section id="home" class="hero">
      <div class="hero-card">
        <h1>Where Milk nourishes the body and Pen nourishes the soul</h1>
        <p class="lead">A modern café designed for quiet mornings, inspired afternoons, and the small acts of creation that make life sweeter. Sip slowly. Scribble freely. Share boldly.</p>
        <div class="actions">
          <button class="btn" onclick="document.getElementById('menu').scrollIntoView({behavior:'smooth'})">View Our Menu</button>
          <button class="btn-ghost" onclick="document.getElementById('creative-space').scrollIntoView({behavior:'smooth'})">Explore Our Space</button>
        </div>
      </div>

      <div class="hero-visual" aria-hidden="true">
        <!-- Replace assets/hero.jpg with your hero photo -->
        <div class="note">Bring a notebook. We'll bring the milk and the pen.</div>
      </div>
    </section>

    <!-- Sip & Savor Scribble & Create -->
    <section id="our-story" class="split" aria-labelledby="our-story-heading">
      <div class="card">
        <div class="icon">🥛</div>
        <div>
          <h3>Sip & Savor</h3>
          <p>Delicious drinks crafted with the comfort of milk. From classic lattes to seasonal milkshakes, each sip is designed to soothe and delight.</p>
        </div>
      </div>

      <div class="card">
        <div class="icon">✒️</div>
        <div>
          <h3>Scribble & Create</h3>
          <p>Inspiring spaces for writing and creativity. Notebooks, pens, and quiet nooks invite you to capture ideas and tell your stories.</p>
        </div>
      </div>
    </section>

    <!-- Share Your Story Gallery -->
    <section id="creative-space">
      <h2 style="font-family:'Playfair Display',serif;margin:6px 0 12px 0;color:var(--slate)">Share Your Story</h2>
      <p style="margin:0 0 12px 0;color:#5b6a70">Leave a note, pin a thought, and be inspired by our community wall.</p>

      <div class="gallery" aria-hidden="true">
        <div class="tile" style="background-image:url('assets/gallery1.jpg')"></div>
        <div class="tile" style="background-image:url('assets/gallery2.jpg')"></div>
        <div class="tile" style="background-image:url('assets/gallery3.jpg')"></div>
      </div>
    </section>

    <!-- Menu -->
    <section id="menu">
      <h2 style="font-family:'Playfair Display',serif;margin:6px 0 12px 0;color:var(--slate)">Our Menu</h2>
      <p style="margin:0 0 12px 0;color:#5b6a70">Warm drinks and creative comforts</p>

      <div class="menu">
        <div class="menu-card">
          <h4>Lattes & Teas</h4>
          <p>Classic latte, chai latte, matcha, and curated teas.</p>
        </div>
        <div class="menu-card">
          <h4>Milkshakes</h4>
          <p>Seasonal flavors made with whole milk and house syrups.</p>
        </div>
        <div class="menu-card">
          <h4>Pastries & More</h4>
          <p>Freshly baked pastries, toast, and light bites.</p>
        </div>
      </div>
    </section>

    <!-- Visit Us -->
    <section id="visit" class="visit">
      <div>
        <h2 style="font-family:'Playfair Display',serif;margin:6px 0 12px 0;color:var(--slate)">Plan Your Visit</h2>
        <p style="margin:0 0 12px 0;color:#5b6a70">A small restaurant tucked between busy streets where time slows and ideas bloom.</p>

        <div class="hours">
          <h4>Address</h4>
          <p>123 Creative Lane, Cityville</p>
          <h4>Hours</h4>
          <p>Open Daily 8 AM – 8 PM</p>
          <h4>Contact</h4>
          <p>Call us to reserve or use the reservation button above</p>
        </div>
      </div>

      <div class="map" aria-hidden="true">
        <!-- Replace with an embedded map or image -->
        Map Placeholder
      </div>
    </section>

    <footer>
      <div style="display:flex;gap:12px;align-items:center">
        <div class="logo-mark" style="width:44px;height:44px">S</div>
        <div>
          <div style="font-weight:700">Sip. Scribble. Share.</div>
          <div style="font-size:12px;color:#6b5b50">Where Milk nourishes the body, and Pen nourishes the soul</div>
        </div>
      </div>

      <div class="socials" aria-hidden="true">
        <a href="#" title="Instagram">IG</a>
        <a href="#" title="Facebook">FB</a>
      </div>
    </footer>
  </div>

  <!-- Reservation Modal -->
  <div class="modal-backdrop" id="modalBackdrop" role="dialog" aria-modal="true" aria-hidden="true">
    <div class="modal" role="document">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px">
        <h3>Reserve a Table</h3>
        <button class="close-btn" id="closeModal">✕</button>
      </div>
      <form id="reserveForm" onsubmit="handleReserve(event)">
        <input type="text" name="name" placeholder="Your name" required />
        <input type="tel" name="phone" placeholder="Phone number" required />
        <select name="party" required>
          <option value="">Party size</option>
          <option>1</option><option>2</option><option>3</option><option>4</option><option>5+</option>
        </select>
        <input type="datetime-local" name="datetime" required />
        <div style="display:flex;gap:8px;justify-content:flex-end">
          <button type="button" class="btn-ghost" id="cancelModal">Cancel</button>
          <button type="submit" class="btn">Confirm</button>
        </div>
      </form>
    </div>
  </div>

  <script>
    // Minimal interactivity for reservation modal and smooth nav
    const reserveBtn = document.getElementById('reserveBtn');
    const modal = document.getElementById('modalBackdrop');
    const closeModal = document.getElementById('closeModal');
    const cancelModal = document.getElementById('cancelModal');

    reserveBtn.addEventListener('click', () => {
      modal.style.display = 'flex';
      modal.setAttribute('aria-hidden','false');
    });

    closeModal.addEventListener('click', hideModal);
    cancelModal.addEventListener('click', hideModal);
    modal.addEventListener('click', (e) => {
      if (e.target === modal) hideModal();
    });

    function hideModal(){
      modal.style.display = 'none';
      modal.setAttribute('aria-hidden','true');
    }

    function handleReserve(e){
      e.preventDefault();
      // Minimal placeholder behavior
      const form = e.target;
      const name = form.name.value.trim();
      // In a real site, send data to server here
      alert('Thanks ' + (name || '') + '. Your reservation request was received.');
      form.reset();
      hideModal();
    }

    // Smooth scroll for nav links
    document.querySelectorAll('nav a').forEach(a => {
      a.addEventListener('click', (ev) => {
        ev.preventDefault();
        const id = a.getAttribute('href').slice(1);
        const el = document.getElementById(id);
        if (el) el.scrollIntoView({behavior:'smooth'});
      });
    });
  </script>
</body>
</html>
