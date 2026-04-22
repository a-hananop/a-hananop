<style>
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;500&display=swap');

*{margin:0;padding:0;box-sizing:border-box}

body{
  font-family:'Outfit',sans-serif;
  background:#03080f;
  color:#cde8f8;
  min-height:100vh;
  overflow-x:hidden;
}

/* ── CRYSTAL BG ── */
.crystal-bg{
  position:fixed;inset:0;z-index:0;
  overflow:hidden;
  pointer-events:none;
}
.crystal-bg::before{
  content:'';
  position:absolute;inset:0;
  background:
    radial-gradient(ellipse 60% 50% at 20% 20%, rgba(0,180,255,0.07) 0%, transparent 70%),
    radial-gradient(ellipse 50% 60% at 80% 10%, rgba(80,120,255,0.06) 0%, transparent 65%),
    radial-gradient(ellipse 40% 50% at 50% 80%, rgba(0,220,180,0.05) 0%, transparent 65%),
    radial-gradient(ellipse 55% 40% at 90% 70%, rgba(100,60,255,0.05) 0%, transparent 65%);
}
.crystal-canvas{position:absolute;inset:0;width:100%;height:100%;}

/* ── PAGE ── */
.page{
  position:relative;z-index:1;
  max-width:820px;
  margin:0 auto;
  padding:0 1.6rem 6rem;
}

/* ── HERO ── */
.hero{
  display:flex;flex-direction:column;align-items:center;
  padding:4rem 1rem 2.8rem;
  text-align:center;
}

.av-shell{
  position:relative;width:120px;height:120px;
  margin-bottom:1.8rem;
}
.av-shell canvas{position:absolute;inset:0;width:120px;height:120px;}
.av-core{
  position:absolute;inset:11px;
  border-radius:50%;
  background:linear-gradient(135deg,#041224,#071e38);
  border:1px solid rgba(0,190,255,0.22);
  display:flex;align-items:center;justify-content:center;
  font-family:'JetBrains Mono',monospace;
  font-size:2rem;font-weight:500;
  color:#00c6ff;
  letter-spacing:.05em;
}

.hero-name{
  font-size:clamp(2rem,5vw,3.2rem);
  font-weight:800;
  letter-spacing:-.03em;
  line-height:1.08;
  color:#eaf6ff;
  margin-bottom:.5rem;
}
.hero-name em{
  font-style:normal;
  background:linear-gradient(120deg,#00c6ff,#5eb8ff);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
  background-clip:text;
}

.hero-role{
  font-family:'JetBrains Mono',monospace;
  font-size:.72rem;
  letter-spacing:.22em;
  color:#2e7aa0;
  text-transform:uppercase;
  margin-bottom:1.2rem;
}

.typer-box{
  font-size:1.05rem;font-weight:500;
  color:#5eb8ff;
  min-height:1.6rem;
  display:flex;align-items:center;gap:3px;
}
.caret{
  display:inline-block;width:2px;height:1.05em;
  background:#00c6ff;vertical-align:text-bottom;
  animation:blink .85s step-end infinite;
}
@keyframes blink{0%,100%{opacity:1}50%{opacity:0}}

.avail{
  display:inline-flex;align-items:center;gap:6px;
  margin-top:1.3rem;
  border:1px solid rgba(0,230,120,.25);
  border-radius:99px;
  padding:.3rem .9rem;
  font-family:'JetBrains Mono',monospace;
  font-size:.7rem;
  color:#00e87a;
  letter-spacing:.07em;
  background:rgba(0,230,120,.06);
}
.avail-dot{
  width:6px;height:6px;border-radius:50%;
  background:#00e87a;
  animation:pulse 1.8s ease-in-out infinite;
}
@keyframes pulse{0%,100%{box-shadow:0 0 0 0 rgba(0,232,122,.55)}50%{box-shadow:0 0 0 6px rgba(0,232,122,0)}}

/* ── GLASS DIVIDER ── */
.gdiv{
  border:none;height:1px;margin:2.2rem 0;
  background:linear-gradient(90deg,transparent,rgba(0,190,255,.25),transparent);
}

/* ── SECTION LABEL ── */
.slabel{
  display:flex;align-items:center;gap:.55rem;
  font-family:'JetBrains Mono',monospace;
  font-size:.66rem;letter-spacing:.22em;
  color:#00c6ff;text-transform:uppercase;
  margin-bottom:1.15rem;
}
.slabel-bar{
  width:22px;height:2px;border-radius:2px;
  background:linear-gradient(90deg,#00c6ff,transparent);
  flex-shrink:0;
}

/* ── GLASS CARD BASE ── */
.gc{
  background:rgba(255,255,255,.032);
  border:1px solid rgba(255,255,255,.07);
  border-radius:16px;
  padding:1.4rem 1.5rem;
  backdrop-filter:blur(12px);
  -webkit-backdrop-filter:blur(12px);
  transition:border-color .28s,background .28s,transform .22s;
}
.gc:hover{
  border-color:rgba(0,190,255,.22);
  background:rgba(0,190,255,.05);
  transform:translateY(-2px);
}

/* ── ABOUT ── */
.about-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:.9rem;
}
.gc-full{grid-column:1/-1;}
.about-text{
  font-size:.94rem;line-height:1.82;
  color:#8dbbd6;
}
.about-text strong{color:#c5e5f7;font-weight:600;}

.chip-wrap{display:flex;flex-wrap:wrap;gap:.4rem;margin-top:.8rem;}
.chip{
  display:inline-flex;align-items:center;gap:.38rem;
  border:1px solid rgba(0,190,255,.18);
  border-radius:7px;
  padding:.26rem .65rem;
  font-size:.76rem;
  font-family:'JetBrains Mono',monospace;
  color:#6ab8d8;
  background:rgba(0,190,255,.05);
  transition:all .2s;
}
.chip:hover{
  border-color:rgba(0,190,255,.45);
  background:rgba(0,190,255,.13);
  color:#b8e0f7;
  transform:translateY(-1px);
}
.cdot{
  width:5px;height:5px;border-radius:50%;
  background:#00c6ff;flex-shrink:0;
}
.csub{
  font-family:'JetBrains Mono',monospace;
  font-size:.61rem;letter-spacing:.18em;
  color:#1e5e7e;text-transform:uppercase;
  margin-bottom:.7rem;
}

/* ── STACK ── */
.stack-wrap{
  display:grid;
  grid-template-columns:repeat(auto-fill,minmax(138px,1fr));
  gap:.65rem;
}
.sp{
  display:flex;align-items:center;gap:.55rem;
  background:rgba(255,255,255,.03);
  border:1px solid rgba(255,255,255,.07);
  border-radius:10px;
  padding:.62rem .9rem;
  font-size:.8rem;
  font-family:'JetBrains Mono',monospace;
  color:#6ab8d8;
  transition:all .22s;
  cursor:default;
}
.sp:hover{
  border-color:rgba(0,190,255,.35);
  background:rgba(0,190,255,.08);
  color:#c0e4f7;
  transform:translateY(-2px);
  box-shadow:0 6px 20px rgba(0,190,255,.08);
}
.sp-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0;}

/* ── WHAT I DO ── */
.do-wrap{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:.75rem;
}
.do-card{
  background:rgba(255,255,255,.03);
  border:1px solid rgba(255,255,255,.07);
  border-radius:14px;
  padding:1.3rem 1rem 1.2rem;
  text-align:center;
  cursor:default;
  transition:all .25s;
}
.do-card:hover{
  border-color:rgba(0,190,255,.3);
  background:rgba(0,190,255,.06);
  transform:translateY(-3px);
  box-shadow:0 10px 28px rgba(0,190,255,.07);
}
.do-icon{
  width:38px;height:38px;border-radius:10px;
  background:rgba(0,190,255,.09);
  border:1px solid rgba(0,190,255,.18);
  display:flex;align-items:center;justify-content:center;
  margin:0 auto .8rem;
  font-size:1.1rem;
}
.do-title{
  font-size:.88rem;font-weight:700;
  color:#c0e4f7;margin-bottom:.3rem;
}
.do-sub{
  font-size:.73rem;color:#2e7aa0;
  line-height:1.5;
}

/* ── STATS ROW ── */
.stats-row{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:.75rem;margin-bottom:1.1rem;
}
.stat-card{
  background:rgba(255,255,255,.03);
  border:1px solid rgba(255,255,255,.07);
  border-radius:14px;
  padding:1.1rem;
  text-align:center;
  cursor:default;
  transition:all .25s;
}
.stat-card:hover{
  border-color:rgba(0,190,255,.3);
  transform:translateY(-2px);
}
.stat-n{
  display:block;
  font-size:1.75rem;font-weight:800;
  font-family:'JetBrains Mono',monospace;
  color:#00c6ff;
  line-height:1.1;margin-bottom:.25rem;
}
.stat-l{
  font-size:.72rem;color:#2e7aa0;
  text-transform:uppercase;letter-spacing:.1em;
}

/* ── GH IMAGES ── */
.gh-pair{
  display:grid;grid-template-columns:1fr 1fr;
  gap:.75rem;margin-bottom:.75rem;
}
.gh-pair img,.gh-full{
  width:100%;border-radius:12px;
  border:1px solid rgba(255,255,255,.06);
  display:block;
}

/* ── QUOTE ── */
.quote-wrap{
  position:relative;
  background:rgba(255,255,255,.03);
  border:1px solid rgba(255,255,255,.07);
  border-left:3px solid #00c6ff;
  border-radius:0 14px 14px 0;
  padding:1.3rem 1.6rem 1.3rem 1.9rem;
  overflow:hidden;
}
.quote-wrap::before{
  content:'\201C';
  position:absolute;top:-.6rem;left:.6rem;
  font-size:5rem;font-family:Georgia,serif;
  color:#00c6ff;opacity:.07;line-height:1;
  pointer-events:none;
}
.quote-text{
  font-style:italic;font-size:1rem;
  color:#6ab8d8;line-height:1.7;
}
.quote-attr{
  margin-top:.55rem;
  font-family:'JetBrains Mono',monospace;
  font-size:.65rem;letter-spacing:.15em;
  color:#1e5e7e;text-transform:uppercase;
}

/* ── CONNECT ── */
.conn-row{display:flex;gap:.75rem;flex-wrap:wrap;}
.conn-btn{
  display:inline-flex;align-items:center;gap:.55rem;
  border:1px solid rgba(0,190,255,.25);
  border-radius:10px;
  padding:.72rem 1.45rem;
  font-family:'Outfit',sans-serif;
  font-size:.88rem;font-weight:600;
  color:#6ab8d8;
  text-decoration:none;
  background:rgba(0,190,255,.05);
  transition:all .22s;
}
.conn-btn:hover{
  border-color:#00c6ff;
  background:rgba(0,190,255,.14);
  color:#c5e8ff;
  transform:translateY(-2px);
  box-shadow:0 6px 20px rgba(0,190,255,.1);
}
.conn-btn svg{width:16px;height:16px;flex-shrink:0;}

/* ── FOOTER ── */
.footer{
  margin-top:2.8rem;
  text-align:center;
  font-family:'JetBrains Mono',monospace;
  font-size:.7rem;
  color:#133550;
  line-height:2;
}
.footer span{color:#00c6ff;}

/* ── RESPONSIVE ── */
@media(max-width:640px){
  .about-grid{grid-template-columns:1fr;}
  .gc-full{grid-column:auto;}
  .do-wrap{grid-template-columns:1fr 1fr;}
  .stats-row{grid-template-columns:1fr 1fr;}
  .gh-pair{grid-template-columns:1fr;}
  .stack-wrap{grid-template-columns:repeat(auto-fill,minmax(120px,1fr));}
  .hero-name{font-size:clamp(1.6rem,7vw,2.2rem);}
}
@media(max-width:400px){
  .do-wrap{grid-template-columns:1fr;}
  .stats-row{grid-template-columns:1fr;}
  .page{padding:0 1rem 4rem;}
}
</style>

<h2 style="position:absolute;width:1px;height:1px;overflow:hidden;clip:rect(0,0,0,0)">Abdul Hanan Saqlain — AI Engineer portfolio profile</h2>

<div class="crystal-bg">
  <canvas class="crystal-canvas" id="crystalCanvas"></canvas>
</div>

<div class="page">

  <!-- HERO -->
  <div class="hero">
    <div class="av-shell">
      <canvas id="ringCanvas" width="120" height="120"></canvas>
      <div class="av-core">AH</div>
    </div>
    <h1 class="hero-name">Abdul Hanan <em>Saqlain</em></h1>
    <div class="hero-role">AI Engineer &nbsp;·&nbsp; Builder &nbsp;·&nbsp; Innovator</div>
    <div class="typer-box"><span id="typer"></span><span class="caret"></span></div>
    <div class="avail"><span class="avail-dot"></span>Available for opportunities</div>
  </div>

  <hr class="gdiv">

  <!-- ABOUT -->
  <div class="slabel"><span class="slabel-bar"></span>About me</div>
  <div class="about-grid">
    <div class="gc gc-full">
      <p class="about-text">I'm an <strong>AI Engineer</strong> who turns ambitious ideas into working intelligent systems. I specialise in <strong>Generative AI</strong>, NLP pipelines, and smart automations — connecting the dots between raw data, intelligent models, and real-world applications that actually ship.</p>
    </div>
    <div class="gc">
      <div class="csub">Core skills</div>
      <div class="chip-wrap">
        <span class="chip"><span class="cdot"></span>Python &amp; Web Scraping</span>
        <span class="chip"><span class="cdot"></span>Generative AI &amp; NLP</span>
        <span class="chip"><span class="cdot"></span>Machine Learning</span>
        <span class="chip"><span class="cdot"></span>API Integration</span>
      </div>
    </div>
    <div class="gc">
      <div class="csub">Databases</div>
      <div class="chip-wrap">
        <span class="chip"><span class="cdot"></span>MySQL</span>
        <span class="chip"><span class="cdot"></span>MongoDB</span>
        <span class="chip"><span class="cdot"></span>Supabase</span>
      </div>
    </div>
  </div>

  <hr class="gdiv">

  <!-- TECH STACK -->
  <div class="slabel"><span class="slabel-bar"></span>Tech stack</div>
  <div class="stack-wrap" id="stackWrap"></div>

  <hr class="gdiv">

  <!-- WHAT I DO -->
  <div class="slabel"><span class="slabel-bar"></span>What I do</div>
  <div class="do-wrap" id="doWrap"></div>

  <hr class="gdiv">

  <!-- GITHUB ANALYTICS -->
  <div class="slabel"><span class="slabel-bar"></span>GitHub analytics</div>
  <div class="gh-pair">
    <img src="https://github-readme-stats.vercel.app/api?username=a-hananop&show_icons=true&theme=tokyonight&hide_border=true&bg_color=03080f&title_color=00c6ff&icon_color=2e7aa0&text_color=6ab8d8&border_radius=12" alt="GitHub Stats">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=a-hananop&layout=compact&theme=tokyonight&hide_border=true&bg_color=03080f&title_color=00c6ff&text_color=6ab8d8&border_radius=12" alt="Top Languages">
  </div>
  <img class="gh-full" src="https://streak-stats.demolab.com/?user=a-hananop&theme=tokyonight&hide_border=true&background=03080f&stroke=00c6ff&ring=00c6ff&fire=2e7aa0&currStreakNum=eaf6ff&sideNums=6ab8d8&currStreakLabel=2e7aa0&sideLabels=2e7aa0&dates=1e4a62&border_radius=12" alt="Contribution Streak">

  <hr class="gdiv">

  <!-- QUOTE -->
  <div class="slabel"><span class="slabel-bar"></span>Philosophy</div>
  <div class="quote-wrap">
    <p class="quote-text">Turning data into intelligence and ideas into reality — one model at a time.</p>
    <p class="quote-attr">— Abdul Hanan Saqlain</p>
  </div>

  <hr class="gdiv">

  <!-- CONNECT -->
  <div class="slabel"><span class="slabel-bar"></span>Connect</div>
  <div class="conn-row">
    <a class="conn-btn" href="https://www.linkedin.com/in/abdul-hanan-saqlain-5a3103375/" target="_blank">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
      LinkedIn
    </a>
    <a class="conn-btn" href="https://github.com/a-hananop" target="_blank">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.374 0 0 5.373 0 12c0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23A11.509 11.509 0 0112 5.803c1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576C20.566 21.797 24 17.3 24 12c0-6.627-5.373-12-12-12z"/></svg>
      GitHub
    </a>
  </div>

  <!-- FOOTER -->
  <div class="footer">
    <span>⭐ Keep Building.</span> &nbsp;Keep Learning.&nbsp; <span>Keep Growing.</span><br>
    <span style="color:#0d2e45;font-size:.62rem">Abdul Hanan Saqlain &nbsp;·&nbsp; AI Engineer &nbsp;·&nbsp; 2025</span>
  </div>

</div>

<script>
const stackItems=[
  {n:'Python',c:'#4f9cf9'},{n:'C++',c:'#9b87f5'},{n:'Java',c:'#f4b942'},
  {n:'JavaScript',c:'#f7df1e'},{n:'HTML / CSS',c:'#e8774a'},{n:'MySQL',c:'#00bcd4'},
  {n:'MongoDB',c:'#4caf50'},{n:'Supabase',c:'#3ecf8e'},{n:'REST APIs',c:'#00c6ff'},
  {n:'NLP / LLMs',c:'#a78bfa'},{n:'Git & GitHub',c:'#8b9eb0'},{n:'Automation',c:'#34d399'},
];
const doItems=[
  {e:'🤖',t:'AI Applications',s:'End-to-end AI-powered tools'},
  {e:'📊',t:'Data Analysis',s:'Clean, model & visualise data'},
  {e:'⚙️',t:'Automation',s:'Smart workflow automation'},
  {e:'🌐',t:'Full-Stack',s:'API & backend integrations'},
  {e:'🧠',t:'Generative AI',s:'LLM pipelines & prompting'},
  {e:'🔗',t:'API Integration',s:'Seamless service connections'},
];

const sw=document.getElementById('stackWrap');
stackItems.forEach(s=>{
  sw.insertAdjacentHTML('beforeend',
    `<div class="sp"><span class="sp-dot" style="background:${s.c};box-shadow:0 0 8px ${s.c}66"></span>${s.n}</div>`);
});

const dw=document.getElementById('doWrap');
doItems.forEach(d=>{
  dw.insertAdjacentHTML('beforeend',
    `<div class="do-card"><div class="do-icon"><span style="font-size:1.1rem">${d.e}</span></div><div class="do-title">${d.t}</div><div class="do-sub">${d.s}</div></div>`);
});

const roles=['AI Engineer','Generative AI Enthusiast','Automation Builder','Data-Driven Developer'];
let ri=0,ci=0,del=false;
const typer=document.getElementById('typer');
function tick(){
  const w=roles[ri];
  if(!del){ci++;typer.textContent=w.slice(0,ci);if(ci===w.length){del=true;setTimeout(tick,1500);return;}}
  else{ci--;typer.textContent=w.slice(0,ci);if(ci===0){del=false;ri=(ri+1)%roles.length;}}
  setTimeout(tick,del?38:65);
}
tick();

/* ── RING ANIMATION ── */
const rc=document.getElementById('ringCanvas');
const rx=rc.getContext('2d');
let ra=0;
(function ringLoop(){
  rx.clearRect(0,0,120,120);
  const cx=60,cy=60,r=54;
  rx.beginPath();rx.arc(cx,cy,r,0,Math.PI*2);
  rx.strokeStyle='rgba(0,190,255,0.1)';rx.lineWidth=1;rx.stroke();
  const g=rx.createConicalGradient?null:null;
  rx.save();rx.beginPath();rx.arc(cx,cy,r,ra,ra+1.8);
  const lg=rx.createLinearGradient(
    cx+r*Math.cos(ra),cy+r*Math.sin(ra),
    cx+r*Math.cos(ra+1.8),cy+r*Math.sin(ra+1.8));
  lg.addColorStop(0,'rgba(0,198,255,0)');
  lg.addColorStop(1,'rgba(0,198,255,0.95)');
  rx.strokeStyle=lg;rx.lineWidth=2.5;rx.lineCap='round';rx.stroke();rx.restore();
  const hx=cx+r*Math.cos(ra+1.8),hy=cy+r*Math.sin(ra+1.8);
  rx.beginPath();rx.arc(hx,hy,3,0,Math.PI*2);
  rx.fillStyle='#00c6ff';rx.fill();
  ra+=0.022;requestAnimationFrame(ringLoop);
})();

/* ── CRYSTAL PARTICLE BG ── */
const cc=document.getElementById('crystalCanvas');
const ct=cc.getContext('2d');
let cw,ch;
function resz(){cw=cc.width=window.innerWidth;ch=cc.height=window.innerHeight;}
resz();window.addEventListener('resize',resz);

const N=55;
const pts=Array.from({length:N},()=>({
  x:Math.random()*window.innerWidth,
  y:Math.random()*window.innerHeight,
  vx:(Math.random()-.5)*.28,
  vy:(Math.random()-.5)*.28,
  r:Math.random()*1.3+.4,
  a:Math.random()*Math.PI*2,
  va:(Math.random()-.5)*.008,
  size:Math.random()*4+2,
}));

const hexPts=Array.from({length:18},()=>({
  x:Math.random()*window.innerWidth,
  y:Math.random()*window.innerHeight,
  vx:(Math.random()-.5)*.12,
  vy:(Math.random()-.5)*.12,
  s:Math.random()*18+8,
  a:0,va:.003+Math.random()*.005,
  op:Math.random()*.06+.02
}));

function drawHex(cx,cy,s,a,op){
  ct.save();ct.translate(cx,cy);ct.rotate(a);
  ct.beginPath();
  for(let i=0;i<6;i++){
    const ang=i*Math.PI/3;
    i===0?ct.moveTo(s*Math.cos(ang),s*Math.sin(ang)):ct.lineTo(s*Math.cos(ang),s*Math.sin(ang));
  }
  ct.closePath();
  ct.strokeStyle=`rgba(0,190,255,${op})`;ct.lineWidth=.6;ct.stroke();
  ct.restore();
}

function crystalLoop(){
  ct.clearRect(0,0,cw,ch);

  hexPts.forEach(h=>{
    drawHex(h.x,h.y,h.s,h.a,h.op);
    h.x+=h.vx;h.y+=h.vy;h.a+=h.va;
    if(h.x<-40)h.x=cw+40;if(h.x>cw+40)h.x=-40;
    if(h.y<-40)h.y=ch+40;if(h.y>ch+40)h.y=-40;
  });

  for(let i=0;i<N;i++){
    for(let j=i+1;j<N;j++){
      const dx=pts[i].x-pts[j].x,dy=pts[i].y-pts[j].y,d=Math.sqrt(dx*dx+dy*dy);
      if(d<130){
        ct.beginPath();ct.moveTo(pts[i].x,pts[i].y);ct.lineTo(pts[j].x,pts[j].y);
        ct.strokeStyle=`rgba(0,190,255,${.09*(1-d/130)})`;ct.lineWidth=.5;ct.stroke();
      }
    }
    const p=pts[i];
    ct.beginPath();ct.arc(p.x,p.y,p.r,0,Math.PI*2);
    ct.fillStyle='rgba(0,198,255,0.45)';ct.fill();
    p.x+=p.vx;p.y+=p.vy;p.a+=p.va;
    if(p.x<0||p.x>cw)p.vx*=-1;
    if(p.y<0||p.y>ch)p.vy*=-1;
  }
  requestAnimationFrame(crystalLoop);
}
crystalLoop();

/* ── SCROLL REVEAL ── */
const obs=new IntersectionObserver(entries=>{
  entries.forEach(e=>{
    if(e.isIntersecting){
      e.target.style.opacity='1';
      e.target.style.transform='translateY(0)';
    }
  });
},{threshold:.08});

document.querySelectorAll('.gc,.sp,.do-card,.stat-card,.quote-wrap,.conn-btn').forEach(el=>{
  el.style.opacity='0';
  el.style.transform='translateY(18px)';
  el.style.transition='opacity .55s ease, transform .55s ease';
  obs.observe(el);
});
</script>
