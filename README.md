<!DOCTYPE html>
<html lang="fr" dir="ltr"><head>
  <meta charset="utf-8">
  <title>Textile Raach - تريكس رعش</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="Tissus d’ameublement haut de gamme – Tunisie">
  <link rel="manifest" href="data:application/json;base64,eyJuYW1lIjoiVGV4dGlsZSBSYWNoIiwic2hvcnRfbmFtZSI6IlJhYWNoIiwic3RhcnRfdXJsIjoiLyIsImRpc3BsYXkiOiJzdGFuZGFsb25lIiwiYmFja2dyb3VuZF9jb2xvciI6IiNmOWY0ZTgiLCJ0aGVtZV9jb2xvciI6IiNjMDU3NDYiLCJpY29ucyI6W3sic3JjIjoiaHR0cHM6Ly9mb250YXdlc29tZS5jb20vaWNvbnMuc3ZnIiwic2l6ZXMiOiIxOTIsNTEyIn1dfQ==">
  <style>
    /* ---------- RESET ---------- */
    *,*::before,*::after{box-sizing:border-box;margin:0;padding:0;font-family:'Inter',system-ui,sans-serif}
    img{max-width:100%;display:block}
    ul{list-style:none}
    a{text-decoration:none;color:inherit}
    button{cursor:pointer;border:none;background:none;font:inherit}

    /* ---------- VARIABLES ---------- */
    :root{
      --primary:#c05746;
      --secondary:#f9f4e8;
      --accent:#e9b44c;
      --dark:#1f1f1f;
      --light:#ffffff;
      --radius:12px;
      --shadow:0 4px 20px rgba(0,0,0,.08);
      --transition:.3s ease;
    }
    body[data-theme="dark"]{background:var(--dark);color:var(--light)}
    body[data-theme="dark"] .header{background:#2a2a2a}
    body[data-theme="dark"] .product-card{background:#2a2a2a;color:var(--light)}
    body.ar{font-family:'Noto Sans Arabic',sans-serif;direction:rtl}

    /* ---------- LAYOUT ---------- */
    .container{width:90%;max-width:1200px;margin-inline:auto}
    .section{padding:80px 0}
    .section__title{font-size:2.5rem;text-align:center;margin-bottom:3rem}

    /* ---------- HEADER ---------- */
    .header{position:sticky;top:0;z-index:100;background:var(--light);box-shadow:var(--shadow)}
    .header__inner{display:flex;align-items:center;justify-content:space-between;padding:1rem 0}
    .logo{font-weight:700;font-size:1.25rem;color:var(--primary)}
    .nav ul{display:flex;gap:1.5rem;align-items:center}
    .nav a:hover{color:var(--accent)}
    .header__actions{display:flex;gap:1rem;align-items:center}
    .cart-count{background:var(--accent);color:#fff;border-radius:50%;padding:.15rem .35rem;font-size:.75rem;margin-left:.25rem}

    /* ---------- HERO ---------- */
    .hero{height:70vh;display:flex;align-items:center;justify-content:center;text-align:center;background:url(https://source.unsplash.com/1600x900/?fabric,sofa) center/cover no-repeat;position:relative}
    .hero::before{content:'';position:absolute;inset:0;background:rgba(0,0,0,.45)}
    .hero__content{position:relative;color:var(--light);z-index:2}
    .hero__title{font-size:clamp(2rem,5vw,3.5rem);margin-bottom:1rem}
    .hero__subtitle{font-size:1.25rem;margin-bottom:2rem}
    .btn{display:inline-block;padding:.9rem 2rem;border-radius:var(--radius);font-weight:600;transition:var(--transition);background:var(--primary);color:var(--light)}
    .btn:hover{background:var(--accent)}

    /* ---------- CATALOGUE ---------- */
    .filters{display:flex;flex-wrap:wrap;gap:.75rem;justify-content:center;margin-bottom:3rem}
    .filter-btn{border:2px solid var(--primary);color:var(--primary);padding:.5rem 1.25rem;border-radius:20px;transition:var(--transition)}
    .filter-btn.active,.filter-btn:hover{background:var(--primary);color:#fff}
    .catalogue__grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:2rem}
    .product-card{background:var(--light);border-radius:var(--radius);overflow:hidden;box-shadow:var(--shadow);transition:var(--transition)}
    .product-card:hover{transform:translateY(-6px)}
    .product-card__img{height:200px;object-fit:cover}
    .product-card__body{padding:1rem}
    .product-card__title{font-size:1.1rem;margin-bottom:.5rem}
    .product-card__price{color:var(--primary);font-weight:600;margin-bottom:1rem}

    /* ---------- CART PANEL ---------- */
    .cart-panel{position:fixed;top:0;right:-400px;width:400px;height:100%;background:var(--light);box-shadow:-4px 0 20px rgba(0,0,0,.1);transition:right var(--transition);z-index:200;display:flex;flex-direction:column}
    .cart-panel.open{right:0}
    .cart-panel__header{display:flex;align-items:center;justify-content:space-between;padding:1rem;border-bottom:1px solid #ddd}
    .cart-panel__body{flex:1;padding:1rem;overflow-y:auto}
    .cart-panel__footer{border-top:1px solid #ddd;padding:1rem}
    .cart-item{display:grid;grid-template-columns:60px 1fr 30px;gap:1rem;align-items:center;margin-bottom:1rem}
    .cart-item img{width:60px;height:60px;object-fit:cover;border-radius:var(--radius)}

    /* ---------- FORM ---------- */
    .form{display:grid;gap:1rem;max-width:600px;margin-inline:auto}
    .form label{font-weight:600;margin-bottom:.25rem}
    .form input,.form textarea{width:100%;padding:.75rem;border:1px solid #ccc;border-radius:var(--radius)}
    .form input:focus,.form textarea:focus{outline:2px solid var(--accent)}

    /* ---------- FOOTER ---------- */
    .footer{background:var(--primary);color:var(--light);padding:3rem 0 1rem}
    .footer__grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:2rem}
    .footer__social{display:flex;gap:1rem;font-size:1.5rem}
    .footer__bottom{text-align:center;margin-top:2rem;font-size:.875rem}

    /* ---------- RESPONSIVE ---------- */
    @media(max-width:768px){.nav ul{flex-direction:column;gap:1rem}.cart-panel{width:100%;right:-100%}}
  </style>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&family=Noto+Sans+Arabic:wght@400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
</head>
<body data-theme="light" data-lang="fr">

  <!-- HEADER -->
  <header class="header">
    <div class="container header__inner">
      <a href="#home" class="logo">Textile Raach</a>
      <nav class="nav">
        <ul>
          <li><a href="#catalogue" data-i18n="nav.catalogue">Catalogue</a></li>
          <li><a href="#showroom" data-i18n="nav.showroom">Showroom</a></li>
          <li><a href="#devis" data-i18n="nav.devis">Devis</a></li>
          <li><a href="#contact" data-i18n="nav.contact">Contact</a></li>
          <li><button id="langBtn" aria-label="Changer langue">عربية</button></li>
          <li><button id="themeBtn" aria-label="Dark mode"><i class="fa-solid fa-circle-half-stroke"></i></button></li>
        </ul>
      </nav>
      <div class="header__actions">
        <button id="cartBtn" aria-label="Panier"><i class="fa-solid fa-bag-shopping"></i><span id="cartCount" class="cart-count">0</span></button>
      </div>
    </div>
  </header>

  <!-- HERO -->
  <section id="home" class="hero">
    <div class="hero__content container">
      <h1 class="hero__title" data-i18n="hero.title">Tissus d’ameublement haut de gamme</h1>
      <p class="hero__subtitle" data-i18n="hero.subtitle">Découvrez notre collection moderne et vibrante, inspirée du savoir-faire tunisien.</p>
      <a href="#catalogue" class="btn" data-i18n="hero.cta">Voir le catalogue</a>
    </div>
  </section>

  <!-- CATALOGUE -->
  <section id="catalogue" class="section catalogue">
    <div class="container">
      <h2 class="section__title" data-i18n="catalogue.title">Nos Tissus</h2>
      <div class="filters">
        <button class="filter-btn active" data-filter="all" data-i18n="filter.all">Tous</button>
        <button class="filter-btn" data-filter="velours">Velours</button>
        <button class="filter-btn" data-filter="lin">Linge</button>
        <button class="filter-btn" data-filter="soie">Soie</button>
        <button class="filter-btn" data-filter="jacquard">Jacquard</button>
      </div>
      <div id="catalogueGrid" class="catalogue__grid"></div>
    </div>
  </section>

  <!-- SHOWROOM -->
  <section id="showroom" class="section">
    <div class="container">
      <h2 class="section__title" data-i18n="showroom.title">Showroom 360°</h2>
      <div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;">
        <iframe src="https://momento360.com/e/u/abcd1234?scene=0&view=360" style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;" allowfullscreen></iframe>
      </div>
    </div>
  </section>

  <!-- DEVIS -->
  <section id="devis" class="section">
    <div class="container">
      <h2 class="section__title" data-i18n="devis.title">Demander un devis</h2>
      <form id="devisForm" class="form">
        <label data-i18n="form.nom">Nom</label>
        <input type="text" name="nom" required>
        <label data-i18n="form.email">Email</label>
        <input type="email" name="email" required>
        <label data-i18n="form.tel">Téléphone</label>
        <input type="tel" name="tel">
        <label data-i18n="form.message">Message</label>
        <textarea name="message" rows="5" required></textarea>
        <button type="submit" class="btn" data-i18n="form.submit">Envoyer</button>
      </form>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="footer">
    <div class="container footer__grid">
      <div>
        <strong>Textile Raach</strong>
        <p data-i18n="footer.desc">Spécialiste du tissu d’ameublement en Tunisie depuis 1998.</p>
      </div>
      <div>
        <strong data-i18n="footer.contact">Contact</strong>
        <p>+216 55 123 456<br>contact@textileraach.tn<br>Tunis, Tunisie</p>
      </div>
      <div>
        <strong data-i18n="footer.follow">Suivez-nous</strong>
        <div class="footer__social">
          <a href="#"><i class="fa-brands fa-facebook"></i></a>
          <a href="#"><i class="fa-brands fa-instagram"></i></a>
        </div>
      </div>
    </div>
    <div class="footer__bottom">
      <p>&copy; 2025 Textile Raach - تريكس رعش</p>
    </div>
  </footer>

  <!-- PANIER OFF-CANVAS -->
  <aside id="cartPanel" class="cart-panel">
    <header class="cart-panel__header">
      <h3 data-i18n="cart.title">Mon panier</h3>
      <button id="closeCart" aria-label="Fermer"><i class="fa-solid fa-xmark"></i></button>
    </header>
    <div id="cartItems" class="cart-panel__body"></div>
    <footer class="cart-panel__footer">
      <button id="downloadDevis" class="btn" data-i18n="cart.download">Télécharger le devis PDF</button>
    </footer>
  </aside>

  <!-- SCRIPTS -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
  <script>
    /* ---------- TRADUCTIONS ---------- */
    const tr = {
      fr: {
        "nav.catalogue": "Catalogue", "nav.showroom": "Showroom", "nav.devis": "Devis", "nav.contact": "Contact",
        "hero.title": "Tissus d’ameublement haut de gamme", "hero.subtitle": "Découvrez notre collection moderne et vibrante, inspirée du savoir-faire tunisien.", "hero.cta": "Voir le catalogue",
        "catalogue.title": "Nos Tissus", "filter.all": "Tous", "cart.title": "Mon panier", "cart.download": "Télécharger le devis PDF",
        "devis.title": "Demander un devis", "form.nom": "Nom", "form.email": "Email", "form.tel": "Téléphone", "form.message": "Message", "form.submit": "Envoyer",
        "footer.desc": "Spécialiste du tissu d’ameublement en Tunisie depuis 1998.", "footer.contact": "Contact", "footer.follow": "Suivez-nous"
      },
      ar: {
        "nav.catalogue": "كتالوج", "nav.showroom": "صالة عرض", "nav.devis": "عرض سعر", "nav.contact": "اتصل",
        "hero.title": "أقمشة أثاث فاخرة", "hero.subtitle": "اكتشف مجموعتنا الحديثة والنابضة بالحياة، مستوحاة من الخبرة التونسية.", "hero.cta": "عرض الكتالوج",
        "catalogue.title": "أقمشتنا", "filter.all": "الكل", "cart.title": "سلتي", "cart.download": "تحميل عرض السعر PDF",
        "devis.title": "اطلب عرض سعر", "form.nom": "الاسم", "form.email": "البريد الإلكتروني", "form.tel": "الهاتف", "form.message": "الرسالة", "form.submit": "إرسال",
        "footer.desc": "متخصص في أقمشة الأثاث بتونس منذ 1998.", "footer.contact": "اتصل", "footer.follow": "تابعنا"
      }
    };

    /* ---------- PRODUITS ---------- */
    const PRODUCTS = [
      {id:1, name:'Velours Luxe', cat:'velours', price:38, img:'https://source.unsplash.com/400x300/?velvet,fabric'},
      {id:2, name:'Linge Naturel', cat:'lin', price:29, img:'https://source.unsplash.com/400x300/?linen,fabric'},
      {id:3, name:'Soie Royale', cat:'soie', price:55, img:'https://source.unsplash.com/400x300/?silk,fabric'},
      {id:4, name:'Jacquard Tradition', cat:'jacquard', price:42, img:'https://source.unsplash.com/400x300/?jacquard,fabric'}
    ];

    /* ---------- PANIER ---------- */
    let cart = JSON.parse(localStorage.getItem('raachCart')) || [];
    function saveCart(){localStorage.setItem('raachCart', JSON.stringify(cart));}
    function addToCart(id){
      const p = PRODUCTS.find(x=>x.id===id);
      const ex = cart.find(x=>x.id===id);
      ex ? ex.qty++ : cart.push({...p, qty:1});
      saveCart(); renderCart(); openCart();
    }
    function renderCart(){
      const cont = document.getElementById('cartItems'), count = document.getElementById('cartCount');
      cont.innerHTML = '';
      if(!cart.length){ cont.innerHTML = '<p>Panier vide</p>'; count.textContent = 0; return; }
      let tot = 0;
      cart.forEach(i=>{
        tot += i.price * i.qty;
        cont.innerHTML += `
          <div class="cart-item">
            <img src="${i.img}" alt="">
            <div>
              <h4>${i.name}</h4>
              <p>${i.price} DT x ${i.qty}</p>
            </div>
            <button onclick="removeFromCart(${i.id})"><i class="fa-solid fa-trash"></i></button>
          </div>`;
      });
      count.textContent = cart.reduce((s,i)=>s+i.qty,0);
    }
    function removeFromCart(id){ cart = cart.filter(i=>i.id!==id); saveCart(); renderCart(); }
    function openCart(){ document.getElementById('cartPanel').classList.add('open'); }
    function closeCart(){ document.getElementById('cartPanel').classList.remove('open'); }
    document.getElementById('cartBtn').addEventListener('click', openCart);
    document.getElementById('closeCart').addEventListener('click', closeCart);

    /* ---------- FILTRES ---------- */
    function renderProducts(filter){
      const grid = document.getElementById('catalogueGrid');
      grid.innerHTML = '';
      const list = filter==='all' ? PRODUCTS : PRODUCTS.filter(p=>p.cat===filter);
      list.forEach(p=>{
        grid.innerHTML += `
          <div class="product-card">
            <img src="${p.img}" alt="${p.name}" class="product-card__img">
            <div class="product-card__body">
              <h3 class="product-card__title">${p.name}</h3>
              <p class="product-card__price">${p.price} DT/m</p>
              <button class="btn product-card__btn" onclick="addToCart(${p.id})">Ajouter</button>
            </div>
          </div>`;
      });
    }
    document.querySelectorAll('.filter-btn').forEach(btn=>{
      btn.addEventListener('click',()=>{
        document.querySelectorAll('.filter-btn').forEach(b=>b.classList.remove('active'));
        btn.classList.add('active');
        renderProducts(btn.dataset.filter);
      });
    });

    /* ---------- DEVIS PDF ---------- */
    document.getElementById('devisForm').addEventListener('submit', e=>{
      e.preventDefault();
      const {jsPDF} = window.jspdf;
      const doc = new jsPDF();
      const data = new FormData(e.target);
      doc.text('Devis Textile Raach', 20, 20);
      doc.text(`Nom : ${data.get('nom')}`, 20, 40);
      doc.text(`Email : ${data.get('email')}`, 20, 50);
      doc.text(`Téléphone : ${data.get('tel')}`, 20, 60);
      doc.text(`Message : ${data.get('message')}`, 20, 70);
      let y = 90;
      cart.forEach(i=>{ y+=10; doc.text(`${i.name} - ${i.qty} m - ${(i.price*i.qty).toFixed(2)} DT`, 20, y); });
      doc.save('devis-raach.pdf');
    });
    document.getElementById('downloadDevis').addEventListener('click',()=>{
      const {jsPDF} = window.jspdf;
      const doc = new jsPDF();
      doc.text('Devis Provisoire - Raach', 20, 20);
      let y = 40;
      cart.forEach(i=>{ y+=10; doc.text(`${i.name} - ${i.qty} m - ${(i.price*i.qty).toFixed(2)} DT`, 20, y); });
      doc.text(`Total : ${cart.reduce((s,i)=>s+i.price*i.qty,0).toFixed(2)} DT`, 20, y+10);
      doc.save('devis-raach.pdf');
    });

    /* ---------- LANGUE / THEME ---------- */
    document.getElementById('langBtn').addEventListener('click',()=>{
      const html = document.documentElement;
      const next = html.lang === 'fr' ? 'ar' : 'fr';
      html.lang = next; html.dir = next==='ar' ? 'rtl' : 'ltr';
      translate(next);
    });
    function translate(lang){
      document.querySelectorAll('[data-i18n]').forEach(el=>{
        const key = el.getAttribute('data-i18n');
        if(tr[lang][key]) el.textContent = tr[lang][key];
      });
    }
    document.getElementById('themeBtn').addEventListener('click',()=>{
      const body = document.body;
      const next = body.getAttribute('data-theme') === 'light' ? 'dark' : 'light';
      body.setAttribute('data-theme', next);
      localStorage.setItem('theme', next);
    });

    /* ---------- INIT ---------- */
    renderProducts('all');
    renderCart();
    translate('fr');
  </script>
</body></html>
