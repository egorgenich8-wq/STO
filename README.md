
запасные части агрегаты
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
  <title>Закупка продуктов • Столовая</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Roboto, system-ui, sans-serif;
    }

    body {
      background: #1a2e1a;
      background-image: radial-gradient(circle at 20% 30%, #2d4a2d 0%, #0f1f0f 100%);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 0.8rem;
    }

    .site-card {
      max-width: 100%;
      width: 100%;
      max-width: 500px;
      background: rgba(40, 60, 40, 0.92);
      backdrop-filter: blur(6px);
      -webkit-backdrop-filter: blur(6px);
      border-radius: 2rem;
      padding: 1.5rem 1.2rem;
      box-shadow: 0 25px 50px -8px rgba(0, 0, 0, 0.8), inset 0 1px 2px rgba(200, 255, 200, 0.15);
      border: 1px solid #5a7a5a;
      margin: 0 auto;
      overflow-x: hidden;
      text-align: center;
    }

    .header {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      margin-bottom: 1.5rem;
      border-bottom: 2px solid #5a7a5a;
      padding-bottom: 0.8rem;
      gap: 0.5rem;
    }

    .header-left {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .header-left .icon-big {
      font-size: 2rem;
      color: #b8e0b8;
      background: #1e3a1e;
      padding: 0.3rem 0.7rem;
      border-radius: 60px;
      border: 1px solid #5a8a5a;
      flex-shrink: 0;
    }

    .header h1 {
      font-size: 1.5rem;
      font-weight: 600;
      letter-spacing: 0.5px;
      color: #e0f0e0;
      text-shadow: 0 4px 10px #0a1a0a;
      line-height: 1.2;
    }

    .header h1 .highlight {
      color: #b8e0b8;
      background: #1e3a1e;
      padding: 0 0.4rem;
      border-radius: 40px;
      font-weight: 500;
      border: 1px solid #4a7a4a;
    }

    .header .tag {
      background: #2a4a2a;
      padding: 0.3rem 0.8rem;
      border-radius: 60px;
      color: #d0ecd0;
      font-weight: 500;
      border: 1px solid #6a9a6a;
      font-size: 0.7rem;
      display: flex;
      align-items: center;
      gap: 4px;
      white-space: nowrap;
    }

    .tag i { color: #a0d0a0; font-size: 0.8rem; }

    .mission-statement {
      background: #1e3a1e;
      border-radius: 1.5rem;
      padding: 0.8rem 1.2rem;
      margin-bottom: 1.5rem;
      border-left: 4px solid #7ab07a;
      color: #c0e0c0;
      font-size: 0.9rem;
      line-height: 1.5;
      box-shadow: inset 0 2px 6px #0a1a0a;
      text-align: left;
    }

    .mission-statement i { color: #7ab07a; font-size: 1.2rem; margin-right: 6px; }
    .mission-statement strong { color: #e0f5e0; }

    .grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 0.8rem;
      margin: 1.2rem 0 1.8rem;
    }

    .sample-card {
      background: #2a462a;
      background: linear-gradient(145deg, #325232, #1e3a1e);
      border-radius: 1.5rem;
      padding: 0.8rem 0.5rem 1rem;
      box-shadow: 0 8px 12px -6px #0a1a0a, inset 0 -2px 0 #4a7a4a;
      border: 1px solid #4a7a4a;
      text-align: center;
      transition: 0.2s;
    }

    .sample-card:active {
      transform: scale(0.97);
    }

    .sample-card .icon { font-size: 2rem; color: #a0d0a0; margin-bottom: 0.2rem; }
    .sample-card h3 { color: #e0f0e0; font-size: 0.85rem; font-weight: 500; }
    .sample-card p { color: #90b890; font-size: 0.7rem; margin-top: 0.1rem; }

    .call-block {
      background: #1e3a1e;
      border-radius: 2rem;
      padding: 1.2rem 1.2rem;
      border: 1px solid #4a7a4a;
      box-shadow: inset 0 2px 8px #0a1a0a;
      margin-bottom: 0.5rem;
    }

    .call-block .sub-text {
      color: #a0c8a0;
      font-size: 0.8rem;
      margin-bottom: 0.9rem;
    }

    .btn-telegram {
      border: none;
      border-bottom: 2px solid #0d4a0d;
      padding: 0.6rem 1.2rem;
      border-radius: 60px;
      font-size: 0.95rem;
      font-weight: 600;
      color: #f0fff0;
      text-shadow: 0 2px 3px #0a1a0a;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      cursor: pointer;
      transition: 0.15s;
      background: linear-gradient(145deg, #2d8a2d, #1a6a1a);
      box-shadow: 0 3px 0 #0d4a0d, 0 4px 10px #0a1a0a;
      letter-spacing: 0.3px;
      width: auto;
      min-width: 200px;
      text-decoration: none;
      color: #f0fff0;
    }

    .btn-telegram:active {
      transform: translateY(2px);
      border-bottom-width: 1px;
      box-shadow: 0 1px 0 #0d4a0d;
    }

    .btn-telegram i {
      font-size: 1.2rem;
      color: #fff;
    }

    .btn-telegram:hover {
      opacity: 0.9;
    }

    .footer-note {
      margin-top: 1.5rem;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      color: #90b890;
      border-top: 1px solid #3a5a3a;
      padding-top: 1rem;
      gap: 0.5rem 1.5rem;
      font-size: 0.75rem;
      text-align: center;
    }

    .footer-note i { color: #6a9a6a; margin-right: 4px; }
    .footer-note .badge {
      background: #1e3a1e;
      padding: 0.2rem 1rem;
      border-radius: 60px;
      border: 1px solid #4a7a4a;
    }

    @media (max-width: 400px) {
      .site-card { padding: 1rem 0.8rem; }
      .header h1 { font-size: 1.2rem; }
      .header-left .icon-big { font-size: 1.4rem; padding: 0.2rem 0.4rem; }
      .header .tag { font-size: 0.6rem; padding: 0.2rem 0.6rem; }
      .mission-statement { font-size: 0.75rem; padding: 0.6rem 0.8rem; }
      .grid { gap: 0.5rem; }
      .sample-card .icon { font-size: 1.6rem; }
      .sample-card h3 { font-size: 0.75rem; }
      .sample-card p { font-size: 0.6rem; }
      .btn-telegram {
        font-size: 0.85rem;
        padding: 0.5rem 1rem;
        min-width: 160px;
      }
      .btn-telegram i { font-size: 1rem; }
    }

    @media (max-width: 360px) {
      .grid { grid-template-columns: 1fr 1fr; gap: 0.4rem; }
      .sample-card { padding: 0.5rem 0.3rem; }
      .btn-telegram {
        font-size: 0.75rem;
        padding: 0.4rem 0.8rem;
        min-width: 140px;
        gap: 6px;
      }
    }
  </style>
</head>
<body>
<div class="site-card">

  <div class="header">
    <div class="header-left">
      <span class="icon-big"><i class="fas fa-utensils"></i></span>
      <h1><span class="highlight">Столовая</span> Закуп</h1>
    </div>
    <div class="tag">
      <i class="fas fa-truck"></i> Покупаем
    </div>
  </div>

  <div class="mission-statement">
    <i class="fas fa-handshake"></i>
    <span><strong>Скупаем продукты питания</strong> для использования в приготовлении пищи в столовой. Работаем с частными лицами и организациями.</span>
  </div>

  <div style="margin-bottom: 0.3rem; text-align: left;">
    <span style="color: #90b890; font-size: 0.8rem;">
      <i class="fas fa-shopping-basket"></i> что закупаем:
    </span>
  </div>
  <div class="grid">
    <div class="sample-card"><div class="icon"><i class="fas fa-drumstick-bite"></i></div><h3>Мясо</h3><p>говядина, свинина, птица</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-egg"></i></div><h3>Тушенка</h3><p>говяжья, свиная</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-oil-can"></i></div><h3>Масло</h3><p>сливочное, растительное</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-cube"></i></div><h3>Сахар</h3><p>песок, рафинад</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-wheat-awn"></i></div><h3>Крупы</h3><p>гречка, рис, овсянка</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-carrot"></i></div><h3>Овощи</h3><p>картофель, лук, морковь</p></div>
  </div>

  <div class="call-block">
    <div class="sub-text">
      <i class="fas fa-tag"></i> Цена договорная — обсудим всё в Telegram
    </div>

    <a href="https://t.me/crom_45" target="_blank" class="btn-telegram">
      <i class="fab fa-telegram-plane"></i> Написать в Telegram
    </a>
  </div>

  <div class="footer-note">
    <span class="badge"><i class="fas fa-envelope"></i> zakup@stolovaya.ru</span>
    <span><i class="fas fa-utensils"></i> столовая</span>
  </div>
</div>
</body>
</html>
