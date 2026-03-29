<DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <title>AMani | Premium Veg & Fruit Exports Worldwide</title>
  <!-- Google Fonts + Font Awesome Icons -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: #fefaf5;
      color: #1e2f2b;
      scroll-behavior: smooth;
      line-height: 1.4;
    }

    .container {
      max-width: 1280px;
      margin: 0 auto;
      padding: 0 32px;
    }

    /* Header / Navigation */
    header {
      background: rgba(255, 255, 245, 0.96);
      backdrop-filter: blur(12px);
      position: sticky;
      top: 0;
      z-index: 100;
      border-bottom: 1px solid #e2e0d4;
    }

    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 18px 0;
      flex-wrap: wrap;
    }

    .logo h1 {
      font-size: 2rem;
      font-weight: 800;
      letter-spacing: -0.5px;
      background: linear-gradient(135deg, #2b6e4c, #e67e22);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }
    .logo span {
      font-size: 0.8rem;
      font-weight: 500;
      color: #6b4e2e;
      display: block;
      letter-spacing: 1px;
    }

    .nav-links {
      display: flex;
      gap: 32px;
      list-style: none;
    }
    .nav-links a {
      text-decoration: none;
      font-weight: 600;
      color: #2c4b3e;
      transition: 0.2s;
      font-size: 1rem;
    }
    .nav-links a:hover {
      color: #e67e22;
    }

    .contact-btn-nav {
      background: #2b6e4c;
      color: white !important;
      padding: 8px 20px;
      border-radius: 40px;
      transition: 0.2s;
    }
    .contact-btn-nav:hover {
      background: #e67e22;
      transform: translateY(-2px);
    }

    /* Hero Section */
    .hero {
      padding: 70px 0 60px;
      background: linear-gradient(112deg, #fef9ef 0%, #eaf7ed 100%);
    }
    .hero-grid {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 40px;
    }
    .hero-text {
      flex: 1.2;
    }
    .badge {
      background: #ffedd5;
      color: #b45f1b;
      display: inline-block;
      padding: 6px 14px;
      border-radius: 40px;
      font-weight: 600;
      font-size: 0.8rem;
      margin-bottom: 20px;
    }
    .hero-text h2 {
      font-size: 3.2rem;
      font-weight: 800;
      line-height: 1.2;
      color: #1e3a2f;
      margin-bottom: 20px;
    }
    .hero-text h2 i {
      color: #e67e22;
    }
    .hero-text p {
      font-size: 1.1rem;
      color: #3a5a4e;
      max-width: 550px;
      margin-bottom: 32px;
    }
    .hero-stats {
      display: flex;
      gap: 32px;
      margin-top: 20px;
    }
    .stat h3 {
      font-size: 1.9rem;
      font-weight: 800;
      color: #2b6e4c;
    }
    .hero-image {
      flex: 0.9;
      text-align: center;
    }
    .hero-image .image-card {
      background: #d9f0e3;
      border-radius: 60px;
      padding: 30px 20px;
      box-shadow: 0 20px 25px -12px rgba(0,0,0,0.1);
    }
    .hero-image i {
      margin: 0 10px;
    }
    .btn-group {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
    }
    .btn-primary {
      background: #2b6e4c;
      color: white;
      padding: 12px 28px;
      border-radius: 40px;
      text-decoration: none;
      font-weight: 700;
      transition: 0.2s;
      display: inline-block;
      border: none;
      cursor: pointer;
    }
    .btn-primary:hover {
      background: #e67e22;
      transform: translateY(-3px);
      box-shadow: 0 12px 20px -8px rgba(43,110,76,0.4);
    }
    .btn-outline {
      background: transparent;
      border: 2px solid #2b6e4c;
      color: #2b6e4c;
      padding: 10px 26px;
      border-radius: 40px;
      font-weight: 700;
      text-decoration: none;
      transition: 0.2s;
    }
    .btn-outline:hover {
      background: #2b6e4c;
      color: white;
    }

    /* Products Section */
    .products {
      padding: 80px 0;
      background: white;
    }
    .section-title {
      text-align: center;
      font-size: 2.2rem;
      font-weight: 700;
      margin-bottom: 20px;
      color: #1e3a2f;
    }
    .section-sub {
      text-align: center;
      color: #5e776b;
      max-width: 650px;
      margin: 0 auto 48px auto;
    }
    .category-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 30px;
    }
    .card {
      background: #ffffff;
      border-radius: 28px;
      overflow: hidden;
      box-shadow: 0 12px 24px -12px rgba(0, 0, 0, 0.08);
      transition: 0.25s ease;
      border: 1px solid #ecf3ef;
      text-align: center;
      padding: 28px 18px 24px;
    }
    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 24px 36px -16px rgba(43, 110, 76, 0.2);
      border-color: #cfe6db;
    }
    .card-icon {
      font-size: 3rem;
      background: #eef6f2;
      width: 80px;
      height: 80px;
      line-height: 80px;
      border-radius: 50%;
      margin: 0 auto 20px;
      color: #2b6e4c;
    }
    .card h3 {
      font-size: 1.5rem;
      margin-bottom: 10px;
    }
    .card p {
      color: #5a6b62;
      font-size: 0.9rem;
    }

    /* Features / Export Advantage */
    .features {
      background: #f4f8f4;
      padding: 70px 0;
    }
    .feature-list {
      display: flex;
      flex-wrap: wrap;
      gap: 40px;
      justify-content: center;
    }
    .feature-item {
      flex: 1;
      min-width: 220px;
      text-align: center;
      background: white;
      padding: 32px 20px;
      border-radius: 32px;
      transition: 0.2s;
      box-shadow: 0 5px 12px rgba(0,0,0,0.02);
    }
    .feature-item i {
      font-size: 2.8rem;
      color: #e67e22;
      margin-bottom: 20px;
    }
    .feature-item h4 {
      font-size: 1.3rem;
      margin-bottom: 12px;
    }

    /* Contact Section */
    .contact-section {
      padding: 80px 0;
      background: linear-gradient(120deg, #fffaf2, #fff5e8);
    }
    .contact-wrapper {
      display: flex;
      flex-wrap: wrap;
      gap: 40px;
      background: white;
      border-radius: 48px;
      padding: 48px 40px;
      box-shadow: 0 20px 35px -15px rgba(0,0,0,0.05);
      border: 1px solid #eee5db;
    }
    .contact-info {
      flex: 1;
    }
    .contact-info h3 {
      font-size: 1.9rem;
      font-weight: 700;
      margin-bottom: 20px;
    }
    .contact-detail {
      display: flex;
      align-items: center;
      gap: 18px;
      margin: 28px 0;
    }
    .contact-detail i {
      font-size: 1.8rem;
      width: 48px;
      color: #2b6e4c;
    }
    .contact-detail p {
      font-size: 1.1rem;
      font-weight: 500;
    }
    .contact-detail a {
      text-decoration: none;
      color: #1e2f2b;
      font-weight: 500;
    }
    .contact-detail a:hover {
      color: #e67e22;
    }
    .contact-buttons-group {
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
      margin-top: 20px;
    }
    .contact-method-btn {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      background: #f0f4f0;
      padding: 10px 20px;
      border-radius: 50px;
      text-decoration: none;
      color: #1e3a2f;
      font-weight: 600;
      transition: 0.2s;
    }
    .contact-method-btn i {
      font-size: 1.2rem;
      color: #2b6e4c;
    }
    .contact-method-btn:hover {
      background: #2b6e4c;
      color: white;
    }
    .contact-method-btn:hover i {
      color: white;
    }
    .social-links {
      display: flex;
      gap: 20px;
      margin-top: 32px;
    }
    .social-links a {
      background: #eff3ef;
      width: 44px;
      height: 44px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #2b6e4c;
      font-size: 1.3rem;
      transition: 0.2s;
    }
    .social-links a:hover {
      background: #2b6e4c;
      color: white;
    }
    .contact-form {
      flex: 1;
    }
    .input-group {
      margin-bottom: 20px;
    }
    .input-group input, .input-group textarea {
      width: 100%;
      padding: 14px 18px;
      border-radius: 30px;
      border: 1px solid #e2dcd2;
      background: #fefcf9;
      font-family: inherit;
      font-size: 1rem;
      transition: 0.2s;
    }
    .input-group textarea {
      border-radius: 24px;
      resize: vertical;
    }
    .input-group input:focus, .input-group textarea:focus {
      outline: none;
      border-color: #e67e22;
      box-shadow: 0 0 0 3px rgba(230,126,34,0.1);
    }
    .btn-submit {
      background: #2b6e4c;
      border: none;
      padding: 14px 28px;
      font-weight: 700;
      border-radius: 40px;
      color: white;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.2s;
      width: 100%;
    }
    .btn-submit:hover {
      background: #e67e22;
    }

    /* Floating Quick Contact */
    .float-contact {
      position: fixed;
      bottom: 28px;
      right: 28px;
      background: #2b6e4c;
      border-radius: 60px;
      padding: 12px 24px;
      display: flex;
      gap: 12px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.2);
      z-index: 99;
      backdrop-filter: blur(4px);
    }
    .float-contact a {
      color: white;
      text-decoration: none;
      font-size: 0.9rem;
      display: flex;
      align-items: center;
      gap: 8px;
      font-weight: 500;
    }
    .float-contact i {
      font-size: 1.1rem;
    }

    /* Footer */
    footer {
      background: #14251f;
      color: #cddfd7;
      padding: 32px 0;
      text-align: center;
    }

    /* Responsive */
    @media (max-width: 800px) {
      .navbar {
        flex-direction: column;
        gap: 16px;
      }
      .hero-text h2 {
        font-size: 2.4rem;
      }
      .contact-wrapper {
        padding: 28px 20px;
      }
      .container {
        padding: 0 20px;
      }
      .float-contact {
        bottom: 16px;
        right: 16px;
        padding: 8px 16px;
      }
      .hero-stats {
        flex-wrap: wrap;
        gap: 20px;
      }
      .contact-buttons-group {
        justify-content: center;
      }
    }
  </style>
</head>
<body>

<header>
  <div class="container">
    <div class="navbar">
      <div class="logo">
        <h1>AMani</h1>
        <span>global harvest, pure taste</span>
      </div>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#products">Produce</a></li>
        <li><a href="#export">Advantage</a></li>
        <li><a href="#contact" class="contact-btn-nav">Contact</a></li>
      </ul>
    </div>
  </div>
</header>

<main>
  <!-- Hero Section -->
  <section id="home" class="hero">
    <div class="container hero-grid">
      <div class="hero-text">
        <div class="badge"><i class="fas fa-globe-asia"></i> Worldwide Exporters</div>
        <h2>Fresh from farms <br> to <i>120+ countries</i></h2>
        <p>Premium quality vegetables & fruits, ethically sourced, cold-chain preserved. AMani delivers nature's finest to global markets.</p>
        <div class="btn-group">
          <a href="#contact" class="btn-primary">Request a quote <i class="fas fa-arrow-right"></i></a>
          <a href="#products" class="btn-outline">Explore range</a>
        </div>
        <div class="hero-stats">
          <div class="stat"><h3>15+</h3><span>Partner farms</span></div>
          <div class="stat"><h3>24/7</h3><span>Cold supply chain</span></div>
          <div class="stat"><h3>⭐ 4.9</h3><span>Client rating</span></div>
        </div>
      </div>
      <div class="hero-image">
        <div class="image-card">
          <i class="fas fa-apple-alt" style="font-size: 6rem; color:#e67e22;"></i>
          <i class="fas fa-carrot" style="font-size: 5.5rem; color:#2b6e4c;"></i>
          <i class="fas fa-pepper-hot" style="font-size: 5rem; color:#c23b22;"></i>
          <p style="margin-top: 20px; font-weight:500;">🍅🥑🥬 premium export grade</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Products / Vegetables & Fruits -->
  <section id="products" class="products">
    <div class="container">
      <h2 class="section-title">Our export selection</h2>
      <p class="section-sub">Handpicked vegetables & fruits, certified for global standards. Shelf-life optimized for international shipping.</p>
      <div class="category-grid">
        <div class="card">
          <div class="card-icon"><i class="fas fa-leaf"></i></div>
          <h3>Premium Greens</h3>
          <p>Spinach, Kale, Lettuce — hydroponic & organic. Freshness sealed.</p>
        </div>
        <div class="card">
          <div class="card-icon"><i class="fas fa-apple-alt"></i></div>
          <h3>Exotic Fruits</h3>
          <p>Mangoes, Pomegranate, Dragon Fruit, Kiwi — sweet & aromatic.</p>
        </div>
        <div class="card">
          <div class="card-icon"><i class="fas fa-pepper-hot"></i></div>
          <h3>Seasonal Vegetables</h3>
          <p>Tomatoes, Onions, Bell Peppers, Zucchini — export-grade size.</p>
        </div>
        <div class="card">
          <div class="card-icon"><i class="fas fa-seedling"></i></div>
          <h3>Roots & Tubers</h3>
          <p>Potato, Ginger, Turmeric, Sweet Potato — high yield & organic.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Export Advantage -->
  <section id="export" class="features">
    <div class="container">
      <h2 class="section-title">Why AMani for global exports?</h2>
      <p class="section-sub">Reliable, sustainable, and built for international trade.</p>
      <div class="feature-list">
        <div class="feature-item"><i class="fas fa-ship"></i><h4>Logistics Excellence</h4><p>Sea & air freight with real-time tracking, phytosanitary certified.</p></div>
        <div class="feature-item"><i class="fas fa-temperature-low"></i><h4>Cold Chain Network</h4><p>Maintains freshness from farm to port, zero spoilage guarantee.</p></div>
        <div class="feature-item"><i class="fas fa-handshake"></i><h4>B2B Partnerships</h4><p>Flexible MOQs, custom packaging, private labeling support.</p></div>
        <div class="feature-item"><i class="fas fa-leaf"></i><h4>Sustainable Farming</h4><p>Eco-friendly practices, GlobalG.A.P. & organic certifications.</p></div>
      </div>
    </div>
  </section>

  <!-- Contact Section with both phone numbers + Telegram -->
  <section id="contact" class="contact-section">
    <div class="container">
      <div class="contact-wrapper">
        <div class="contact-info">
          <h3>Let's talk exports 🚢</h3>
          <p style="margin-bottom: 20px;">Reach out for bulk inquiries, partnerships, or sample orders. We respond within 24 hours.</p>
          
          <!-- India Number (WhatsApp/Call) -->
          <div class="contact-detail">
            <i class="fas fa-phone-alt"></i>
            <p><strong>India Office (Call / WhatsApp)</strong><br><a href="tel:+917040118014">+91 70401 18014</a></p>
          </div>
          
          <!-- New International Number + Telegram -->
          <div class="contact-detail">
            <i class="fab fa-telegram-plane"></i>
            <p><strong>International / Telegram</strong><br><a href="tel:+79934674423">+7 993 467 4423</a></p>
          </div>
          
          <!-- Email -->
          <div class="contact-detail">
            <i class="fas fa-envelope"></i>
            <p><strong>Email us</strong><br><a href="mailto:rafeymaniyar7@gmail.com">rafeymaniyar7@gmail.com</a></p>
          </div>
          
          <!-- Quick contact buttons: WhatsApp, Telegram, Call -->
          <div class="contact-buttons-group">
            <a href="https://wa.me/917040118014?text=Hello%20AMani%2C%20I'm%20interested%20in%20export%20products" target="_blank" class="contact-method-btn">
              <i class="fab fa-whatsapp"></i> WhatsApp (India)
            </a>
            <a href="https://t.me/+79934674423" target="_blank" class="contact-method-btn">
              <i class="fab fa-telegram"></i> Telegram
            </a>
            <a href="tel:+79934674423" class="contact-method-btn">
              <i class="fas fa-phone"></i> Call Intl.
            </a>
          </div>
          
          <div class="social-links">
            <a href="#" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
            <a href="#" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
            <a href="#" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
          </div>
        </div>
        <div class="contact-form">
          <form id="inquiryForm" action="#" method="post">
            <div class="input-group">
              <input type="text" placeholder="Your name / Company" required id="name">
            </div>
            <div class="input-group">
              <input type="email" placeholder="Email address" required id="email">
            </div>
            <div class="input-group">
              <input type="tel" placeholder="Phone (with country code)" id="phone">
            </div>
            <div class="input-group">
              <textarea rows="4" placeholder="Tell us about your export requirement (product, quantity, destination)" id="message"></textarea>
            </div>
            <button type="submit" class="btn-submit">Send inquiry <i class="fas fa-paper-plane"></i></button>
            <p id="formFeedback" style="margin-top: 12px; font-size: 0.85rem; color: #2b6e4c;"></p>
          </form>
        </div>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="container">
    <p>© 2025 AMani Exports — Fresh vegetables & fruits, delivered worldwide. 🌍</p>
    <p style="margin-top: 10px; font-size: 0.8rem;">
      📞 +91 70401 18014 (India) | 📞 +7 993 467 4423 (Intl / Telegram) | ✉️ rafeymaniyar7@gmail.com
    </p>
  </div>
</footer>

<!-- Floating quick contact bar with both numbers and Telegram -->
<div class="float-contact">
  <a href="tel:+917040118014"><i class="fas fa-phone-alt"></i> India</a>
  <a href="https://wa.me/917040118014?text=Hello%20AMani%2C%20I'm%20interested%20in%20export%20products" target="_blank"><i class="fab fa-whatsapp"></i> WhatsApp</a>
  <a href="https://t.me/+79934674423" target="_blank"><i class="fab fa-telegram"></i> Telegram</a>
  <a href="mailto:rafeymaniyar7@gmail.com"><i class="fas fa-envelope"></i> Mail</a>
</div>

<script>
  // Simple contact form handler with feedback
  const form = document.getElementById('inquiryForm');
  const feedback = document.getElementById('formFeedback');
  form.addEventListener('submit', function(e) {
    e.preventDefault();
    const name = document.getElementById('name').value.trim();
    const email = document.getElementById('email').value.trim();
    if(!name || !email) {
      feedback.style.color = "#c23b22";
      feedback.innerText = "⚠️ Please enter your name and email address.";
      return;
    }
    // Simulate successful submission
    feedback.style.color = "#2b6e4c";
    feedback.innerHTML = "✅ Thank you! Our export team will reach you shortly (within 24h).";
    form.reset();
    setTimeout(() => {
      feedback.innerText = "";
    }, 5000);
    console.log(`Inquiry from ${name}, ${email}`);
  });
</script>
</body>
</html>
