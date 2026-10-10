<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Message d'au revoir de Yves Mouaha Handy après quatre années à la SGCI.">
  <title>Merci pour ces 4 années | Yves Mouaha Handy</title>
  <style>
    :root {
      --sg-red: #e9041e;
      --sg-red-dark: #b90017;
      --sg-black: #111111;
      --sg-anthracite: #252525;
      --sg-grey: #6b6b6b;
      --sg-light: #f5f5f5;
      --white: #ffffff;
      --gold: #e6b263;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; }

    body {
      min-height: 100vh;
      overflow-x: hidden;
      font-family: "Segoe UI", Arial, Helvetica, sans-serif;
      color: var(--sg-black);
      background: #ececec;
    }

    button, a { font: inherit; }

    .page {
      position: relative;
      min-height: 100vh;
      padding: 42px 18px;
      display: flex;
      justify-content: center;
      overflow: hidden;
      background:
        linear-gradient(120deg, rgba(233, 4, 30, .95) 0 7px, transparent 7px 100%),
        radial-gradient(circle at 8% 12%, rgba(233, 4, 30, .18), transparent 24%),
        radial-gradient(circle at 90% 75%, rgba(230, 178, 99, .13), transparent 26%),
        linear-gradient(135deg, #0b0b0b 0%, #252525 52%, #111 100%);
    }

    .page::before {
      content: "";
      position: fixed;
      inset: 0;
      pointer-events: none;
      opacity: .22;
      background-image:
        linear-gradient(rgba(255,255,255,.05) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255,255,255,.05) 1px, transparent 1px);
      background-size: 44px 44px;
      mask-image: linear-gradient(to bottom, #000, transparent 88%);
    }

    .particles, .messages-container {
      position: fixed;
      inset: 0;
      overflow: hidden;
      pointer-events: none;
    }

    .particles { z-index: 0; }
    .messages-container { z-index: 4; }

    .particle {
      position: absolute;
      bottom: -80px;
      width: var(--size);
      height: var(--size);
      border-radius: 50%;
      opacity: var(--opacity);
      background: radial-gradient(circle at 34% 30%, #fff, var(--color) 32%, rgba(255,255,255,.04) 72%);
      border: 1px solid rgba(255,255,255,.25);
      box-shadow: 0 0 24px color-mix(in srgb, var(--color) 55%, transparent);
      animation: rise var(--duration) linear var(--delay) infinite;
    }

    @keyframes rise {
      0% { transform: translate3d(0, 0, 0) scale(.75); }
      40% { transform: translate3d(34px, -48vh, 0) scale(1); }
      70% { transform: translate3d(-28px, -82vh, 0) scale(.9); }
      100% { transform: translate3d(20px, -125vh, 0) scale(.65); }
    }

    .card {
      position: relative;
      z-index: 2;
      width: min(960px, 100%);
      overflow: hidden;
      border-radius: 28px;
      background: rgba(255,255,255,.98);
      box-shadow: 0 26px 90px rgba(0,0,0,.55);
      animation: reveal .9s ease both;
    }

    @keyframes reveal {
      from { opacity: 0; transform: translateY(26px) scale(.98); }
      to { opacity: 1; transform: none; }
    }

    .brand-bar {
      height: 12px;
      background: linear-gradient(90deg, var(--sg-red) 0 48%, #fff 48% 52%, #171717 52% 100%);
    }

    .hero {
      position: relative;
      padding: 48px 48px 42px;
      color: white;
      text-align: center;
      background:
        linear-gradient(135deg, rgba(233,4,30,.96), rgba(185,0,23,.95)),
        #e9041e;
    }

    .hero::after {
      content: "";
      position: absolute;
      right: -90px;
      top: -115px;
      width: 330px;
      height: 330px;
      border: 54px solid rgba(255,255,255,.08);
      border-radius: 50%;
    }

    .profile {
      position: relative;
      z-index: 1;
      width: 130px;
      height: 130px;
      margin: 0 auto 22px;
      object-fit: cover;
      object-position: center;
      border-radius: 50%;
      border: 5px solid white;
      background: #ddd;
      box-shadow: 0 12px 34px rgba(0,0,0,.28);
    }

    .eyebrow {
      position: relative;
      z-index: 1;
      margin-bottom: 9px;
      font-size: .82rem;
      font-weight: 800;
      letter-spacing: 2.3px;
      text-transform: uppercase;
    }

    .title {
      position: relative;
      z-index: 1;
      font-size: clamp(2.4rem, 7vw, 5rem);
      line-height: 1;
      letter-spacing: -2px;
    }

    .subtitle {
      position: relative;
      z-index: 1;
      max-width: 700px;
      margin: 15px auto 0;
      font-size: clamp(1.05rem, 2.5vw, 1.55rem);
      line-height: 1.4;
      font-weight: 500;
    }

    .content { padding: 44px 54px 50px; }

    .intro {
      margin-bottom: 28px;
      padding-left: 20px;
      border-left: 5px solid var(--sg-red);
      font-size: 1.13rem;
      line-height: 1.75;
      color: #333;
    }

    .section-title {
      margin: 34px 0 14px;
      font-size: 1.35rem;
      color: var(--sg-red-dark);
    }

    .content p {
      margin: 0 0 18px;
      line-height: 1.8;
      color: #3d3d3d;
    }

    .journey {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 14px;
      margin: 24px 0 34px;
    }

    .role {
      min-height: 150px;
      padding: 22px 19px;
      border: 1px solid #e3e3e3;
      border-top: 4px solid var(--sg-red);
      border-radius: 14px;
      background: #fafafa;
      box-shadow: 0 8px 22px rgba(0,0,0,.06);
    }

    .role-number {
      display: inline-grid;
      width: 34px;
      height: 34px;
      place-items: center;
      margin-bottom: 12px;
      border-radius: 50%;
      color: white;
      background: var(--sg-black);
      font-weight: 800;
    }

    .role strong { display: block; line-height: 1.5; }

    .highlight {
      margin: 32px 0;
      padding: 25px 28px;
      border-radius: 16px;
      color: white;
      background: linear-gradient(135deg, #171717, #333);
      box-shadow: inset 5px 0 0 var(--sg-red);
    }

    .highlight p { margin: 0; color: #f7f7f7; }

    .quote {
      margin: 38px auto 30px;
      padding: 27px 20px;
      text-align: center;
      border-top: 1px solid #ddd;
      border-bottom: 1px solid #ddd;
      color: var(--sg-red-dark);
      font-size: clamp(1.2rem, 3vw, 1.6rem);
      font-weight: 700;
      font-style: italic;
      line-height: 1.55;
    }

    .signature { margin-top: 30px; text-align: center; }
    .signature-name { font-size: 1.55rem; color: #171717; }
    .signature-role { margin-top: 7px; color: #666; line-height: 1.55; }

    .contacts {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 11px;
      margin-top: 24px;
    }

    .contact-link {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 11px 16px;
      border-radius: 999px;
      color: white;
      background: var(--sg-black);
      text-decoration: none;
      transition: transform .2s ease, background .2s ease;
    }

    .contact-link:hover, .contact-link:focus-visible {
      transform: translateY(-2px);
      background: var(--sg-red);
      outline: none;
    }

    .footer {
      padding: 20px;
      color: #ddd;
      text-align: center;
      background: #161616;
      font-size: .9rem;
    }

    .message-bubble {
      position: absolute;
      max-width: min(310px, 76vw);
      padding: 11px 17px;
      opacity: 0;
      color: white;
      border: 1px solid rgba(255,255,255,.5);
      border-radius: 999px;
      background: rgba(20,20,20,.88);
      box-shadow: 0 8px 28px rgba(0,0,0,.3), 0 0 0 3px rgba(233,4,30,.18);
      backdrop-filter: blur(10px);
      animation: messageFloat 5.5s ease-in-out both;
      font-weight: 700;
      text-align: center;
    }

    @keyframes messageFloat {
      0% { opacity: 0; transform: translate(-50%, 30px) scale(.5); }
      18%, 68% { opacity: 1; transform: translate(-50%, 0) scale(1); }
      100% { opacity: 0; transform: translate(-50%, -90px) scale(.9); }
    }

    .replay {
      position: fixed;
      z-index: 6;
      right: 18px;
      bottom: 18px;
      padding: 12px 17px;
      border: 0;
      border-radius: 999px;
      color: white;
      background: var(--sg-red);
      box-shadow: 0 8px 24px rgba(0,0,0,.3);
      cursor: pointer;
    }

    .replay:hover { background: var(--sg-red-dark); }

    @media (max-width: 760px) {
      .page { padding: 18px 10px 70px; }
      .hero { padding: 36px 20px 32px; }
      .profile { width: 108px; height: 108px; }
      .content { padding: 32px 23px 38px; }
      .journey { grid-template-columns: 1fr; }
      .role { min-height: auto; }
      .contacts { flex-direction: column; align-items: stretch; }
      .contact-link { justify-content: center; text-align: center; }
    }

    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after {
        animation-duration: .01ms !important;
        animation-iteration-count: 1 !important;
        scroll-behavior: auto !important;
      }
      .replay { display: none; }
    }

    @media print {
      body, .page { background: white; }
      .page { padding: 0; }
      .card { box-shadow: none; border: 1px solid #ddd; }
      .particles, .messages-container, .replay { display: none; }
      .contact-link { color: #111; background: #eee; }
    }
  </style>
</head>
<body>
  <main class="page">
    <div class="particles" id="particles" aria-hidden="true"></div>
    <div class="messages-container" id="messagesContainer" aria-hidden="true"></div>

    <article class="card">
      <div class="brand-bar" aria-hidden="true"></div>

      <header class="hero">
        <img
          class="profile"
          src="https://media.licdn.com/dms/image/v2/D4D03AQEyYvOQZ_j70w/profile-displayphoto-scale_100_100/B4DZibIuXmHwAg-/0/1754949413758?e=1793232000&amp;v=beta&amp;t=o1-EPtKqaR1fLkH61MWqPg3TGNo6-ngcsGxH-psWdxo"
          alt="Photo professionnelle de Yves Mouaha Handy"
          referrerpolicy="no-referrer"
        >
        <p class="eyebrow">Un nouveau chapitre commence</p>
        <h1 class="title">Merci.</h1>
        <p class="subtitle">Pour quatre années d'aventure humaine, professionnelle et collective à la SGCI.</p>
      </header>

      <div class="content">
        <p class="intro"><strong>Chers tous,</strong><br>Après près de quatre années riches en apprentissages, en défis et en réalisations, il est temps pour moi d'ouvrir un nouveau chapitre professionnel.</p>

        <h2 class="section-title">Un parcours porté par la Data, l'IA et l'innovation</h2>
        <p>Au cours de ces années, j'ai eu l'opportunité de contribuer à plusieurs chantiers passionnants :</p>

        <div class="journey">
          <div class="role"><span class="role-number">1</span><strong>Data Scientist Crédit Régional pour 11 filiales d'Afrique subsaharienne, au sein du Hub Marketing AFS</strong></div>
          <div class="role"><span class="role-number">2</span><strong>GenAI &amp; Data Product Owner à la Direction de l'Innovation</strong></div>
          <div class="role"><span class="role-number">3</span><strong>Squad Lead Data &amp; AI, avec la responsabilité d'accompagner les projets Data et Intelligence Artificielle de la banque</strong></div>
        </div>

        <p>Au-delà des projets, des indicateurs et des réalisations, ce sont avant tout les rencontres humaines qui resteront gravées dans ma mémoire. Je souhaitais adresser quelques mots de remerciement à celles et ceux avec qui j'ai eu la chance de collaborer tout au long de cette aventure.</p>

        <h2 class="section-title">À la Direction Générale et au Comité de Direction</h2>
        <p>Mes sincères remerciements à la Direction Générale, et particulièrement à notre Directeur Général, pour la confiance accordée, l'accompagnement constant et le sponsoring des initiatives innovantes, notamment autour de la Data et de l'Intelligence Artificielle. Votre soutien a permis de transformer des idées ambitieuses en projets concrets, créateurs de valeur pour la banque.</p>
        <p>Je remercie également l'ensemble des membres du Comité de Direction pour leur bienveillance, leur ouverture d'esprit et leur capacité à accueillir des approches parfois disruptives afin de répondre à leurs enjeux métiers. Nos échanges ont largement contribué à faire émerger de nouvelles façons de travailler et d'innover.</p>

        <div class="highlight">
          <p><strong>Une pensée toute particulière pour Oscar, Directeur de l'Innovation Digitale,</strong> dont la confiance a été déterminante dans mon parcours à la SGCI. Son ouverture aux nouvelles idées, sa capacité à challenger les équipes avec bienveillance et son exigence d'excellence ont largement contribué à mon développement professionnel. Merci pour la liberté d'action accordée, pour les défis stimulants proposés et pour avoir toujours privilégié la valeur des idées et des réalisations. Cette vision du management restera pour moi une source d'inspiration.</p>
        </div>

        <h2 class="section-title">À toutes les équipes et à tous les collègues</h2>
        <p>Une pensée particulière va à tous les collègues avec lesquels j'ai collaboré au quotidien. Du siège à Paris aux différentes filiales, du Marketing au Juridique, de la Conformité au Commercial, des Risques à la Monétique, en passant par les Opérations, l'Innovation, la Finance, l'IT/SGABS et bien d'autres équipes encore. Chacun de vous a contribué à enrichir mon parcours à travers la diversité de vos expériences, vos expertises et les moments partagés ensemble.</p>

        <h2 class="section-title">À la Direction de l'Innovation et aux jeunes talents</h2>
        <p>Enfin, je souhaite adresser un message tout particulier aux équipes de la Direction de l'Innovation que j'ai eu le privilège d'accompagner et de manager au quotidien : développeurs Front-End et Back-End, Data Scientists, UX/UI Designers et, plus largement, tous les talents ayant contribué aux projets que nous avons portés ensemble.</p>
        <p>Merci pour votre engagement, votre professionnalisme et votre capacité à transformer des idées en réalisations concrètes. Je suis particulièrement fier du chemin parcouru avec les stagiaires et les jeunes talents que j'ai eu l'opportunité de former, de coacher et d'accompagner. J'espère avoir transmis bien plus que des connaissances techniques : une passion pour l'apprentissage continu, le sens de l'excellence, l'esprit d'équipe et la conviction que l'innovation naît avant tout de la curiosité et de la persévérance.</p>

        <p class="quote">« Ce n'est pas un adieu, mais simplement un au revoir. »</p>

        <p>J'espère sincèrement que nos chemins se recroiseront et que nous aurons l'occasion de collaborer à nouveau. Je vous souhaite à toutes et à tous beaucoup de succès, d'épanouissement et de belles réussites, tant sur le plan professionnel que personnel.</p>
        <p style="text-align:center"><strong>Au plaisir de rester en contact.</strong></p>

        <div class="signature">
          <div class="signature-name"><strong>Yves Mouaha Handy</strong></div>
          <div class="signature-role">Anciennement Squad Lead Data &amp; AI<br>GenAI &amp; Data Product Owner<br>Regional Data Scientist Credit Risk Manager</div>
          <div class="contacts">
            <a class="contact-link" href="mailto:yvesmouaha@yahoo.fr">✉️ yvesmouaha@yahoo.fr</a>
            <a class="contact-link" href="tel:+2250748782517">📱 +225 07 48 78 25 17</a>
            <a class="contact-link" href="https://www.linkedin.com/in/yves-mouaha-handy-084932120/" target="_blank" rel="noopener noreferrer">in LinkedIn</a>
          </div>
        </div>
      </div>

      <footer class="footer">Merci pour votre confiance, votre énergie et tous les moments partagés.</footer>
    </article>

    <button class="replay" id="replay" type="button" title="Relancer les messages">✨ Relancer</button>
  </main>

  <script>
    const PARTICLE_COUNT = 46;
    const MESSAGES = [
      "Merci SGCI ❤️",
      "4 années de défis et de réussites",
      "Merci à la Direction Générale",
      "Merci aux équipes Data & AI",
      "Merci à la Direction de l'Innovation",
      "11 filiales accompagnées en Afrique",
      "Fier du chemin parcouru",
      "Merci aux stagiaires et jeunes talents",
      "L'innovation continue 🚀",
      "À très bientôt 👋",
      "Restons connectés 🤝",
      "Un nouveau chapitre commence"
    ];

    const COLORS = ["#e9041e", "#ffffff", "#e6b263", "#9b9b9b"];
    const particles = document.getElementById("particles");
    const messagesContainer = document.getElementById("messagesContainer");
    const replay = document.getElementById("replay");

    const random = (min, max) => Math.random() * (max - min) + min;
    const choose = array => array[Math.floor(Math.random() * array.length)];

    function generateParticles() {
      particles.innerHTML = "";
      for (let i = 0; i < PARTICLE_COUNT; i++) {
        const particle = document.createElement("span");
        particle.className = "particle";
        particle.style.left = `${random(0, 100)}%`;
        particle.style.setProperty("--size", `${random(7, 42)}px`);
        particle.style.setProperty("--opacity", random(.12, .46).toFixed(2));
        particle.style.setProperty("--color", choose(COLORS));
        particle.style.setProperty("--duration", `${random(12, 25).toFixed(2)}s`);
        particle.style.setProperty("--delay", `${random(-22, 0).toFixed(2)}s`);
        particles.appendChild(particle);
      }
    }

    function showMessages() {
      messagesContainer.innerHTML = "";
      MESSAGES.forEach((text, index) => {
        const bubble = document.createElement("div");
        bubble.className = "message-bubble";
        bubble.textContent = text;
        bubble.style.left = `${random(15, 85)}%`;
        bubble.style.top = `${random(12, 84)}%`;
        bubble.style.animationDelay = `${(index * 1.15 + .5).toFixed(2)}s`;
        messagesContainer.appendChild(bubble);
      });

      window.setTimeout(() => {
        messagesContainer.innerHTML = "";
      }, MESSAGES.length * 1150 + 6500);
    }

    function replayEffects() {
      generateParticles();
      showMessages();
    }

    window.addEventListener("DOMContentLoaded", replayEffects);
    replay.addEventListener("click", replayEffects);
  </script>
</body>
</html>
