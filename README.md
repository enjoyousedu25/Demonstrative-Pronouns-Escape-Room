<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0">
<title>Demonstrative Pronouns Escape Room – EnJoyous Education</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Creepster&family=Orbitron:wght@400;700&family=MedievalSharp&display=swap');
*{box-sizing:border-box;margin:0;padding:0}
:root{
  --bg:#f0f4fa;--card:#fff;--border:#dce6f5;--text:#1a2a3a;--sub:#555;
  --accent:#185fa5;--accent2:#0c447c;--btn-bg:#fff;--btn-col:#185fa5;
  --opt-bg:#f5f8fd;--opt-border:#c8d8ee;--badge-bg:#cce5ff;--badge-col:#004085;
  --prog:#185fa5;--story-bg:#f0f7ff;--story-border:#185fa5;
  --room-bg:#e8f0fa;--room-border:#b0c4de;--hint:#185fa5;
  --font-main:'Segoe UI',Arial,sans-serif;--font-title:'Segoe UI',Arial,sans-serif;
}
body.theme-haunted{
  --bg:#0d0d1a;--card:#1a1a2e;--border:#3a2060;--text:#e8d5ff;--sub:#a89bc0;
  --accent:#9b59b6;--accent2:#6c3483;--btn-bg:#1a1a2e;--btn-col:#d7a8ff;
  --opt-bg:#120e20;--opt-border:#5a3a8a;--badge-bg:#2d1b5e;--badge-col:#c39dff;
  --prog:#9b59b6;--story-bg:#120e20;--story-border:#7d3c98;
  --room-bg:#0a0a18;--room-border:#3a2060;--hint:#c39dff;
  --font-title:'Creepster',cursive;
}
body.theme-space{
  --bg:#050510;--card:#0a0a1f;--border:#1a3a6a;--text:#c8e0ff;--sub:#7a9fc0;
  --accent:#3a9ad9;--accent2:#1a5fa0;--btn-bg:#0a0a1f;--btn-col:#7dd6ff;
  --opt-bg:#060618;--opt-border:#1a3a6a;--badge-bg:#0a1a40;--badge-col:#7dd6ff;
  --prog:#3a9ad9;--story-bg:#060618;--story-border:#3a9ad9;
  --room-bg:#03030e;--room-border:#1a3a6a;--hint:#7dd6ff;
  --font-title:'Orbitron',sans-serif;
}
body.theme-pirate{
  --bg:#3d2000;--card:#4a2800;--border:#8b5e00;--text:#ffe8b0;--sub:#c8a060;
  --accent:#d4870a;--accent2:#a05e00;--btn-bg:#4a2800;--btn-col:#ffe8b0;
  --opt-bg:#3a1e00;--opt-border:#8b5e00;--badge-bg:#5a3000;--badge-col:#ffe8b0;
  --prog:#d4870a;--story-bg:#2a1500;--story-border:#d4870a;
  --room-bg:#2a1500;--room-border:#8b5e00;--hint:#ffe8b0;
  --font-title:'Georgia',serif;
}
body.theme-lab{
  --bg:#001a00;--card:#001f00;--border:#006600;--text:#b0ffb0;--sub:#60c060;
  --accent:#00cc44;--accent2:#008833;--btn-bg:#001f00;--btn-col:#b0ffb0;
  --opt-bg:#001200;--opt-border:#006600;--badge-bg:#002a00;--badge-col:#b0ffb0;
  --prog:#00cc44;--story-bg:#001200;--story-border:#00cc44;
  --room-bg:#000e00;--room-border:#006600;--hint:#b0ffb0;
  --font-title:'Courier New',monospace;
}
body{font-family:var(--font-main);background:var(--bg);color:var(--text);min-height:100vh;transition:background .4s,color .4s}
#app{max-width:700px;margin:0 auto;padding:1.5rem 1rem}
.screen{display:none}.screen.active{display:block}
.brand{font-size:11px;color:var(--sub);text-align:center;letter-spacing:.8px;text-transform:uppercase;margin-top:4px}
h1.game-title{font-size:26px;font-weight:700;text-align:center;color:var(--accent);line-height:1.2;margin-bottom:4px;font-family:var(--font-title)}
h2.game-sub{font-size:15px;font-weight:400;text-align:center;color:var(--sub);margin-bottom:12px}
.theme-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-top:1.2rem}
.theme-btn{background:var(--btn-bg);border:1.5px solid var(--border);border-radius:14px;padding:1.2rem 1rem;cursor:pointer;text-align:left;transition:border-color .15s,transform .12s,box-shadow .12s;box-shadow:0 2px 6px rgba(0,0,0,.3)}
.theme-btn:hover{border-color:var(--accent);transform:translateY(-2px);box-shadow:0 4px 14px rgba(0,0,0,.4)}
.theme-btn .t-icon{font-size:32px;margin-bottom:8px;display:block}
.theme-btn .t-name{font-size:15px;font-weight:700;color:var(--accent)}
.theme-btn .t-desc{font-size:12px;color:var(--sub);margin-top:3px}
.btn{display:inline-flex;align-items:center;gap:6px;padding:10px 20px;border-radius:8px;border:1.5px solid var(--border);background:var(--btn-bg);cursor:pointer;font-size:14px;font-weight:600;color:var(--btn-col);transition:opacity .15s,transform .1s}
.btn:hover{opacity:.85;transform:scale(1.02)}
.btn-primary{background:var(--accent);color:#fff;border-color:var(--accent)}
.btn-success{background:#1e7e34;color:#fff;border-color:#1e7e34}
.btn-row{display:flex;gap:8px;justify-content:center;flex-wrap:wrap;margin-top:1rem}
.grammar-table{width:100%;border-collapse:collapse;font-size:13px;margin:12px 0}
.grammar-table th{background:var(--accent);color:#fff;padding:8px 12px;text-align:left;font-weight:600}
.grammar-table td{padding:8px 12px;border-bottom:1px solid var(--border);color:var(--text)}
.grammar-table tr:nth-child(even) td{background:var(--opt-bg)}
.card{background:var(--card);border:1.5px solid var(--border);border-radius:14px;padding:1.25rem;box-shadow:0 2px 8px rgba(0,0,0,.3)}
.progress-bar{background:var(--opt-bg);border-radius:4px;height:8px;margin:10px 0}
.progress-fill{background:var(--prog);height:8px;border-radius:4px;transition:width .35s}
.q-text{font-size:16px;font-weight:600;color:var(--text);margin-bottom:1rem;line-height:1.55}
.opts{display:grid;grid-template-columns:1fr 1fr;gap:8px}
.opt-btn{background:var(--opt-bg);border:1.5px solid var(--opt-border);border-radius:10px;padding:14px 10px;cursor:pointer;text-align:center;font-size:15px;font-weight:700;color:var(--accent);transition:background .12s,border-color .12s,transform .1s}
.opt-btn:hover{border-color:var(--accent);transform:scale(1.03)}
.opt-btn.correct{background:#1e5c1e;border-color:#28a745;color:#a0ffb0;pointer-events:none}
.opt-btn.wrong{background:#5c1e1e;border-color:#dc3545;color:#ffb0b0;pointer-events:none}
.opt-btn:disabled{pointer-events:none}
.feedback{margin-top:12px;padding:12px 16px;border-radius:10px;font-size:13px;line-height:1.6}
.feedback.ok{background:#1e4a1e;color:#a0ffb0;border-left:4px solid #28a745}
.feedback.err{background:#4a1e1e;color:#ffb0b0;border-left:4px solid #dc3545}
.level-badge{display:inline-block;padding:4px 14px;border-radius:12px;font-size:12px;font-weight:700;margin-bottom:8px;letter-spacing:.3px;background:var(--badge-bg);color:var(--badge-col)}
.story-box{background:var(--story-bg);border-left:4px solid var(--story-border);border-radius:0 10px 10px 0;padding:14px 18px;font-size:14px;color:var(--text);margin:12px 0;line-height:1.7}
.nav{display:flex;align-items:center;justify-content:space-between;margin-bottom:1rem}
.nav-back{cursor:pointer;font-size:13px;color:var(--accent);display:flex;align-items:center;gap:4px;font-weight:600;background:none;border:none}
.items-row{display:flex;gap:6px;flex-wrap:wrap;margin:8px 0;min-height:28px}
.item-chip{background:var(--badge-bg);color:var(--badge-col);border-radius:10px;padding:4px 10px;font-size:11px;font-weight:600}
.code-display{display:flex;gap:10px;justify-content:center;margin:14px 0}
.code-digit{width:52px;height:60px;background:var(--opt-bg);border:2px solid var(--border);border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:26px;font-weight:700;color:var(--accent);transition:all .3s}
.code-digit.revealed{background:var(--accent);color:#fff;border-color:var(--accent2);transform:scale(1.08)}
.rules-list{font-size:14px;color:var(--sub);line-height:2.1;padding-left:1.4rem}

/* ROOM SCENE */
.room-scene{position:relative;width:100%;min-height:260px;background:var(--room-bg);border:2px solid var(--room-border);border-radius:16px;overflow:hidden;margin:12px 0;cursor:default}
.room-scene svg{width:100%;height:100%}
.room-hint{text-align:center;font-size:13px;color:var(--hint);margin-bottom:8px;font-style:italic;animation:pulse 2s infinite}
@keyframes pulse{0%,100%{opacity:.7}50%{opacity:1}}
.room-obj{cursor:pointer;transition:transform .2s,filter .2s}
.room-obj:hover{transform:scale(1.12);filter:brightness(1.4)}
.room-obj.glow{animation:glow-anim 1.5s infinite}
@keyframes glow-anim{0%,100%{filter:drop-shadow(0 0 4px var(--hint))}50%{filter:drop-shadow(0 0 14px var(--hint)) brightness(1.3)}}
.question-overlay{display:none;position:fixed;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,.7);z-index:100;align-items:center;justify-content:center;padding:1rem}
.question-overlay.active{display:flex}
.q-modal{background:var(--card);border:2px solid var(--accent);border-radius:16px;padding:1.5rem;max-width:480px;width:100%;box-shadow:0 8px 40px rgba(0,0,0,.8)}
.q-modal .q-num{font-size:11px;color:var(--sub);letter-spacing:.8px;margin-bottom:6px}
.q-modal .q-text{font-size:15px;font-weight:600;color:var(--text);margin-bottom:14px;line-height:1.6}
.q-modal .opts{display:grid;grid-template-columns:1fr 1fr;gap:8px}
.q-modal .feedback{margin-top:10px;padding:10px 14px;border-radius:8px;font-size:13px}
.q-modal .btn-row{margin-top:10px}

/* TROPHY */
.trophy-scene{text-align:center;padding:2.5rem 1rem}
.trophy-icon{font-size:80px;display:block;margin:0 auto 1rem;animation:pop .55s cubic-bezier(.175,.885,.32,1.275)}
@keyframes pop{0%{transform:scale(0) rotate(-10deg)}70%{transform:scale(1.12)}100%{transform:scale(1)}}
.stars{font-size:30px;letter-spacing:6px;margin:8px 0;animation:fadein .8s .3s both}
@keyframes fadein{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:none}}

/* CERTIFICATE */
.cert-wrap{border:3px double var(--accent);border-radius:14px;padding:2rem;text-align:center;max-width:520px;margin:1rem auto;background:var(--card)}
.cert-title-text{font-size:22px;font-weight:700;color:var(--accent);margin-bottom:6px}
.cert-input{width:220px;text-align:center;font-size:16px;border:none;border-bottom:2px solid var(--accent);background:transparent;padding:6px;color:var(--text);outline:none;display:block;margin:10px auto}
.cert-body{font-size:13px;color:var(--sub);line-height:1.9}
.sig-row{display:flex;gap:2rem;justify-content:center;margin-top:1.5rem}
.sig-line{border-bottom:1.5px solid var(--sub);width:130px;font-size:11px;color:var(--sub);padding-top:4px;text-align:center}

@media print{
  body{background:#fff!important;color:#000!important}
  #app>.screen:not(#s-cert){display:none!important}
  #s-cert{display:block!important}
  .no-print{display:none!important}
  .cert-wrap{border:3px double #185fa5!important;background:#fff!important;color:#000!important;max-width:100%!important;margin:0!important}
  .cert-title-text{color:#185fa5!important}
  .cert-input{color:#000!important;border-bottom:1.5px solid #185fa5!important}
  .cert-body{color:#333!important}
  .sig-line{border-bottom:1px solid #333!important;color:#555!important}
  .nav,.btn-row,.no-print{display:none!important}
}
@media(max-width:500px){
  .theme-grid{grid-template-columns:1fr}
  .opts,.q-modal .opts{grid-template-columns:1fr}
  h1.game-title{font-size:20px}
  #app{padding:1rem .75rem}
  .room-scene{min-height:180px}
}

/* Haunted extras */
body.theme-haunted .room-scene::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse at center,rgba(80,0,120,.3) 0%,rgba(0,0,0,.8) 100%);pointer-events:none;z-index:1}
body.theme-space .room-scene::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse at 50% 30%,rgba(20,40,120,.4) 0%,rgba(0,0,20,.9) 100%);pointer-events:none;z-index:1}
body.theme-pirate .room-scene::before{content:'';position:absolute;inset:0;background:linear-gradient(180deg,rgba(80,40,0,.2) 0%,rgba(20,10,0,.5) 100%);pointer-events:none;z-index:1}
body.theme-lab .room-scene::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse at 50% 80%,rgba(0,100,0,.15) 0%,rgba(0,10,0,.9) 100%);pointer-events:none;z-index:1}

.flicker{animation:flicker 3s infinite}
@keyframes flicker{0%,100%{opacity:1}92%{opacity:1}93%{opacity:.3}94%{opacity:1}96%{opacity:.6}97%{opacity:1}}
</style>
</head>
<body>
<div id="app">

<!-- HOME -->
<div id="s-home" class="screen active">
  <div style="text-align:center;padding:1.5rem 0 1rem">
    <div style="font-size:48px;margin-bottom:8px">🔐</div>
    <h1 class="game-title">Demonstrative Pronouns<br>Escape Room</h1>
    <h2 class="game-sub">Can you escape using <em>this, that, these,</em> and <em>those</em>?</h2>
    <div class="brand">EnJoyous Education</div>
  </div>
  <div class="btn-row" style="margin-bottom:1.2rem">
    <button class="btn btn-primary" onclick="show('s-rules')">▶ How to play</button>
    <button class="btn" onclick="show('s-grammar')">📖 Grammar reminder</button>
  </div>
  <div style="font-size:13px;text-align:center;color:var(--sub);margin-bottom:.8rem;font-weight:600">Choose your escape room theme:</div>
  <div class="theme-grid">
    <button class="theme-btn" onclick="selectTheme(0)"><span class="t-icon">📚</span><div class="t-name">Haunted Library</div><div class="t-desc">Spooky books &amp; ghostly clues</div></button>
    <button class="theme-btn" onclick="selectTheme(1)"><span class="t-icon">🚀</span><div class="t-name">Space Station</div><div class="t-desc">Stars, circuits &amp; alien codes</div></button>
    <button class="theme-btn" onclick="selectTheme(2)"><span class="t-icon">🏴‍☠️</span><div class="t-name">Pirate Treasure Island</div><div class="t-desc">X marks the spot</div></button>
    <button class="theme-btn" onclick="selectTheme(3)"><span class="t-icon">🔬</span><div class="t-name">Secret Laboratory</div><div class="t-desc">Potions, formulas &amp; secrets</div></button>
  </div>
  <div style="font-size:10px;color:var(--sub);text-align:center;margin-top:16px">© EnJoyous Education</div>
</div>

<!-- RULES -->
<div id="s-rules" class="screen">
  <div class="nav"><button class="nav-back" onclick="show('s-home')">← Back</button><span style="font-size:13px;color:var(--sub)">How to play</span></div>
  <div class="card">
    <h2 style="font-size:16px;font-weight:700;margin-bottom:12px;color:var(--accent)">🎮 Game rules</h2>
    <ul class="rules-list">
      <li>Choose a theme to enter your escape room.</li>
      <li>You'll enter a room — <strong>look for the glowing object</strong> and click it!</li>
      <li>A question will appear. Pick the correct pronoun to collect the item.</li>
      <li>✅ Correct answers unlock clues and collect items.</li>
      <li>❌ Wrong answers give a hint — try again!</li>
      <li>Complete all 3 levels to reach the final code challenge.</li>
      <li>Enter the correct 4-digit code to escape and earn your trophy! 🏆</li>
    </ul>
    <div style="margin-top:14px;font-size:13px;color:var(--sub);line-height:2">
      <span style="background:#d4edda;color:#155724;padding:2px 10px;border-radius:10px;font-weight:700;font-size:11px">Level 1</span> Basic identification — 8 questions<br>
      <span style="background:#fff3cd;color:#856404;padding:2px 10px;border-radius:10px;font-weight:700;font-size:11px">Level 2</span> Sentence completion — 8 questions<br>
      <span style="background:#f8d7da;color:#721c24;padding:2px 10px;border-radius:10px;font-weight:700;font-size:11px">Level 3</span> Context challenge — 8 questions<br>
      <span style="background:#cce5ff;color:#004085;padding:2px 10px;border-radius:10px;font-weight:700;font-size:11px">Final</span> 4 code questions → escape!
    </div>
  </div>
  <div class="btn-row"><button class="btn btn-primary" onclick="show('s-home')">Choose a theme →</button></div>
</div>

<!-- GRAMMAR -->
<div id="s-grammar" class="screen">
  <div class="nav"><button class="nav-back" onclick="show('s-home')">← Back</button><span style="font-size:13px;color:var(--sub)">Grammar reminder</span></div>
  <div class="card">
    <h2 style="font-size:16px;font-weight:700;margin-bottom:12px;color:var(--accent)">📖 Demonstrative pronouns</h2>
    <table class="grammar-table">
      <tr><th>Pronoun</th><th>Number</th><th>Distance</th><th>Example</th></tr>
      <tr><td><strong>this</strong></td><td>singular</td><td>🟢 near</td><td><em>This book is mine.</em></td></tr>
      <tr><td><strong>that</strong></td><td>singular</td><td>🔵 far</td><td><em>That bag is yours.</em></td></tr>
      <tr><td><strong>these</strong></td><td>plural</td><td>🟢 near</td><td><em>These pencils are sharp.</em></td></tr>
      <tr><td><strong>those</strong></td><td>plural</td><td>🔵 far</td><td><em>Those birds are noisy.</em></td></tr>
    </table>
    <div style="margin-top:10px;font-size:13px;color:var(--sub);line-height:1.8;background:var(--opt-bg);padding:10px 14px;border-radius:8px">
      🟢 <strong>Near</strong> = close to you &nbsp;|&nbsp; 🔵 <strong>Far</strong> = away from you<br>
      <strong>Singular</strong> = one &nbsp;|&nbsp; <strong>Plural</strong> = more than one
    </div>
  </div>
  <div class="btn-row"><button class="btn btn-primary" onclick="show('s-home')">Start playing →</button></div>
</div>

<!-- GAME (room + question overlay) -->
<div id="s-game" class="screen">
  <div class="nav">
    <button class="nav-back" onclick="show('s-home')">← Home</button>
    <span id="g-theme-label" style="font-size:13px;color:var(--sub);font-weight:600"></span>
  </div>
  <div id="g-level-badge" class="level-badge"></div>
  <div id="g-level-title" style="font-size:16px;font-weight:700;margin-bottom:4px;color:var(--text)"></div>
  <div id="g-level-desc" style="font-size:13px;color:var(--sub);margin-bottom:8px"></div>
  <div class="progress-bar"><div id="g-progress" class="progress-fill" style="width:0%"></div></div>
  <div style="font-size:12px;color:var(--sub);text-align:right;margin-bottom:4px" id="g-qcount"></div>
  <div id="g-story" class="story-box" style="display:none"></div>
  <div class="items-row" id="g-items"></div>

  <!-- ROOM SCENE -->
  <div class="room-hint" id="g-hint">👆 Find the glowing object and click it!</div>
  <div class="room-scene" id="g-room"></div>

  <div style="font-size:10px;color:var(--sub);text-align:center;margin-top:12px">© EnJoyous Education</div>
</div>

<!-- QUESTION OVERLAY (modal) -->
<div class="question-overlay" id="q-overlay">
  <div class="q-modal">
    <div class="q-num" id="qm-num"></div>
    <div class="q-text" id="qm-text"></div>
    <div class="opts" id="qm-opts"></div>
    <div class="feedback" id="qm-feedback" style="display:none"></div>
    <div class="btn-row" id="qm-next-row" style="display:none">
      <button class="btn btn-primary" id="qm-next-btn">Next →</button>
    </div>
  </div>
</div>

<!-- UNLOCK -->
<div id="s-unlock" class="screen">
  <div style="text-align:center;padding:2.5rem 1rem">
    <div style="font-size:60px;animation:pop .5s cubic-bezier(.175,.885,.32,1.275)" id="ul-icon">🔓</div>
    <h2 style="font-size:22px;font-weight:700;margin:14px 0 8px;color:var(--accent)" id="ul-title"></h2>
    <p style="font-size:14px;color:var(--sub);margin-bottom:16px;line-height:1.7" id="ul-msg"></p>
    <div class="btn-row"><button class="btn btn-primary" id="ul-btn"></button></div>
  </div>
</div>

<!-- FINAL CODE -->
<div id="s-final" class="screen">
  <div class="nav"><button class="nav-back" onclick="show('s-home')">← Home</button><span style="font-size:13px;color:var(--sub);font-weight:600">Final escape code</span></div>
  <div class="card">
    <div class="level-badge" style="background:var(--badge-bg);color:var(--badge-col);margin-bottom:8px">🔐 Final challenge</div>
    <div style="font-size:15px;font-weight:700;margin-bottom:4px;color:var(--text)">Decode and escape!</div>
    <div style="font-size:13px;color:var(--sub);margin-bottom:12px">Answer each question to reveal a code digit.</div>
    <div class="code-display" id="f-code-display">
      <div class="code-digit">?</div><div class="code-digit">?</div><div class="code-digit">?</div><div class="code-digit">?</div>
    </div>
    <div id="f-question" class="q-text" style="margin-top:14px"></div>
    <div class="opts" id="f-opts"></div>
    <div class="feedback" id="f-feedback" style="display:none"></div>
    <div class="btn-row" id="f-next-row" style="display:none"><button class="btn btn-primary" id="f-next-btn"></button></div>
  </div>
  <div style="font-size:10px;color:var(--sub);text-align:center;margin-top:12px">© EnJoyous Education</div>
</div>

<!-- TROPHY -->
<div id="s-trophy" class="screen">
  <div class="trophy-scene">
    <span class="trophy-icon">🏆</span>
    <div class="stars">⭐⭐⭐</div>
    <h1 style="font-size:26px;font-weight:700;color:var(--accent);margin-bottom:8px;font-family:var(--font-title)">Escape complete!</h1>
    <p style="font-size:15px;color:var(--sub);max-width:380px;margin:0 auto 1rem;line-height:1.8">Congratulations! You used <em>this, that, these,</em> and <em>those</em> correctly to escape. You are a grammar champion! 🎉</p>
    <div style="font-size:16px;font-weight:700;margin:8px 0;color:var(--accent)" id="t-theme-name"></div>
    <div style="font-size:12px;color:var(--sub);margin-bottom:1.5rem">Awarded by EnJoyous Education</div>
    <div class="btn-row">
      <button class="btn btn-success" onclick="show('s-cert')">🎓 Get certificate</button>
      <button class="btn" onclick="show('s-home')">🏠 Play again</button>
    </div>
  </div>
</div>

<!-- CERTIFICATE -->
<div id="s-cert" class="screen">
  <div class="nav no-print"><button class="nav-back" onclick="show('s-trophy')">← Back</button><span style="font-size:13px;color:var(--sub)">Certificate of completion</span></div>
  <div class="cert-wrap">
    <div style="font-size:11px;letter-spacing:1.2px;color:var(--sub);text-transform:uppercase;margin-bottom:4px">EnJoyous Education</div>
    <div class="cert-title-text">Certificate of Completion</div>
    <div style="font-size:30px;margin:8px 0">🏆</div>
    <div class="cert-body">This certificate is proudly awarded to</div>
    <input class="cert-input" id="cert-name" type="text" placeholder="Student name">
    <div class="cert-body" style="margin-top:6px">
      for successfully completing the<br>
      <strong>Demonstrative Pronouns Escape Room</strong><br>
      and showing understanding of <em>this, that, these,</em> and <em>those.</em>
    </div>
    <div id="cert-theme-line" style="font-size:13px;color:var(--sub);margin-top:8px"></div>
    <div class="sig-row" style="margin-top:1.5rem">
      <div>
        <input class="cert-input" id="cert-date" type="text" placeholder="Date" style="width:140px">
        <div class="sig-line" style="margin:0 auto">Date</div>
      </div>
      <div>
        <input class="cert-input" id="cert-teacher" type="text" placeholder="Teacher's name">
        <div class="sig-line" style="margin:0 auto">Teacher</div>
      </div>
    </div>
    <div style="font-size:10px;color:var(--sub);margin-top:14px">© EnJoyous Education</div>
  </div>
  <div class="btn-row no-print">
    <button class="btn btn-primary" onclick="printCert()">🖨 Print certificate</button>
    <button class="btn" onclick="show('s-home')">🏠 Play again</button>
  </div>
</div>

</div><!-- #app -->

<script>
// ─── DATA ──────────────────────────────────────────────────
const THEMES=[
{name:"Haunted Library",icon:"📚",cls:"haunted",
story:"You are trapped in the old haunted library at midnight. The ghost librarian has locked all the doors! Click on the glowing objects to reveal grammar scrolls. Answer correctly to collect items and escape!",
rooms:[
  {hint:"🕯️ Something is glowing near you...",obj:{emoji:"🕯️",label:"Old Candle",x:20,y:55,near:true},
   q:"You are holding a single old candle. '_____ candle is very dim.' (one candle, in your hand)",opts:["This","That","These","Those"],ans:0,exp:"One thing near you → this."},
  {hint:"📖 A book is floating in the dark...",obj:{emoji:"📖",label:"Floating Book",x:70,y:30,near:false},
   q:"Across the dark room you see one floating book. '_____ book is moving on its own!' (one book, far away)",opts:["This","That","These","Those"],ans:1,exp:"One thing far away → that."},
  {hint:"🗝️ You feel something cold in your pocket...",obj:{emoji:"🗝️",label:"Icy Keys",x:25,y:70,near:true},
   q:"You are touching two cold keys in your pocket. '_____ keys feel icy!' (two keys, near you)",opts:["This","That","These","Those"],ans:2,exp:"More than one thing near you → these."},
  {hint:"🕯️ Candles flicker far at the end of the hall...",obj:{emoji:"🕯️",label:"Spooky Candles",x:75,y:60,near:false},
   q:"You see three candles flickering at the far end of the hall. '_____ candles are so spooky!'",opts:["This","That","These","Those"],ans:3,exp:"More than one thing far away → those."},
  {hint:"📜 A dusty scroll is right in front of you...",obj:{emoji:"📜",label:"Dusty Scroll",x:40,y:65,near:true},
   q:"You pick up one dusty scroll right in front of you. '_____ scroll has a clue!'",opts:["This","That","These","Those"],ans:0,exp:"One thing near you → this."},
  {hint:"👻 Something stirs outside the window far away...",obj:{emoji:"👻",label:"Ghost",x:80,y:25,near:false},
   q:"Through the window, far away, you see one ghost. '_____ ghost is staring at me!'",opts:["This","That","These","Those"],ans:1,exp:"One thing far away → that."},
  {hint:"📚 Heavy books are in your arms...",obj:{emoji:"📚",label:"Library Books",x:30,y:50,near:true},
   q:"You hold two heavy library books in your arms. '_____ books are too heavy to carry.'",opts:["This","That","These","Those"],ans:2,exp:"More than one thing near you → these."},
  {hint:"🚪 Many sealed doors are at the far end...",obj:{emoji:"🚪",label:"Sealed Doors",x:72,y:50,near:false},
   q:"At the far end of the hallway you spot several locked doors. '_____ doors are all sealed shut.'",opts:["This","That","These","Those"],ans:3,exp:"More than one thing far away → those."}
],
rooms2:[
  {hint:"📄 A page glows right in front of you...",obj:{emoji:"📄",label:"Spell Page",x:38,y:60,near:true},q:"I am looking at the page right in front of me. '_____ page has a secret spell written on it.'",opts:["This","That","These","Those"],ans:0,exp:"'Right in front of me' = near, one page → this."},
  {hint:"🚪 A door looms at the end of the hall...",obj:{emoji:"🚪",label:"Hall Door",x:75,y:45,near:false},q:"My friend calls from the other side of the library. '_____ door at the end of the hall is locked.'",opts:["This","That","These","Those"],ans:1,exp:"'End of the hall' = far, one door → that."},
  {hint:"🔮 Glowing orbs float near you...",obj:{emoji:"🔮",label:"Glowing Orbs",x:22,y:50,near:true},q:"I am surrounded by several glowing orbs floating near me. '_____ orbs are giving off a strange light.'",opts:["This","That","These","Those"],ans:2,exp:"Several things near me → these."},
  {hint:"🖼️ Portraits hang far on the wall...",obj:{emoji:"🖼️",label:"Portraits",x:78,y:30,near:false},q:"We can see some old portraits hanging far away on the wall. '_____ portraits look like they are moving.'",opts:["This","That","These","Those"],ans:3,exp:"Many things far away → those."},
  {hint:"🗝️ A ghost hands you a key...",obj:{emoji:"🗝️",label:"Ghost Key",x:32,y:65,near:true},q:"A librarian ghost hands you a single key. '_____ key might open the exit.'",opts:["This","That","These","Those"],ans:0,exp:"One thing in your hand (near) → this."},
  {hint:"🕐 A broken clock ticks across the room...",obj:{emoji:"🕐",label:"Broken Clock",x:72,y:55,near:false},q:"You notice a single broken clock on the wall across the room. '_____ clock stopped at midnight.'",opts:["This","That","These","Those"],ans:1,exp:"One thing far across the room → that."},
  {hint:"🕸️ Cobwebs hang right above your head...",obj:{emoji:"🕸️",label:"Cobwebs",x:28,y:28,near:true},q:"Several cobwebs are hanging right above your head. '_____ cobwebs are tickling my face.'",opts:["This","That","These","Those"],ans:2,exp:"More than one thing near you → these."},
  {hint:"📚 Spell books glow far in the corner...",obj:{emoji:"📚",label:"Spell Books",x:76,y:62,near:false},q:"At the far corner, many spell books are stacked in a pile. '_____ spell books contain the escape clue.'",opts:["This","That","These","Those"],ans:3,exp:"Many things far away → those."}
],
rooms3:[
  {hint:"🗺️ Emma is holding a map — click it!",obj:{emoji:"🗺️",label:"Emma's Map",x:35,y:58,near:true},q:"Emma holds a single map and says, 'I just found _____ map behind the bookshelf!' She is holding it.",opts:["This","That","These","Those"],ans:0,exp:"She is holding it (near her), one map → this."},
  {hint:"🪟 The ghost points to a window far away...",obj:{emoji:"🪟",label:"Far Window",x:78,y:32,near:false},q:"From outside the locked room, the ghost points to a single window across the hall. '_____ window is your way out.'",opts:["This","That","These","Those"],ans:1,exp:"Pointing to something far away, one window → that."},
  {hint:"📡 Two detectors are near the teacher...",obj:{emoji:"📡",label:"Ghost Detectors",x:28,y:55,near:true},q:"Two students are each wearing a ghost detector. 'Are _____ detectors working?' the teacher asks, standing next to them.",opts:["This","That","These","Those"],ans:2,exp:"Two detectors right next to the teacher (near) → these."},
  {hint:"📚 The librarian points to far shelves...",obj:{emoji:"📚",label:"Old Shelves",x:74,y:50,near:false},q:"The librarian points to several rows of bookshelves at the back of the library. '_____ shelves have not been opened in 100 years.'",opts:["This","That","These","Those"],ans:3,exp:"Multiple shelves far away → those."},
  {hint:"📝 A note is stuck right on the door in front of you...",obj:{emoji:"📝",label:"Secret Note",x:40,y:65,near:true},q:"A student finds a note stuck on the door in front of him. '_____ note says the code is hidden in the clock.'",opts:["This","That","These","Those"],ans:0,exp:"The note is right in front of him (near), one note → this."},
  {hint:"🪑 The teacher points to a chair far away...",obj:{emoji:"🪑",label:"Far Chair",x:76,y:60,near:false},q:"The teacher stands at one end of the library and points to a single chair at the other end. 'Do not sit in _____ chair.'",opts:["This","That","These","Those"],ans:1,exp:"The chair is far from the teacher → that."},
  {hint:"🔦 Three students hold torches near the teacher...",obj:{emoji:"🔦",label:"Torches",x:30,y:48,near:true},q:"Three students are all holding torches in their hands. 'Turn on _____ torches now!' the teacher says, standing beside them.",opts:["This","That","These","Those"],ans:2,exp:"Three torches in the students' hands (near the teacher) → these."},
  {hint:"🪦 Gravestones appear far below the window...",obj:{emoji:"🪦",label:"Gravestones",x:72,y:58,near:false},q:"Looking out the window, the students see several gravestones in the dark garden far below. '_____ gravestones were not there yesterday.'",opts:["This","That","These","Those"],ans:3,exp:"Multiple gravestones far away → those."}
],
final:[
  {q:"You hold the last key in your hand. '_____ key in my hand opens the final door.'",opts:["This → 7","That → 2","These → 5","Those → 4"],ans:0,digit:7,exp:"One key in your hand (near) → this. Code digit: 7"},
  {q:"Across the room, you see a single glowing exit sign. '_____ exit sign is showing the way out.'",opts:["This → 3","That → 9","These → 6","Those → 1"],ans:1,digit:9,exp:"One sign far across the room → that. Code digit: 9"},
  {q:"You are carrying several spell papers in your arms. '_____ spell papers will break the ghost's curse.'",opts:["This → 4","That → 8","These → 2","Those → 6"],ans:2,digit:2,exp:"More than one paper in your arms (near) → these. Code digit: 2"},
  {q:"You look back and see many locked chains on the doors far behind you. '_____ chains will never hold me again!'",opts:["This → 5","That → 1","These → 8","Those → 3"],ans:3,digit:3,exp:"Many chains far behind you → those. Code digit: 3"}
],code:"7923"},

{name:"Space Station",icon:"🚀",cls:"space",
story:"You are an astronaut stranded on a damaged space station. The AI system has locked all escape pods! Click glowing equipment to reveal grammar challenges. Solve them to unlock your escape!",
rooms:[
  {hint:"🪖 Your cracked helmet is right here...",obj:{emoji:"🪖",label:"Space Helmet",x:28,y:58,near:true},q:"You are holding one space helmet in your hands. '_____ helmet has a crack in it.'",opts:["This","That","These","Those"],ans:0,exp:"One thing near you → this."},
  {hint:"⚡ A broken panel sparks far across the ship...",obj:{emoji:"⚡",label:"Broken Panel",x:72,y:40,near:false},q:"Far away on the other side of the ship, you see one broken panel. '_____ panel is sparking.'",opts:["This","That","These","Those"],ans:1,exp:"One thing far away → that."},
  {hint:"🫧 Two oxygen tanks are right next to you...",obj:{emoji:"🫧",label:"O₂ Tanks",x:22,y:60,near:true},q:"You are touching two oxygen tanks right next to you. '_____ tanks are almost empty.'",opts:["This","That","These","Those"],ans:2,exp:"More than one thing near you → these."},
  {hint:"☄️ Asteroids glow far through the window...",obj:{emoji:"☄️",label:"Asteroids",x:78,y:28,near:false},q:"Through the window, you see several distant asteroids. '_____ asteroids are heading our way.'",opts:["This","That","These","Those"],ans:3,exp:"More than one thing far away → those."},
  {hint:"💾 A chip sits on the desk right in front of you...",obj:{emoji:"💾",label:"Control Chip",x:42,y:65,near:true},q:"You pick up a single control chip from the desk in front of you. '_____ chip controls the escape pod.'",opts:["This","That","These","Those"],ans:0,exp:"One thing near you → this."},
  {hint:"🚨 An alarm light blinks far across the station...",obj:{emoji:"🚨",label:"Alarm Light",x:74,y:55,near:false},q:"Far across the station, you notice one blinking alarm light. '_____ light means danger.'",opts:["This","That","These","Those"],ans:1,exp:"One thing far away → that."},
  {hint:"💿 Two data discs are in your hands...",obj:{emoji:"💿",label:"Data Discs",x:30,y:50,near:true},q:"You are carrying two data discs in your hands. '_____ discs have the unlock codes.'",opts:["This","That","These","Those"],ans:2,exp:"More than one thing near you → these."},
  {hint:"🌟 Stars shine far through the porthole...",obj:{emoji:"🌟",label:"Star Map",x:76,y:32,near:false},q:"You look out the window and see many distant stars. '_____ stars look so bright from here.'",opts:["This","That","These","Those"],ans:3,exp:"More than one thing far away → those."}
],
rooms2:[
  {hint:"🖥️ The screen glows right in front of the astronaut...",obj:{emoji:"🖥️",label:"Fuel Screen",x:36,y:60,near:true},q:"The astronaut taps the control screen directly in front of her. '_____ screen shows the fuel level.'",opts:["This","That","These","Those"],ans:0,exp:"Directly in front = near, one screen → this."},
  {hint:"🛰️ A satellite floats far out in space...",obj:{emoji:"🛰️",label:"Satellite",x:76,y:28,near:false},q:"Mission Control points to a satellite floating far out in space. '_____ satellite is sending a signal.'",opts:["This","That","These","Those"],ans:1,exp:"Far out in space, one satellite → that."},
  {hint:"🔧 Two astronauts hold repair tools near you...",obj:{emoji:"🔧",label:"Repair Tools",x:26,y:55,near:true},q:"Two astronauts are holding repair tools right in their hands. '_____ tools can fix the air lock.'",opts:["This","That","These","Those"],ans:2,exp:"More than one tool near them → these."},
  {hint:"☀️ Broken solar panels glow far along the hull...",obj:{emoji:"☀️",label:"Solar Panels",x:74,y:48,near:false},q:"You can see several broken solar panels far along the hull of the ship. '_____ panels need replacing immediately.'",opts:["This","That","These","Those"],ans:3,exp:"Many panels far away → those."},
  {hint:"💳 A password card is under your seat...",obj:{emoji:"💳",label:"Password Card",x:38,y:70,near:true},q:"You find a single password card tucked under your seat. '_____ card has the access code.'",opts:["This","That","These","Those"],ans:0,exp:"One card under your seat (near) → this."},
  {hint:"🚪 One emergency exit glows far at the back...",obj:{emoji:"🚪",label:"Emergency Exit",x:76,y:52,near:false},q:"Far at the back of the station, there is one emergency exit. '_____ exit is the only way out.'",opts:["This","That","These","Those"],ans:1,exp:"One exit far away → that."},
  {hint:"⚠️ Warning lights flash all around you...",obj:{emoji:"⚠️",label:"Warning Lights",x:24,y:42,near:true},q:"Several warning lights are flashing all around you. '_____ lights are warning us about a system failure.'",opts:["This","That","These","Those"],ans:2,exp:"Many lights near you → these."},
  {hint:"🪐 Distant planets appear on the monitor...",obj:{emoji:"🪐",label:"Distant Planets",x:72,y:35,near:false},q:"A camera shows many distant planets on the monitor. '_____ planets are outside our solar system.'",opts:["This","That","These","Those"],ans:3,exp:"Many planets far away → those."}
],
rooms3:[
  {hint:"⚡ The astronaut holds up a broken wire...",obj:{emoji:"⚡",label:"Broken Wire",x:34,y:58,near:true},q:"An astronaut holds up a single broken wire and says, '_____ wire caused the blackout.' She is showing it to the team.",opts:["This","That","These","Those"],ans:0,exp:"She is holding it (near her), one wire → this."},
  {hint:"🪨 A space rock drifts far through the porthole...",obj:{emoji:"🪨",label:"Space Rock",x:76,y:30,near:false},q:"Through the porthole, an astronaut points to a single space rock drifting far away. 'Avoid _____ rock — it is dangerous.'",opts:["This","That","These","Those"],ans:1,exp:"One rock, far away through the porthole → that."},
  {hint:"👨‍🚀 Two crew members stand in suits beside the commander...",obj:{emoji:"👨‍🚀",label:"Space Suits",x:28,y:52,near:true},q:"Two crew members are wearing their suits beside the commander. 'Are _____ suits fully sealed?' the commander asks.",opts:["This","That","These","Those"],ans:2,exp:"Two suits right next to the commander (near) → these."},
  {hint:"🛸 Many enemy ships appear on the far radar...",obj:{emoji:"🛸",label:"Enemy Ships",x:74,y:45,near:false},q:"The pilot looks at the radar and sees many enemy ships far behind the station. '_____ ships are getting closer.'",opts:["This","That","These","Those"],ans:3,exp:"Many ships far away on the radar → those."},
  {hint:"🔴 A hidden button is inside the panel right in front of her...",obj:{emoji:"🔴",label:"Hidden Button",x:40,y:68,near:true},q:"A crew member finds a single hidden button inside the control panel right in front of her. 'Press _____ button to open the pod bay door.'",opts:["This","That","These","Those"],ans:0,exp:"One button right in front of her (near) → this."},
  {hint:"🪟 A cracked window glows at the far end of the ship...",obj:{emoji:"🪟",label:"Cracked Window",x:74,y:38,near:false},q:"The commander points across the ship to a single cracked window at the far end. '_____ window must be repaired before we launch.'",opts:["This","That","These","Those"],ans:1,exp:"One window, far across the ship → that."},
  {hint:"⛽ Fuel canisters sit at the engineers' feet...",obj:{emoji:"⛽",label:"Fuel Canisters",x:26,y:62,near:true},q:"Three engineers are standing next to several fuel canisters at their feet. 'Connect _____ canisters to the engine now.'",opts:["This","That","These","Those"],ans:2,exp:"Multiple canisters near the engineers → these."},
  {hint:"🌌 Distant galaxies appear on the navigation map...",obj:{emoji:"🌌",label:"Galaxies",x:76,y:55,near:false},q:"Looking at a map, the crew sees several distant galaxies marked with red. '_____ galaxies are too far to reach.'",opts:["This","That","These","Those"],ans:3,exp:"Multiple galaxies far away → those."}
],
final:[
  {q:"You hold one access card in your hand. '_____ access card opens the escape pod.'",opts:["This → 4","That → 8","These → 1","Those → 6"],ans:0,digit:4,exp:"One card in your hand (near) → this. Code digit: 4"},
  {q:"Across the ship, a single red button is flashing. 'Do NOT press _____ button — it will destroy the ship!'",opts:["This → 2","That → 5","These → 9","Those → 3"],ans:1,digit:5,exp:"One button far across the ship → that. Code digit: 5"},
  {q:"You are gripping two escape handles right in front of you. 'Pull _____ handles at the same time!'",opts:["This → 7","That → 3","These → 6","Those → 8"],ans:2,digit:6,exp:"Two handles right in front of you (near) → these. Code digit: 6"},
  {q:"Far away on the planet's surface, you see many landing lights. '_____ lights will guide us down safely.'",opts:["This → 3","That → 1","These → 4","Those → 2"],ans:3,digit:2,exp:"Many lights far away → those. Code digit: 2"}
],code:"4562"},

{name:"Pirate Treasure Island",icon:"🏴‍☠️",cls:"pirate",
story:"Ahoy! You are marooned on a mysterious island. The pirate captain has hidden the treasure and locked the ship! Click on glowing island objects to reveal grammar riddles. Solve them to find the treasure and sail away!",
rooms:[
  {hint:"🪙 A gold coin glints in your palm...",obj:{emoji:"🪙",label:"Gold Coin",x:30,y:62,near:true},q:"You are holding a single gold coin in your palm. '_____ coin has a strange mark on it.'",opts:["This","That","These","Those"],ans:0,exp:"One thing near you → this."},
  {hint:"⚓ An old shipwreck looms far across the beach...",obj:{emoji:"⚓",label:"Shipwreck",x:74,y:42,near:false},q:"Across the beach, far away, you see one old shipwreck. '_____ shipwreck has been there for years.'",opts:["This","That","These","Those"],ans:1,exp:"One thing far away → that."},
  {hint:"🗺️ Two treasure maps are in your hands...",obj:{emoji:"🗺️",label:"Treasure Maps",x:28,y:55,near:true},q:"You are carrying two treasure maps in your hands. '_____ maps show two different routes.'",opts:["This","That","These","Those"],ans:2,exp:"More than one thing near you → these."},
  {hint:"🚢 Pirate ships sail far on the horizon...",obj:{emoji:"🚢",label:"Pirate Ships",x:76,y:30,near:false},q:"Far out at sea, you spot several pirate ships on the horizon. '_____ ships are heading toward the island.'",opts:["This","That","These","Those"],ans:3,exp:"More than one thing far away → those."},
  {hint:"🗝️ A key is in your pocket — reach for it...",obj:{emoji:"🗝️",label:"Chest Key",x:38,y:70,near:true},q:"You reach into your pocket and pull out a single key. '_____ key must open the treasure chest.'",opts:["This","That","These","Those"],ans:0,exp:"One thing near you → this."},
  {hint:"🌴 One tall palm tree stands far along the beach...",obj:{emoji:"🌴",label:"Palm Tree",x:72,y:35,near:false},q:"Far along the beach, you notice one tall palm tree. '_____ palm tree is the landmark on the map.'",opts:["This","That","These","Those"],ans:1,exp:"One thing far away → that."},
  {hint:"💍 Gold rings are in your hand...",obj:{emoji:"💍",label:"Gold Rings",x:26,y:58,near:true},q:"You are holding several gold rings in your hand. '_____ rings belong to the pirate captain.'",opts:["This","That","These","Those"],ans:2,exp:"More than one thing near you → these."},
  {hint:"🏝️ Many islands shimmer far out at sea...",obj:{emoji:"🏝️",label:"Distant Islands",x:78,y:45,near:false},q:"You look out to sea and see many distant islands. '_____ islands are not on our map.'",opts:["This","That","These","Those"],ans:3,exp:"More than one thing far away → those."}
],
rooms2:[
  {hint:"💰 The treasure chest sits right in front of the pirate...",obj:{emoji:"💰",label:"Treasure Chest",x:35,y:65,near:true},q:"The pirate taps the chest sitting right in front of him. '_____ chest is heavier than it looks.'",opts:["This","That","These","Those"],ans:0,exp:"Right in front of him = near, one chest → this."},
  {hint:"💀 A skull rock glows far out at sea...",obj:{emoji:"💀",label:"Skull Rock",x:75,y:35,near:false},q:"The lookout points to a single rock formation far out at sea. '_____ rock is shaped like a skull.'",opts:["This","That","These","Those"],ans:1,exp:"Far out at sea, one rock → that."},
  {hint:"⛏️ Two pirates hold shovels beside the captain...",obj:{emoji:"⛏️",label:"Shovels",x:28,y:55,near:true},q:"Two pirates are holding shovels right beside the captain. '_____ shovels are needed for digging.'",opts:["This","That","These","Those"],ans:2,exp:"Two shovels next to the captain (near) → these."},
  {hint:"🏝️ Many islands sparkle far through the telescope...",obj:{emoji:"🏝️",label:"Far Islands",x:76,y:38,near:false},q:"Looking through the telescope, the captain sees many islands far in the distance. '_____ islands might have more treasure.'",opts:["This","That","These","Those"],ans:3,exp:"Many islands far away → those."},
  {hint:"🧭 A golden compass is in your bag...",obj:{emoji:"🧭",label:"Compass",x:34,y:68,near:true},q:"You reach into your bag and find a single golden compass. '_____ compass will guide us to the treasure.'",opts:["This","That","These","Those"],ans:0,exp:"One compass in your bag (near) → this."},
  {hint:"💦 A waterfall shimmers far across the jungle...",obj:{emoji:"💦",label:"Waterfall",x:74,y:52,near:false},q:"Across the jungle, there is a single waterfall far in the distance. '_____ waterfall is where the treasure is buried.'",opts:["This","That","These","Those"],ans:1,exp:"One waterfall far away → that."},
  {hint:"🦀 Crabs crawl near your feet...",obj:{emoji:"🦀",label:"Crabs",x:26,y:70,near:true},q:"Several crabs are crawling near your feet right now. '_____ crabs are pinching my toes!'",opts:["This","That","These","Those"],ans:2,exp:"More than one crab near you → these."},
  {hint:"💣 Enemy cannons glint on the far cliff...",obj:{emoji:"💣",label:"Cannons",x:76,y:44,near:false},q:"The captain peers through his telescope at several enemy cannons on the far cliff. '_____ cannons are aimed at us!'",opts:["This","That","These","Those"],ans:3,exp:"Many cannons far away → those."}
],
rooms3:[
  {hint:"🗺️ A pirate holds up a rolled map — click it!",obj:{emoji:"🗺️",label:"Rolled Map",x:33,y:60,near:true},q:"A pirate holds up a single rolled-up map and says, '_____ map shows where the gold is.' He is waving it in the air.",opts:["This","That","These","Those"],ans:0,exp:"He is holding it (near him), one map → this."},
  {hint:"🏚️ The captain points to a hut far along the beach...",obj:{emoji:"🏚️",label:"Far Hut",x:75,y:45,near:false},q:"Standing on the ship, the captain points to a single hut far along the beach. 'The treasure is hidden under _____ hut.'",opts:["This","That","These","Those"],ans:1,exp:"One hut far away on the beach → that."},
  {hint:"🔦 Three lanterns glow right around you...",obj:{emoji:"🔦",label:"Lanterns",x:27,y:55,near:true},q:"Three pirates are each holding a lantern right around you. 'Are _____ lanterns bright enough to see in the cave?'",opts:["This","That","These","Those"],ans:2,exp:"Three lanterns near the captain → these."},
  {hint:"🏴‍☠️ Enemy flags wave far through the telescope...",obj:{emoji:"🏴‍☠️",label:"Enemy Flags",x:76,y:32,near:false},q:"Looking through the telescope, the captain sees many enemy flags on ships in the distance. '_____ flags mean they are pirates too!'",opts:["This","That","These","Those"],ans:3,exp:"Many flags far away → those."},
  {hint:"📦 A metal box is right at your feet...",obj:{emoji:"📦",label:"Metal Box",x:40,y:72,near:true},q:"You dig in the sand and find a single metal box right at your feet. '_____ box must be the treasure chest!'",opts:["This","That","These","Those"],ans:0,exp:"One box right at your feet (near) → this."},
  {hint:"💥 A broken cannon stands far down the beach...",obj:{emoji:"💥",label:"Broken Cannon",x:74,y:54,near:false},q:"A sailor calls from far down the beach pointing to a single broken cannon. 'Stay away from _____ cannon — it is unstable!'",opts:["This","That","These","Those"],ans:1,exp:"One cannon far down the beach → that."},
  {hint:"🛢️ Barrels sit right beside the crew...",obj:{emoji:"🛢️",label:"Supply Barrels",x:28,y:60,near:true},q:"The crew is standing around several barrels of supplies right beside them. 'Load _____ barrels onto the ship.'",opts:["This","That","These","Those"],ans:2,exp:"Multiple barrels right beside the crew (near) → these."},
  {hint:"🌩️ Storm clouds gather far off the coast...",obj:{emoji:"🌩️",label:"Storm Clouds",x:76,y:28,near:false},q:"Far off the coast, the crew sees many dark storm clouds gathering. '_____ clouds mean a big storm is coming.'",opts:["This","That","These","Those"],ans:3,exp:"Many clouds far away → those."}
],
final:[
  {q:"You hold the golden key tightly in your fist. '_____ golden key will unlock the ship's helm.'",opts:["This → 6","That → 3","These → 9","Those → 5"],ans:0,digit:6,exp:"One key in your hand (near) → this. Code digit: 6"},
  {q:"The lookout points to a single lighthouse far across the sea. 'Sail toward _____ lighthouse — it marks the safe harbor.'",opts:["This → 2","That → 8","These → 4","Those → 7"],ans:1,digit:8,exp:"One lighthouse far across the sea → that. Code digit: 8"},
  {q:"You find two old coins stuck in the lock right in front of you. 'Remove _____ coins to open the lock!'",opts:["This → 5","That → 1","These → 3","Those → 9"],ans:2,digit:3,exp:"Two coins right in front of you (near) → these. Code digit: 3"},
  {q:"The captain looks across the water and sees many enemy boats in the distance. 'We must outrun _____ boats before nightfall!'",opts:["This → 4","That → 6","These → 7","Those → 1"],ans:3,digit:1,exp:"Many boats far away → those. Code digit: 1"}
],code:"6831"},

{name:"Secret Laboratory",icon:"🔬",cls:"lab",
story:"You have been locked inside a secret laboratory! Strange potions bubble, machines beep, and the exit is sealed. Click glowing lab equipment to reveal grammar experiments. Solve them to earn the unlock formula!",
rooms:[
  {hint:"🧪 A test tube glows in your hand...",obj:{emoji:"🧪",label:"Test Tube",x:32,y:60,near:true},q:"You hold a single test tube of blue liquid in your hand. '_____ test tube contains the antidote.'",opts:["This","That","These","Those"],ans:0,exp:"One thing near you → this."},
  {hint:"⚙️ A large machine hums far across the lab...",obj:{emoji:"⚙️",label:"Exit Machine",x:74,y:42,near:false},q:"Across the lab, far away, you see one large machine. '_____ machine controls the exit.'",opts:["This","That","These","Those"],ans:1,exp:"One thing far away → that."},
  {hint:"🧫 Two beakers sit right beside you...",obj:{emoji:"🧫",label:"Beakers",x:26,y:58,near:true},q:"You have two beakers sitting right beside you on the bench. '_____ beakers must be mixed together.'",opts:["This","That","These","Those"],ans:2,exp:"More than one thing near you → these."},
  {hint:"🫧 Glowing bottles line the far shelves...",obj:{emoji:"🫧",label:"Potion Bottles",x:76,y:35,near:false},q:"You can see several glowing bottles on the shelves at the far end of the lab. '_____ bottles are dangerous!'",opts:["This","That","These","Those"],ans:3,exp:"More than one thing far away → those."},
  {hint:"📋 A formula card is right in front of you...",obj:{emoji:"📋",label:"Formula Card",x:40,y:68,near:true},q:"You pick up a single formula card from the desk right in front of you. '_____ formula is the key to the antidote.'",opts:["This","That","These","Those"],ans:0,exp:"One thing near you → this."},
  {hint:"🔴 A red button flashes far at the end of the room...",obj:{emoji:"🔴",label:"Red Button",x:74,y:55,near:false},q:"At the far end of the room, one big red button is flashing. '_____ button will unlock the door.'",opts:["This","That","These","Those"],ans:1,exp:"One thing far away → that."},
  {hint:"🧫 Three petri dishes are in your hands...",obj:{emoji:"🧫",label:"Petri Dishes",x:28,y:52,near:true},q:"You are holding three petri dishes in your hands. '_____ dishes contain the bacteria samples.'",opts:["This","That","These","Those"],ans:2,exp:"More than one thing near you → these."},
  {hint:"🧪 Many test tubes glow on a far rack...",obj:{emoji:"🧪",label:"Test Rack",x:76,y:44,near:false},q:"Far across the lab, many test tubes are lined up on a rack. '_____ test tubes have already been tested.'",opts:["This","That","These","Those"],ans:3,exp:"More than one thing far away → those."}
],
rooms2:[
  {hint:"📓 A notebook glows right in front of the scientist...",obj:{emoji:"📓",label:"Notebook",x:36,y:62,near:true},q:"The scientist taps the single notebook on the desk right in front of her. '_____ notebook contains all the secret formulas.'",opts:["This","That","These","Those"],ans:0,exp:"Right in front of her = near, one notebook → this."},
  {hint:"🗄️ A locked cabinet gleams far across the room...",obj:{emoji:"🗄️",label:"Locked Cabinet",x:74,y:40,near:false},q:"The scientist points to a single locked cabinet far across the room. '_____ cabinet holds the master formula.'",opts:["This","That","These","Those"],ans:1,exp:"Far across the room, one cabinet → that."},
  {hint:"💉 Two assistants hold syringes beside the scientist...",obj:{emoji:"💉",label:"Syringes",x:26,y:55,near:true},q:"Two assistants are standing beside the scientist holding syringes. '_____ syringes must be sterilised first.'",opts:["This","That","These","Those"],ans:2,exp:"Two syringes near the scientist → these."},
  {hint:"🛢️ Chemical drums sit far below in the yard...",obj:{emoji:"🛢️",label:"Chemical Drums",x:76,y:50,near:false},q:"Through the window, the scientist can see many chemical drums stored in the yard far below. '_____ drums contain hazardous waste.'",opts:["This","That","These","Those"],ans:3,exp:"Many drums far away → those."},
  {hint:"💳 A magnetic card is in your coat pocket...",obj:{emoji:"💳",label:"Magnetic Card",x:38,y:68,near:true},q:"You reach into your coat pocket and pull out a single magnetic card. '_____ card will deactivate the alarm.'",opts:["This","That","These","Those"],ans:0,exp:"One card in your pocket (near) → this."},
  {hint:"🌀 A broken fan turns slowly far across the lab...",obj:{emoji:"🌀",label:"Broken Fan",x:74,y:44,near:false},q:"Far across the lab, there is one broken ventilation fan. '_____ fan needs to be fixed urgently.'",opts:["This","That","These","Those"],ans:1,exp:"One fan far away → that."},
  {hint:"🔬 Glass slides are on the desk right in front of you...",obj:{emoji:"🔬",label:"Glass Slides",x:30,y:58,near:true},q:"Several glass slides are laid out on the desk right in front of you. '_____ slides are ready for the microscope.'",opts:["This","That","These","Those"],ans:2,exp:"More than one slide near you → these."},
  {hint:"👮 Guards patrol far outside the building...",obj:{emoji:"👮",label:"Guards",x:76,y:38,near:false},q:"Looking through the periscope, you can see many guards patrolling far outside the building. '_____ guards cannot see us yet.'",opts:["This","That","These","Those"],ans:3,exp:"Many guards far away → those."}
],
rooms3:[
  {hint:"💡 A scientist holds up a glowing vial — click it!",obj:{emoji:"💡",label:"Glowing Vial",x:34,y:60,near:true},q:"A scientist holds up a single glowing vial and says, 'Careful — _____ vial contains an explosive formula.' She is gripping it.",opts:["This","That","These","Those"],ans:0,exp:"She is holding it (near her), one vial → this."},
  {hint:"⚛️ A reactor glows far below on the ground floor...",obj:{emoji:"⚛️",label:"Reactor",x:76,y:50,near:false},q:"From the observation deck, the professor points at a single reactor far below on the ground floor. '_____ reactor is about to overheat.'",opts:["This","That","These","Those"],ans:1,exp:"One reactor far below → that."},
  {hint:"🔭 Three lab stations sit right next to the teacher...",obj:{emoji:"🔭",label:"Lab Stations",x:26,y:55,near:true},q:"Three students are standing beside their lab stations right next to the teacher. '_____ stations must be cleaned before you leave.'",opts:["This","That","These","Those"],ans:2,exp:"Three stations near the teacher → these."},
  {hint:"🛢️ Many barrels are stacked far in the storage room...",obj:{emoji:"🛢️",label:"Far Barrels",x:74,y:42,near:false},q:"Using a security camera, the scientist sees many barrels stacked far in the storage room. '_____ barrels were moved overnight.'",opts:["This","That","These","Those"],ans:3,exp:"Many barrels far away → those."},
  {hint:"🔌 A switch is hidden beneath the table right in front of you...",obj:{emoji:"🔌",label:"Hidden Switch",x:38,y:72,near:true},q:"You spot a single small switch hidden beneath the table right in front of you. 'Flip _____ switch to open the emergency exit.'",opts:["This","That","These","Those"],ans:0,exp:"One switch right in front of you (near) → this."},
  {hint:"🖥️ An error screen blinks far at the other end of the lab...",obj:{emoji:"🖥️",label:"Error Screen",x:74,y:38,near:false},q:"The head scientist stands at one end of the lab and points to a single error screen at the other end. 'Fix _____ error before the system shuts down.'",opts:["This","That","These","Those"],ans:1,exp:"One screen far away → that."},
  {hint:"🧫 Lab assistants hold petri dishes near the exit...",obj:{emoji:"🧫",label:"Petri Dishes",x:28,y:60,near:true},q:"Two lab assistants are carrying several petri dishes in their hands near the exit. 'Handle _____ dishes carefully — they are fragile.'",opts:["This","That","These","Those"],ans:2,exp:"Several dishes near the exit (near) → these."},
  {hint:"🚨 Many sensors flash across the far wing...",obj:{emoji:"🚨",label:"Far Sensors",x:76,y:48,near:false},q:"The alarm shows many broken sensors spread across the far wing of the building. '_____ sensors need to be replaced before the experiment can continue.'",opts:["This","That","These","Those"],ans:3,exp:"Many sensors far away → those."}
],
final:[
  {q:"You hold a single glowing key card right in your hand. '_____ key card will unlock the main exit.'",opts:["This → 5","That → 2","These → 8","Those → 4"],ans:0,digit:5,exp:"One card in your hand (near) → this. Code digit: 5"},
  {q:"Across the lab, a single control dial is slowly turning. '_____ dial controls the door lock.'",opts:["This → 1","That → 7","These → 3","Those → 9"],ans:1,digit:7,exp:"One dial far across the lab → that. Code digit: 7"},
  {q:"You are holding two data drives in your hands. '_____ drives contain the escape formula!'",opts:["This → 4","That → 6","These → 1","Those → 8"],ans:2,digit:1,exp:"Two drives in your hands (near) → these. Code digit: 1"},
  {q:"The security camera shows many alarm sensors flashing far outside the building. '_____ sensors will go off if we open the door the wrong way.'",opts:["This → 3","That → 5","These → 6","Those → 4"],ans:3,digit:4,exp:"Many sensors far outside → those. Code digit: 4"}
],code:"5714"}
];

// ─── STATE ─────────────────────────────────────────────────
let theme=-1,level=1,qIdx=0,collected=[],codeDigits=["?","?","?","?"],finalQIdx=0;

// ─── UTIL ──────────────────────────────────────────────────
function show(id){
  document.querySelectorAll('.screen').forEach(s=>s.classList.remove('active'));
  document.getElementById(id).classList.add('active');
  window.scrollTo(0,0);
}

function setThemeCls(cls){
  document.body.className='theme-'+cls;
}

function getCurrentRooms(){
  const T=THEMES[theme];
  return level===1?T.rooms:level===2?T.rooms2:T.rooms3;
}

// ─── THEME SELECT ──────────────────────────────────────────
function selectTheme(t){
  theme=t;level=1;qIdx=0;collected=[];codeDigits=["?","?","?","?"];finalQIdx=0;
  const T=THEMES[t];
  setThemeCls(T.cls);
  document.getElementById('g-theme-label').textContent=T.icon+' '+T.name;
  document.getElementById('g-story').textContent=T.story;
  document.getElementById('g-story').style.display='block';
  document.getElementById('cert-theme-line').textContent='Theme completed: '+T.name;
  document.getElementById('t-theme-name').textContent=T.icon+' '+T.name;
  loadLevel();
  show('s-game');
}

// ─── LEVEL SETUP ───────────────────────────────────────────
function loadLevel(){
  const badge=document.getElementById('g-level-badge');
  badge.textContent=['🔑 Level 1','🔓 Level 2','🧩 Level 3'][level-1];
  document.getElementById('g-level-title').textContent=['Level 1 — Basic Identification','Level 2 — Sentence Completion','Level 3 — Context Challenge'][level-1];
  document.getElementById('g-level-desc').textContent=['Choose the correct pronoun based on number and distance clues.','Complete the sentence with the right demonstrative pronoun.','Read the situation carefully and choose the correct pronoun.'][level-1];
  collected=[];
  renderItems();
  renderRoom();
}

function renderItems(){
  const T=THEMES[theme];
  const rooms=getCurrentRooms();
  document.getElementById('g-items').innerHTML=collected.map((c,i)=>{
    const item=rooms[i]||{};
    return`<span class="item-chip">${item.obj?item.obj.emoji:'✅'} ${item.obj?item.obj.label:'Item'}</span>`;
  }).join('');
}

// ─── ROOM RENDERER ─────────────────────────────────────────
function renderRoom(){
  const T=THEMES[theme];
  const rooms=getCurrentRooms();
  if(qIdx>=rooms.length) return;
  const room=rooms[qIdx];
  const obj=room.obj;
  const total=rooms.length;

  // Progress
  document.getElementById('g-progress').style.width=((qIdx/total)*100)+'%';
  document.getElementById('g-qcount').textContent=`Question ${qIdx+1} of ${total}`;
  document.getElementById('g-hint').textContent=room.hint;

  // Draw scene
  const near=obj.near;
  const x=obj.x,y=obj.y;
  const bg=getBgSVG(T.cls,near,x,y);

  document.getElementById('g-room').innerHTML=`
    <svg viewBox="0 0 400 220" xmlns="http://www.w3.org/2000/svg" style="display:block">
      ${bg}
      <!-- near/far indicator -->
      <text x="200" y="15" font-size="9" fill="rgba(255,255,255,0.5)" text-anchor="middle" font-family="sans-serif">
        ${near?'👤 YOU are HERE':'👁️ Looking from afar...'}
      </text>
      <!-- clickable object -->
      <text x="${x*4}" y="${y*2.2}" font-size="36"
        class="room-obj glow"
        style="cursor:pointer;user-select:none"
        text-anchor="middle"
        onclick="openQuestion()"
        role="button"
        aria-label="${obj.label}">${obj.emoji}</text>
      <!-- label -->
      <rect x="${x*4-32}" y="${y*2.2+4}" width="64" height="14" rx="7" fill="rgba(0,0,0,0.55)"/>
      <text x="${x*4}" y="${y*2.2+14}" font-size="9" fill="#fff" text-anchor="middle" font-family="sans-serif" pointer-events="none">${obj.label}</text>
    </svg>`;
}

function getBgSVG(cls,near,ox,oy){
  // Theme-specific atmospheric background SVG elements
  const themes={
    haunted:`
      <rect width="400" height="220" fill="#080818"/>
      <ellipse cx="200" cy="110" rx="180" ry="100" fill="rgba(60,0,100,0.35)"/>
      <!-- floor -->
      <rect x="0" y="170" width="400" height="50" fill="#0d0d22"/>
      <!-- bookshelves far -->
      <rect x="300" y="60" width="90" height="110" fill="#1a0a30" rx="4"/>
      <line x1="300" x2="390" y1="90" y2="90" stroke="#2a1050" stroke-width="1.5"/>
      <line x1="300" x2="390" y1="120" y2="120" stroke="#2a1050" stroke-width="1.5"/>
      <line x1="300" x2="390" y1="150" y2="150" stroke="#2a1050" stroke-width="1.5"/>
      <!-- bookshelf near -->
      <rect x="10" y="60" width="80" height="110" fill="#1a0a30" rx="4"/>
      <line x1="10" x2="90" y1="90" y2="90" stroke="#2a1050" stroke-width="1.5"/>
      <line x1="10" x2="90" y1="120" y2="120" stroke="#2a1050" stroke-width="1.5"/>
      <line x1="10" x2="90" y1="150" y2="150" stroke="#2a1050" stroke-width="1.5"/>
      <!-- window -->
      <rect x="170" y="20" width="60" height="80" fill="#0a0a30" rx="4" stroke="#3a2060" stroke-width="2"/>
      <line x1="200" x2="200" y1="20" y2="100" stroke="#3a2060" stroke-width="1.5"/>
      <line x1="170" x2="230" y1="60" y2="60" stroke="#3a2060" stroke-width="1.5"/>
      <!-- moon glow -->
      <circle cx="200" cy="50" r="16" fill="rgba(200,180,255,0.12)"/>
      <!-- spider web top-right -->
      <line x1="360" x2="400" y1="0" y2="40" stroke="rgba(200,180,255,0.3)" stroke-width="0.8"/>
      <line x1="400" x2="360" y1="0" y2="40" stroke="rgba(200,180,255,0.3)" stroke-width="0.8"/>
      <line x1="380" x2="380" y1="0" y2="40" stroke="rgba(200,180,255,0.3)" stroke-width="0.8"/>
      <line x1="360" x2="400" y1="20" y2="20" stroke="rgba(200,180,255,0.3)" stroke-width="0.8"/>
      <circle cx="380" cy="40" r="4" fill="rgba(120,80,200,0.5)"/>
    `,
    space:`
      <rect width="400" height="220" fill="#030308"/>
      <!-- stars -->
      ${[...Array(28)].map((_,i)=>{
        const sx=(i*37+13)%400,sy=(i*23+7)%200;
        return`<circle cx="${sx}" cy="${sy}" r="${0.8+(i%3)*0.5}" fill="rgba(200,220,255,${0.4+(i%4)*0.15})"/>`;
      }).join('')}
      <!-- planet -->
      <circle cx="320" cy="55" r="28" fill="#1a2060" opacity=".7"/>
      <ellipse cx="320" cy="55" rx="40" ry="8" fill="none" stroke="rgba(100,160,255,0.4)" stroke-width="2"/>
      <!-- ship hull lines -->
      <rect x="0" y="160" width="400" height="60" fill="#080820"/>
      <line x1="0" x2="400" y1="160" y2="160" stroke="#1a3a6a" stroke-width="2"/>
      <rect x="80" y="130" width="40" height="30" fill="#0a0a20" rx="4" stroke="#1a3a6a" stroke-width="1.5"/>
      <rect x="280" y="130" width="40" height="30" fill="#0a0a20" rx="4" stroke="#1a3a6a" stroke-width="1.5"/>
      <!-- porthole -->
      <circle cx="200" cy="80" r="30" fill="#030318" stroke="#1a4a8a" stroke-width="3"/>
      <circle cx="200" cy="80" r="24" fill="rgba(10,30,80,0.8)"/>
    `,
    pirate:`
      <rect width="400" height="220" fill="#1a0e00"/>
      <!-- sky -->
      <rect width="400" height="140" fill="#2a1800"/>
      <!-- sun -->
      <circle cx="320" cy="40" r="22" fill="#d4870a" opacity=".8"/>
      <!-- sea -->
      <rect x="0" y="140" width="400" height="80" fill="#1a3a50" rx="0"/>
      <ellipse cx="80" cy="148" rx="60" ry="6" fill="rgba(40,80,120,0.5)"/>
      <ellipse cx="280" cy="155" rx="80" ry="5" fill="rgba(40,80,120,0.5)"/>
      <!-- beach -->
      <rect x="0" y="155" width="240" height="65" fill="#4a3010"/>
      <!-- ship far -->
      <rect x="310" y="105" width="70" height="40" fill="#3a1a00" rx="4"/>
      <line x1="345" x2="345" y1="70" y2="105" stroke="#5a3000" stroke-width="2"/>
      <polygon points="345,70 370,88 345,88" fill="#8b0000" opacity=".8"/>
      <!-- palm near -->
      <line x1="60" x2="65" y1="155" y2="80" stroke="#3a2000" stroke-width="5"/>
      <ellipse cx="65" cy="80" rx="28" ry="14" fill="#1a6a00" opacity=".9"/>
    `,
    lab:`
      <rect width="400" height="220" fill="#000e00"/>
      <!-- grid lines -->
      ${[...Array(8)].map((_,i)=>`<line x1="${i*55}" x2="${i*55}" y1="0" y2="220" stroke="rgba(0,100,0,0.12)" stroke-width="1"/>`).join('')}
      ${[...Array(5)].map((_,i)=>`<line x1="0" x2="400" y1="${i*50}" y2="${i*50}" stroke="rgba(0,100,0,0.12)" stroke-width="1"/>`).join('')}
      <!-- lab bench near -->
      <rect x="0" y="160" width="160" height="20" fill="#001a00" rx="3" stroke="#004400" stroke-width="1.5"/>
      <!-- lab bench far -->
      <rect x="240" y="160" width="160" height="20" fill="#001a00" rx="3" stroke="#004400" stroke-width="1.5"/>
      <!-- monitor -->
      <rect x="170" y="90" width="60" height="50" fill="#001200" rx="6" stroke="#006600" stroke-width="2"/>
      <rect x="175" y="95" width="50" height="38" fill="#002200" rx="3"/>
      <text x="200" y="118" text-anchor="middle" font-size="10" fill="#00cc44" font-family="monospace">LAB-SYS</text>
      <!-- bubbling flask near -->
      <ellipse cx="70" cy="155" rx="16" ry="8" fill="#001800" stroke="#006600" stroke-width="1.5"/>
      <rect x="62" y="130" width="16" height="25" fill="#001800" stroke="#006600" stroke-width="1"/>
      <!-- glowing flask -->
      <ellipse cx="70" cy="155" rx="14" ry="6" fill="rgba(0,200,50,0.18)"/>
      <!-- far shelf -->
      <rect x="320" y="50" width="70" height="110" fill="#001200" rx="4" stroke="#004400" stroke-width="1.5"/>
      <line x1="320" x2="390" y1="80" y2="80" stroke="#004400" stroke-width="1"/>
      <line x1="320" x2="390" y1="110" y2="110" stroke="#004400" stroke-width="1"/>
      <line x1="320" x2="390" y1="140" y2="140" stroke="#004400" stroke-width="1"/>
    `
  };
  return themes[cls]||themes.lab;
}

// ─── QUESTION MODAL ────────────────────────────────────────
function openQuestion(){
  const rooms=getCurrentRooms();
  const room=rooms[qIdx];
  const total=rooms.length;
  document.getElementById('qm-num').textContent=`Question ${qIdx+1} of ${total} · Level ${level}`;
  document.getElementById('qm-text').textContent=room.q;
  document.getElementById('qm-feedback').style.display='none';
  document.getElementById('qm-next-row').style.display='none';
  document.getElementById('qm-opts').innerHTML=room.opts.map((o,i)=>
    `<button class="opt-btn" onclick="answerQ(${i})">${o}</button>`
  ).join('');
  document.getElementById('q-overlay').classList.add('active');
}

function answerQ(i){
  const rooms=getCurrentRooms();
  const room=rooms[qIdx];
  document.querySelectorAll('#qm-opts .opt-btn').forEach(b=>b.disabled=true);
  const fb=document.getElementById('qm-feedback');
  if(i===room.ans){
    document.querySelectorAll('#qm-opts .opt-btn')[i].classList.add('correct');
    fb.className='feedback ok';fb.textContent='✅ Correct! '+room.exp;fb.style.display='block';
    collected.push(room.obj.label);
    const btn=document.getElementById('qm-next-btn');
    const total=rooms.length;
    if(qIdx+1>=total){
      btn.textContent=level<3?'Unlock Level '+(level+1)+' 🔓':'Go to Final Code 🔐';
    } else {
      btn.textContent='Back to room →';
    }
    btn.onclick=closeAndNext;
    document.getElementById('qm-next-row').style.display='flex';
  } else {
    document.querySelectorAll('#qm-opts .opt-btn')[i].classList.add('wrong');
    fb.className='feedback err';fb.textContent='❌ Not quite. '+room.exp+' Try again!';fb.style.display='block';
    setTimeout(()=>{
      document.querySelectorAll('#qm-opts .opt-btn').forEach(b=>{b.disabled=false;b.classList.remove('wrong','correct')});
      fb.style.display='none';
    },2200);
  }
}

function closeAndNext(){
  document.getElementById('q-overlay').classList.remove('active');
  const rooms=getCurrentRooms();
  if(qIdx+1>=rooms.length){
    // level complete
    if(level<3){
      document.getElementById('ul-icon').textContent='🔓';
      document.getElementById('ul-title').textContent='Level '+(level+1)+' Unlocked!';
      document.getElementById('ul-msg').textContent=['Great work! Now try completing sentences.','Amazing! Read each situation carefully for Level 3.'][level-1];
      const btn=document.getElementById('ul-btn');
      btn.textContent='Enter Level '+(level+1)+' →';
      btn.onclick=function(){level++;qIdx=0;loadLevel();show('s-game')};
      show('s-unlock');
    } else {
      // go to final
      codeDigits=["?","?","?","?"];finalQIdx=0;
      updateCodeDisplay();loadFinalQuestion();show('s-final');
    }
  } else {
    qIdx++;
    renderItems();
    renderRoom();
  }
}

// ─── FINAL CODE ────────────────────────────────────────────
function updateCodeDisplay(){
  document.getElementById('f-code-display').innerHTML=codeDigits.map((c,i)=>
    `<div class="code-digit${c!=='?'?' revealed':''}">${c}</div>`
  ).join('');
}

function loadFinalQuestion(){
  const T=THEMES[theme];const q=T.final[finalQIdx];
  document.getElementById('f-question').textContent=q.q;
  document.getElementById('f-feedback').style.display='none';
  document.getElementById('f-next-row').style.display='none';
  document.getElementById('f-opts').innerHTML=q.opts.map((o,i)=>
    `<button class="opt-btn" onclick="answerFinal(${i})">${o}</button>`
  ).join('');
}

function answerFinal(i){
  const T=THEMES[theme];const q=T.final[finalQIdx];
  document.querySelectorAll('#f-opts .opt-btn').forEach(b=>b.disabled=true);
  const fb=document.getElementById('f-feedback');
  if(i===q.ans){
    document.querySelectorAll('#f-opts .opt-btn')[i].classList.add('correct');
    codeDigits[finalQIdx]=q.digit;updateCodeDisplay();
    fb.className='feedback ok';fb.textContent='✅ '+q.exp;fb.style.display='block';
    const btn=document.getElementById('f-next-btn');
    if(finalQIdx+1>=T.final.length){
      btn.textContent='🔐 Escape now!';btn.onclick=showEscape;
    } else {
      btn.textContent='Next →';btn.onclick=()=>{finalQIdx++;loadFinalQuestion()};
    }
    document.getElementById('f-next-row').style.display='flex';
  } else {
    document.querySelectorAll('#f-opts .opt-btn')[i].classList.add('wrong');
    fb.className='feedback err';fb.textContent='❌ '+q.exp+' Try again!';fb.style.display='block';
    setTimeout(()=>{
      document.querySelectorAll('#f-opts .opt-btn').forEach(b=>{b.disabled=false;b.classList.remove('wrong','correct')});
      fb.style.display='none';
    },2200);
  }
}

function showEscape(){show('s-trophy');}

// ─── PRINT CERT ────────────────────────────────────────────
function printCert(){
  // Save current theme screens
  const allScreens=document.querySelectorAll('.screen');
  allScreens.forEach(s=>s.classList.remove('active'));
  document.getElementById('s-cert').classList.add('active');
  // Force white background for print
  const prevBg=document.body.style.background;
  document.body.style.background='#fff';
  window.print();
  document.body.style.background=prevBg;
  // Restore
  allScreens.forEach(s=>s.classList.remove('active'));
  document.getElementById('s-cert').classList.add('active');
}

// Close overlay on outside click
document.getElementById('q-overlay').addEventListener('click',function(e){
  if(e.target===this) this.classList.remove('active');
});
</script>
</body>
</html>
