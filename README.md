<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Srivatsan Sheshathri | Mechanical Design & Automation Engineer</title>
<meta name="description" content="Portfolio of Srivatsan Sheshathri — Mechanical Design & Automation Engineer specializing in CAD, manufacturing simulation, plant layout, digital twin and Industry 4.0.">
<style>
:root{
  --navy:#0b1220; --navy2:#111a2b; --panel:#141f33; --line:#22314d;
  --text:#e8ecf3; --muted:#9fb0c8; --amber:#e8952b; --amber2:#ffb454;
  --radius:10px;
  padding-top: env(safe-area-inset-top,0px); padding-bottom: env(safe-area-inset-bottom,0px);
}
*{box-sizing:border-box; margin:0; padding:0;}
html{scroll-behavior:smooth; scroll-padding-top: calc(72px + env(safe-area-inset-top,0px));}
body{
  background:var(--navy); color:var(--text);
  font-family:'Segoe UI',Arial,Helvetica,sans-serif;
  line-height:1.6;
  background-image:
   linear-gradient(rgba(232,149,43,.035) 1px, transparent 1px),
   linear-gradient(90deg, rgba(232,149,43,.035) 1px, transparent 1px);
  background-size:40px 40px;
}
img{max-width:100%; display:block;}
a{color:inherit; text-decoration:none;}
.wrap{max-width:1180px; margin:0 auto; padding:0 24px;}
h1,h2,h3{font-family:'Segoe UI',Arial,sans-serif; letter-spacing:.3px;}
.eyebrow{color:var(--amber2); font-size:13px; letter-spacing:3px; text-transform:uppercase; font-weight:700;}
.section-title{font-size:clamp(26px,3.5vw,38px); margin:10px 0 8px; color:#fff;}
.section-sub{color:var(--muted); max-width:640px; margin-bottom:36px;}
section{padding:90px 0;}
.reveal{opacity:0; transform:translateY(24px); transition:opacity .7s ease, transform .7s ease;}
.reveal.show{opacity:1; transform:translateY(0);}

/* NAV */
header{position:fixed; top:0; left:0; right:0; z-index:100;
  padding: calc(14px + env(safe-area-inset-top,0px)) 0 14px;
  background:rgba(11,18,32,.85); backdrop-filter:blur(10px);
  border-bottom:1px solid var(--line); transition:.3s;}
nav{display:flex; align-items:center; justify-content:space-between;}
.logo{font-weight:800; letter-spacing:1px; font-size:15px;}
.logo span{color:var(--amber);}
.navlinks{display:flex; gap:26px; align-items:center;}
.navlinks a{font-size:13.5px; color:var(--muted); font-weight:600; letter-spacing:.3px;}
.navlinks a:hover{color:var(--amber2);}
.btn{display:inline-block; padding:11px 22px; border-radius:6px; font-weight:700; font-size:13.5px; letter-spacing:.4px; cursor:pointer; border:1px solid transparent; transition:.25s;}
.btn-primary{background:var(--amber); color:#101010;}
.btn-primary:hover{background:var(--amber2); transform:translateY(-2px);}
.btn-outline{border-color:var(--amber); color:var(--amber2);}
.btn-outline:hover{background:rgba(232,149,43,.1);}
.navcta{display:flex; gap:12px; align-items:center;}
.hamb{display:none; flex-direction:column; gap:5px; cursor:pointer;}
.hamb span{width:24px; height:2px; background:#fff;}
@media(max-width:900px){
  .navlinks{position:fixed; top:64px; right:0; left:0; background:var(--navy2); flex-direction:column; padding:20px; gap:16px; border-bottom:1px solid var(--line); transform:translateY(-130%); transition:.3s;}
  .navlinks.open{transform:translateY(0);}
  .hamb{display:flex;}
  .navcta .btn-outline{display:none;}
}

/* HERO */
.hero{padding:170px 0 100px; position:relative; overflow:hidden;}
.hero-grid{display:grid; grid-template-columns:1.15fr .85fr; gap:50px; align-items:center;}
@media(max-width:900px){.hero-grid{grid-template-columns:1fr;}}
.hero h1{font-size:clamp(32px,5vw,54px); line-height:1.12; color:#fff; margin-bottom:20px;}
.hero h1 em{font-style:normal; color:var(--amber2);}
.hero p.sub{color:#c4d0e2; font-size:17px; max-width:560px; margin-bottom:14px;}
.hero p.support{color:var(--muted); font-size:14.5px; max-width:560px; margin-bottom:30px;}
.hero-actions{display:flex; gap:14px; flex-wrap:wrap; align-items:center; margin-bottom:18px;}
.connect{color:var(--amber2); font-weight:700; font-size:14px;}
.hero-visual{position:relative; border:1px solid var(--line); border-radius:14px; background:var(--panel); padding:26px; box-shadow:0 30px 60px rgba(0,0,0,.4);}
.hero-visual .tag{position:absolute; top:-12px; left:20px; background:var(--amber); color:#101010; font-size:11px; font-weight:800; letter-spacing:1px; padding:5px 12px; border-radius:20px;}
.profile-row{display:flex; gap:16px; align-items:center; margin-bottom:18px;}
.profile-row img{width:70px; height:70px; border-radius:50%; object-fit:cover; border:2px solid var(--amber);}
.profile-row .name{font-weight:800; color:#fff;}
.profile-row .role{color:var(--amber2); font-size:12.5px;}
.blueprint{border:1px dashed var(--line); border-radius:10px; padding:16px; font-family:monospace; font-size:11.5px; color:#7f93b3; background:repeating-linear-gradient(0deg, rgba(255,255,255,.02) 0 1px, transparent 1px 20px);}
.blueprint .ln{display:flex; justify-content:space-between; padding:4px 0; border-bottom:1px solid rgba(255,255,255,.05);}
.blueprint .ln b{color:var(--amber2);}
.stats{display:grid; grid-template-columns:repeat(3,1fr); gap:10px; margin-top:18px;}
.stat{background:var(--navy2); border:1px solid var(--line); border-radius:8px; padding:14px 8px; text-align:center;}
.stat b{display:block; font-size:22px; color:var(--amber2);}
.stat span{font-size:11px; color:var(--muted);}

/* ABOUT */
.about-grid{display:grid; grid-template-columns:1.3fr .9fr; gap:50px;}
@media(max-width:900px){.about-grid{grid-template-columns:1fr;}}
.about-grid p{color:#c4d0e2; margin-bottom:14px;}
.focus-box{border:1px solid var(--line); border-radius:12px; padding:22px; background:var(--panel);}
.focus-box h4{color:var(--amber2); font-size:13px; letter-spacing:1.5px; margin-bottom:14px;}
.focus-chip{display:flex; align-items:center; gap:10px; padding:10px 0; border-bottom:1px solid var(--line); font-size:13.5px; font-weight:600;}
.focus-chip:last-child{border:none;}
.dot{width:7px; height:7px; border-radius:50%; background:var(--amber);}

/* CARDS GRID */
.grid4{display:grid; grid-template-columns:repeat(4,1fr); gap:18px;}
@media(max-width:900px){.grid4{grid-template-columns:repeat(2,1fr);}}
@media(max-width:520px){.grid4{grid-template-columns:1fr;}}
.card{background:var(--panel); border:1px solid var(--line); border-radius:12px; padding:22px; transition:.25s;}
.card:hover{border-color:var(--amber); transform:translateY(-4px);}
.card .ic{font-size:24px; margin-bottom:10px;}
.card h4{font-size:15px; color:#fff; margin-bottom:6px;}
.card p{font-size:12.5px; color:var(--muted);}

/* SKILLS */
.skill-grid{display:grid; grid-template-columns:repeat(2,1fr); gap:20px;}
@media(max-width:800px){.skill-grid{grid-template-columns:1fr;}}
.skill-cat{background:var(--panel); border:1px solid var(--line); border-radius:12px; padding:24px;}
.skill-cat h4{color:var(--amber2); font-size:13px; letter-spacing:1.5px; margin-bottom:16px; text-transform:uppercase;}
.tagrow{display:flex; flex-wrap:wrap; gap:9px;}
.tagrow span{background:var(--navy2); border:1px solid var(--line); padding:7px 13px; border-radius:20px; font-size:12.5px; color:#dbe4f2;}

/* TIMELINE */
.timeline{position:relative; padding-left:34px;}
.timeline::before{content:''; position:absolute; left:8px; top:6px; bottom:6px; width:2px; background:var(--line);}
.tl-item{position:relative; margin-bottom:44px;}
.tl-item::before{content:''; position:absolute; left:-30px; top:4px; width:16px; height:16px; border-radius:50%; background:var(--amber); border:3px solid var(--navy);}
.tl-item .role{color:var(--amber2); font-weight:700; font-size:13px; letter-spacing:1px;}
.tl-item h3{color:#fff; font-size:19px; margin:4px 0 2px;}
.tl-item .date{color:var(--muted); font-size:12.5px; margin-bottom:10px;}
.tl-item ul{padding-left:18px; color:#c4d0e2; font-size:14px;}
.tl-item li{margin-bottom:6px;}

/* PROJECTS */
.proj-grid{display:grid; grid-template-columns:repeat(2,1fr); gap:22px; max-width:920px; margin:0 auto;}
@media(max-width:760px){.proj-grid{grid-template-columns:1fr;}}
.proj-card{background:var(--panel); border:1px solid var(--line); border-radius:14px; overflow:hidden; display:flex; flex-direction:column;}
.proj-thumb{height:140px; background:linear-gradient(135deg,#1a2740,#0d1524); position:relative; display:flex; align-items:center; justify-content:center; font-size:38px; border-bottom:1px solid var(--line);}
.proj-body{padding:20px; flex:1; display:flex; flex-direction:column;}
.proj-cat{color:var(--amber2); font-size:11px; letter-spacing:1px; text-transform:uppercase; font-weight:700; margin-bottom:8px;}
.proj-body h3{color:#fff; font-size:17px; margin-bottom:8px;}
.proj-body p{color:var(--muted); font-size:13px; margin-bottom:14px; flex:1;}
.proj-body .btn{align-self:flex-start;}

/* MODAL */
.modal-overlay{position:fixed; inset:0; background:rgba(4,7,14,.85); z-index:200; display:none; align-items:center; justify-content:center; padding:20px;}
.modal-overlay.open{display:flex;}
.modal{background:var(--navy2); border:1px solid var(--line); border-radius:14px; max-width:640px; width:100%; max-height:86vh; overflow-y:auto; padding:32px; position:relative;}
.modal-close{position:absolute; top:16px; right:18px; cursor:pointer; font-size:22px; color:var(--muted); background:none; border:none;}
.modal h3{color:#fff; font-size:22px; margin-bottom:4px;}
.modal .proj-cat{margin-bottom:18px;}
.modal h5{color:var(--amber2); font-size:12px; letter-spacing:1.5px; text-transform:uppercase; margin:18px 0 6px;}
.modal p, .modal li{color:#c4d0e2; font-size:14px;}
.modal ul{padding-left:18px;}

/* RESEARCH */
.pub-card{background:var(--panel); border:1px solid var(--line); border-left:3px solid var(--amber); border-radius:10px; padding:26px; margin-bottom:20px;}
.pub-card h3{color:#fff; font-size:18px; margin-bottom:6px;}
.pub-card .meta{color:var(--amber2); font-size:12.5px; margin-bottom:12px;}
.pub-card p{color:var(--muted); font-size:13.5px; margin-bottom:14px;}
.chiprow{display:flex; flex-wrap:wrap; gap:8px; margin-bottom:16px;}
.chiprow span{font-size:11.5px; background:var(--navy2); border:1px solid var(--line); padding:5px 11px; border-radius:14px; color:#c4d0e2;}

/* CERTS */
.cert-grid{display:grid; grid-template-columns:repeat(3,1fr); gap:20px;}
@media(max-width:900px){.cert-grid{grid-template-columns:1fr;}}
.cert-card{background:var(--panel); border:1px solid var(--line); border-radius:12px; overflow:hidden;}
.cert-card img{height:150px; width:100%; object-fit:cover; cursor:pointer; border-bottom:1px solid var(--line);}
.cert-body{padding:16px;}
.cert-body h4{color:#fff; font-size:14px; margin-bottom:4px;}
.cert-body p{color:var(--muted); font-size:12px; margin-bottom:10px;}
.viewlink{color:var(--amber2); font-size:12.5px; font-weight:700; cursor:pointer;}

/* ACHIEVEMENTS */
.ach-grid{display:grid; grid-template-columns:repeat(4,1fr); gap:18px;}
@media(max-width:960px){.ach-grid{grid-template-columns:repeat(2,1fr);}}
@media(max-width:520px){.ach-grid{grid-template-columns:1fr;}}
.ach-card{background:var(--panel); border:1px solid var(--line); border-radius:12px; overflow:hidden;}
.ach-card img{height:130px; width:100%; object-fit:cover; cursor:pointer;}
.ach-card .cap{padding:12px 14px; font-size:12.5px; color:#dbe4f2; font-weight:600;}

/* GALLERY */
.gallery{columns:4 220px; column-gap:14px;}
@media(max-width:700px){.gallery{columns:2 160px;}}
.gallery img{width:100%; margin-bottom:14px; border-radius:8px; cursor:pointer; border:1px solid var(--line);}

/* LIGHTBOX */
.lightbox{position:fixed; inset:0; background:rgba(3,5,10,.92); z-index:300; display:none; align-items:center; justify-content:center; padding:24px;}
.lightbox.open{display:flex;}
.lightbox img{max-width:90vw; max-height:85vh; border-radius:6px;}
.lightbox .lb-close{position:absolute; top:20px; right:30px; font-size:32px; color:#fff; cursor:pointer; background:none; border:none;}

/* EDUCATION */
.edu-item{background:var(--panel); border:1px solid var(--line); border-radius:12px; padding:24px; margin-bottom:18px; display:flex; justify-content:space-between; flex-wrap:wrap; gap:10px;}
.edu-item h3{color:#fff; font-size:17px;}
.edu-item .deg{color:var(--amber2); font-size:13.5px; margin:4px 0;}
.edu-item .meta{color:var(--muted); font-size:12.5px;}
.edu-item .yr{color:var(--muted); font-size:13px; white-space:nowrap;}

/* CTA */
.cta{background:linear-gradient(135deg,#182642,#0b1220); border-top:1px solid var(--line); border-bottom:1px solid var(--line); text-align:center;}
.cta h2{color:#fff; font-size:clamp(24px,4vw,36px); margin-bottom:14px;}
.cta p{color:var(--muted); max-width:560px; margin:0 auto 26px;}
.cta .hero-actions{justify-content:center;}

/* CONTACT */
.contact-grid{display:grid; grid-template-columns:1fr 1fr; gap:40px;}
@media(max-width:800px){.contact-grid{grid-template-columns:1fr;}}
.contact-item{display:flex; gap:14px; align-items:center; padding:16px 0; border-bottom:1px solid var(--line);}
.contact-item .ic{width:38px; height:38px; border-radius:8px; background:var(--navy2); border:1px solid var(--line); display:flex; align-items:center; justify-content:center; font-size:16px; color:var(--amber2);}
.contact-item a{color:#dbe4f2; font-weight:600; font-size:14.5px;}

footer{border-top:1px solid var(--line); padding:40px 0; text-align:center; color:var(--muted); font-size:12.5px;}
footer .logo{margin-bottom:8px; font-size:15px;}
footer .tag{color:var(--amber2); margin-bottom:14px; font-size:12px; letter-spacing:1px;}
</style>
</head>
<body>

<header id="header">
  <div class="wrap nav">
    <div class="logo">SRIVATSAN <span>SHESHATHRI</span></div>
    <div class="navlinks" id="navlinks">
      <a href="#about" class="navlink">About</a>
      <a href="#skills" class="navlink">Skills</a>
      <a href="#experience" class="navlink">Experience</a>
      <a href="#projects" class="navlink">Projects</a>
      <a href="#research" class="navlink">Research</a>
      <a href="#achievements" class="navlink">Achievements</a>
      <a href="#gallery" class="navlink">Gallery</a>
      <a href="#contact" class="navlink">Contact</a>
    </div>
    <div class="navcta">
      <a href="RESUME_HREF" download class="btn btn-outline">Download Resume</a>
      <div class="hamb" id="hamb"><span></span><span></span><span></span></div>
    </div>
  </div>
</header>

<!-- HERO -->
<section class="hero">
  <div class="wrap hero-grid">
    <div class="reveal show">
      <div class="eyebrow">Mechanical Design &amp; Automation Engineer</div>
      <h1>Designing Mechanical Systems for <em>Smarter Manufacturing</em></h1>
      <p class="sub">Mechanical Design &amp; Automation Engineer focused on CAD, manufacturing simulation, plant layout, material handling, digital twin technologies, and Industry 4.0.</p>
      <p class="support">Hands-on experience in 3D modelling, DELMIA-based manufacturing simulation, plant layout optimization, engineering analysis, and smart manufacturing systems.</p>
      <div class="hero-actions">
        <a href="#projects" class="btn btn-primary">Explore My Work</a>
        <a href="RESUME_HREF" download class="btn btn-outline">Download Resume</a>
      </div>
      <a href="#contact" class="connect">Let's Connect →</a>
    </div>
    <div class="hero-visual reveal show">
      <span class="tag">ENGINEERING PROFILE</span>
      <div class="profile-row">
        <img src="PLACEHOLDER_PROFILE" alt="Srivatsan Sheshathri profile photo">
        <div>
          <div class="name">Srivatsan Sheshathri</div>
          <div class="role">Design Engineer · Chennai, TN</div>
        </div>
      </div>
      <div class="blueprint">
        <div class="ln"><span>MODULE</span><b>Gearbox Assembly Layout</b></div>
        <div class="ln"><span>TOOL</span><b>DELMIA 3DEXPERIENCE</b></div>
        <div class="ln"><span>PROCESS</span><b>Plant Layout · Material Handling</b></div>
        <div class="ln"><span>SYSTEM</span><b>Digital Twin · AMR Logistics</b></div>
        <div class="ln"><span>STATUS</span><b style="color:#7ee08a">Simulation Verified</b></div>
      </div>
      <div class="stats">
        <div class="stat"><b>2</b><span>Industry Internships</span></div>
        <div class="stat"><b>3</b><span>Core Projects</span></div>
        <div class="stat"><b>2</b><span>Publications</span></div>
      </div>
    </div>
  </div>
</section>

<!-- ABOUT -->
<section id="about">
  <div class="wrap">
    <div class="eyebrow reveal">Who I Am</div>
    <h2 class="section-title reveal">About Me</h2>
    <div class="about-grid">
      <div class="reveal">
        <p>I am a Mechanical and Automation Engineering graduate with a strong interest in mechanical design, digital manufacturing, automation and Industry 4.0. My experience includes 3D modelling, manufacturing simulation, plant layout development, material handling and engineering analysis.</p>
        <p>I have worked with <b>Creo Parametric</b>, <b>SolidWorks</b>, <b>CATIA</b>, and <b>DELMIA</b> for manufacturing simulation, alongside <b>ANSYS</b> for engineering analysis — applying these tools to real shop-floor layout and material-handling challenges during my industry internships.</p>
        <p>I also hold a Minor Degree in Cloud Computing and IoT, which complements my interest in smart manufacturing, predictive maintenance and connected factory systems.</p>
      </div>
      <div class="focus-box reveal">
        <h4>ENGINEERING FOCUS</h4>
        <div class="focus-chip"><span class="dot"></span> Mechanical Design</div>
        <div class="focus-chip"><span class="dot"></span> Manufacturing</div>
        <div class="focus-chip"><span class="dot"></span> Automation</div>
        <div class="focus-chip"><span class="dot"></span> Digital Twin</div>
        <div class="focus-chip"><span class="dot"></span> Smart Factory</div>
        <div class="focus-chip"><span class="dot"></span> Industry 4.0</div>
      </div>
    </div>
  </div>
</section>

<!-- HIGHLIGHTS -->
<section style="background:var(--navy2); border-top:1px solid var(--line); border-bottom:1px solid var(--line);">
  <div class="wrap">
    <div class="eyebrow reveal">Engineering Profile</div>
    <h2 class="section-title reveal">Highlights</h2>
    <div class="grid4 reveal">
      <div class="card"><div class="ic">📐</div><h4>3D CAD &amp; Modelling</h4><p>Creo, SolidWorks, CATIA</p></div>
      <div class="card"><div class="ic">🏭</div><h4>Manufacturing Simulation</h4><p>DELMIA shop-floor simulation</p></div>
      <div class="card"><div class="ic">🗺️</div><h4>Plant Layout</h4><p>Layout optimization &amp; flow</p></div>
      <div class="card"><div class="ic">📦</div><h4>Material Handling</h4><p>Shop-floor logistics</p></div>
      <div class="card"><div class="ic">📊</div><h4>Engineering Analysis</h4><p>ANSYS structural analysis</p></div>
      <div class="card"><div class="ic">🔁</div><h4>Digital Twin</h4><p>Simulation-optimization frameworks</p></div>
      <div class="card"><div class="ic">🤖</div><h4>Automation</h4><p>AMR-based logistics concepts</p></div>
      <div class="card"><div class="ic">🌐</div><h4>Industry 4.0</h4><p>Smart, connected manufacturing</p></div>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="wrap">
    <div class="eyebrow reveal">Capabilities</div>
    <h2 class="section-title reveal">Engineering Toolkit</h2>
    <div class="skill-grid reveal">
      <div class="skill-cat">
        <h4>Mechanical Design &amp; CAD</h4>
        <div class="tagrow"><span>Creo Parametric</span><span>SolidWorks</span><span>CATIA</span><span>Autodesk Fusion</span><span>DraftSight</span></div>
      </div>
      <div class="skill-cat">
        <h4>Manufacturing &amp; Simulation</h4>
        <div class="tagrow"><span>DELMIA</span><span>Visual Components</span><span>SEE NC Mill &amp; Turn</span><span>FluidSIM</span></div>
      </div>
      <div class="skill-cat">
        <h4>Engineering Analysis</h4>
        <div class="tagrow"><span>ANSYS</span><span>Structural Analysis</span><span>3D Modelling</span><span>Simulation</span></div>
      </div>
      <div class="skill-cat">
        <h4>Manufacturing</h4>
        <div class="tagrow"><span>Manufacturing Operations</span><span>Plant Layout</span><span>Material Handling</span><span>Process Improvement</span><span>Kaizen</span></div>
      </div>
    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience" style="background:var(--navy2); border-top:1px solid var(--line); border-bottom:1px solid var(--line);">
  <div class="wrap">
    <div class="eyebrow reveal">Where I've Worked</div>
    <h2 class="section-title reveal">Industry Exposure</h2>
    <div class="timeline reveal">
      <div class="tl-item">
        <div class="role">EXPERIENCE 01 · MANUFACTURING SIMULATION / PLANT LAYOUT</div>
        <h3>Ashok Leyland — Ennore Unit</h3>
        <div class="date">Aug 2025 – Oct 2025</div>
        <ul>
          <li>Trained in 3DEXPERIENCE DELMIA for 3D modelling and simulation.</li>
          <li>Developed a 9-speed gearbox assembly shop-floor layout.</li>
          <li>Worked on Hosur H1 plant layout optimization.</li>
          <li>Applied manufacturing simulation and material-handling concepts to improve shop-floor flow and layout efficiency.</li>
        </ul>
        <div style="margin-top:10px; display:flex; gap:16px; flex-wrap:wrap;">
          <span class="viewlink" onclick="openLB('PLACEHOLDER_ALCOMPLETION')">View Completion Certificate →</span>
          <span class="viewlink" onclick="openLB('PLACEHOLDER_LORAL')">View Letter of Recommendation →</span>
        </div>
      </div>
      <div class="tl-item">
        <div class="role">EXPERIENCE 02</div>
        <h3>Sundaram Industries — TVS Rubber Factory</h3>
        <div class="date">Jun 2024 – Jul 2024</div>
        <ul>
          <li>Gained hands-on exposure to manufacturing operations.</li>
          <li>Observed shop-floor processes and workflow management.</li>
          <li>Applied Kaizen and continuous improvement principles to understand operational efficiency.</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects">
  <div class="wrap">
    <div class="eyebrow reveal">Centerpiece Work</div>
    <h2 class="section-title reveal">Engineering Projects</h2>
    <div class="proj-grid reveal">
      <div class="proj-card">
        <div class="proj-thumb">🏭</div>
        <div class="proj-body">
          <div class="proj-cat">Manufacturing Simulation · DELMIA · Plant Layout · Material Handling</div>
          <h3>Plant Layout & Manufacturing Simulation — Gearbox Assembly Line &amp; Hosur H1</h3>
          <p>Designed and simulated a 3D gearbox assembly shop-floor layout in DELMIA, and optimized the Hosur H1 plant layout and material-handling system using 3D modelling and manufacturing simulation.</p>
          <button class="btn btn-outline" onclick="openModal('p1')">View Details</button>
        </div>
      </div>
      <div class="proj-card">
        <div class="proj-thumb">📡</div>
        <div class="proj-body">
          <div class="proj-cat">IoT · Predictive Maintenance</div>
          <h3>IoT-Enabled Predictive Maintenance</h3>
          <p>IoT-based predictive maintenance system for a mechanical system using ESP32, MPU6050 and DHT11 sensors with real-time vibration &amp; temperature monitoring.</p>
          <button class="btn btn-outline" onclick="openModal('p3')">View Details</button>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- MODALS -->
<div class="modal-overlay" id="modal-p1"><div class="modal">
  <button class="modal-close" onclick="closeModal('p1')">&times;</button>
  <div class="proj-cat">Manufacturing Simulation · DELMIA · Plant Layout · Material Handling</div>
  <h3>Plant Layout &amp; Manufacturing Simulation — Gearbox Assembly Line &amp; Hosur H1</h3>
  <h5>Problem</h5><p>Shop-floor layouts for new assembly lines, and existing plant layouts with material-flow inefficiencies, need validation and optimization before physical implementation to avoid costly rework.</p>
  <h5>Objective</h5><p>Design and simulate a 3D gearbox assembly shop-floor layout, and optimize the Hosur H1 plant layout and material-handling system for improved flow.</p>
  <h5>Methodology</h5><p>Modelled the shop floor in DELMIA, laid out assembly stations for the 9-speed gearbox line, and simulated manufacturing flow and material movement. Applied the same 3D modelling and simulation approach to analyze and re-arrange the Hosur H1 layout.</p>
  <h5>Tools Used</h5><p>DELMIA 3DEXPERIENCE, 3D modelling tools</p>
  <h5>Engineering Approach</h5><p>Applied manufacturing simulation, plant-layout and material-handling principles to sequence stations, validate material movement paths, and identify flow-efficiency improvements.</p>
  <h5>Outcome</h5><p>A validated 3D shop-floor and assembly line layout for the gearbox line, and an optimized layout concept for improved shop-floor flow and efficiency at Hosur H1.</p>
  <h5>Key Takeaways</h5><p>Practical, end-to-end exposure to DELMIA-based simulation and plant layout optimization for real industrial assembly and material-handling decisions.</p>
  <p style="margin-top:14px; font-size:12.5px; color:var(--muted);">Part of the team B.E. project "Modelling, Simulation and Optimization of Plant Layout and Material Handling Systems in Manufacturing Industry" (SVCE, May 2026).</p>
  <a href="MN08_HREF" download class="btn btn-outline" style="margin-top:14px;">Download Full Project Report</a>
</div></div>

<div class="modal-overlay" id="modal-p3"><div class="modal">
  <button class="modal-close" onclick="closeModal('p3')">&times;</button>
  <div class="proj-cat">IoT · Predictive Maintenance · Smart Manufacturing</div>
  <h3>IoT &amp; Cloud-Enabled Predictive Maintenance</h3>
  <h5>Problem</h5><p>Mechanical systems can fail unexpectedly without early condition monitoring.</p>
  <h5>Objective</h5><p>Build a predictive maintenance system that detects early signs of mechanical faults.</p>
  <h5>Methodology</h5><p>Collected real-time vibration and temperature data using ESP32, MPU6050 and DHT11 sensors; applied RMS and FFT signal analysis; trained a Random Forest model for machine-condition classification.</p>
  <h5>Tools Used</h5><p>ESP32, MPU6050, DHT11, ThingSpeak, Random Forest ML</p>
  <h5>Engineering Approach</h5><p>Framed as a mechanical/automation smart-manufacturing project — using sensor data and signal analysis to support condition-based maintenance decisions.</p>
  <h5>Outcome</h5><p>A system capable of detecting imbalance, misalignment and wear with real-time monitoring and automated alerts via ThingSpeak cloud integration.</p>
  <h5>Key Takeaways</h5><p>Applying IoT and cloud tools to strengthen mechanical predictive-maintenance workflows.</p>
  <p style="margin-top:14px; font-size:12.5px; color:var(--muted);">Minor degree project report — "IoT and Cloud-Enabled Predictive Maintenance for a Mechanical System" (SVCE, May 2026).</p>
  <a href="MINORREPORT_HREF" download class="btn btn-outline" style="margin-top:14px;">Download Full Project Report</a>
</div></div>

<!-- RESEARCH -->
<section id="research" style="background:var(--navy2); border-top:1px solid var(--line); border-bottom:1px solid var(--line);">
  <div class="wrap">
    <div class="eyebrow reveal">Publications</div>
    <h2 class="section-title reveal">Research &amp; Technical Publications</h2>
    <div class="reveal">
      <div class="pub-card">
        <h3>Digital Twin-enabled Simulation-optimization Framework for Autonomous Mobile Robot Logistics in Smart Manufacturing</h3>
        <div class="meta">Asian Journal of Advanced Research and Reports · 2026</div>
        <div class="chiprow"><span>Digital Twin</span><span>AMR</span><span>Smart Manufacturing</span><span>Manufacturing Optimization</span><span>DELMIA 3DEXPERIENCE</span></div>
        <p>DOI: <a href="https://doi.org/10.9734/ajarr/2026/v20i91448" target="_blank" style="color:var(--amber2)">10.9734/ajarr/2026/v20i91448</a></p>
        <a href="https://doi.org/10.9734/ajarr/2026/v20i91448" target="_blank" class="btn btn-outline">View Publication</a>
      </div>
      <div class="pub-card">
        <h3>Soft Robotics: Progress and Prospects</h3>
        <div class="meta">4th International Conference on Multifunctional Materials and Radiation Measurements (ICMMRM 2025)</div>
        <div class="chiprow"><span>Shape Memory Alloys</span><span>Elastomers</span><span>Robotic Actuation</span><span>Soft Robotics</span></div>
        <a href="https://drive.google.com/file/d/1kR0dcQVFXKcXWcKF0xw9rW0uCly7aikr/view?usp=sharing" target="_blank" class="btn btn-outline">View Paper / Presentation</a>
        <span class="viewlink" style="margin-left:16px;" onclick="openLB('PLACEHOLDER_ICMMRM')">View Certificate of Appreciation →</span>
      </div>
    </div>
  </div>
</section>

<!-- CERTIFICATIONS -->
<section id="certs">
  <div class="wrap">
    <div class="eyebrow reveal">Professional Development</div>
    <h2 class="section-title reveal">Certifications &amp; Training</h2>
    <div class="cert-grid reveal">
      <div class="cert-card">
        <img src="PLACEHOLDER_NPTEL" alt="NPTEL Biomass Conversion and Biorefinery certificate" onclick="openLB(this.src)">
        <div class="cert-body"><h4>Biomass Conversion and Biorefinery</h4><p>NPTEL Online Certification · Jan–Apr 2025 · 12-week course · Score: 60%</p><span class="viewlink" onclick="openLB('PLACEHOLDER_NPTEL')">View Certificate →</span></div>
      </div>
      <div class="cert-card">
        <img src="PLACEHOLDER_ISTTP" alt="AI-Driven Smart Systems training certificate" onclick="openLB(this.src)">
        <div class="cert-body"><h4>AI-Driven Smart Systems</h4><p>International Short-Term Training Programme · SVCE, Dept. of ECE · 7–12 July 2025</p><span class="viewlink" onclick="openLB('PLACEHOLDER_ISTTP')">View Certificate →</span></div>
      </div>
      <div class="cert-card">
        <img src="PLACEHOLDER_ENG23" alt="Engineering 23 certificate of participation" onclick="openLB(this.src)">
        <div class="cert-body"><h4>Engineering '23</h4><p>Certificate of Participation · SVCE, Dept. of Mechanical &amp; Automation Engineering</p><span class="viewlink" onclick="openLB('PLACEHOLDER_ENG23')">View Certificate →</span></div>
      </div>
      <div class="cert-card">
        <img src="PLACEHOLDER_ICMMRM" alt="ICMMRM 2025 certificate of appreciation" onclick="openLB(this.src)">
        <div class="cert-body"><h4>ICMMRM-2025 Certificate of Appreciation</h4><p>For presenting "Bio-Inspired Soft Robots: Progress and Prospects" · SSN &amp; SVCE · 21–22 Mar 2025</p><span class="viewlink" onclick="openLB('PLACEHOLDER_ICMMRM')">View Certificate →</span></div>
      </div>
      <div class="cert-card">
        <img src="PLACEHOLDER_ALCOMPLETION" alt="Ashok Leyland internship completion certificate" onclick="openLB(this.src)">
        <div class="cert-body"><h4>Ashok Leyland — Internship Completion</h4><p>Institution Training Certificate · 21 Aug – 17 Oct 2025</p><span class="viewlink" onclick="openLB('PLACEHOLDER_ALCOMPLETION')">View Certificate →</span></div>
      </div>
      <div class="cert-card">
        <img src="PLACEHOLDER_LORAL" alt="Letter of recommendation from Ashok Leyland" onclick="openLB(this.src)">
        <div class="cert-body"><h4>Letter of Recommendation — Ashok Leyland</h4><p>Project Planning Division · Deputy General Manager, Dr. Arvind A R</p><span class="viewlink" onclick="openLB('PLACEHOLDER_LORAL')">View Letter →</span></div>
      </div>
      <div class="cert-card">
        <img src="PLACEHOLDER_SUNDARAM" alt="Sundaram Industries internship completion certificate" onclick="openLB(this.src)">
        <div class="cert-body"><h4>Sundaram Industries — Internship Completion</h4><p>In-Plant Training Certificate, TVS Rubber · 24 Jun – 5 Jul 2024</p><span class="viewlink" onclick="openLB('PLACEHOLDER_SUNDARAM')">View Certificate →</span></div>
      </div>
    </div>
  </div>
</section>

<!-- ACHIEVEMENTS -->
<section id="achievements" style="background:var(--navy2); border-top:1px solid var(--line); border-bottom:1px solid var(--line);">
  <div class="wrap">
    <div class="eyebrow reveal">Beyond Engineering</div>
    <h2 class="section-title reveal">Achievements &amp; Activities</h2>
    <div class="ach-grid reveal">
      <div class="ach-card"><img src="PLACEHOLDER_BLOOD" alt="Blood donation certificate" onclick="openLB(this.src)"><div class="cap">Certificate of Appreciation – Blood Donation (15-03-2025)</div></div>
      <div class="ach-card"><img src="PLACEHOLDER_G6" alt="Presenting on Soft Robotics and Shape Memory Alloys" onclick="openLB(this.src)"><div class="cap">Technical Presentation on Soft Robotics (ICMMRM 2025)</div></div>
      <div class="ach-card"><img src="PLACEHOLDER_G5" alt="Ashok Leyland project completion felicitation programme" onclick="openLB(this.src)"><div class="cap">Ashok Leyland Project Completion Felicitation</div></div>
      <div class="ach-card"><img src="PLACEHOLDER_ENG23" alt="Engineering activity certificate" onclick="openLB(this.src)"><div class="cap">Engineering Participation — Engineering '23</div></div>
      <div class="ach-card"><img src="PLACEHOLDER_DESIGNDUEL" alt="Conducting the Design Duel event at Ignition 25" onclick="openLB(this.src)"><div class="cap">Event Coordinator — Design Duel, Ignition '25</div></div>
      <div class="ach-card"><img src="PLACEHOLDER_STANDARDSCLUB" alt="Standards Club SVCE Joint Secretary" onclick="openLB(this.src)"><div class="cap">Joint Secretary — Standards Club, SVCE (2024–25)</div></div>
      <div class="ach-card"><img src="PLACEHOLDER_MUSICCLUB" alt="Music Club SVCE Content Team Head" onclick="openLB(this.src)"><div class="cap">Content Team Head — Music Club, SVCE (2024–25)</div></div>
    </div>
  </div>
</section>

<!-- GALLERY -->
<section id="gallery">
  <div class="wrap">
    <div class="eyebrow reveal">Engineering Journey</div>
    <h2 class="section-title reveal">Gallery</h2>
    <div class="gallery reveal">
      <img src="PLACEHOLDER_G1" alt="Presenting on Soft Robotics" onclick="openLB(this.src)">
      <img src="PLACEHOLDER_G2" alt="Presenting on Shape Memory Alloys and Soft Robotics" onclick="openLB(this.src)">
      <img src="PLACEHOLDER_G3" alt="Ashok Leyland project completion felicitation programme" onclick="openLB(this.src)">
      <img src="PLACEHOLDER_G4" alt="Ashok Leyland project completion felicitation programme" onclick="openLB(this.src)">
      <img src="PLACEHOLDER_G5" alt="Ashok Leyland project completion felicitation programme" onclick="openLB(this.src)">
      <img src="PLACEHOLDER_G6" alt="Presenting on Soft Robotics and Shape Memory Alloys" onclick="openLB(this.src)">
      <img src="PLACEHOLDER_DESIGNDUEL" alt="Conducting the Design Duel event at Ignition 25" onclick="openLB(this.src)">
      <img src="PLACEHOLDER_HVK" alt="Presenting a project workflow to HVK Group" onclick="openLB(this.src)">
      <img src="PLACEHOLDER_NPTEL" alt="NPTEL certificate" onclick="openLB(this.src)">
      <img src="PLACEHOLDER_ENG23" alt="Engineering 23 certificate" onclick="openLB(this.src)">
    </div>
  </div>
</section>

<div class="lightbox" id="lightbox"><button class="lb-close" onclick="closeLB()">&times;</button><img id="lb-img" src="" alt="Enlarged view"></div>

<!-- EDUCATION -->
<section style="background:var(--navy2); border-top:1px solid var(--line); border-bottom:1px solid var(--line);">
  <div class="wrap">
    <div class="eyebrow reveal">Academics</div>
    <h2 class="section-title reveal">Education</h2>
    <div class="reveal">
      <div class="edu-item">
        <div><h3>Sri Venkateswara College of Engineering, Sriperumbudur</h3><div class="deg">B.E. Mechanical and Automation Engineering · Minor: Cloud Computing &amp; IoT</div><div class="meta">CGPA: 8.26</div></div>
        <div class="yr">2022 – 2026</div>
      </div>
      <div class="edu-item">
        <div><h3>Lord PCAA Lions Matric Higher Secondary School, Sivakasi</h3><div class="deg">Higher Secondary Certificate</div><div class="meta">HSC: 84%</div></div>
        <div class="yr">2018 – 2022</div>
      </div>
    </div>
  </div>
</section>

<!-- INTERESTS -->
<section>
  <div class="wrap">
    <div class="eyebrow reveal">Career Direction</div>
    <h2 class="section-title reveal">What I Want to Build</h2>
    <div class="grid4 reveal">
      <div class="card"><h4>Mechanical Design</h4></div>
      <div class="card"><h4>Digital Manufacturing</h4></div>
      <div class="card"><h4>Smart Factories</h4></div>
      <div class="card"><h4>Manufacturing Automation</h4></div>
      <div class="card"><h4>Digital Twins</h4></div>
      <div class="card"><h4>AMR-Based Material Handling</h4></div>
      <div class="card"><h4>Plant Layout Optimization</h4></div>
      <div class="card"><h4>Industrial IoT</h4></div>
    </div>
  </div>
</section>

<!-- CTA -->
<section class="cta">
  <div class="wrap">
    <h2 class="reveal">Let's Build the Future of Manufacturing.</h2>
    <p class="reveal">I am interested in opportunities where mechanical engineering, design, manufacturing and automation come together to solve real-world industrial problems.</p>
    <div class="hero-actions reveal">
      <a href="RESUME_HREF" download class="btn btn-primary">Download Resume</a>
      <a href="#contact" class="btn btn-outline">Contact Me</a>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="wrap">
    <div class="eyebrow reveal">Get In Touch</div>
    <h2 class="section-title reveal">Let's Connect</h2>
    <div class="contact-grid reveal">
      <div>
        <div class="contact-item"><div class="ic">✉</div><a href="mailto:srivatsanseshadri1027@email.com">srivatsanseshadri1027@email.com</a></div>
        <div class="contact-item"><div class="ic">in</div><a href="#" target="_blank">Srivatsan Sheshathri — LinkedIn</a></div>
        <div class="contact-item"><div class="ic">☎</div><a href="tel:6374463983">+91 6374463983</a></div>
      </div>
      <div>
        <p style="color:var(--muted);">Srivatsan Sheshathri<br>Chennai, Tamil Nadu, India</p>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="logo">SRIVATSAN <span style="color:var(--amber)">SHESHATHRI</span></div>
  <div>Mechanical Design &amp; Automation Engineer</div>
  <div class="tag">DESIGN · MANUFACTURING · AUTOMATION · INDUSTRY 4.0</div>
  <div>© 2026 Srivatsan Sheshathri</div>
</footer>

<script>
document.getElementById('hamb').onclick=function(){document.getElementById('navlinks').classList.toggle('open');};
document.querySelectorAll('.navlink').forEach(a=>a.onclick=()=>document.getElementById('navlinks').classList.remove('open'));
function openModal(id){document.getElementById('modal-'+id).classList.add('open');}
function closeModal(id){document.getElementById('modal-'+id).classList.remove('open');}
document.querySelectorAll('.modal-overlay').forEach(m=>m.onclick=e=>{if(e.target===m)m.classList.remove('open');});
function openLB(src){document.getElementById('lb-img').src=src; document.getElementById('lightbox').classList.add('open');}
function closeLB(){document.getElementById('lightbox').classList.remove('open');}
document.getElementById('lightbox').onclick=function(e){if(e.target===this)closeLB();};
const obs=new IntersectionObserver(es=>es.forEach(e=>{if(e.isIntersecting)e.target.classList.add('show');}),{threshold:.12});
document.querySelectorAll('.reveal').forEach(el=>obs.observe(el));
</script>
</body>
</html>
