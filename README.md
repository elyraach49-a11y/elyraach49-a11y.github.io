<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Textile Raach - Tissus d'ameublement en Tunisie</title>
  <style>
    :root {
      --primary: #d35400;
      --secondary: #f4f4f4;
      --accent: #f39c12;
      --text: #333;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--secondary);
      color: var(--text);
    }

    header {
      background-color: white;
      padding: 20px 40px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    header .logo {
      font-size: 24px;
      font-weight: bold;
      color: var(--primary);
    }

    nav {
      float: right;
      margin-top: -30px;
    }

    nav a {
      margin-left: 20px;
      text-decoration: none;
      color: var(--text);
      font-weight: 500;
    }

    nav a:hover {
      color: var(--accent);
    }

    .hero {
      background: url('https://source.unsplash.com/1600x600/?fabric,sofa') center/cover no-repeat;
      color: white;
      padding: 100px 40px;
      text-align: center;
    }

    .hero h1 {
      font-size: 48px;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: 20px;
      margin-bottom: 30px;
    }

    .btn {
      background-color: var(--primary);
      color: white;
      padding: 15px 30px;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
    }

    .btn:hover {
      background-color: var(--accent);
    }

    .section {
      padding: 60px 40px;
    }

    .section h2 {
      text-align: center;
      margin-bottom: 40px;
      font-size: 32px;
      color: var(--primary);
    }

    .products {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }

    .product-card {
      background: white;
      border-radius: 8px;
      width: 250px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      overflow: hidden;
      text-align: center;
    }

    .product-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .product-card h3 {
      margin: 15px 0 5px;
      font-size: 20px;
    }

    .product-card p {
      padding: 0 10px 20px;
      color: #666;
    }

    footer {
      background-color: var(--primary);
      color: white;
      text-align: center;
      padding: 20px;
    }

    @media (max-width: 768px) {
      nav {
        float: none;
        text-align: center;
        margin-top: 10px;
      }

      .hero h1 {
        font-size: 32px;
      }
    }
  </style>
</head>
<body>

  <header>
    <div class="logo">Textile Raach</div>
    <nav>
      <a href="#home">Accueil</a>
      <a href="#products">Produits</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="home" class="hero">
    <h1>Tissus d'ameublement haut de gamme</h1>
    <p>Découvrez notre collection moderne et élégante, adaptée au goût tunisien.</p>
    <a href="#products" class="btn">Voir les produits</a>
  </section>

  <section id="products" class="section">
    <h2>Nos Tissus</h2>
    <div class="products">
      <div class="product-card">
        <img src="https://source.unsplash.com/250x200/?velvet,fabric" alt="Velours">
        <h3>Velours Luxe</h3>
        <p>Idéal pour canapés et rideaux. Disponible en plusieurs couleurs.</p>
      </div>
      <div class="product-card">
        <img src="https://source.unsplash.com/250x200/?linen,fabric" alt="Linge">
        <h3>Linge Naturel</h3>
        <p>Respirant et élégant, parfait pour l'été tunisien.</p>
      </div>
      <div class="product-card">
        <img src="https://source.unsplash.com/250x200/?jacquard,fabric" alt="Jacquard">
        <h3>Jacquard Moderne</h3>
        <p>Motifs traditionnels revisités pour un intérieur chic.</p>
      </div>
      <div class="product-card">
        <img src="https://source.unsplash.com/250x200/?silk,fabric" alt="Soie">
        <h3>Soie Royale</h3>
        <p>Pour un toucher luxueux et une finissement haut de gamme.</p>
      </div>
    </div>
  </section>

  <footer id="contact">
    <p>Contactez-nous : +216 55 123 456 | Email : contact@textileraach.tn</p>
    <p>&copy; 2025 Textile Raach - Tous droits réservés.</p>
  </footer>

</body>
</html>
