[dr_hariharan_portfolio_v3_photo.html](https://github.com/user-attachments/files/29285959/dr_hariharan_portfolio_v3_photo.html)

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:wght@300;400;500&display=swap');
*{box-sizing:border-box;margin:0;padding:0}
:root{
  --bg:#0d0f14;--bg2:#13161d;--bg3:#1a1e28;
  --card:#161a24;--card2:#1e2330;
  --teal:#1d9e75;--teal2:#9fe1cb;--teal3:#04342c;
  --text:#e8eaf0;--text2:#8b90a0;--text3:#555c70;
  --line:rgba(255,255,255,0.07);--line2:rgba(29,158,117,0.3);
}
body{font-family:'DM Sans',sans-serif;background:var(--bg);color:var(--text);min-height:100vh;position:relative;overflow-x:hidden}

/* ANIMATED BACKGROUND ILLUSTRATIONS */
.bg-illustration{position:fixed;top:0;left:0;width:100%;height:100%;pointer-events:none;z-index:0;opacity:0.045}
.bg-illustration svg{width:100%;height:100%}

.wrap{max-width:960px;margin:0 auto;padding:0 2.5rem 5rem;position:relative;z-index:1}

/* NAV */
nav{display:flex;justify-content:space-between;align-items:center;padding:2rem 0;border-bottom:1px solid var(--line)}
.logo{font-family:'DM Serif Display',serif;font-size:1rem;color:var(--text)}
.logo span{color:var(--teal)}
.nav-links{display:flex;gap:2.5rem}
.nav-links a{font-size:.72rem;letter-spacing:.12em;text-transform:uppercase;color:var(--text2);text-decoration:none;cursor:pointer;transition:color .2s}
.nav-links a:hover{color:var(--teal2)}

/* HERO */
.hero{display:grid;grid-template-columns:1fr 400px;gap:4rem;padding:5rem 0 4rem;align-items:center}
.hero-eyebrow{display:flex;align-items:center;gap:.8rem;margin-bottom:1.8rem}
.dot{width:6px;height:6px;border-radius:50%;background:var(--teal);flex-shrink:0}
.eyebrow-text{font-size:.7rem;letter-spacing:.15em;text-transform:uppercase;color:var(--teal);font-weight:500}
h1{font-family:'DM Serif Display',serif;font-size:3.2rem;line-height:1.1;color:var(--text);font-weight:400}
h1 em{font-style:italic;color:var(--teal2)}
.hero-desc{margin-top:1.5rem;font-size:.92rem;color:var(--text2);line-height:1.85;font-weight:300}
.hero-cta{display:flex;gap:.8rem;margin-top:2rem;flex-wrap:wrap}
.btn-primary{background:var(--teal);color:#fff;border:none;padding:.65rem 1.4rem;border-radius:6px;font-size:.78rem;font-family:'DM Sans',sans-serif;letter-spacing:.06em;cursor:pointer;transition:opacity .2s;display:flex;align-items:center;gap:.4rem}
.btn-primary:hover{opacity:.85}
.btn-ghost{background:transparent;color:var(--text2);border:1px solid var(--line2);padding:.65rem 1.4rem;border-radius:6px;font-size:.78rem;font-family:'DM Sans',sans-serif;letter-spacing:.06em;cursor:pointer;transition:all .2s;display:flex;align-items:center;gap:.4rem}
.btn-ghost:hover{color:var(--teal2);border-color:var(--teal)}
.social-links{display:flex;gap:.6rem;margin-top:1.2rem}
.social-btn{background:var(--card);border:1px solid var(--line);color:var(--text2);padding:.5rem 1rem;border-radius:6px;font-size:.72rem;text-decoration:none;display:flex;align-items:center;gap:.4rem;transition:all .2s;letter-spacing:.04em}
.social-btn:hover{border-color:var(--teal);color:var(--teal2)}

/* PROFILE CARD */
.profile-card{background:var(--card);border:1px solid var(--line);border-radius:16px;overflow:hidden;position:relative}
.profile-card::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,var(--teal),var(--teal2))}
.profile-photo{width:100%;aspect-ratio:3/3.5;object-fit:cover;object-position:top center;display:block}
.profile-info{padding:1.4rem}
.profile-name{font-family:'DM Serif Display',serif;font-size:1.1rem;color:var(--text);margin-bottom:.2rem}
.profile-title{font-size:.75rem;color:var(--teal2);margin-bottom:.1rem}
.profile-inst{font-size:.72rem;color:var(--text2);margin-bottom:1rem;line-height:1.5;font-weight:300}
.profile-divider{height:1px;background:var(--line);margin-bottom:1rem}
.profile-row{display:flex;align-items:flex-start;gap:.6rem;margin-bottom:.7rem}
.profile-row i{color:var(--teal);font-size:13px;margin-top:2px;flex-shrink:0}
.profile-row-text{font-size:.72rem;color:var(--text2)}
.profile-row-text a{color:var(--teal2);text-decoration:none}
.badge-row{display:flex;gap:.4rem;flex-wrap:wrap;margin-top:1rem}
.badge{font-size:.62rem;letter-spacing:.08em;padding:.25rem .6rem;border-radius:4px;border:1px solid var(--line2);color:var(--teal2);text-transform:uppercase}

/* STATS */
.stats-row{display:grid;grid-template-columns:repeat(4,1fr);gap:1px;background:var(--line);border:1px solid var(--line);border-radius:12px;overflow:hidden;margin:0 0 4rem}
.stat{background:var(--card);padding:1.5rem 1rem;text-align:center}
.stat-num{font-family:'DM Serif Display',serif;font-size:2.4rem;color:var(--text);line-height:1}
.stat-num span{font-size:1.5rem;color:var(--teal)}
.stat-label{font-size:.66rem;color:var(--text3);margin-top:.4rem;letter-spacing:.06em;text-transform:uppercase}

/* SECTION */
section{padding:3.5rem 0;border-top:1px solid var(--line)}
.sec-header{display:flex;align-items:center;gap:1rem;margin-bottom:2.5rem}
.sec-label{font-size:.66rem;letter-spacing:.18em;text-transform:uppercase;color:var(--teal);font-weight:500}
.sec-line{flex:1;height:1px;background:var(--line)}

/* TIMELINE */
.tl-item{display:grid;grid-template-columns:130px 1fr;gap:2rem;padding:2rem 0;border-bottom:1px solid var(--line)}
.tl-item:last-child{border-bottom:none}
.tl-date{font-size:.7rem;color:var(--text3);line-height:1.6;padding-top:.3rem;letter-spacing:.04em}
.tl-role{font-family:'DM Serif Display',serif;font-size:1rem;color:var(--text);margin-bottom:.3rem}
.tl-org{font-size:.76rem;color:var(--teal2);margin-bottom:.7rem}
.tl-desc{font-size:.8rem;color:var(--text2);line-height:1.75;font-weight:300}
.tl-tags{display:flex;flex-wrap:wrap;gap:.3rem;margin-top:.7rem}
.tl-tag{font-size:.62rem;background:rgba(29,158,117,.1);color:var(--teal2);border:1px solid rgba(29,158,117,.2);padding:.2rem .55rem;border-radius:4px}

/* PUBS */
.pub-list{display:flex;flex-direction:column;gap:.7rem}
.pub-card{background:var(--card);border:1px solid var(--line);border-radius:10px;padding:1.2rem 1.4rem;display:grid;grid-template-columns:2.5rem 1fr;gap:1rem;align-items:start;transition:border-color .2s}
.pub-card:hover{border-color:var(--line2);background:var(--card2)}
.pub-year{font-family:'DM Serif Display',serif;font-size:1.4rem;color:var(--text3);line-height:1;text-align:center;padding-top:.1rem}
.pub-journal{font-size:.64rem;letter-spacing:.1em;text-transform:uppercase;color:var(--teal);margin-bottom:.3rem}
.pub-title{font-size:.85rem;color:var(--text);line-height:1.5;margin-bottom:.3rem}
.pub-authors{font-size:.72rem;color:var(--text2);font-weight:300}

/* LABS */
.lab-grid{display:grid;grid-template-columns:1fr 1fr;gap:.8rem}
.lab-card{background:var(--card);border:1px solid var(--line);border-radius:12px;padding:1.5rem;transition:border-color .2s,background .2s;position:relative;overflow:hidden}
.lab-card:hover{border-color:var(--line2);background:var(--card2)}
.lab-card::after{content:'';position:absolute;bottom:0;left:0;right:0;height:2px;background:var(--teal);opacity:0;transition:opacity .25s}
.lab-card:hover::after{opacity:1}
.lab-icon{width:36px;height:36px;border-radius:8px;background:rgba(29,158,117,.1);border:1px solid rgba(29,158,117,.2);display:flex;align-items:center;justify-content:center;margin-bottom:.9rem}
.lab-icon i{color:var(--teal);font-size:17px}
.lab-name{font-size:.88rem;font-weight:500;color:var(--text);margin-bottom:.3rem}
.lab-period{font-size:.66rem;color:var(--teal2);margin-bottom:.4rem}
.lab-desc{font-size:.73rem;color:var(--text2);font-weight:300;line-height:1.6}

/* EDU */
.edu-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:.8rem}
.edu-card{background:var(--card);border:1px solid var(--line);border-radius:10px;padding:1.3rem}
.edu-deg{font-family:'DM Serif Display',serif;font-size:.95rem;color:var(--text);margin-bottom:.3rem}
.edu-field{font-size:.73rem;color:var(--teal2);margin-bottom:.3rem}
.edu-inst{font-size:.71rem;color:var(--text2);font-weight:300;margin-bottom:.2rem}
.edu-year{font-size:.66rem;color:var(--text3);letter-spacing:.04em}

/* SKILLS */
.skills-cols{display:grid;grid-template-columns:repeat(3,1fr);gap:.5rem}
.skill-item{display:flex;align-items:center;gap:.6rem;padding:.65rem .9rem;background:var(--card);border:1px solid var(--line);border-radius:8px;transition:border-color .2s}
.skill-item:hover{border-color:var(--line2)}
.skill-item i{color:var(--teal);font-size:14px;flex-shrink:0}
.skill-item span{font-size:.76rem;color:var(--text2)}

/* FOOTER */
footer{padding:2rem 0;border-top:1px solid var(--line);display:flex;justify-content:space-between;align-items:center}
footer p{font-size:.7rem;color:var(--text3)}
.footer-right{display:flex;gap:1.2rem}
.footer-right a{font-size:.7rem;color:var(--text2);text-decoration:none}
.footer-right a:hover{color:var(--teal2)}
</style>

<!-- BACKGROUND ILLUSTRATION: research-themed SVG -->
<div class="bg-illustration">
<svg viewBox="0 0 1200 800" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <!-- Wave / shock wave rings -->
  <circle cx="200" cy="400" r="80" fill="none" stroke="#1d9e75" stroke-width="1.5"/>
  <circle cx="200" cy="400" r="140" fill="none" stroke="#1d9e75" stroke-width="1"/>
  <circle cx="200" cy="400" r="200" fill="none" stroke="#1d9e75" stroke-width=".6"/>
  <circle cx="200" cy="400" r="270" fill="none" stroke="#1d9e75" stroke-width=".4"/>
  <!-- Layered structure diagram -->
  <rect x="700" y="100" width="300" height="20" fill="#9fe1cb" opacity=".6" rx="2"/>
  <rect x="700" y="130" width="300" height="20" fill="#1d9e75" opacity=".4" rx="2"/>
  <rect x="700" y="160" width="300" height="20" fill="#9fe1cb" opacity=".6" rx="2"/>
  <rect x="700" y="190" width="300" height="20" fill="#1d9e75" opacity=".4" rx="2"/>
  <rect x="700" y="220" width="300" height="20" fill="#9fe1cb" opacity=".6" rx="2"/>
  <!-- Arrow showing impact -->
  <line x1="850" y1="60" x2="850" y2="95" stroke="#1d9e75" stroke-width="2" marker-end="url(#arr)"/>
  <defs><marker id="arr" markerWidth="6" markerHeight="6" refX="3" refY="3" orient="auto"><path d="M0,0 L6,3 L0,6 Z" fill="#1d9e75"/></marker></defs>
  <!-- FEM mesh grid -->
  <g opacity=".35" stroke="#1d9e75" stroke-width=".5" fill="none">
    <line x1="900" y1="350" x2="1150" y2="350"/>
    <line x1="900" y1="380" x2="1150" y2="380"/>
    <line x1="900" y1="410" x2="1150" y2="410"/>
    <line x1="900" y1="440" x2="1150" y2="440"/>
    <line x1="900" y1="470" x2="1150" y2="470"/>
    <line x1="900" y1="500" x2="1150" y2="500"/>
    <line x1="900" y1="350" x2="900" y2="500"/>
    <line x1="930" y1="350" x2="930" y2="500"/>
    <line x1="960" y1="350" x2="960" y2="500"/>
    <line x1="990" y1="350" x2="990" y2="500"/>
    <line x1="1020" y1="350" x2="1020" y2="500"/>
    <line x1="1050" y1="350" x2="1050" y2="500"/>
    <line x1="1080" y1="350" x2="1080" y2="500"/>
    <line x1="1110" y1="350" x2="1110" y2="500"/>
    <line x1="1140" y1="350" x2="1140" y2="500"/>
  </g>
  <!-- Vibration sine wave -->
  <path d="M50,600 Q100,550 150,600 Q200,650 250,600 Q300,550 350,600 Q400,650 450,600 Q500,550 550,600 Q600,650 650,600 Q700,550 750,600" fill="none" stroke="#1d9e75" stroke-width="1.5" opacity=".5"/>
  <!-- Composite honeycomb -->
  <g opacity=".25" stroke="#9fe1cb" stroke-width=".8" fill="none" transform="translate(30,150)">
    <polygon points="30,0 60,17 60,51 30,68 0,51 0,17"/>
    <polygon points="90,0 120,17 120,51 90,68 60,51 60,17"/>
    <polygon points="60,68 90,85 90,119 60,136 30,119 30,85"/>
    <polygon points="30,136 60,153 60,187 30,204 0,187 0,153"/>
    <polygon points="90,136 120,153 120,187 90,204 60,187 60,153"/>
  </g>
  <!-- Velocity arrow cluster -->
  <g opacity=".3" fill="#9fe1cb">
    <line x1="1080" y1="630" x2="1130" y2="630" stroke="#9fe1cb" stroke-width="2" marker-end="url(#arr)"/>
    <line x1="1070" y1="650" x2="1130" y2="650" stroke="#9fe1cb" stroke-width="1.5" marker-end="url(#arr)"/>
    <line x1="1060" y1="670" x2="1130" y2="670" stroke="#9fe1cb" stroke-width="1" marker-end="url(#arr)"/>
  </g>
</svg>
</div>

<div class="wrap">
  <nav>
    <span class="logo">Dr. Hariharan <span>Elangovan</span></span>
    <div class="nav-links">
      <a>Research</a>
      <a>Publications</a>
      <a>Labs</a>
      <a>Contact</a>
    </div>
  </nav>

  <div class="hero">
    <div>
      <div class="hero-eyebrow"><div class="dot"></div><span class="eyebrow-text">Structural Impact · Composite Materials · Shock Mechanics</span></div>
      <h1>Engineering<br>resilience at the<br><em>material level</em></h1>
      <p class="hero-desc">Advancing how structures survive shock, high-velocity impact, and dynamic loading — from naval vessels to aerospace composites — through rigorous numerical simulation and experimental investigation.</p>
      <div class="hero-cta">
        <button class="btn-primary"><i class="ti ti-book-2" aria-hidden="true"></i> View Publications</button>
        <button class="btn-ghost" onclick="window.location.href='mailto:dr.hariharanelangovan@gmail.com'"><i class="ti ti-mail" aria-hidden="true"></i> Get in Touch</button>
      </div>
      <div class="social-links">
        <a class="social-btn" href="https://scholar.google.com" target="_blank"><i class="ti ti-school" aria-hidden="true"></i> Google Scholar</a>
        <a class="social-btn" href="https://www.researchgate.net" target="_blank"><i class="ti ti-flask" aria-hidden="true"></i> ResearchGate</a>
        <a class="social-btn" href="https://www.linkedin.com" target="_blank"><i class="ti ti-brand-linkedin" aria-hidden="true"></i> LinkedIn</a>
      </div>
    </div>
    <div>
      <div class="profile-card">
        <img class="profile-photo" src="data:image/jpeg;base64,/9j/4QQaRXhpZgAATU0AKgAAAAgADwEDAAMAAAABAAYAAAIBAAQAAAABAAADRgICAAQAAAABAACeAAEBAAMAAAABCVgAAAEPAAIAAAAbAAAAqgEQAAIAAAAbAAAAxQESAAMAAAABAAEAAAEaAAUAAAABAAAA4AEbAAUAAAABAAAA6AEoAAMAAAABAAIAAAExAAIAAAAcAAAA8AEyAAIAAAAUAAABDAIHAAQAAAABAAAAIAgAAIMAAAABAAAA3wgAAAMAAAACAAIACgAAACwAAAEgAAoAAAAQAAAATAAAACwAAAEgAAAAEAAAACwAAAAqAAAAKgAAACwAAAAqAAAAIgAAACAAAAAoAAAAHAAAABwAAAAUAAAAFAAAAA4AAAAOAAAACAAAACAAAACAAAACAAAACAAAA==" alt="Dr. Hariharan Elangovan" onerror="this.style.display='none';this.nextElementSibling.style.display='flex'">
        <div style="display:none;width:100%;height:200px;background:var(--teal3);align-items:center;justify-content:center;font-family:'DM Serif Display',serif;font-size:3rem;color:var(--teal2)">HE</div>
        <div class="profile-info">
          <div class="profile-name">Dr. Hariharan Elangovan</div>
          <div class="profile-title">Senior Project Scientist &amp; Postdoctoral Researcher</div>
          <div class="profile-inst">Dept. of Earth Sciences, IIT Kanpur<br>HEMRL – DRDO, Ministry of Defence</div>
          <div class="profile-divider"></div>
          <div class="profile-row"><i class="ti ti-mail" aria-hidden="true"></i><div class="profile-row-text"><a href="mailto:dr.hariharanelangovan@gmail.com">dr.hariharanelangovan@gmail.com</a></div></div>
          <div class="profile-row"><i class="ti ti-phone" aria-hidden="true"></i><div class="profile-row-text">+91 99522 89040</div></div>
          <div class="profile-row"><i class="ti ti-map-pin" aria-hidden="true"></i><div class="profile-row-text">IIT Kanpur, India</div></div>
          <div class="badge-row"><span class="badge">B.E.</span><span class="badge">M.Tech</span><span class="badge">Ph.D</span></div>
        </div>
      </div>
    </div>
  </div>

  <div class="stats-row">
    <div class="stat"><div class="stat-num">7<span>+</span></div><div class="stat-label">Publications</div></div>
    <div class="stat"><div class="stat-num">4</div><div class="stat-label">Labs Built</div></div>
    <div class="stat"><div class="stat-num">6<span>+</span></div><div class="stat-label">Yrs Research</div></div>
    <div class="stat"><div class="stat-num">3</div><div class="stat-label">DRDO Projects</div></div>
  </div>

  <section>
    <div class="sec-header"><span class="sec-label">Work History</span><div class="sec-line"></div></div>
    <div class="tl-item">
      <div class="tl-date">Nov 2025<br>– Present</div>
      <div>
        <div class="tl-role">Senior Project Scientist &amp; Postdoctoral Researcher</div>
        <div class="tl-org">Dept. of Earth Sciences, IIT Kanpur · HEMRL–DRDO</div>
        <div class="tl-desc">Building the Shock Deformation Laboratory — integrating LS-DYNA FEM simulations with a high-velocity impact test facility. Conducting numerical and experimental analysis of shock attenuation in layered structures using high-speed cameras and sensor arrays.</div>
        <div class="tl-tags"><span class="tl-tag">LS-DYNA</span><span class="tl-tag">Shock attenuation</span><span class="tl-tag">Layered structures</span><span class="tl-tag">High-speed imaging</span></div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-date">Oct 2023<br>– Sep 2025</div>
      <div>
        <div class="tl-role">Senior Research Associate</div>
        <div class="tl-org">SIMCRACH Centre, Aerospace Engg., HITS Chennai · NSTL–DRDO</div>
        <div class="tl-desc">Delivered two DRDO-funded projects on marine vessel shock standards and underwater shock excitation. Led hail-ice and projectile impact testing on composite structures. Directed team planning, resource allocation, and project timelines.</div>
        <div class="tl-tags"><span class="tl-tag">Marine vessels</span><span class="tl-tag">Underwater shock</span><span class="tl-tag">Hail-ice impact</span><span class="tl-tag">Projectile impact</span></div>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-date">Jul 2018<br>– Oct 2023</div>
      <div>
        <div class="tl-role">Teaching cum Research Associate</div>
        <div class="tl-org">School of Mechanical Engineering, VIT Vellore</div>
        <div class="tl-desc">Supervised research projects, developed courses, and established the Advanced Vibration Laboratory funded by AR&amp;DB and DRDL. Collaborated with Cranfield University, UK on a Royal Academy of Engineering–funded composite curriculum project.</div>
        <div class="tl-tags"><span class="tl-tag">VIT Vellore</span><span class="tl-tag">Cranfield University</span><span class="tl-tag">AR&amp;DB</span><span class="tl-tag">Curriculum</span></div>
      </div>
    </div>
  </section>

  <section>
    <div class="sec-header"><span class="sec-label">Publications</span><div class="sec-line"></div></div>
    <div class="pub-list">
      <div class="pub-card"><div class="pub-year">25</div><div><div class="pub-journal">Mechanics of Advanced Materials and Structures</div><div class="pub-title">Numerical and experimental approach on vibration characterization of non-uniform hybrid sandwich plates</div><div class="pub-authors">Hariharan Elangovan &amp; Vasudevan Rajamohan · pp.1–33</div></div></div>
      <div class="pub-card"><div class="pub-year">24</div><div><div class="pub-journal">Steel and Composite Structures · Vol. 53, No. 3</div><div class="pub-title">Dynamic response of hybrid composite semi-ellipsoidal dome structure: Numerical and experimental investigations</div><div class="pub-authors">Hariharan Elangovan, Gnanasekar S., Barathan V. et al.</div></div></div>
      <div class="pub-card"><div class="pub-year">24</div><div><div class="pub-journal">Int. Journal of Mechanics and Materials in Design</div><div class="pub-title">Strength and stability analysis of composite inverted conical structure</div><div class="pub-authors">Gnanasekar S., Santhosh B., Rajamohan V., Hariharan Elangovan et al.</div></div></div>
      <div class="pub-card"><div class="pub-year">22</div><div><div class="pub-journal">Thin-Walled Structures · Vol. 178 · 109515</div><div class="pub-title">Dynamic characterization of tapered composite sandwich plate with honeycomb core: Numerical and experimental investigations</div><div class="pub-authors">Hariharan Elangovan &amp; Vasudevan Rajamohan</div></div></div>
      <div class="pub-card"><div class="pub-year">22</div><div><div class="pub-journal">AIP Conference Proceedings · Vol. 2545</div><div class="pub-title">Vibration fatigue analysis of spur gear drive under random loading</div><div class="pub-authors">Dutta S., Tambare A., Harshith D., Hariharan Elangovan &amp; Vemuluri R.B.</div></div></div>
      <div class="pub-card"><div class="pub-year">17</div><div><div class="pub-journal">Int. J. Eng. Sci. Res. Technol.</div><div class="pub-title">Testing and analysis of composite materials under tensile loading with different lap joints</div><div class="pub-authors">Hariharan E. &amp; Amutheesan R.</div></div></div>
    </div>
  </section>

  <section>
    <div class="sec-header"><span class="sec-label">Laboratories Established</span><div class="sec-line"></div></div>
    <div class="lab-grid">
      <div class="lab-card"><div class="lab-icon"><i class="ti ti-bolt" aria-hidden="true"></i></div><div class="lab-name">Shock Deformation Laboratory</div><div class="lab-period">2025 – Present · IIT Kanpur</div><div class="lab-desc">LS-DYNA FEM + high-velocity impact test facility. Funded by HEMRL–DRDO.</div></div>
      <div class="lab-card"><div class="lab-icon"><i class="ti ti-anchor" aria-hidden="true"></i></div><div class="lab-name">NSTL–HITS Research Laboratory</div><div class="lab-period">2023 – 2024 · HITS Chennai</div><div class="lab-desc">Naval shock research. Funded jointly by NSTL–DRDO and HITS SEED grant.</div></div>
      <div class="lab-card"><div class="lab-icon"><i class="ti ti-target" aria-hidden="true"></i></div><div class="lab-name">Hail Ice &amp; Projectile Impact Lab</div><div class="lab-period">2023 – 2024 · HITS Chennai</div><div class="lab-desc">Aerospace composite impact testing. Funded by AR&amp;DB and HITS SEED grant.</div></div>
      <div class="lab-card"><div class="lab-icon"><i class="ti ti-wave-sine" aria-hidden="true"></i></div><div class="lab-name">Advanced Vibration Laboratory</div><div class="lab-period">2018 – 2022 · VIT Vellore</div><div class="lab-desc">Vibration characterization facility. Funded by AR&amp;DB, DRDL and VIT SEED grant.</div></div>
    </div>
  </section>

  <section>
    <div class="sec-header"><span class="sec-label">Education</span><div class="sec-line"></div></div>
    <div class="edu-grid">
      <div class="edu-card"><div class="edu-deg">Ph.D. in Engineering</div><div class="edu-field">Dynamic characterization of hybrid tapered composite sandwich plates</div><div class="edu-inst">Vellore Institute of Technology</div><div class="edu-year">2018 – 2025 · AR&amp;DB &amp; VIT funded</div></div>
      <div class="edu-card"><div class="edu-deg">M.Tech</div><div class="edu-field">Aeronautical Engineering — Composites</div><div class="edu-inst">Hindustan University, Chennai</div><div class="edu-year">2014 – 2016</div></div>
      <div class="edu-card"><div class="edu-deg">B.E.</div><div class="edu-field">Aeronautical Engineering</div><div class="edu-inst">Anna University, Chennai</div><div class="edu-year">2010 – 2014</div></div>
    </div>
  </section>

  <section>
    <div class="sec-header"><span class="sec-label">Expertise</span><div class="sec-line"></div></div>
    <div class="skills-cols">
      <div class="skill-item"><i class="ti ti-cpu" aria-hidden="true"></i><span>LS-DYNA / FEM Simulation</span></div>
      <div class="skill-item"><i class="ti ti-layers" aria-hidden="true"></i><span>Composite Materials</span></div>
      <div class="skill-item"><i class="ti ti-wave-sine" aria-hidden="true"></i><span>Vibration Analysis</span></div>
      <div class="skill-item"><i class="ti ti-bolt" aria-hidden="true"></i><span>Shock &amp; Impact Mechanics</span></div>
      <div class="skill-item"><i class="ti ti-microscope" aria-hidden="true"></i><span>Experimental Mechanics</span></div>
      <div class="skill-item"><i class="ti ti-camera" aria-hidden="true"></i><span>High-Speed Imaging</span></div>
      <div class="skill-item"><i class="ti ti-chart-line" aria-hidden="true"></i><span>Research Management</span></div>
      <div class="skill-item"><i class="ti ti-file-text" aria-hidden="true"></i><span>Grant Writing &amp; Funding</span></div>
      <div class="skill-item"><i class="ti ti-school" aria-hidden="true"></i><span>Curriculum Development</span></div>
    </div>
  </section>

  <footer>
    <p>© 2026 · Dr. Hariharan Elangovan · IIT Kanpur, India</p>
    <div class="footer-right">
      <a href="mailto:dr.hariharanelangovan@gmail.com">Email</a>
      <a href="https://scholar.google.com" target="_blank">Scholar</a>
      <a href="https://www.researchgate.net" target="_blank">ResearchGate</a>
      <a href="https://www.linkedin.com" target="_blank">LinkedIn</a>
    </div>
  </footer>
</div>
