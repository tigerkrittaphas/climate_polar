<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Ice Is Melting Unevenly</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,400;0,9..144,600;0,9..144,800;1,9..144,400&family=Inter+Tight:wght@300;400;500;600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="./app.css">
</head>
<body>
<main>
  <section class="title-card">
    <h1><em>Climate Vulnerability in Greater Boston</em></h1>
    <p class="byline">Climate change affects us unequally.</p>
    <div class="scroll-hint">
      <span>Scroll</span>
      <svg width="12" height="20" viewBox="0 0 12 20">
        <path d="M 6 2 L 6 16 M 2 12 L 6 16 L 10 12" stroke="currentColor" stroke-width="1.2" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </div>
  </section>

  <section class="scrolly" id="scrolly">
    <div class="sticky-wrapper">
      <div class="scene-column">
        <div class="scene-container">
          <img id="bear-plain" src="/images/polar_bear_plain.png" class="bear-img" alt="Polar bear" />
          <img id="bear-shake" src="/images/polar_bear_shake.png" class="bear-img" alt="Polar bear shaking" />
          <div id="water-fill" class="water-fill"></div>
          <div id="water-wrapper" class="water-wrapper">
            <img id="water-img" src="/images/water.png" class="water-img" alt="" />
          </div>
        </div>
      </div>

      <div class="text-column">
        <div class="step" data-step="0"><p>You've seen the picture before.</p></div>
        <div class="step" data-step="1"><p>A polar bear on a piece of ice. The ocean closing in.</p></div>
        <div class="step" data-step="2"><p>Climate changes. Their house shrinks.</p></div>
        <div class="step" data-step="3"><p>There is nowhere else to go.</p></div>
      </div>
    </div>
  </section>

  <section class="pivot">
    <img class="pivot-bear" src="/images/polar_bear_sitting.png" alt="Polar bear sitting" />
    <div class="pivot-inner">
      <p class="pivot-lead">Humans do too.</p>
      <p class="pivot-body">
        Worsening climate conditions are making some places unlivable. Especially for those who are already vulnerable.
      </p>
      <p class="pivot-body">
        Some of us are like the polar bear: their home is disappearing, and there is nowhere else to go.       
      </p>
    </div>
  </section>

  <section class="timeline-intro">
    <p class="eyebrow">Boston, Massachusetts</p>
    <h2>This isn't abstract.<br>It's already here.</h2>
    <p class="next-body">
      Greater Boston has seen record-breaking floods, storms, and heat in just the past decade.
      Each one a preview of what comes next — and a question of who bears the cost.
    </p>
  </section>

  <section class="timeline">
    <div class="timeline-track">

      <div class="timeline-event" data-reveal>
        <div class="timeline-date">
          <span class="tl-year">2018</span>
          <span class="tl-month">Jan 4</span>
        </div>
        <div class="timeline-content">
          <p class="tl-tag">Nor'easter · Bomb Cyclone</p>
          <h3 class="tl-title">Boston Harbor hits its highest water level ever recorded.</h3>
          <p class="tl-stat">15.16 <span>feet</span></p>
          <p class="tl-body">
            A rapidly intensifying nor'easter struck at peak high tide. The surge flooded the Seaport
            District, poured into the MBTA Aquarium station, and sent ice chunks floating down Atlantic
            Avenue. USGS classified it a 50–100 year flood event — beating the record set during the Blizzard of '78.
          </p>
          <p class="tl-source">USGS · Boston Globe</p>
        </div>
      </div>

      <div class="timeline-event" data-reveal>
        <div class="timeline-date">
          <span class="tl-year">2018</span>
          <span class="tl-month">Mar 1–3</span>
        </div>
        <div class="timeline-content">
          <p class="tl-tag">Nor'easter · Winter Storm Riley</p>
          <h3 class="tl-title">Over 100 people rescued from floodwaters in Quincy alone.</h3>
          <p class="tl-stat">400,000+ <span>MA households lost power</span></p>
          <p class="tl-body">
            The first of four back-to-back nor'easters in three weeks. Riley arrived on a spring tide
            with 70 mph gusts; Boston Harbor peaked at 14.67 feet — third highest on record. Rescuers
            used rafts and front-end loaders to reach trapped residents across the South Shore.
          </p>
          <p class="tl-source">FloodList · USGS · NWS Boston</p>
        </div>
      </div>

      <div class="timeline-event" data-reveal>
        <div class="timeline-date">
          <span class="tl-year">2022</span>
          <span class="tl-month">Jul 19–25</span>
        </div>
        <div class="timeline-content">
          <p class="tl-tag">Extreme Heat · 7-Day Emergency</p>
          <h3 class="tl-title">Boston hits 100°F. EMS calls surge 30% for a week straight.</h3>
          <p class="tl-stat">26 <span>consecutive days above 80°F — an all-time record</span></p>
          <p class="tl-body">
            Mayor Wu declared a heat emergency that lasted seven days. Extreme heat is the leading
            weather-related killer in the US — yet Massachusetts has no mandatory system to track heat deaths.
            MAPC projects the region will see more than twice as many days above 90°F by 2030.
          </p>
          <p class="tl-source">MAPC · NWS Boston · WBUR</p>
        </div>
      </div>

    </div>
  </section>

  <!-- <section class="next">
    <p class="eyebrow">Chapter Two</p>
    <h2>Two houses, one storm.</h2>
    <p class="next-body">
      A hurricane hits a coastline. One family is back in their rebuilt house
      within a year. Their neighbors three blocks inland are still in a motel
      two years later. The difference is not the weather.
    </p>
    <p class="continue">Continue reading →</p>
  </section> -->
</main>

<script type="module">
  const scrolly = document.getElementById('scrolly');
  const bearPlain = document.getElementById('bear-plain');
  const bearShake = document.getElementById('bear-shake');
  const waterFill = document.getElementById('water-fill');
  const waterWrapper = document.getElementById('water-wrapper');
  const waterImg = document.getElementById('water-img');
  const steps = document.querySelectorAll('.step');

  function update() {
    const rect = scrolly.getBoundingClientRect();
    const vh = window.innerHeight;
    const total = rect.height - vh;
    const scrolled = -rect.top;
    const progress = Math.max(0, Math.min(1, scrolled / total));

    // Water rises
    const waterHeight = 150 + progress * 70;
    waterWrapper.style.height = waterHeight + '%';

    // Water translates left-right — 3 oscillation cycles during the full scroll
    const waterX = Math.sin(progress * Math.PI * 3) * 1;
    waterImg.style.transform = `translateX(${waterX}%)`;

    // Bear transition: plain → shake over the last 30% of scroll
    const bearShaking = progress > 0.3;
    if (bearShaking) {
      bearPlain.style.opacity = 0;
      bearShake.style.opacity = 1;
    } else {
      bearPlain.style.opacity = 1;
      bearShake.style.opacity = 0;
    }

    // Text steps
    const activeStep = Math.min(steps.length - 1, Math.floor(progress * steps.length));
    steps.forEach((el, i) => el.classList.toggle('active', i === activeStep));
  }

  window.addEventListener('scroll', update, { passive: true });
  window.addEventListener('resize', update);
  update();

  // Timeline scroll-reveal
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(el => {
      if (el.isIntersecting) {
        el.target.classList.add('revealed');
        observer.unobserve(el.target);
      }
    });
  }, { threshold: 0.2 });

  document.querySelectorAll('[data-reveal]').forEach(el => observer.observe(el));
</script>
</body>
</html>
