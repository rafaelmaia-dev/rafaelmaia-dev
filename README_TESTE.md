<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Botões Interativos</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    :root {
      --bg: #0b1120;
      --bg-2: #111827;
      --surface: rgba(255, 255, 255, 0.04);
      --surface-strong: #0f172a;
      --border: rgba(255, 255, 255, 0.08);
      --text: #f8fafc;
      --muted: #cbd5e1;

      --blue-1: #2563eb;
      --blue-2: #3b82f6;

      --green-1: #16a34a;
      --green-2: #22c55e;

      --purple-1: #7c3aed;
      --purple-2: #a855f7;

      --dark-1: #111827;
      --dark-2: #1f2937;

      --shadow: 0 10px 30px rgba(0, 0, 0, 0.35);
      --shadow-hover: 0 14px 35px rgba(0, 0, 0, 0.45);
    }

    body {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 40px 20px;
      font-family: Inter, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background:
        radial-gradient(circle at top, #182235 0%, #0d1423 45%, #070b14 100%);
      color: var(--text);
    }

    .container {
      width: 100%;
      max-width: 900px;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 18px;
    }

    .row {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 14px;
      width: 100%;
    }

    .chip,
    .btn-social {
      position: relative;
      display: inline-flex;
      align-items: center;
      overflow: hidden;
      border-radius: 14px;
      border: 1px solid var(--border);
      backdrop-filter: blur(12px);
      box-shadow: var(--shadow);
      transition:
        transform 0.2s ease,
        box-shadow 0.2s ease,
        border-color 0.2s ease,
        filter 0.2s ease;
    }

    .chip:hover,
    .btn-social:hover {
      transform: translateY(-3px);
      box-shadow: var(--shadow-hover);
      border-color: rgba(255, 255, 255, 0.14);
    }

    .chip:active,
    .btn-social:active {
      transform: translateY(0);
    }

    .chip::before,
    .btn-social::before {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(
        120deg,
        transparent 20%,
        rgba(255, 255, 255, 0.08) 50%,
        transparent 80%
      );
      transform: translateX(-120%);
      transition: transform 0.8s ease;
      pointer-events: none;
    }

    .chip:hover::before,
    .btn-social:hover::before {
      transform: translateX(120%);
    }

    .chip__label,
    .chip__value,
    .btn-social {
      height: 48px;
      font-size: 13px;
      font-weight: 800;
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    .chip__label,
    .chip__value {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      padding: 0 18px;
      white-space: nowrap;
    }

    .chip__label {
      background: rgba(15, 23, 42, 0.95);
      color: var(--text);
    }

    .chip__value {
      color: white;
    }

    .chip__value--success {
      background: linear-gradient(135deg, var(--green-1), var(--green-2));
    }

    .chip__value--accent {
      background: linear-gradient(135deg, var(--purple-1), var(--purple-2));
    }

    .chip__value--neutral {
      background: linear-gradient(135deg, #334155, #475569);
    }

    .btn-social {
      gap: 10px;
      padding: 0 18px;
      text-decoration: none;
      color: white;
      min-width: 140px;
      justify-content: center;
    }

    .btn-social.linkedin {
      background: linear-gradient(135deg, var(--blue-1), var(--blue-2));
    }

    .btn-social.github {
      background: linear-gradient(135deg, var(--dark-1), var(--dark-2));
    }

    .btn-social svg {
      width: 17px;
      height: 17px;
      flex-shrink: 0;
    }

    .dot {
      width: 10px;
      height: 10px;
      border-radius: 999px;
      background: #22c55e;
      box-shadow: 0 0 10px rgba(34, 197, 94, 0.8);
      flex-shrink: 0;
    }

    .pin {
      font-size: 14px;
      line-height: 1;
    }

    .cap {
      font-size: 13px;
      line-height: 1;
    }

    @media (max-width: 600px) {
      .chip,
      .btn-social {
        width: 100%;
        justify-content: center;
      }

      .chip {
        flex-wrap: wrap;
      }

      .chip__label,
      .chip__value {
        justify-content: center;
        width: 100%;
      }
    }
  </style>
</head>
<body>
  <div class="container">

    <div class="row">
      <div class="chip">
        <span class="chip__label">Visitas no perfil</span>
        <span class="chip__value chip__value--accent">177</span>
      </div>
    </div>

    <div class="row">
      <a href="https://linkedin.com" target="_blank" class="btn-social linkedin">
        <span>LinkedIn</span>
      </a>

      <a href="https://github.com" target="_blank" class="btn-social github">
        <svg viewBox="0 0 24 24" aria-hidden="true">
          <path fill="currentColor" d="M12 .5a12 12 0 0 0-3.79 23.39c.6.11.82-.26.82-.58v-2.03c-3.34.73-4.04-1.42-4.04-1.42-.55-1.38-1.34-1.75-1.34-1.75-1.09-.75.08-.74.08-.74 1.2.08 1.84 1.25 1.84 1.25 1.08 1.84 2.82 1.31 3.5 1 .1-.79.42-1.31.76-1.61-2.67-.31-5.47-1.36-5.47-6.03 0-1.33.46-2.42 1.24-3.27-.12-.31-.54-1.57.12-3.27 0 0 1.01-.33 3.3 1.25a11.3 11.3 0 0 1 6 0c2.28-1.58 3.29-1.25 3.29-1.25.67 1.7.25 2.96.13 3.27.77.85 1.24 1.94 1.24 3.27 0 4.68-2.8 5.72-5.48 6.03.43.38.81 1.1.81 2.22v3.29c0 .32.21.7.82.58A12 12 0 0 0 12 .5Z"/>
        </svg>
        <span>GitHub</span>
      </a>
    </div>

    <div class="row">
      <div class="chip">
        <span class="chip__label">
          <span class="dot"></span>
          Status
        </span>
        <span class="chip__value chip__value--success">Aberto para estágio</span>
      </div>

      <div class="chip">
        <span class="chip__label">
          <span class="pin">📍</span>
          Localização
        </span>
        <span class="chip__value chip__value--success">Brasil</span>
      </div>
    </div>

    <div class="row">
      <div class="chip">
        <span class="chip__label">
          <span class="cap">🎓</span>
          Curso
        </span>
        <span class="chip__value chip__value--accent">5º semestre</span>
      </div>
    </div>

  </div>
</body>
</html>
