# ofabworld
home of beauty
<!doctype html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="theme-color" content="#201c20" />
  <title>OFab World — Beauty, made personal.</title>
  <link rel="manifest" href="manifest.webmanifest" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:ital,wght@0,600;0,700;1,600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <div class="announcement">Lagos beauty, without limits <span>•</span> Book your experience today</div>
  <header>
    <a href="#top" class="logo">O<span>Fab</span> World<sup>®</sup></a>
    <nav><a href="#shop">Shop</a><a href="#services">Studio</a><a href="#story">Our world</a></nav>
    <div class="header-actions"><button class="text-button" id="openEditor">Edit site</button><button class="bag" id="bagButton" aria-label="Shopping bag">Bag <b id="bagCount">0</b></button></div>
  </header>

  <main id="top">
    <section class="hero">
      <div class="hero-copy"><p class="eyebrow">The art of becoming</p><h1>Wear the<br><em>world</em> you want.</h1><p class="hero-text">Luxury wigs, expressive piercings and beauty rituals created around your individuality.</p><a class="button dark" href="#shop">Explore the collection <span>↗</span></a></div>
      <div class="hero-art"><div class="orb orb-one"></div><div class="orb orb-two"></div><div class="portrait"><img id="heroImage" alt="OFab World beauty campaign" src="https://images.unsplash.com/photo-1595476108010-b4d1f102b1b1?auto=format&fit=crop&w=1000&q=85"><div class="portrait-label">OFW <span>EST. 2024</span></div></div><div class="hero-note">Made to<br>be noticed <i>↘</i></div></div>
    </section>

    <section class="marquee"><span>YOUR LOOK. YOUR RULES.</span><i>✦</i><span>YOUR LOOK. YOUR RULES.</span><i>✦</i><span>YOUR LOOK. YOUR RULES.</span></section>

    <section id="shop" class="section products-section"><div class="section-heading"><div><p class="eyebrow">Shop OFab</p><h2>Find your <em>signature.</em></h2></div><a href="#services" class="arrow-link">View studio services <span>→</span></a></div><div class="filters" id="filters"></div><div class="product-grid" id="products"></div></section>

    <section id="services" class="services"><div class="services-visual"><img id="serviceImage" alt="OFab World studio detail" src="https://images.unsplash.com/photo-1616394584738-fc6e612e71b9?auto=format&fit=crop&w=1000&q=85"><div class="stamp">OFAB<br>WORLD<br><span>STUDIO</span></div></div><div class="services-copy"><p class="eyebrow">OFab Studio</p><h2>A little ritual.<br><em>A lot of you.</em></h2><p>Come as you are. Leave feeling like the main character. Our artists are here for every bold idea, finishing touch, and fresh start.</p><div id="serviceList" class="service-list"></div></div></section>

    <section id="story" class="story"><p class="eyebrow">Welcome to our world</p><h2>Beauty is not a look.<br>It's a <em>language.</em></h2><p>OFab World is a beauty house for the expressive ones. From crown to cartilage, we make space for the version of you that wants to be seen.</p><a href="#services" class="button light">Book your moment <span>↗</span></a></section>
  </main>
  <footer><div class="logo">O<span>Fab</span> World<sup>®</sup></div><p>Made for the beautifully undone.</p><p>© 2026 OFab World</p></footer>

  <aside class="cart" id="cart"><div class="panel-head"><h3>Your selection</h3><button class="icon-close" data-close="cart">×</button></div><div id="cartItems" class="cart-items"><p class="empty">Your bag is waiting for its first obsession.</p></div><div class="cart-foot"><div class="total"><span>Total</span><b id="total">₦0</b></div><button class="button dark full" id="checkout">Continue on WhatsApp <span>↗</span></button></div></aside>
  <div class="overlay" id="overlay"></div>

  <dialog id="bookingDialog"><button class="icon-close modal-close" data-close="bookingDialog">×</button><p class="eyebrow">Let's make it happen</p><h2 id="bookingTitle">Book a service</h2><p id="bookingDescription">Choose your preferred day and we’ll begin the conversation on WhatsApp.</p><label>Preferred date<input id="bookingDate" type="date"></label><label>Anything we should know?<textarea id="bookingNote" placeholder="Tell us the look you're dreaming of..."></textarea></label><button class="button dark full" id="agreeBooking">Agree & chat on WhatsApp <span>↗</span></button><small>By continuing, you agree to start a WhatsApp chat with OFab World.</small></dialog>

  <dialog id="editorDialog" class="editor"><button class="icon-close modal-close" data-close="editorDialog">×</button><p class="eyebrow">Owner controls</p><h2>Make it yours.</h2><p>Update your WhatsApp number, campaign photos and offerings. Changes are saved in this browser for this live preview.</p><form id="editorForm"><label>Owner WhatsApp number<input name="whatsapp" placeholder="2348012345678" inputmode="numeric"></label><label>Hero image URL<input name="heroImage" type="url"></label><label>Studio image URL<input name="serviceImage" type="url"></label><label>Products (one per line: Name | Category | Price | Image URL)<textarea name="products" rows="7"></textarea></label><button class="button dark full" type="submit">Save changes</button></form><button class="reset" id="resetSite">Reset demo content</button></dialog>
  <div class="toast" id="toast"></div>
  <script src="app.js"></script>
</body>
</html>
