
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Soumyatanu Singha | Full-Stack Developer</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:wght@500;700;800&family=Instrument+Sans:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#eef2f7; --dot:#c9d3e0; --ink:#101827; --muted:#4b5a70; --panel:#ffffff; --line:#d3dce8;
  --accent:#2f4bff; --accent-ink:#ffffff; --signal:#e8453c;
  --display:'Bricolage Grotesque','Segoe UI',Helvetica,Arial,sans-serif;
  --body:'Instrument Sans','Segoe UI',Helvetica,Arial,sans-serif;
  box-sizing:border-box;
  padding-top:env(safe-area-inset-top,0px);
  padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme:dark){
  :root:not([data-theme="light"]){
    --bg:#0d1320; --dot:#1f2a3f; --ink:#e8edf7; --muted:#9aa8bf; --panel:#141c2e; --line:#26324a;
    --accent:#7d90ff; --accent-ink:#0d1320; --signal:#ff7a70;
  }
}
:root[data-theme="dark"]{
  --bg:#0d1320; --dot:#1f2a3f; --ink:#e8edf7; --muted:#9aa8bf; --panel:#141c2e; --line:#26324a;
  --accent:#7d90ff; --accent-ink:#0d1320; --signal:#ff7a70;
}
html{scroll-padding-top:env(safe-area-inset-top,0px);scroll-behavior:smooth}
*,*::before,*::after{box-sizing:border-box}
body{
  margin:0;background-color:var(--bg);
  background-image:radial-gradient(var(--dot) 1.2px,transparent 1.2px);
  background-size:26px 26px;
  color:var(--ink);font-family:var(--body);font-size:17px;line-height:1.6;
}
a{color:inherit}
:focus-visible{outline:3px solid var(--accent);outline-offset:3px;border-radius:4px}
.wrap{max-width:1040px;margin:0 auto;padding:0 24px}
 
/* hero */
.hero{display:grid;grid-template-columns:1.05fr 1fr;gap:32px;align-items:center;padding:72px 0 56px}
.hero h1{font-family:var(--display);font-weight:800;font-size:clamp(2.6rem,7vw,4.6rem);line-height:.98;letter-spacing:-.03em;margin:0 0 18px}
.hero p.lead{font-size:1.15rem;color:var(--muted);max-width:30em;margin:0 0 24px}
.facts{display:flex;flex-wrap:wrap;gap:8px 20px;margin:0 0 28px;padding:0;list-style:none;font-weight:500}
.facts li{padding-left:14px;position:relative}
.facts li::before{content:"";position:absolute;left:0;top:.62em;width:7px;height:7px;border-radius:50%;background:var(--accent)}
.btns{display:flex;flex-wrap:wrap;gap:12px}
.btn{display:inline-block;padding:11px 20px;border-radius:999px;font-weight:600;text-decoration:none;border:2px solid var(--ink)}
.btn.primary{background:var(--accent);border-color:var(--accent);color:var(--accent-ink)}
.btn:hover{background:var(--ink);border-color:var(--ink);color:var(--bg)}
 
/* mind map */
.map{width:100%;height:auto;display:block}
.map .edge{stroke:var(--ink);stroke-width:2;fill:none;stroke-dasharray:200;stroke-dashoffset:200;animation:draw 1.1s .2s ease-out forwards}
.map .node rect{fill:var(--panel);stroke:var(--ink);stroke-width:2;transition:fill .15s}
.map .node text{font-family:var(--display);font-weight:700;font-size:15px;fill:var(--ink);text-anchor:middle}
.map a:hover rect,.map a:focus-visible rect{fill:var(--accent)}
.map a:hover text,.map a:focus-visible text{fill:var(--accent-ink)}
.map .core circle{fill:var(--accent);stroke:var(--ink);stroke-width:2}
.map .core text{font-family:var(--display);font-weight:800;font-size:34px;fill:var(--accent-ink);text-anchor:middle}
@keyframes draw{to{stroke-dashoffset:0}}
@media (prefers-reduced-motion:reduce){.map .edge{animation:none;stroke-dashoffset:0}html{scroll-behavior:auto}}
 
/* sections */
section{padding:44px 0;border-top:2px solid var(--ink)}
h2{font-family:var(--display);font-weight:800;font-size:clamp(1.7rem,4vw,2.3rem);letter-spacing:-.02em;margin:0 0 26px}
.projects{display:grid;grid-template-columns:1fr 1fr;gap:24px}
.proj{background:var(--panel);border:2px solid var(--ink);border-radius:14px;padding:26px;box-shadow:6px 6px 0 var(--ink)}
.proj.alt{box-shadow:6px 6px 0 var(--signal)}
.proj h3{font-family:var(--display);font-size:1.45rem;margin:0 0 4px}
.proj .sub{color:var(--muted);margin:0 0 14px}
.proj ul{margin:0 0 18px;padding-left:1.1em}
.proj li{margin-bottom:8px}
.tags{display:flex;flex-wrap:wrap;gap:6px;margin:0;padding:0;list-style:none}
.tags li{font-size:.82rem;font-weight:600;padding:3px 10px;border:1.5px solid var(--line);border-radius:6px;background:var(--bg)}
.also{margin-top:26px;color:var(--muted)}
 
dl.skills{display:grid;grid-template-columns:150px 1fr;gap:14px 24px;margin:0}
dl.skills dt{font-family:var(--display);font-weight:700}
dl.skills dd{margin:0;display:flex;flex-wrap:wrap;gap:6px}
dl.skills dd span{font-size:.9rem;font-weight:500;padding:3px 12px;border-radius:999px;background:var(--panel);border:1.5px solid var(--line)}
 
.ach{display:grid;grid-template-columns:repeat(2,1fr);gap:18px 40px;margin:0;padding:0;list-style:none}
.ach li{padding-left:18px;border-left:4px solid var(--accent)}
.ach b{display:block;font-family:var(--display);font-size:1.1rem}
 
.contact p{max-width:34em;color:var(--muted);margin:0 0 20px}
footer{padding:28px 0 40px;color:var(--muted);font-size:.9rem;border-top:2px solid var(--ink)}
 
@media (max-width:820px){
  .hero{grid-template-columns:1fr;padding-top:40px}
  .projects,.ach{grid-template-columns:1fr}
  dl.skills{grid-template-columns:1fr;gap:6px}
  dl.skills dd{margin-bottom:12px}
}
</style>
</head>
<body>
<div class="wrap">
 
<header class="hero">
  <div>
    <h1>Soumyatanu Singha</h1>
    <p class="lead">Computer science student building real-time, full-stack web apps and solving problems with data structures and algorithms.</p>
    <ul class="facts">
      <li>CGPA 9.44</li>
      <li>500+ LeetCode problems</li>
      <li>GCECT Kolkata, class of 2029</li>
    </ul>
    <div class="btns">
      <a class="btn primary" href="#projects">See my projects</a>
      <a class="btn" href="mailto:soumyatanusingha@gmail.com">Email me</a>
    </div>
  </div>
 
  <svg class="map" viewBox="0 0 440 400" role="img" aria-label="Mind map linking to Projects, Skills, Achievements and Contact">
    <path class="edge" d="M220 200 L110 90"/>
    <path class="edge" d="M220 200 L335 95"/>
    <path class="edge" d="M220 200 L105 315"/>
    <path class="edge" d="M220 200 L335 310"/>
    <g class="core"><circle cx="220" cy="200" r="52"/><text x="220" y="212">SS</text></g>
    <g class="node"><a href="#projects"><rect x="50" y="68" width="120" height="44" rx="22"/><text x="110" y="96">Projects</text></a></g>
    <g class="node"><a href="#skills"><rect x="275" y="73" width="120" height="44" rx="22"/><text x="335" y="101">Skills</text></a></g>
    <g class="node"><a href="#achievements"><rect x="35" y="293" width="140" height="44" rx="22"/><text x="105" y="321">Achievements</text></a></g>
    <g class="node"><a href="#contact"><rect x="275" y="288" width="120" height="44" rx="22"/><text x="335" y="316">Contact</text></a></g>
  </svg>
</header>
 
<section id="projects">
  <h2>Projects</h2>
  <div class="projects">
    <article class="proj alt">
      <h3>Ambulance</h3>
      <p class="sub">Real-time ambulance booking and tracking</p>
      <ul>
        <li>Book ambulances within a 10 km radius and follow their live location.</li>
        <li>Streams movement and status updates over Socket.IO, fetched within 1 second.</li>
        <li>Separate sign-in flows for users and service providers with Google OAuth.</li>
        <li>Interactive LeafletJS maps with route visualization over 1000+ km.</li>
      </ul>
      <ul class="tags"><li>Next.js</li><li>Prisma</li><li>MongoDB</li><li>Socket.IO</li><li>LeafletJS</li><li>Tailwind CSS</li></ul>
    </article>
    <article class="proj">
      <h3>NeuralNotes</h3>
      <p class="sub">AI learning and mind mapping platform</p>
      <ul>
        <li>Uses the Gemini API to summarize images and YouTube videos up to 2 hours long.</li>
        <li>ReactFlow canvas handling mind maps with up to 500 connected nodes.</li>
        <li>OAuth login, with maps and history stored in MongoDB.</li>
        <li>Cut UI development time by 35% using Tailwind components.</li>
      </ul>
      <ul class="tags"><li>Next.js</li><li>ReactFlow</li><li>Prisma</li><li>MongoDB</li><li>Gemini API</li><li>Tailwind CSS</li></ul>
    </article>
  </div>
  <p class="also">Also built: a Spotify clone, a real-time chat app, an e-commerce store and a Twitter clone.</p>
</section>
 
<section id="skills">
  <h2>Skills</h2>
  <dl class="skills">
    <dt>Languages</dt><dd><span>Java</span><span>JavaScript</span><span>HTML</span><span>CSS</span></dd>
    <dt>Frontend</dt><dd><span>React</span><span>Next.js</span><span>Tailwind CSS</span><span>React Flow</span><span>LeafletJS</span></dd>
    <dt>Backend</dt><dd><span>Node.js</span><span>Express.js</span><span>Socket.IO</span><span>Prisma ORM</span><span>MongoDB</span></dd>
    <dt>Auth</dt><dd><span>OAuth</span><span>JWT</span></dd>
    <dt>Fundamentals</dt><dd><span>Data Structures &amp; Algorithms</span><span>OOP</span><span>Git</span></dd>
  </dl>
</section>
 
<section id="achievements">
  <h2>Achievements</h2>
  <ul class="ach">
    <li><b>500+ problems on LeetCode</b>Steady practice in data structures and algorithms.</li>
    <li><b>95% in ISC, 98% in ICSE</b>Class 12 and Class 10, with class topper rank throughout high school.</li>
    <li><b>House Captain</b>Led my house and anchored annual school events.</li>
    <li><b>Debate, chess and elocution</b>Won several inter-school and intra-school competitions.</li>
  </ul>
</section>
 
<section id="contact" class="contact">
  <h2>Contact</h2>
  <p>I'm open to internships and projects. The quickest way to reach me is email.</p>
  <div class="btns">
    <a class="btn primary" href="mailto:soumyatanusingha@gmail.com">soumyatanusingha@gmail.com</a>
    <a class="btn" href="https://github.com/soumyatanusingha">GitHub</a>
  </div>
</section>
 
<footer>Soumyatanu Singha, Kolkata, West Bengal</footer>
</div>
</body>
</html>
 
