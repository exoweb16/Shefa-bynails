
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Shefa bynails | Estudio de Uñas en Saltillo</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,500;0,600;1,500&family=Plus+Jakarta+Sans:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-cream: #faf7f4;
      --bg-card: #ffffff;
      --bg-soft: #f3ece6;
      --ink-dark: #152420;
      --ink-muted: #5b6662;
      --accent-rose: #c97b76;
      --accent-rose-dark: #ab615c;
      --border-soft: #e7ddd5;
      --whatsapp: #1fa855;
      --whatsapp-hover: #178a44;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, sans-serif;
      background-color: var(--bg-cream);
      color: var(--ink-dark);
      line-height: 1.65;
      -webkit-font-smoothing: antialiased;
    }

    .container {
      width: 100%;
      max-width: 980px;
      margin: 0 auto;
      padding: 0 20px;
    }

    /* Encabezado */
    header {
      position: sticky;
      top: 0;
      z-index: 50;
      background: rgba(250, 247, 244, 0.92);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid var(--border-soft);
    }

    .nav-inner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 12px 0;
      gap: 16px;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 12px;
      text-decoration: none;
      color: var(--ink-dark);
    }

    .brand-logo {
      width: 50px;
      height: 50px;
      flex-shrink: 0;
    }

    .brand-name {
      font-family: 'Cormorant Garamond', Georgia, serif;
      font-size: 1.45rem;
      font-weight: 600;
      letter-spacing: 0.02em;
      display: block;
      line-height: 1.1;
    }

    .brand-sub {
      font-size: 0.75rem;
      color: var(--ink-muted);
      letter-spacing: 0.06em;
      text-transform: uppercase;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 22px;
    }

    .nav-links a {
      text-decoration: none;
      color: var(--ink-dark);
      font-size: 0.92rem;
      font-weight: 500;
      transition: color 0.2s ease;
    }

    .nav-links a:hover {
      color: var(--accent-rose-dark);
    }

    .btn-wa {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      background-color: var(--whatsapp);
      color: #ffffff;
      text-decoration: none;
      font-weight: 600;
      font-size: 0.92rem;
      padding: 11px 18px;
      border-radius: 999px;
      transition: transform 0.2s ease, background-color 0.2s ease, box-shadow 0.2s ease;
      box-shadow: 0 6px 18px rgba(31, 168, 85, 0.22);
    }

    .btn-wa:hover {
      background-color: var(--whatsapp-hover);
      transform: translateY(-1px);
    }

    /* Hero */
    .hero {
      padding: 56px 0 48px;
      text-align: center;
    }

    .hero-badge {
      display: inline-block;
      background-color: var(--bg-soft);
      color: var(--accent-rose-dark);
      border: 1px solid var(--border-soft);
      padding: 6px 16px;
      border-radius: 999px;
      font-size: 0.85rem;
      font-weight: 600;
      margin-bottom: 20px;
    }

    .hero-logo-wrap {
      display: flex;
      justify-content: center;
      margin-bottom: 18px;
    }

    .hero-logo {
      width: 148px;
      height: 148px;
      background: #ffffff;
      border-radius: 50%;
      padding: 10px;
      border: 1px solid var(--border-soft);
      box-shadow: 0 12px 30px rgba(21, 36, 32, 0.06);
    }

    .hero h1 {
      font-family: 'Cormorant Garamond', Georgia, serif;
      font-size: clamp(2.3rem, 5vw, 3.4rem);
      font-weight: 600;
      line-height: 1.12;
      color: var(--ink-dark);
      margin-bottom: 14px;
    }

    .hero p {
      max-width: 620px;
      margin: 0 auto 28px;
      color: var(--ink-muted);
      font-size: 1.03rem;
    }

    .hero-actions {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 14px;
    }

    .btn-wa-lg {
      padding: 14px 26px;
      font-size: 1rem;
    }

    .btn-secondary {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 14px 24px;
      border-radius: 999px;
      text-decoration: none;
      color: var(--ink-dark);
      background-color: #ffffff;
      border: 1px solid var(--border-soft);
      font-weight: 500;
      font-size: 0.98rem;
      transition: border-color 0.2s ease, background-color 0.2s ease;
    }

    .btn-secondary:hover {
      border-color: var(--ink-dark);
      background-color: var(--bg-soft);
    }

    /* Secciones */
    section {
      padding: 44px 0;
    }

    .section-header {
      text-align: center;
      margin-bottom: 28px;
    }

    .section-header h2 {
      font-family: 'Cormorant Garamond', Georgia, serif;
      font-size: clamp(1.85rem, 3.5vw, 2.5rem);
      font-weight: 600;
      color: var(--ink-dark);
      margin-bottom: 8px;
    }

    .section-header p {
      color: var(--ink-muted);
      max-width: 560px;
      margin: 0 auto;
      font-size: 0.97rem;
    }

    /* Técnicas y sistemas */
    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
      gap: 16px;
    }

    .service-card {
      background-color: var(--bg-card);
      border: 1px solid var(--border-soft);
      border-radius: 18px;
      padding: 20px 18px;
      display: flex;
      align-items: center;
      gap: 12px;
      box-shadow: 0 6px 20px rgba(21, 36, 32, 0.03);
      transition: transform 0.2s ease, border-color 0.2s ease;
    }

    .service-card:hover {
      transform: translateY(-2px);
      border-color: var(--accent-rose);
    }

    .sparkle {
      width: 34px;
      height: 34px;
      border-radius: 50%;
      background-color: var(--bg-soft);
      color: var(--accent-rose-dark);
      display: grid;
      place-items: center;
      font-size: 1rem;
      flex-shrink: 0;
    }

    .service-name {
      font-weight: 600;
      font-size: 0.98rem;
      color: var(--ink-dark);
    }

    /* Compromiso */
    .care-box {
      background-color: var(--bg-card);
      border: 1px solid var(--border-soft);
      border-radius: 24px;
      padding: 32px 26px;
      text-align: center;
      box-shadow: 0 10px 28px rgba(21, 36, 32, 0.04);
    }

    .care-box h2 {
      font-family: 'Cormorant Garamond', Georgia, serif;
      font-size: 2rem;
      margin-bottom: 12px;
    }

    .care-box p {
      max-width: 640px;
      margin: 0 auto 22px;
      color: var(--ink-muted);
    }

    /* Ubicación y Citas */
    .info-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }

    .info-card {
      background-color: var(--bg-card);
      border: 1px solid var(--border-soft);
      border-radius: 20px;
      padding: 26px 24px;
      box-shadow: 0 8px 24px rgba(21, 36, 32, 0.04);
    }

    .info-label {
      font-size: 0.78rem;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--accent-rose-dark);
      font-weight: 600;
      margin-bottom: 8px;
      display: block;
    }

    .info-card h3 {
      font-family: 'Cormorant Garamond', Georgia, serif;
      font-size: 1.55rem;
      margin-bottom: 10px;
    }

    .info-card p {
      color: var(--ink-muted);
      margin-bottom: 18px;
      font-size: 0.96rem;
    }

    .phone-highlight {
      display: block;
      font-size: 1.2rem;
      font-weight: 600;
      color: var(--ink-dark);
      margin-bottom: 16px;
      text-decoration: none;
    }

    /* Footer */
    footer {
      border-top: 1px solid var(--border-soft);
      padding: 28px 0 42px;
      text-align: center;
      color: var(--ink-muted);
      font-size: 0.88rem;
    }

    /* Botón flotante de WhatsApp */
    .floating-wa {
      position: fixed;
      right: 20px;
      bottom: 20px;
      z-index: 60;
      display: inline-flex;
      align-items: center;
      gap: 9px;
      background-color: var(--whatsapp);
      color: #ffffff;
      text-decoration: none;
      font-weight: 600;
      font-size: 0.92rem;
      padding: 13px 18px;
      border-radius: 999px;
      box-shadow: 0 10px 24px rgba(23, 138, 68, 0.35);
      transition: transform 0.2s ease, background-color 0.2s ease;
    }

    .floating-wa:hover {
      background-color: var(--whatsapp-hover);
      transform: translateY(-2px);
    }

    @media (max-width: 720px) {
      .nav-links {
        display: none;
      }

      .floating-wa span {
        display: none;
      }

      .floating-wa {
        width: 56px;
        height: 56px;
        padding: 0;
        justify-content: center;
      }
    }
  </style>
</head>
<body>

  <header>
    <div class="container nav-inner">
      <a href="#" class="brand" aria-label="Shefa bynails inicio">
        <!-- Logotipo SVG basado en el diseño circular Shefa bynails -->
        <svg class="brand-logo" viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Logo Shefa bynails">
          <circle cx="60" cy="60" r="56" fill="#ffffff" stroke="#e7ddd5" stroke-width="2"/>
          <path d="M 22 76 A 42 42 0 1 1 98 76" fill="none" stroke="#152420" stroke-width="3.2" stroke-linecap="round"/>
          <text x="60" y="65" text-anchor="middle" fill="#152420" font-family="'Cormorant Garamond', Georgia, serif" font-style="italic" font-weight="600" font-size="31">shefa</text>
          <text x="60" y="96" text-anchor="middle" fill="#152420" font-family="'Plus Jakarta Sans', sans-serif" font-weight="600" font-size="11.5" letter-spacing="3.5">BY NAILS</text>
        </svg>
        <div>
          <span class="brand-name">Shefa bynails</span>
          <span class="brand-sub">Estudio de uñas · Alejandra Castillo</span>
        </div>
      </a>

      <nav class="nav-links" aria-label="Navegación principal">
        <a href="#servicios">Servicios</a>
        <a href="#ubicacion">Ubicación</a>
        <a href="#citas">Citas</a>
      </nav>

      <a
        class="btn-wa"
        href="https://wa.me/528442111646?text=%C2%A1Hola%2C%20Alejandra!%20Vi%20la%20p%C3%A1gina%20de%20Shefa%20bynails%20y%20me%20gustar%C3%ADa%20agendar%20una%20cita."
        target="_blank"
        rel="noopener noreferrer"
      >
        WhatsApp
      </a>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container">
        <div class="hero-badge">Agenda abierta para diciembre</div>

        <div class="hero-logo-wrap">
          <svg class="hero-logo" viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Logotipo principal Shefa bynails">
            <path d="M 20 77 A 43 43 0 1 1 100 77" fill="none" stroke="#152420" stroke-width="3.4" stroke-linecap="round"/>
            <text x="60" y="65" text-anchor="middle" fill="#152420" font-family="'Cormorant Garamond', Georgia, serif" font-style="italic" font-weight="600" font-size="32">shefa</text>
            <text x="60" y="97" text-anchor="middle" fill="#152420" font-family="'Plus Jakarta Sans', sans-serif" font-weight="600" font-size="11.5" letter-spacing="3.5">BY NAILS</text>
          </svg>
        </div>

        <h1>Shefa bynails</h1>
        <p>
          ¡Hola, chicas! Bienvenidas a mi estudio de uñas con <strong>Alejandra Castillo</strong>.
          Diferentes técnicas y sistemas para consentir tus manitas y pies con dedicación y cuidado en cada detalle.
        </p>

        <div class="hero-actions">
          <a
            class="btn-wa btn-wa-lg"
            href="https://wa.me/528442111646?text=%C2%A1Hola!%20Quiero%20agendar%20una%20cita%20en%20Shefa%20bynails."
            target="_blank"
            rel="noopener noreferrer"
          >
            Agendar por WhatsApp
          </a>
          <a class="btn-secondary" href="#servicios">Ver técnicas y servicios</a>
        </div>
      </div>
    </section>

    <section id="servicios">
      <div class="container">
        <div class="section-header">
          <h2>Técnicas y sistemas</h2>
          <p>Opciones diseñadas para cuidar tus uñas naturales y lograr el acabado que buscas.</p>
        </div>

        <div class="services-grid">
          <article class="service-card">
            <span class="sparkle" aria-hidden="true">✦</span>
            <span class="service-name">Uñas acrílicas</span>
          </article>
          <article class="service-card">
            <span class="sparkle" aria-hidden="true">✦</span>
            <span class="service-name">Polygel</span>
          </article>
          <article class="service-card">
            <span class="sparkle" aria-hidden="true">✦</span>
            <span class="service-name">Dual System</span>
          </article>
          <article class="service-card">
            <span class="sparkle" aria-hidden="true">✦</span>
            <span class="service-name">Soft Gel</span>
          </article>
          <article class="service-card">
            <span class="sparkle" aria-hidden="true">✦</span>
            <span class="service-name">Rubber Base</span>
          </article>
          <article class="service-card">
            <span class="sparkle" aria-hidden="true">✦</span>
            <span class="service-name">Builder Gel</span>
          </article>
          <article class="service-card">
            <span class="sparkle" aria-hidden="true">✦</span>
            <span class="service-name">Gelish</span>
          </article>
          <article class="service-card">
            <span class="sparkle" aria-hidden="true">✦</span>
            <span class="service-name">Pediespa y pedicure</span>
          </article>
        </div>
      </div>
    </section>

    <section>
      <div class="container">
        <div class="care-box">
          <h2>Calidad y cuidado en cada detalle</h2>
          <p>
            Trabajo con dedicación, productos de calidad y mucho cuidado en cada detalle para que disfrutes de una bonita experiencia. Ya tengo agenda abierta para diciembre. ¡Será un gusto atenderlas!
          </p>
          <a
            class="btn-wa btn-wa-lg"
            href="https://wa.me/528442111646?text=%C2%A1Hola!%20Me%20interesa%20apartar%20lugar%20en%20la%20agenda%20de%20diciembre%20en%20Shefa%20bynails."
            target="_blank"
            rel="noopener noreferrer"
          >
            Apartar cita en WhatsApp
          </a>
        </div>
      </div>
    </section>

    <section id="ubicacion">
      <div class="container">
        <div class="section-header">
          <h2>Ubicación y contacto</h2>
          <p>Visítanos en Saltillo o escríbenos directamente para confirmar disponibilidad.</p>
        </div>

        <div class="info-grid">
          <div class="info-card">
            <span class="info-label">Ubicación</span>
            <h3>Estudio Shefa bynails</h3>
            <p>
              Museo del Desierto #1362,<br />
              Saltillo 2000, Saltillo, Coahuila.
            </p>
            <a
              class="btn-secondary"
              href="https://maps.google.com/?q=Museo+del+Desierto+1362,+Saltillo+2000,+Saltillo,+Coahuila"
              target="_blank"
              rel="noopener noreferrer"
            >
              Ver en Google Maps
            </a>
          </div>

          <div class="info-card" id="citas">
            <span class="info-label">Citas y WhatsApp</span>
            <h3>Atención directa</h3>
            <a class="phone-highlight" href="tel:+528442111646">844 211 1646</a>
            <p>
              Escríbeme por WhatsApp para consultar disponibilidad, técnicas y apartar tu espacio.
            </p>
            <a
              class="btn-wa"
              href="https://wa.me/528442111646?text=%C2%A1Hola!%20Quisiera%20informaci%C3%B3n%20sobre%20citas%20en%20Shefa%20bynails."
              target="_blank"
              rel="noopener noreferrer"
            >
              Chatear por WhatsApp
            </a>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p><strong>Shefa bynails</strong> · Alejandra Castillo · Museo del Desierto #1362, Saltillo 2000, Saltillo, Coahuila · WhatsApp: 844 211 1646</p>
    </div>
  </footer>

  <a
    class="floating-wa"
    href="https://wa.me/528442111646?text=%C2%A1Hola!%20Quiero%20agendar%20una%20cita%20en%20Shefa%20bynails."
    target="_blank"
    rel="noopener noreferrer"
    aria-label="Enviar mensaje por WhatsApp al 844 211 1646"
  >
    <svg width="22" height="22" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true">
      <path d="M20.52 3.48A11.82 11.82 0 0 0 12.07 0C5.5 0 .16 5.34.16 11.91c0 2.1.55 4.15 1.6 5.96L0 24l6.3-1.65a11.88 11.88 0 0 0 5.77 1.47h.01c6.57 0 11.91-5.34 11.91-11.91 0-3.18-1.24-6.17-3.47-8.43ZM12.08 21.8h-.01a9.87 9.87 0 0 1-5.03-1.38l-.36-.21-3.74.98 1-3.65-.24-.37a9.85 9.85 0 0 1-1.51-5.25c0-5.45 4.44-9.89 9.9-9.89 2.64 0 5.12 1.03 6.99 2.9a9.83 9.83 0 0 1 2.89 7c0 5.45-4.44 9.89-9.85 9.89Zm5.42-7.4c-.3-.15-1.76-.87-2.03-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.95 1.17-.17.2-.35.22-.65.07-.3-.15-1.26-.46-2.4-1.48-.89-.79-1.49-1.77-1.66-2.07-.17-.3-.02-.46.13-.61.13-.13.3-.35.45-.52.15-.17.2-.3.3-.5.1-.2.05-.37-.02-.52-.07-.15-.67-1.62-.92-2.22-.24-.58-.49-.5-.67-.51h-.57c-.2 0-.52.07-.8.37-.27.3-1.05 1.02-1.05 2.5s1.07 2.9 1.22 3.1c.15.2 2.11 3.22 5.11 4.52.71.31 1.27.49 1.71.63.72.23 1.37.2 1.89.12.58-.09 1.76-.72 2.01-1.41.25-.7.25-1.3.17-1.42-.07-.12-.27-.2-.57-.35Z"/>
    </svg>
    <span>WhatsApp</span>
  </a>

</body>
</html>
