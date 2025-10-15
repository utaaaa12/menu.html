# menu.html
<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Dimsum Cihuy — Menu</title>

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg: #0f0f10;
      --panel: #0d0d0d;
      --gold: #d9b573;
      --muted: #b9a786;
      --accent: #ffffff;
      --maxwidth: 880px;
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: "Poppins", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: linear-gradient(180deg, var(--bg) 0%, #0b0b0b 100%);
      color: var(--accent);
      display:flex;
      align-items:center;
      justify-content:center;
      padding:40px 18px;
    }

    .menu-card{
      width:100%;
      max-width:var(--maxwidth);
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.00));
      border-radius:14px;
      padding:34px 44px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.7);
      border: 1px solid rgba(217,181,115,0.08);
    }

    .brand{
      text-align:center;
      margin-bottom:22px;
    }
    .brand-content{
      display:flex;
      align-items:center;
      justify-content:center;
      gap:15px;
    }
    .brand img{
      width:80px;
      height:auto;
      border-radius:8px;
    }
    .brand h1{
      font-family: "Playfair Display", serif;
      font-size:42px;
      letter-spacing:1px;
      margin:0;
      color:var(--gold);
      font-weight:700;
      text-transform:uppercase;
    }
    .brand p{
      margin:5px 0 0;
      color:var(--muted);
      font-style:italic;
      font-size:15px;
    }

    .divider{
      height:1px;
      background: linear-gradient(90deg, rgba(217,181,115,0.08), rgba(217,181,115,0.14), rgba(217,181,115,0.08));
      margin:20px 0 24px;
      border-radius:2px;
    }

    .section-title{
      font-family: "Playfair Display", serif;
      font-size:20px;
      color:var(--gold);
      margin:6px 0 14px;
      letter-spacing:1px;
      text-transform:uppercase;
    }

    .menu-list{
      display:flex;
      flex-direction:column;
      gap:12px;
    }

    .item{
      display:flex;
      justify-content:space-between;
      align-items:flex-start;
      gap:16px;
    }
    .item .meta{
      max-width:calc(100% - 110px);
    }
    .item .name{
      color:var(--gold);
      font-weight:600;
      font-size:18px;
      font-family: "Playfair Display", serif;
      margin:0 0 4px;
    }
    .item .desc{
      margin:0;
      color:var(--muted);
      font-size:13px;
      line-height:1.35;
    }
    .item .price{
      color:var(--gold);
      font-weight:600;
      min-width:90px;
      text-align:right;
      font-size:16px;
    }

    .note{
      margin-top:30px;
      padding-top:16px;
      border-top:1px solid rgba(217,181,115,0.06);
      color:var(--muted);
      font-size:13px;
      display:flex;
      justify-content:space-between;
      flex-wrap:wrap;
      gap:10px;
    }

    @media (max-width:700px){
      .brand-content{ flex-direction:column; }
      .brand h1{ font-size:34px; }
      .brand img{ width:70px; }
    }

    @media print{
      body{ background:white; color:black; }
      .menu-card{ box-shadow:none; border:none; background:white; }
      .item .price{ color:black; }
      .brand h1{ color:black; }
    }
  </style>
</head>

<body>

  <article class="menu-card" role="region" aria-label="Menu Dimsum Cihuy">
    <header class="brand">
      <div class="brand-content">
        <img src="C77D4E8D-8EFE-4EC3-8625-FD08B67FF256.jpeg" alt="Logo Dimsum Cihuy">
        <div>
          <h1>Dimsum Cihuy</h1>
          <p>Pasti Enak Euy!</p>
        </div>
      </div>
    </header>

    <div class="divider"></div>

    <section aria-labelledby="menu-title">
      <h2 id="menu-title" class="section-title">Menu Dimsum</h2>

      <div class="menu-list">
        <div class="item">
          <div class="meta">
            <h3 class="name">Dimsum Original</h3>
            <p class="desc">Rasa klasik dengan bumbu gurih lembut khas Dimsum Cihuy.</p>
          </div>
          <div class="price">Rp15.000</div>
        </div>

        <div class="item">
          <div class="meta">
            <h3 class="name">Dimsum Chili Oil</h3>
            <p class="desc">Pedas gurih dengan sensasi chili oil homemade yang menggoda.</p>
          </div>
          <div class="price">Rp25.000</div>
        </div>

        <div class="item">
          <div class="meta">
            <h3 class="name">Dimsum Mentai</h3>
            <p class="desc">Lelehan saus mentai creamy di atas dimsum lembut — favorit anak muda!</p>
          </div>
          <div class="price">Rp25.000</div>
        </div>

        <div class="item">
          <div class="meta">
            <h3 class="name">Dimsum Mix</h3>
            <p class="desc">Perpaduan semua varian dalam satu porsi — cocok untuk sharing!</p>
          </div>
          <div class="price">Rp25.000</div>
        </div>
      </div>
    </section>

    <footer class="note">
      <div>• Semua dimsum dibuat <em>fresh</em> setiap hari<br>• Free sambal & saus oriental</div>
      <div>📍 KP.RancaHaur Desa Karang Tengah Kabupaten Tangerang | 📞 089516486819
    </footer>
  </article>

</body>
</html>
