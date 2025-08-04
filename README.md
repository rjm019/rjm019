<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ricardo Jiménez – Portafolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500;700&display=swap" rel="stylesheet">
  <style>
    :root{--bg:#ffffff;--fg:#000000;--accent:#0066ff;--accent-light:#e6f0ff}
    [data-theme="dark"]{--bg:#0c0c0c;--fg:#f1f1f1;--accent:#66a3ff;--accent-light:#142447}
    *{margin:0;padding:0;box-sizing:border-box;font-family:'Montserrat',sans-serif;scroll-behavior:smooth}
    body{background:var(--bg);color:var(--fg);line-height:1.7}
    nav{position:fixed;top:0;left:0;width:100%;background:var(--bg);border-bottom:1px solid var(--fg);display:flex;justify-content:center;gap:2rem;padding:.8rem 0;z-index:99;transition:background .3s}
    nav a{font-weight:500;text-decoration:none;color:var(--fg);padding:.2rem .4rem;transition:color .3s}
    nav a.active{color:var(--accent)}
    header{min-height:100vh;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;padding:0 2rem}
    h1{font-size:3.4rem;font-weight:700;letter-spacing:-1px}
    .tagline{font-size:1.5rem;font-weight:500;margin-top:1rem;background:linear-gradient(90deg,var(--accent),var(--fg));-webkit-background-clip:text;color:transparent;animation:slide 6s linear infinite}
    @keyframes slide{0%{background-position:0%}100%{background-position:200%}}
    section{padding:6rem 2rem;max-width:1100px;margin:auto}
    h2{font-size:2.2rem;font-weight:600;margin-bottom:2.5rem;position:relative}
    h2::after{content:"";position:absolute;left:0;bottom:-8px;height:4px;width:60px;background:var(--accent)}
    .projects-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:2rem}
    .project-card{background:var(--accent-light);border:1px solid var(--accent);padding:1.8rem;border-radius:12px;display:flex;flex-direction:column;gap:1rem;transition:transform .3s}
    .project-card:hover{transform:translateY(-6px)}
    .project-card h3{font-size:1.3rem;font-weight:600}
    .project-card a{margin-top:auto;color:var(--accent);text-decoration:none;font-weight:500}
    .skills-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:1rem}
    .skills-grid span{border:1px solid var(--fg);padding:.6rem;border-radius:8px;text-align:center;font-size:.9rem;background:var(--bg);transition:background .2s,transform .2s}
    .skills-grid span:hover{background:var(--accent-light);transform:translateY(-3px)}
    footer{padding:4rem 2rem;text-align:center;border-top:1px solid var(--fg)}
    .theme-toggle{position:fixed;right:1rem;bottom:1rem;background:var(--accent);border:none;color:#fff;padding:.6rem .8rem;border-radius:50%;cursor:pointer;font-size:1rem}
    @media(max-width:600px){h1{font-size:2.5rem}.tagline{font-size:1.2rem}nav{gap:1rem}}
  </style>
</head>
<body>
  <nav id="navbar">
    <a href="#sobre-mi">Sobre mí</a>
    <a href="#proyectos">Proyectos</a>
    <a href="#habilidades">Habilidades</a>
    <a href="#contacto">Contacto</a>
  </nav>

  <header>
    <h1>Ricardo Yair Jiménez Martínez</h1>
    <p class="tagline">Desarrollador de múltiples soluciones</p>
  </header>

  <section id="sobre-mi">
    <h2>Sobre mí</h2>
    <p>Soy un desarrollador full‑stack mexicano de 24 años con hambre constante de aprender. Desde los 17 construyo todo tipo de software: desde ERPs complejos hasta aplicaciones móviles. He liderado equipos, gestionado infraestructura y optimizado procesos, pero mi mayor fascinación siempre será programar.</p>
  </section>

  <section id="proyectos">
    <h2>Proyectos destacados</h2>
    <div class="projects-grid">
      <div class="project-card">
        <h3>POS Dinámico para Restaurantes</h3>
        <p>Punto de venta en tiempo real: arrastra mesas para unir o dividir cuentas, pagos parciales y control de inventario. Clientes piden vía QR; cocina recibe al instante. Panel de ingresos y gastos para dueños.</p>
        <p><strong>Stack:</strong> Vue 3 · Vite · TypeScript · Laravel 11 · OAuth2 · MySQL</p>
        <a href="https://github.com/USERNAME/pos" target="_blank">Código en GitHub →</a>
      </div>
      <div class="project-card">
        <h3>Taskly – Recordatorios de Voz</h3>
        <p>App Android que convierte notas de voz en tareas. Notificaciones automáticas y organización por categorías.</p>
        <p><strong>Stack:</strong> Kotlin · Jetpack Compose · Firebase</p>
        <a href="https://github.com/USERNAME/taskly" target="_blank">Código en GitHub →</a>
      </div>
      <div class="project-card">
        <h3>Sistema Gestión de Invitados</h3>
        <p>Suite web para eventos: invitaciones interactivas, registro de asistentes, pases con QR y control de acceso.</p>
        <p><strong>Stack:</strong> Vue 3 · Laravel 10 · AWS S3</p>
        <a href="https://github.com/USERNAME/guest-manager" target="_blank">Código en GitHub →</a>
      </div>
      <div class="project-card">
        <h3>En curso…</h3>
        <p>Siempre hay algo nuevo en el horno. ¡Mantente al tanto!</p>
      </div>
    </div>
  </section>

  <section id="habilidades">
    <h2>Habilidades técnicas</h2>
    <div class="skills-grid">
      <span>PHP</span><span>Laravel</span><span>JavaScript</span><span>TypeScript</span><span>Vue 3</span><span>Angular</span><span>Express</span><span>Python</span><span>Django</span><span>Spring</span><span>Kotlin</span><span>MySQL</span><span>Docker</span><span>AWS</span><span>DevOps</span><span>CI/CD</span>
    </div>
  </section>

  <section id="contacto">
    <h2>Contacto</h2>
    <p><strong>Email:</strong> <a href="mailto:ricardojimenez@micorreo.upp.edu.mx">ricardojimenez@micorreo.upp.edu.mx</a></p>
    <p><strong>WhatsApp:</strong> <a href="https://wa.me/525655908318" target="_blank">+52 56 5590 8318</a></p>
    <p><a href="https://github.com/USERNAME" target="_blank" rel="noopener">GitHub</a> • <a href="https://www.linkedin.com/in/USERNAME" target="_blank" rel="noopener">LinkedIn</a></p>
  </section>

  <footer>
    © 2025 Ricardo Jiménez
  </footer>

  <button class="theme-toggle" id="toggleTheme">☀️</button>

  <script>
    const navLinks=[...document.querySelectorAll('nav a')]
    const sections=navLinks.map(a=>document.querySelector(a.getAttribute('href')))
    const highlight=()=>{const pos=window.scrollY+80;sections.forEach((sec,i)=>{if(pos>=sec.offsetTop&&pos<sec.offsetTop+sec.offsetHeight){navLinks.forEach(l=>l.classList.remove('active'));navLinks[i].classList.add('active')}})}
    document.addEventListener('scroll',highlight)
    highlight()
    const btn=document.getElementById('toggleTheme')
    const setTheme=mode=>{document.documentElement.dataset.theme=mode;btn.textContent=mode==='dark'?'🌙':'☀️';localStorage.setItem('theme',mode)}
    btn.addEventListener('click',()=>{const t=document.documentElement.dataset.theme==='dark'?'light':'dark';setTheme(t)})
    const saved=localStorage.getItem('theme')||'light';setTheme(saved)
  </script>
</body>
</html>
