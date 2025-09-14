<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>LEOPARD TURI BABA Courier Services</title>
  <style>
    :root{--accent:#f6c90e;--dark:#0f1724;--muted:#6b7280}
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;background:#f8fafc;color:#0b1220}
    header{background:linear-gradient(90deg,#111827 0%, #0b1220 60%);color:#fff;padding:18px 24px;display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:48px;height:48px;border-radius:8px;background:var(--accent);display:flex;align-items:center;justify-content:center;font-weight:800;color:#08121a}
    nav a{color:#d1d5db;margin-left:18px;text-decoration:none;font-weight:600}
    .hero{display:flex;flex-wrap:wrap;gap:24px;padding:48px 24px;align-items:center}
    .hero-left{flex:1;min-width:280px}
    .hero h1{font-size:28px;margin:0 0 8px}
    .hero p{color:var(--muted);margin:0 0 18px}
    .btn{background:var(--accent);border:none;padding:12px 18px;border-radius:8px;font-weight:700;cursor:pointer}
    .track-card{background:#fff;padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(2,6,23,0.06);max-width:520px}
    .services{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:18px;padding:24px}
    .service{background:#fff;padding:18px;border-radius:10px}
    .footer{background:#071025;color:#9aa4b2;padding:24px;text-align:center;margin-top:24px}
    form input, form select{width:100%;padding:10px;margin:6px 0 12px;border:1px solid #e6e9ee;border-radius:8px}
    .cols{display:grid;grid-template-columns:1fr 1fr;gap:12px}
    @media(max-width:720px){header{flex-direction:column;align-items:flex-start} .cols{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <div class="logo">LTB</div>
      <div>
        <div style="font-weight:800">LEOPARD TURI BABA</div>
        <div style="font-size:12px;color:#cbd5e1">Reliable courier across Pakistan</div>
      </div>
    </div>
    <nav>
      <a href="#services">Services</a>
      <a href="#track">Track</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>  <section class="hero">
    <div class="hero-left">
      <h1>Fast • Safe • Nationwide — LEOPARD TURI BABA</h1>
      <p>We deliver parcels, documents and e-commerce shipments with real-time tracking and door-to-door service. Enter your tracking number to see live status.</p>
      <div style="display:flex;gap:12px;align-items:center">
        <button class="btn" onclick="document.getElementById('track-input').focus()">Track Parcel</button>
        <a href="#contact" style="text-decoration:none;color:var(--dark);background:#fff;padding:10px 14px;border-radius:8px;font-weight:700">Ship Now</a>
      </div>
    </div><div class="track-card" id="track">
  <h3 style="margin:0 0 8px">Track Your Shipment</h3>
  <p style="margin:0 0 12px;color:var(--muted)">Type your tracking number below and click "Check"</p>
  <form onsubmit="checkTrack(event)">
    <input id="track-input" placeholder="e.g. LTB123456789" required>
    <button class="btn" type="submit">Check</button>
  </form>
  <div id="track-result" style="margin-top:12px;color:var(--muted)"></div>
</div>

  </section>  <section id="services">
    <h2 style="padding:0 24px;margin:0 0 6px">Our Services</h2>
    <div class="services">
      <div class="service"><strong>Same-day Delivery</strong><p style="color:var(--muted);margin:8px 0 0">City-to-city express delivery for urgent parcels.</p></div>
      <div class="service"><strong>Cash on Delivery (COD)</strong><p style="color:var(--muted);margin:8px 0 0">COD collection and secure remittance to sellers.</p></div>
      <div class="service"><strong>eCommerce Shipping</strong><p style="color:var(--muted);margin:8px 0 0">Integration-ready options for online shops.</p></div>
      <div class="service"><strong>Document Courier</strong><p style="color:var(--muted);margin:8px 0 0">Fast delivery for legal and official papers.</p></div>
    </div>
  </section>  <section style="padding:24px">
    <h2 style="margin:0 0 12px">Get a Quote / Contact Us</h2>
    <div class="cols">
      <div style="background:#fff;padding:18px;border-radius:10px">
        <form id="contact" onsubmit="submitContact(event)">
          <input name="name" placeholder="Full name" required>
          <input name="phone" placeholder="Phone number" required>
          <input name="email" placeholder="Email (optional)">
          <select name="service">
            <option>Choose service</option>
            <option>Same-day Delivery</option>
            <option>COD</option>
            <option>eCommerce Shipping</option>
          </select>
          <textarea name="message" placeholder="Message / pickup address" style="width:100%;min-height:90px;padding:10px;border-radius:8px;border:1px solid #e6e9ee"></textarea>
          <button class="btn" type="submit">Send Request</button>
        </form>
      </div><div style="background:#fff;padding:18px;border-radius:10px">
    <h3 style="margin-top:0">Office & Support</h3>
    <p style="margin:6px 0;color:var(--muted)">Head Office: 123 Main Street, Lahore</p>
    <p style="margin:6px 0;color:var(--muted)">Phone: +92 300 0000000</p>
    <p style="margin:6px 0;color:var(--muted)">Email: support@leopardturibaba.example</p>
    <hr style="border:none;border-top:1px solid #eef2f6;margin:12px 0">
    <p style="margin:0;color:var(--muted)"><strong>Working hours:</strong><br>Mon–Sat 9:00 — 18:00</p>
  </div>
</div>

  </section>  <footer class="footer">
    <div>© <span id="year"></span> LEOPARD TURI BABA — All rights reserved.</div>
  </footer>  <script>
    document.getElementById('year').textContent = new Date().getFullYear();

    function checkTrack(e){
      e.preventDefault();
      const n = document.getElementById('track-input').value.trim();
      const res = document.getElementById('track-result');
      if(!n){res.textContent='Please enter a tracking number.';return}
      // Demo response (replace with real API integration)
      res.innerHTML = 'Searching...';
      setTimeout(()=>{
        res.innerHTML = '<strong>' + n + '</strong> — In transit. Next update: Lahore sorting hub.';
      },800);
    }

    function submitContact(e){
      e.preventDefault();
      alert('Thank you! Your request has been received. (Demo site)');
      e.target.reset();
    }
  </script></body>
</html>
