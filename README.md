<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
  <title>Закупка запчастей • Автосервис</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Roboto, system-ui, sans-serif;
    }

    body {
      background: #1a1a1a;
      background-image: radial-gradient(circle at 20% 30%, #3a3a3a 0%, #0d0d0d 100%);
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
      background: rgba(35, 35, 35, 0.92);
      backdrop-filter: blur(6px);
      -webkit-backdrop-filter: blur(6px);
      border-radius: 2rem;
      padding: 1.5rem 1.2rem;
      box-shadow: 0 25px 50px -8px rgba(0, 0, 0, 0.9), inset 0 1px 2px rgba(200, 200, 200, 0.08);
      border: 1px solid #555555;
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
      border-bottom: 2px solid #555555;
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
      color: #cccccc;
      background: #2a2a2a;
      padding: 0.3rem 0.7rem;
      border-radius: 60px;
      border: 1px solid #666666;
      flex-shrink: 0;
    }

    .header h1 {
      font-size: 1.5rem;
      font-weight: 600;
      letter-spacing: 0.5px;
      color: #e0e0e0;
      text-shadow: 0 4px 10px #0a0a0a;
      line-height: 1.2;
    }

    .header h1 .highlight {
      color: #cccccc;
      background: #2a2a2a;
      padding: 0 0.4rem;
      border-radius: 40px;
      font-weight: 500;
      border: 1px solid #666666;
    }

    .header .tag {
      background: #333333;
      padding: 0.3rem 0.8rem;
      border-radius: 60px;
      color: #d0d0d0;
      font-weight: 500;
      border: 1px solid #777777;
      font-size: 0.7rem;
      display: flex;
      align-items: center;
      gap: 4px;
      white-space: nowrap;
    }

    .tag i { color: #aaaaaa; font-size: 0.8rem; }

    .mission-statement {
      background: #252525;
      border-radius: 1.5rem;
      padding: 0.8rem 1.2rem;
      margin-bottom: 1.5rem;
      border-left: 4px solid #888888;
      color: #c0c0c0;
      font-size: 0.9rem;
      line-height: 1.5;
      box-shadow: inset 0 2px 6px #0a0a0a;
      text-align: left;
    }

    .mission-statement i { color: #888888; font-size: 1.2rem; margin-right: 6px; }
    .mission-statement strong { color: #e8e8e8; }

    .grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 0.8rem;
      margin: 1.2rem 0 1.8rem;
    }

    .sample-card {
      background: #2a2a2a;
      background: linear-gradient(145deg, #353535, #222222);
      border-radius: 1.5rem;
      padding: 0.8rem 0.5rem 1rem;
      box-shadow: 0 8px 12px -6px #0a0a0a, inset 0 -2px 0 #4a4a4a;
      border: 1px solid #4a4a4a;
      text-align: center;
      transition: 0.2s;
    }

    .sample-card:active {
      transform: scale(0.97);
    }

    .sample-card .icon { font-size: 2rem; color: #aaaaaa; margin-bottom: 0.2rem; }
    .sample-card h3 { color: #e0e0e0; font-size: 0.85rem; font-weight: 500; }
    .sample-card p { color: #909090; font-size: 0.7rem; margin-top: 0.1rem; }

    .call-block {
      background: #252525;
      border-radius: 2rem;
      padding: 1.2rem 1.2rem;
      border: 1px solid #4a4a4a;
      box-shadow: inset 0 2px 8px #0a0a0a;
      margin-bottom: 0.5rem;
    }

    .call-block .sub-text {
      color: #a0a0a0;
      font-size: 0.8rem;
      margin-bottom: 0.9rem;
    }

    .btn-telegram {
      border: none;
      border-bottom: 2px solid #333333;
      padding: 0.6rem 1.2rem;
      border-radius: 60px;
      font-size: 0.95rem;
      font-weight: 600;
      color: #f0f0f0;
      text-shadow: 0 2px 3px #0a0a0a;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      cursor: pointer;
      transition: 0.15s;
      background: linear-gradient(145deg, #555555, #3a3a3a);
      box-shadow: 0 3px 0 #2a2a2a, 0 4px 10px #0a0a0a;
      letter-spacing: 0.3px;
      width: auto;
      min-width: 200px;
      text-decoration: none;
      color: #f0f0f0;
    }

    .btn-telegram:active {
      transform: translateY(2px);
      border-bottom-width: 1px;
      box-shadow: 0 1px 0 #2a2a2a;
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
      color: #909090;
      border-top: 1px solid #3a3a3a;
      padding-top: 1rem;
      gap: 0.5rem 1.5rem;
      font-size: 0.75rem;
      text-align: center;
    }

    .footer-note i { color: #6a6a6a; margin-right: 4px; }
    .footer-note .badge {
      background: #252525;
      padding: 0.2rem 1rem;
      border-radius: 60px;
      border: 1px solid #4a4a4a;
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
      <span class="icon-big"><i class="fas fa-car"></i></span>
      <h1><span class="highlight">Автосервис</span> Закуп</h1>
    </div>
    <div class="tag">
      <i class="fas fa-truck"></i> Скупаем
    </div>
  </div>

  <div class="mission-statement">
    <i class="fas fa-handshake"></i>
    <span><strong>Скупаем запчасти от автомобилей</strong> для ремонта грузовой, специальной техники, УАЗов и Газелей. Работаем с частными лицами и организациями.</span>
  </div>

  <div style="margin-bottom: 0.3rem; text-align: left;">
    <span style="color: #909090; font-size: 0.8rem;">
      <i class="fas fa-tools"></i> что скупаем:
    </span>
  </div>
  <div class="grid">
    <div class="sample-card"><div class="icon"><i class="fas fa-car-side"></i></div><h3>Запчасти</h3><p>оригинал и аналоги</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-microchip"></i></div><h3>Электроника</h3><p>датчики, блоки, проводка</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-gear"></i></div><h3>Коробки передач</h3><p>механика, автомат</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-cogs"></i></div><h3>Двигатели</h3><p>дизель, бензин</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-truck"></i></div><h3>Для УАЗов</h3><p>все модели</p></div>
    <div class="sample-card"><div class="icon"><i class="fas fa-truck"></i></div><h3>Для Газелей</h3><p>б/у и новые</p></div>
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
    <span class="badge"><i class="fas fa-envelope"></i> zakup@avto.ru</span>
    <span><i class="fas fa-car"></i> автосервис</span>
  </div>
</div>
</body>
</html>
