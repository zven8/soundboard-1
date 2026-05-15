<!DOCTYPE html><html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Выездной тимбилдинг глубокого восстановления</title>
  <meta name="description" content="Выездные корпоративные практики: крепкая йога, научное объяснение усталости и зажимов, шавасана под живую этническую музыку." />
  <style>
    :root {
      --bg: #f8f1e8;
      --bg-soft: #fff9f0;
      --text: #25221f;
      --muted: #6d6258;
      --accent: #b86f45;
      --accent-dark: #7f432c;
      --green: #506b53;
      --sand: #e6d2bd;
      --cream: #fffaf3;
      --shadow: 0 24px 80px rgba(65, 41, 24, 0.14);
      --radius: 28px;
    }* { box-sizing: border-box; }

html { scroll-behavior: smooth; }

body {
  margin: 0;
  font-family: Inter, Arial, sans-serif;
  color: var(--text);
  background:
    radial-gradient(circle at 15% 10%, rgba(184, 111, 69, 0.18), transparent 28%),
    radial-gradient(circle at 82% 8%, rgba(80, 107, 83, 0.16), transparent 30%),
    linear-gradient(180deg, #fff8ef 0%, var(--bg) 55%, #efe0d0 100%);
  line-height: 1.55;
}

a { color: inherit; text-decoration: none; }

.container {
  width: min(1160px, calc(100% - 40px));
  margin: 0 auto;
}

.nav {
  position: sticky;
  top: 0;
  z-index: 20;
  backdrop-filter: blur(18px);
  background: rgba(255, 248, 239, 0.75);
  border-bottom: 1px solid rgba(127, 67, 44, 0.12);
}

.nav-inner {
  min-height: 76px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 24px;
}

.logo {
  display: flex;
  align-items: center;
  gap: 12px;
  font-weight: 800;
  letter-spacing: -0.03em;
  font-size: 18px;
}

.logo-mark {
  width: 42px;
  height: 42px;
  border-radius: 50%;
  display: grid;
  place-items: center;
  background: conic-gradient(from 160deg, var(--accent), #e3b180, var(--green), var(--accent));
  box-shadow: 0 12px 30px rgba(184, 111, 69, 0.25);
}

.logo-mark::after {
  content: "";
  width: 18px;
  height: 18px;
  border-radius: 50%;
  background: var(--cream);
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 24px;
  font-size: 14px;
  color: var(--muted);
}

.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  min-height: 52px;
  padding: 0 24px;
  border-radius: 999px;
  border: 0;
  background: var(--text);
  color: white;
  font-weight: 700;
  cursor: pointer;
  box-shadow: 0 16px 40px rgba(37, 34, 31, 0.18);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.btn:hover { transform: translateY(-2px); box-shadow: 0 20px 46px rgba(37, 34, 31, 0.24); }

.btn.secondary {
  background: rgba(255, 255, 255, 0.65);
  color: var(--text);
  border: 1px solid rgba(37, 34, 31, 0.12);
  box-shadow: none;
}

.hero {
  position: relative;
  padding: 92px 0 88px;
  overflow: hidden;
}

.hero-grid {
  display: grid;
  grid-template-columns: 1.05fr 0.95fr;
  gap: 52px;
  align-items: center;
}

.eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 8px 14px;
  border-radius: 999px;
  background: rgba(184, 111, 69, 0.12);
  color: var(--accent-dark);
  font-weight: 800;
  font-size: 13px;
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

h1 {
  margin: 22px 0 22px;
  font-size: clamp(44px, 6vw, 82px);
  line-height: 0.95;
  letter-spacing: -0.075em;
}

.lead {
  max-width: 620px;
  font-size: 21px;
  color: var(--muted);
  margin: 0 0 30px;
}

.hero-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 14px;
  margin-bottom: 32px;
}

.stats {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 14px;
  max-width: 650px;
}

.stat {
  padding: 18px;
  background: rgba(255, 250, 243, 0.78);
  border: 1px solid rgba(127, 67, 44, 0.1);
  border-radius: 22px;
}

.stat strong { display: block; font-size: 24px; letter-spacing: -0.04em; }
.stat span { color: var(--muted); font-size: 14px; }

.hero-card {
  position: relative;
  min-height: 560px;
  border-radius: 44px;
  padding: 26px;
  background:
    linear-gradient(145deg, rgba(255,255,255,0.7), rgba(255,255,255,0.28)),
    radial-gradient(circle at 50% 30%, rgba(184,111,69,0.22), transparent 35%),
    linear-gradient(180deg, #f3ddc6, #d5b89b);
  box-shadow: var(--shadow);
  overflow: hidden;
  border: 1px solid rgba(255, 255, 255, 0.55);
}

.sun {
  position: absolute;
  width: 220px;
  height: 220px;
  border-radius: 50%;
  background: radial-gradient(circle, #f8d59c 0%, #d98b56 58%, rgba(217,139,86,0) 70%);
  top: 54px;
  right: 66px;
  opacity: 0.9;
}

.person {
  position: absolute;
  left: 50%;
  bottom: 84px;
  transform: translateX(-50%);
  width: 330px;
  height: 220px;
}

.person .mat {
  position: absolute;
  left: 5px;
  right: 5px;
  bottom: 0;
  height: 42px;
  border-radius: 999px;
  background: rgba(80, 107, 83, 0.88);
  box-shadow: 0 22px 50px rgba(80,107,83,0.3);
}

.person .body {
  position: absolute;
  width: 210px;
  height: 78px;
  left: 58px;
  bottom: 48px;
  border-radius: 70px 70px 42px 42px;
  background: var(--accent-dark);
  transform: rotate(-2deg);
}

.person .head {
  position: absolute;
  width: 54px;
  height: 54px;
  left: 30px;
  bottom: 72px;
  border-radius: 50%;
  background: #74402c;
}

.person .leg1, .person .leg2 {
  position: absolute;
  height: 28px;
  border-radius: 999px;
  background: #e6b58d;
  bottom: 46px;
}

.person .leg1 { width: 145px; right: 2px; transform: rotate(8deg); }
.person .leg2 { width: 130px; right: 35px; transform: rotate(-16deg); bottom: 75px; }

.music-orbits {
  position: absolute;
  inset: 40px;
  pointer-events: none;
}

.orbit {
  position: absolute;
  border: 1px solid rgba(255, 250, 243, 0.55);
  border-radius: 50%;
  animation: float 7s ease-in-out infinite;
}

.orbit:nth-child(1) { width: 120px; height: 120px; left: 40px; top: 70px; }
.orbit:nth-child(2) { width: 92px; height: 92px; right: 38px; bottom: 150px; animation-delay: -2s; }
.orbit:nth-child(3) { width: 62px; height: 62px; left: 110px; bottom: 205px; animation-delay: -3.5s; }

.instrument-tag {
  position: absolute;
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 10px 14px;
  border-radius: 999px;
  background: rgba(255, 250, 243, 0.78);
  color: var(--accent-dark);
  font-weight: 800;
  font-size: 13px;
  box-shadow: 0 12px 30px rgba(65,41,24,0.12);
}

.tag-1 { left: 28px; bottom: 34px; }
.tag-2 { right: 28px; top: 28px; }
.tag-3 { right: 42px; bottom: 64px; }

@keyframes float {
  0%, 100% { transform: translateY(0) scale(1); }
  50% { transform: translateY(-16px) scale(1.04); }
}

section { padding: 88px 0; }

.section-head {
  max-width: 760px;
  margin-bottom: 38px;
}

.section-head h2 {
  margin: 0 0 16px;
  font-size: clamp(34px, 4vw, 58px);
  line-height: 1;
  letter-spacing: -0.06em;
}

.section-head p {
  margin: 0;
  font-size: 19px;
  color: var(--muted);
}

.cards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 22px;
}

.card {
  padding: 28px;
  border-radius: var(--radius);
  background: rgba(255, 250, 243, 0.78);
  border: 1px solid rgba(127, 67, 44, 0.1);
  box-shadow: 0 18px 50px rgba(65,41,24,0.08);
}

.icon {
  width: 58px;
  height: 58px;
  border-radius: 20px;
  display: grid;
  place-items: center;
  background: rgba(184, 111, 69, 0.14);
  color: var(--accent-dark);
  font-size: 26px;
  margin-bottom: 22px;
}

.card h3 {
  margin: 0 0 12px;
  font-size: 23px;
  letter-spacing: -0.03em;
}

.card p { margin: 0; color: var(--muted); }

.program {
  background: rgba(255, 250, 243, 0.52);
  border-top: 1px solid rgba(127, 67, 44, 0.08);
  border-bottom: 1px solid rgba(127, 67, 44, 0.08);
}

.timeline {
  display: grid;
  gap: 16px;
}

.step {
  display: grid;
  grid-template-columns: 120px 1fr;
  gap: 24px;
  align-items: start;
  padding: 24px;
  border-radius: 26px;
  background: var(--cream);
  border: 1px solid rgba(127, 67, 44, 0.1);
}

.time {
  font-size: 15px;
  font-weight: 900;
  color: var(--accent-dark);
  padding: 8px 12px;
  border-radius: 999px;
  background: rgba(184, 111, 69, 0.12);
  text-align: center;
}

.step h3 { margin: 0 0 8px; font-size: 22px; }
.step p { margin: 0; color: var(--muted); }

.science-grid {
  display: grid;
  grid-template-columns: 0.9fr 1.1fr;
  gap: 28px;
  align-items: stretch;
}

.quote-card {
  position: relative;
  padding: 34px;
  border-radius: 34px;
  color: white;
  background:
    radial-gradient(circle at 20% 15%, rgba(255,255,255,0.22), transparent 30%),
    linear-gradient(145deg, var(--green), #24372b);
  box-shadow: var(--shadow);
  overflow: hidden;
}

.quote-card h3 {
  margin: 0 0 14px;
  font-size: 32px;
  line-height: 1.05;
  letter-spacing: -0.05em;
}

.quote-card p { color: rgba(255,255,255,0.78); margin: 0; }

.sound-waves {
  margin-top: 34px;
  height: 150px;
  display: flex;
  align-items: center;
  gap: 9px;
}

.wave {
  width: 12px;
  border-radius: 999px;
  background: rgba(255, 250, 243, 0.72);
  animation: pulse 1.8s ease-in-out infinite;
}

.wave:nth-child(1) { height: 40px; }
.wave:nth-child(2) { height: 86px; animation-delay: -0.2s; }
.wave:nth-child(3) { height: 120px; animation-delay: -0.5s; }
.wave:nth-child(4) { height: 68px; animation-delay: -0.8s; }
.wave:nth-child(5) { height: 104px; animation-delay: -1s; }
.wave:nth-child(6) { height: 48px; animation-delay: -1.2s; }
.wave:nth-child(7) { height: 92px; animation-delay: -1.4s; }
.wave:nth-child(8) { height: 58px; animation-delay: -1.6s; }

@keyframes pulse {
  0%, 100% { transform: scaleY(0.7); opacity: 0.58; }
  50% { transform: scaleY(1.08); opacity: 1; }
}

.accordion-like {
  display: grid;
  gap: 14px;
}

.science-item {
  padding: 24px;
  border-radius: 24px;
  background: rgba(255, 250, 243, 0.78);
  border: 1px solid rgba(127, 67, 44, 0.1);
}

.science-item strong { display: block; margin-bottom: 8px; font-size: 19px; }
.science-item span { color: var(--muted); }

.instruments {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 16px;
}

.instrument {
  min-height: 190px;
  padding: 18px;
  border-radius: 28px;
  background: var(--cream);
  border: 1px solid rgba(127, 67, 44, 0.1);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  overflow: hidden;
}

.instrument-visual {
  height: 92px;
  display: grid;
  place-items: center;
}

.circle-instrument {
  width: 74px;
  height: 74px;
  border-radius: 50%;
  background: radial-gradient(circle at 35% 28%, #fff0bd, #b86f45 50%, #5e3525 78%);
  box-shadow: inset 0 0 0 8px rgba(255,255,255,0.18), 0 12px 26px rgba(65,41,24,0.14);
}

.bowl {
  width: 90px;
  height: 45px;
  border-radius: 0 0 90px 90px;
  background: linear-gradient(180deg, #f9e5bd, #a26c42);
  box-shadow: inset 0 8px 0 rgba(255,255,255,0.45), 0 12px 24px rgba(65,41,24,0.12);
}

.harp {
  width: 70px;
  height: 88px;
  border-left: 8px solid #b86f45;
  border-bottom: 8px solid #b86f45;
  border-radius: 0 0 0 38px;
  position: relative;
}

.harp::after {
  content: "";
  position: absolute;
  inset: 10px 10px 6px 16px;
  background: repeating-linear-gradient(90deg, rgba(127,67,44,0.42) 0 2px, transparent 2px 10px);
  border-radius: 12px;
}

.drum {
  width: 78px;
  height: 78px;
  border-radius: 50%;
  background: radial-gradient(circle, #f5dfc5 0 46%, #7f432c 47% 55%, #e7b27d 56%);
  box-shadow: 0 12px 24px rgba(65,41,24,0.13);
}

.bell {
  width: 56px;
  height: 80px;
  border-radius: 28px 28px 12px 12px;
  background: linear-gradient(180deg, #f2d28e, #b86f45);
  position: relative;
}

.bell::after {
  content: "";
  position: absolute;
  left: 50%;
  bottom: -8px;
  width: 18px;
  height: 18px;
  transform: translateX(-50%);
  border-radius: 50%;
  background: #7f432c;
}

.instrument h3 { margin: 0 0 6px; font-size: 18px; }
.instrument p { margin: 0; color: var(--muted); font-size: 14px; }

.result {
  padding: 56px;
  border-radius: 42px;
  background:
    linear-gradient(145deg, rgba(255,255,255,0.78), rgba(255,255,255,0.42)),
    radial-gradient(circle at 85% 15%, rgba(80,107,83,0.18), transparent 34%),
    var(--cream);
  box-shadow: var(--shadow);
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 34px;
  align-items: center;
}

.result h2 {
  margin: 0 0 16px;
  font-size: clamp(34px, 4vw, 58px);
  line-height: 1;
  letter-spacing: -0.06em;
}

.check-list {
  display: grid;
  gap: 14px;
  margin-top: 24px;
}

.check {
  display: flex;
  gap: 12px;
  align-items: flex-start;
  color: var(--muted);
}

.check::before {
  content: "✓";
  flex: 0 0 26px;
  width: 26px;
  height: 26px;
  border-radius: 50%;
  background: rgba(80,107,83,0.15);
  color: var(--green);
  display: grid;
  place-items: center;
  font-weight: 900;
}

.cta {
  padding-bottom: 110px;
}

.cta-box {
  text-align: center;
  padding: 70px 28px;
  border-radius: 44px;
  background:
    radial-gradient(circle at 50% 10%, rgba(255,255,255,0.22), transparent 36%),
    linear-gradient(145deg, #2d241f, #6b3a29);
  color: white;
  box-shadow: var(--shadow);
}

.cta-box h2 {
  max-width: 820px;
  margin: 0 auto 18px;
  font-size: clamp(36px, 5vw, 68px);
  line-height: 0.98;
  letter-spacing: -0.065em;
}

.cta-box p {
  max-width: 680px;
  margin: 0 auto 30px;
  color: rgba(255,255,255,0.76);
  font-size: 19px;
}

.cta-box .btn {
  background: #fffaf3;
  color: #2d241f;
  box-shadow: 0 20px 46px rgba(0,0,0,0.22);
}

footer {
  padding: 34px 0;
  color: var(--muted);
  border-top: 1px solid rgba(127, 67, 44, 0.1);
}

.footer-inner {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  flex-wrap: wrap;
  font-size: 14px;
}

@media (max-width: 920px) {
  .hero-grid, .science-grid, .result { grid-template-columns: 1fr; }
  .cards { grid-template-columns: 1fr; }
  .instruments { grid-template-columns: repeat(2, 1fr); }
  .nav-links { display: none; }
  .hero-card { min-height: 480px; }
  .stats { grid-template-columns: 1fr; }
}

@media (max-width: 560px) {
  .container { width: min(100% - 24px, 1160px); }
  .hero { padding-top: 56px; }
  section { padding: 62px 0; }
  .hero-actions { flex-direction: column; }
  .btn { width: 100%; }
  .step { grid-template-columns: 1fr; }
  .instruments { grid-template-columns: 1fr; }
  .result { padding: 30px; }
  .hero-card { border-radius: 30px; min-height: 420px; }
  .person { transform: translateX(-50%) scale(0.78); }
  .instrument-tag { font-size: 12px; }
  .tag-3 { display: none; }
}

  </style>
</head>
<body>
  <nav class="nav">
    <div class="container nav-inner">
      <a class="logo" href="#top" aria-label="На главную">
        <span class="logo-mark"></span>
        <span>Reset Team</span>
      </a>
      <div class="nav-links">
        <a href="#format">Формат</a>
        <a href="#program">Программа</a>
        <a href="#science">Почему работает</a>
        <a href="#contact">Заявка</a>
      </div>
      <a class="btn" href="#contact">Обсудить мероприятие</a>
    </div>
  </nav>  <main id="top">
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <div class="eyebrow">Выездной тимбилдинг восстановления</div>
          <h1>Сильная практика, глубокий отдых и живая музыка</h1>
          <p class="lead">Мы приезжаем к вашей команде и проводим телесный корпоративный формат: крепкая йога, понятное объяснение стресса и мышечных зажимов, а затем час шавасаны под живые этнические инструменты.</p>
          <div class="hero-actions">
            <a class="btn" href="#contact">Заказать выезд</a>
            <a class="btn secondary" href="#program">Посмотреть программу</a>
          </div>
          <div class="stats" aria-label="Ключевые преимущества">
            <div class="stat"><strong>2–3 часа</strong><span>готовый формат для офиса, ретрита или выезда</span></div>
            <div class="stat"><strong>15–120</strong><span>участников в одной группе</span></div>
            <div class="stat"><strong>100%</strong><span>фокус на восстановлении, а не на соревновании</span></div>
          </div>
        </div><div class="hero-card" aria-label="Иллюстрация практики расслабления под живую музыку">
      <div class="sun"></div>
      <div class="music-orbits">
        <span class="orbit"></span>
        <span class="orbit"></span>
        <span class="orbit"></span>
      </div>
      <div class="instrument-tag tag-1">● ханг</div>
      <div class="instrument-tag tag-2">● чаши</div>
      <div class="instrument-tag tag-3">● хрустальная арфа</div>
      <div class="person">
        <div class="head"></div>
        <div class="body"></div>
        <div class="leg1"></div>
        <div class="leg2"></div>
        <div class="mat"></div>
      </div>
    </div>
  </div>
</section>

<section id="format">
  <div class="container">
    <div class="section-head">
      <h2>Это не просто йога и не просто концерт</h2>
      <p>Это мягко выстроенный путь: сначала тело получает здоровую нагрузку и выпускает напряжение, затем нервная система переходит в режим восстановления через покой, дыхание и живой акустический звук.</p>
    </div>

    <div class="cards">
      <article class="card">
        <div class="icon">↯</div>
        <h3>Крепкая йога без эзотерики</h3>
        <p>Динамичная, доступная практика для офисной команды: мобилизация, вытяжение, работа с дыханием и безопасная физическая нагрузка.</p>
      </article>
      <article class="card">
        <div class="icon">◎</div>
        <h3>Понятная наука о стрессе</h3>
        <p>Объясняем, почему устают шея, плечи, спина и голова, как стресс связан с мышечным тонусом и почему телу нужен осознанный сброс нагрузки.</p>
      </article>
      <article class="card">
        <div class="icon">♫</div>
        <h3>Живая музыка для глубокого отдыха</h3>
        <p>После практики участники ложатся в шавасану и час отдыхают под звонницу, ханги, чаши, бубны и хрустальную арфу.</p>
      </article>
    </div>
  </div>
</section>

<section class="program" id="program">
  <div class="container">
    <div class="section-head">
      <h2>Как проходит мероприятие</h2>
      <p>Формат можно адаптировать под офис, загородный отель, корпоративный ретрит, конференцию или выездной день команды.</p>
    </div>

    <div class="timeline">
      <div class="step">
        <div class="time">15 мин</div>
        <div>
          <h3>Вход в формат</h3>
          <p>Коротко настраиваем группу, объясняем правила безопасности и переводим внимание из рабочих задач в тело.</p>
        </div>
      </div>
      <div class="step">
        <div class="time">45–60 мин</div>
        <div>
          <h3>Крепкая телесная практика</h3>
          <p>Последовательность из йоги, функциональной мобилизации и дыхания: достаточно интенсивно, чтобы почувствовать тело, но без спортивной гонки.</p>
        </div>
      </div>
      <div class="step">
        <div class="time">15 мин</div>
        <div>
          <h3>Мини-лекция: зажимы, усталость, нервная система</h3>
          <p>На простом языке рассказываем, как длительное сидение, стресс и постоянная концентрация повышают тонус мышц и перегружают внимание.</p>
        </div>
      </div>
      <div class="step">
        <div class="time">60 мин</div>
        <div>
          <h3>Шавасана под живую этническую музыку</h3>
          <p>Участники лежат, восстанавливаются и погружаются в звук. Музыка создаётся вживую и мягко ведёт состояние от напряжения к покою.</p>
        </div>
      </div>
      <div class="step">
        <div class="time">10 мин</div>
        <div>
          <h3>Мягкое возвращение</h3>
          <p>Завершаем практику, даём простые инструменты для самостоятельного восстановления в рабочие дни.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="science">
  <div class="container">
    <div class="section-head">
      <h2>Почему это работает</h2>
      <p>Мы говорим о восстановлении языком тела и физиологии: без мистики, давления и обещаний «чудесного исцеления».</p>
    </div>

    <div class="science-grid">
      <div class="quote-card">
        <h3>После нагрузки телу легче отпустить контроль</h3>
        <p>Когда человек безопасно двигается, дышит и чувствует мышцы, внимание переключается с бесконечного анализа на телесные ощущения. Это помогает выйти из режима «надо срочно решать».</p>
        <div class="sound-waves" aria-label="Звуковые волны">
          <span class="wave"></span><span class="wave"></span><span class="wave"></span><span class="wave"></span><span class="wave"></span><span class="wave"></span><span class="wave"></span><span class="wave"></span>
        </div>
      </div>

      <div class="accordion-like">
        <div class="science-item">
          <strong>Движение снижает ощущение скованности</strong>
          <span>Мягкая силовая нагрузка, вытяжение и мобилизация помогают вернуть подвижность участкам, которые обычно «застревают» от сидячей работы: шее, плечам, грудному отделу, пояснице и тазу.</span>
        </div>
        <div class="science-item">
          <strong>Дыхание влияет на уровень возбуждения нервной системы</strong>
          <span>Удлинённый выдох, паузы и спокойный ритм дыхания помогают телу переходить от мобилизации к восстановлению.</span>
        </div>
        <div class="science-item">
          <strong>Ритм и тембр музыки помогают синхронизироваться</strong>
          <span>Повторяющиеся акустические паттерны, низкие обертона и плавная динамика создают предсказуемую среду. Мозгу не нужно постоянно анализировать новые сигналы — легче расслабиться.</span>
        </div>
        <div class="science-item">
          <strong>Шавасана закрепляет эффект</strong>
          <span>После физической части глубокий покой воспринимается ярче: мышцы уже поработали, тело согрето, внимание собрано, и отдых становится не абстрактной идеей, а реальным состоянием.</span>
        </div>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="container">
    <div class="section-head">
      <h2>Инструменты живого звучания</h2>
      <p>Мы используем акустические инструменты с богатым спектром обертонов. Они не забивают внимание, а создают объёмное звуковое пространство для восстановления.</p>
    </div>

    <div class="instruments">
      <div class="instrument">
        <div class="instrument-visual"><div class="bell"></div></div>
        <div><h3>Звонница</h3><p>Чистые переливы и мягкие высокие частоты.</p></div>
      </div>
      <div class="instrument">
        <div class="instrument-visual"><div class="circle-instrument"></div></div>
        <div><h3>Ханги</h3><p>Тёплый металлический тембр и медитативный ритм.</p></div>
      </div>
      <div class="instrument">
        <div class="instrument-visual"><div class="harp"></div></div>
        <div><h3>Хрустальная арфа</h3><p>Прозрачные вибрации и ощущение пространства.</p></div>
      </div>
      <div class="instrument">
        <div class="instrument-visual"><div class="drum"></div></div>
        <div><h3>Бубны</h3><p>Ритм, заземление и телесное ощущение пульса.</p></div>
      </div>
      <div class="instrument">
        <div class="instrument-visual"><div class="bowl"></div></div>
        <div><h3>Чаши</h3><p>Долгие обертоны и мягкое звуковое поле.</p></div>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="container">
    <div class="result">
      <div>
        <h2>Что получает команда</h2>
        <p class="lead">Участники уходят не «заряженными на рывок», а действительно отдохнувшими: с ясной головой, расслабленным телом и ощущением общего прожитого опыта.</p>
      </div>
      <div class="check-list">
        <div class="check">Снижается телесное напряжение после долгой работы за компьютером.</div>
        <div class="check">Появляется общее безопасное переживание вне рабочих ролей.</div>
        <div class="check">Команда отдыхает вместе, без алкоголя, соревнования и неловких активностей.</div>
        <div class="check">Формат запоминается: это необычно, красиво и по-настоящему восстанавливает.</div>
      </div>
    </div>
  </div>
</section>

<section class="cta" id="contact">
  <div class="container">
    <div class="cta-box">
      <h2>Привезём вашей команде практику глубокого восстановления</h2>
      <p>Подберём длительность, состав музыкантов, уровень физической нагрузки и формат под вашу площадку, количество участников и цель мероприятия.</p>
      <a class="btn" href="mailto:hello@example.com?subject=Заявка%20на%20выездной%20тимбилдинг">Оставить заявку</a>
    </div>
  </div>
</section>

  </main>  <footer>
    <div class="container footer-inner">
      <div>© Reset Team — выездные практики восстановления</div>
      <div>Йога · Наука о стрессе · Живая этническая музыка</div>
    </div>
  </footer>
</body>
</html>