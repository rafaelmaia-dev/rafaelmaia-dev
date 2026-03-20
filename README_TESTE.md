<div class="chips-row">
  <a class="btn-social linkedin" href="#">
    <span>LINKEDIN</span>
  </a>

  <a class="btn-social github" href="#">
    <svg viewBox="0 0 24 24" aria-hidden="true">
      <path fill="currentColor" d="M12 .5a12 12 0 0 0-3.79 23.39c.6.11.82-.26.82-.58v-2.03c-3.34.73-4.04-1.42-4.04-1.42-.55-1.38-1.34-1.75-1.34-1.75-1.09-.75.08-.74.08-.74 1.2.08 1.84 1.25 1.84 1.25 1.08 1.84 2.82 1.31 3.5 1 .1-.79.42-1.31.76-1.61-2.67-.31-5.47-1.36-5.47-6.03 0-1.33.46-2.42 1.24-3.27-.12-.31-.54-1.57.12-3.27 0 0 1.01-.33 3.3 1.25a11.3 11.3 0 0 1 6 0c2.28-1.58 3.29-1.25 3.29-1.25.67 1.7.25 2.96.13 3.27.77.85 1.24 1.94 1.24 3.27 0 4.68-2.8 5.72-5.48 6.03.43.38.81 1.1.81 2.22v3.29c0 .32.21.7.82.58A12 12 0 0 0 12 .5Z"/>
    </svg>
    <span>GITHUB</span>
  </a>
</div>

<div class="chips-row">
  <div class="chip">
    <span class="chip__label">
      <span class="dot"></span>
      STATUS
    </span>
    <span class="chip__value chip__value--success">ABERTO PARA ESTÁGIO</span>
  </div>

  <div class="chip">
    <span class="chip__label">📍 LOCALIZAÇÃO</span>
    <span class="chip__value chip__value--success">BRASIL</span>
  </div>
</div>

<div class="chips-row">
  <div class="chip">
    <span class="chip__label">🎓 CURSO</span>
    <span class="chip__value chip__value--accent">5º SEMESTRE</span>
  </div>
</div>


:root {
  --bg: #0b1120;
  --surface: #111827;
  --surface-2: #0f172a;
  --border: rgba(255,255,255,.08);
  --text: #e5e7eb;
  --muted: #94a3b8;

  --accent: #7c3aed;
  --accent-2: #2563eb;
  --success: #16a34a;

  --shadow: 0 10px 30px rgba(0,0,0,.35);
  --shadow-hover: 0 14px 40px rgba(0,0,0,.45);
}

body {
  background: radial-gradient(circle at top, #111827 0%, #0b1120 50%, #070b14 100%);
  color: var(--text);
  font-family: Inter, system-ui, sans-serif;
}

.chips-row {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  justify-content: center;
  margin-bottom: 14px;
}

.btn-social,
.chip {
  height: 46px;
  display: inline-flex;
  align-items: center;
  border-radius: 12px;
  overflow: hidden;
  border: 1px solid var(--border);
  box-shadow: var(--shadow);
  backdrop-filter: blur(10px);
}

.btn-social {
  position: relative;
  gap: 10px;
  padding: 0 16px;
  text-decoration: none;
  color: white;
  font-weight: 700;
  letter-spacing: .08em;
  font-size: 13px;
  transition: transform .18s ease, box-shadow .18s ease, border-color .18s ease, filter .18s ease;
}

.btn-social svg {
  width: 16px;
  height: 16px;
}

.btn-social:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-hover);
  filter: brightness(1.06);
}

.btn-social:active {
  transform: translateY(0);
}

.btn-social:focus-visible,
.chip:focus-visible {
  outline: none;
  box-shadow:
    0 0 0 3px rgba(124,58,237,.35),
    var(--shadow-hover);
}

.linkedin {
  background: linear-gradient(135deg, #1d4ed8, #2563eb);
}

.github {
  background: linear-gradient(135deg, #111827, #1f2937);
}

.chip {
  background: linear-gradient(180deg, rgba(255,255,255,.02), rgba(255,255,255,.01));
  transition: transform .18s ease, box-shadow .18s ease, border-color .18s ease;
}

.chip:hover {
  transform: translateY(-1px);
  box-shadow: var(--shadow-hover);
  border-color: rgba(255,255,255,.14);
}

.chip__label,
.chip__value {
  height: 100%;
  display: inline-flex;
  align-items: center;
  padding: 0 16px;
  font-size: 13px;
  font-weight: 700;
  letter-spacing: .08em;
}

.chip__label {
  background: rgba(15, 23, 42, .92);
  color: var(--text);
  gap: 8px;
}

.chip__value {
  color: white;
}

.chip__value--success {
  background: linear-gradient(135deg, #16a34a, #22c55e);
}

.chip__value--accent {
  background: linear-gradient(135deg, #6d28d9, #8b5cf6);
}

.dot {
  width: 10px;
  height: 10px;
  border-radius: 999px;
  background: #22c55e;
  box-shadow: 0 0 10px rgba(34,197,94,.7);
}



  
  height: 10px;
  border-radius: 999px;
  background: #22c55e;
  box-shadow: 0 0 10px rgba(34,197,94,.7);
}

