<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NOVA — AI Command Center</title>
<style>
:root{
  --bg:#080610;--panel:#100b1c;--panel2:#171027;--line:rgba(177,120,255,.18);
  --purple:#a855f7;--purple2:#7c3aed;--pink:#d946ef;--text:#f7f2ff;
  --muted:#a79bb8;--good:#48e0a4;--bad:#ff718d;
}
*{box-sizing:border-box}
body{margin:0;background:radial-gradient(ellipse at 50% -20%,#281044 0%,#10091b 38%,var(--bg) 75%);color:var(--text);font-family:Inter,Segoe UI,Arial,sans-serif;min-height:100vh}
button,textarea{font:inherit}
.app{display:grid;grid-template-columns:250px minmax(0,1fr);min-height:100vh}
.sidebar{background:rgba(12,8,21,.88);border-right:1px solid var(--line);padding:22px 16px;display:flex;flex-direction:column;gap:24px}
.brand{display:flex;align-items:center;gap:12px;padding:2px 8px}
.logo{width:42px;height:42px;border-radius:14px;background:linear-gradient(135deg,#c084fc,#7c3aed 60%,#4c1d95);display:grid;place-items:center;box-shadow:0 0 28px #9333ea66;font-weight:900;font-size:20px}
.brand-name{font-size:21px;font-weight:800;letter-spacing:3px}
.brand-sub{font-size:9px;color:#b99bd8;letter-spacing:2px;margin-top:3px}
.new-chat{border:1px solid #a855f766;background:linear-gradient(110deg,#7c3aed,#9333ea);color:white;border-radius:12px;padding:13px 14px;text-align:left;font-weight:700;cursor:pointer;box-shadow:0 8px 28px #7c3aed33}
.nav-label{font-size:10px;letter-spacing:2px;color:#7f718f;padding:0 10px;margin-bottom:-12px}
.nav{display:grid;gap:7px}
.nav button{background:transparent;border:1px solid transparent;color:#bcb0ca;padding:11px 12px;border-radius:10px;text-align:left;cursor:pointer}
.nav button:hover,.nav button.active{background:#241638;border-color:#8b5cf633;color:white}
.nav button span{display:inline-block;width:25px;color:#c084fc}
.sidebar-bottom{margin-top:auto;border:1px solid var(--line);border-radius:14px;padding:14px;background:#130d20}
.status-line{display:flex;align-items:center;gap:8px;font-size:12px;color:#d9cce8}
.dot{width:8px;height:8px;border-radius:50%;background:var(--good);box-shadow:0 0 10px var(--good)}
.status-detail{font-size:11px;color:#8f829f;margin:8px 0 0 16px}
main{padding:26px clamp(18px,4vw,54px) 30px;max-width:1500px;width:100%;margin:0 auto}
.topbar{display:flex;align-items:center;justify-content:space-between;gap:16px;margin-bottom:34px}
.eyebrow{font-size:10px;color:#bd8aff;letter-spacing:2.5px;text-transform:uppercase}
.top-title{font-size:14px;color:#cfc2dc;margin-top:6px}
.avatar{width:38px;height:38px;border-radius:50%;display:grid;place-items:center;background:#28153e;border:1px solid #a855f766;color:#e9d5ff;font-weight:800}
.hero{display:flex;justify-content:space-between;align-items:end;gap:20px;margin-bottom:25px}
h1{font-size:clamp(29px,4vw,44px);line-height:1.08;margin:9px 0 10px;letter-spacing:-1.5px}
.gradient{background:linear-gradient(90deg,#fff,#d8b4fe 48%,#a855f7);-webkit-background-clip:text;background-clip:text;color:transparent}
.subtitle{color:var(--muted);font-size:14px;line-height:1.6}
.pill{border:1px solid #a855f744;background:#1c112b;color:#d9b8ff;border-radius:99px;padding:9px 13px;font-size:11px;white-space:nowrap}
.grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:14px;margin:22px 0 27px}
.tool-card{border:1px solid var(--line);background:linear-gradient(145deg,#171027,#100b19);border-radius:16px;padding:17px;min-height:130px;position:relative;overflow:hidden}
.tool-card:after{content:"";position:absolute;width:110px;height:110px;border-radius:50%;background:#9333ea12;right:-40px;top:-45px;filter:blur(4px)}
.tool-icon{width:35px;height:35px;border-radius:11px;background:#382052;color:#d8b4fe;display:grid;place-items:center;font-size:17px;margin-bottom:14px}
.tool-card h3{margin:0 0 5px;font-size:14px}
.tool-card p{margin:0;color:#9688a7;font-size:11px;line-height:1.5}
.tool-card small{display:inline-block;color:#bb91e9;font-size:9px;letter-spacing:1px;margin-top:12px}
.section-head{display:flex;justify-content:space-between;align-items:center;margin:24px 0 12px}
.section-head h2{font-size:15px;margin:0}
.section-head span{font-size:10px;color:#93849f;letter-spacing:1px}
.chat-shell{border:1px solid #9d5cf344;border-radius:18px;background:rgba(15,10,24,.88);box-shadow:0 15px 55px #0005,0 0 35px #7c3aed0c;overflow:hidden}
.chat-head{padding:15px 18px;border-bottom:1px solid var(--line);display:flex;align-items:center;justify-content:space-between}
.chat-head-left{display:flex;align-items:center;gap:10px;font-size:13px;font-weight:700}
.mini-logo{width:28px;height:28px;border-radius:9px;background:linear-gradient(135deg,#c084fc,#6d28d9);display:grid;place-items:center;font-size:13px}
.model-tag{font-size:10px;color:#b69acb;border:1px solid var(--line);border-radius:99px;padding:6px 9px}
.messages{height:310px;overflow-y:auto;padding:20px;display:flex;flex-direction:column;gap:15px}
.message{display:flex;gap:10px;max-width:88%;align-items:flex-start}
.message.user{align-self:flex-end;flex-direction:row-reverse}
.msg-icon{width:27px;height:27px;flex:0 0 27px;border-radius:9px;background:#35204b;color:#e9d5ff;display:grid;place-items:center;font-size:11px;font-weight:800}
.message.user .msg-icon{background:#6d28d9}
.bubble{padding:11px 14px;border-radius:4px 14px 14px 14px;background:#1a1226;border:1px solid #a855f722;color:#e9e0f2;font-size:13px;line-height:1.6;white-space:pre-wrap;overflow-wrap:anywhere}
.message.user .bubble{background:#39205b;border-color:#a855f744;border-radius:14px 4px 14px 14px}
.composer{padding:14px 16px 16px;border-top:1px solid var(--line);background:#0e0917}
.composer-tools{display:flex;gap:8px;margin-bottom:10px;flex-wrap:wrap}
.tool-chip{border:1px solid #49305e;background:#1b1228;color:#c9b5dc;border-radius:8px;padding:6px 9px;font-size:10px;cursor:pointer}
.tool-chip.active{border-color:#a855f7;color:#e9d5ff;background:#32184b}
.input-row{display:flex;gap:10px;align-items:end}
textarea{resize:vertical;min-height:48px;max-height:130px;flex:1;background:#1a1225;border:1px solid #50346b;border-radius:12px;color:white;padding:14px;outline:none;font-size:13px}
textarea:focus{border-color:#a855f7;box-shadow:0 0 0 3px #a855f71a}
.send{width:48px;height:48px;border:0;border-radius:12px;background:linear-gradient(135deg,#a855f7,#6d28d9);color:white;font-size:19px;cursor:pointer;box-shadow:0 5px 20px #7c3aed55}
.send:disabled{opacity:.5;cursor:wait}
.hint{font-size:10px;color:#71647f;margin:9px 2px 0}
.mobile-menu{display:none;background:#1b1228;border:1px solid var(--line);color:white;border-radius:9px;padding:8px 10px}
@media(max-width:850px){.app{grid-template-columns:1fr}.sidebar{position:fixed;z-index:5;left:-270px;top:0;bottom:0;width:250px;transition:left .2s}.sidebar.open{left:0;box-shadow:20px 0 50px #0009}.mobile-menu{display:block}.topbar{margin-bottom:24px}.grid{grid-template-columns:1fr 1fr}}
@media(max-width:560px){main{padding:17px 13px}.hero{align-items:flex-start;flex-direction:column}.grid{grid-template-columns:1fr}.messages{height:350px;padding:14px}.message{max-width:96%}.model-tag{display:none}.topbar{gap:10px}}

/* NOVA MOTION UPGRADE */
body::before{
  content:"";position:fixed;inset:-30%;z-index:-2;pointer-events:none;
  background:radial-gradient(circle at 25% 30%,#7c3aed20,transparent 28%),
             radial-gradient(circle at 75% 65%,#d946ef12,transparent 25%),
             radial-gradient(circle at 50% 50%,#4c1d9515,transparent 40%);
  animation:nebulaDrift 18s ease-in-out infinite alternate;
}
body::after{
  content:"";position:fixed;inset:0;z-index:-1;pointer-events:none;opacity:.18;
  background-image:linear-gradient(#b78aff12 1px,transparent 1px),
                   linear-gradient(90deg,#b78aff12 1px,transparent 1px);
  background-size:48px 48px;
  mask-image:linear-gradient(to bottom,black,transparent 85%);
  animation:gridFloat 30s linear infinite;
}
@keyframes nebulaDrift{0%{transform:translate3d(-2%,0,0) scale(1)}100%{transform:translate3d(2%,2%,0) scale(1.08)}}
@keyframes gridFloat{from{background-position:0 0}to{background-position:48px 48px}}
@keyframes logoPulse{0%,100%{box-shadow:0 0 18px #9333ea55,0 0 0 0 #a855f700}50%{box-shadow:0 0 32px #a855f7aa,0 0 0 8px #a855f711}}
@keyframes softFloat{0%,100%{transform:translateY(0)}50%{transform:translateY(-5px)}}
@keyframes cardShine{0%{transform:translateX(-140%) skewX(-18deg)}100%{transform:translateX(240%) skewX(-18deg)}}
@keyframes messageIn{from{opacity:0;transform:translateY(10px) scale(.985)}to{opacity:1;transform:translateY(0) scale(1)}}
@keyframes statusPulse{0%,100%{box-shadow:0 0 5px var(--good)}50%{box-shadow:0 0 14px var(--good),0 0 22px #48e0a455}}
.logo{animation:logoPulse 3.4s ease-in-out infinite}
.hero .pill{animation:softFloat 5s ease-in-out infinite}
.tool-card{transition:transform .28s ease,border-color .28s ease,box-shadow .28s ease}
.tool-card::before{content:"";position:absolute;top:-30%;left:-45%;width:35%;height:160%;background:linear-gradient(90deg,transparent,#ffffff12,transparent);transform:translateX(-140%) skewX(-18deg);pointer-events:none}
.tool-card:hover{transform:translateY(-5px);border-color:#b76aff88;box-shadow:0 12px 35px #7c3aed20}
.tool-card:hover::before{animation:cardShine .9s ease}
.new-chat,.send{position:relative;overflow:hidden;transition:transform .2s ease,filter .2s ease,box-shadow .2s ease}
.new-chat:hover,.send:hover{transform:translateY(-2px);filter:brightness(1.12);box-shadow:0 8px 28px #9333ea66}
.message{animation:messageIn .28s ease both}
.dot{animation:statusPulse 2s ease-in-out infinite}
.chat-shell{transition:box-shadow .3s ease,border-color .3s ease}
.chat-shell:focus-within{border-color:#b76aff88;box-shadow:0 15px 55px #0005,0 0 32px #9333ea20}
button:focus-visible,textarea:focus-visible{outline:2px solid #c084fc;outline-offset:3px}
@media(prefers-reduced-motion:reduce){
  *,*::before,*::after{animation-duration:.01ms!important;animation-iteration-count:1!important;scroll-behavior:auto!important;transition-duration:.01ms!important}
}


/* HOLOGRAPHIC NOVA CORE */
.hero{position:relative}
.hero-orb-wrap{width:190px;height:190px;flex:0 0 190px;position:relative;display:grid;place-items:center;margin:0 24px 0 0}
.nova-orb{width:116px;height:116px;border-radius:50%;position:relative;isolation:isolate;
  background:radial-gradient(circle at 35% 28%,#fff 0%,#e9d5ff 5%,#c084fc 14%,#9333ea 34%,#4c1d95 62%,#160922 78%);
  box-shadow:0 0 18px #c084fcaa,0 0 42px #9333ea88,0 0 85px #7c3aed55,inset -12px -12px 24px #090411;
  animation:orbFloat 4s ease-in-out infinite,orbGlow 3s ease-in-out infinite}
.nova-orb:before{content:"";position:absolute;inset:-10px;border-radius:50%;border:1px solid #d8b4fe88;
  box-shadow:0 0 18px #a855f766,inset 0 0 16px #a855f733;animation:orbSpin 9s linear infinite}
.nova-orb:after{content:"";position:absolute;inset:14px;border-radius:50%;
  background:radial-gradient(circle at 30% 25%,#ffffffaa,transparent 18%),radial-gradient(circle at 60% 70%,#d8b4fe44,transparent 45%);
  filter:blur(2px);mix-blend-mode:screen}
.orb-ring{position:absolute;width:164px;height:64px;border:1px solid #c084fc99;border-radius:50%;
  transform:rotate(-28deg);box-shadow:0 0 15px #9333ea55;animation:orbRing 7s linear infinite}
.orb-ring.ring-two{width:174px;height:78px;transform:rotate(58deg);border-color:#e9d5ff66;animation-duration:11s;animation-direction:reverse}
.orb-ring.ring-three{width:142px;height:142px;border-style:dashed;border-color:#a855f755;animation-duration:24s}
.orb-core-label{position:absolute;bottom:-8px;left:50%;transform:translateX(-50%);white-space:nowrap;
  color:#d8b4fe;font-size:9px;letter-spacing:2px;text-shadow:0 0 10px #a855f7}
.orb-spark{position:absolute;width:5px;height:5px;border-radius:50%;background:#fff;box-shadow:0 0 12px 3px #c084fc;top:22px;right:28px;animation:sparkBlink 1.8s ease-in-out infinite alternate}
@keyframes orbFloat{0%,100%{transform:translateY(0) scale(1)}50%{transform:translateY(-9px) scale(1.025)}}
@keyframes orbGlow{0%,100%{filter:saturate(1);box-shadow:0 0 18px #c084fc88,0 0 42px #9333ea66,0 0 75px #7c3aed44,inset -12px -12px 24px #090411}50%{filter:saturate(1.35);box-shadow:0 0 26px #e9d5ffcc,0 0 58px #a855f7aa,0 0 100px #7c3aed77,inset -12px -12px 24px #090411}}
@keyframes orbSpin{to{transform:rotate(360deg)}}
@keyframes orbRing{to{transform:rotate(332deg)}}
@keyframes sparkBlink{from{opacity:.25;transform:scale(.7)}to{opacity:1;transform:scale(1.4)}}
.hero-orb-wrap.thinking .nova-orb{animation:orbFloat 1s ease-in-out infinite,orbGlow .7s ease-in-out infinite}
.hero-orb-wrap.thinking .orb-ring{animation-duration:1.8s}
.hero-orb-wrap.thinking .orb-core-label{color:#fff;text-shadow:0 0 12px #fff,0 0 22px #a855f7}
@media(max-width:700px){.hero-orb-wrap{width:130px;height:130px;flex-basis:130px;margin:0 auto}.nova-orb{width:82px;height:82px}.orb-ring{width:120px;height:48px}.orb-ring.ring-two{width:125px;height:55px}.orb-ring.ring-three{width:108px;height:108px}}


/* NOVA MEMORY PANEL */
.memory-panel{display:none;position:fixed;inset:0;z-index:25;background:#05030bd9;backdrop-filter:blur(12px);align-items:center;justify-content:center;padding:20px}
.memory-panel.open{display:flex}
.memory-card{width:min(540px,100%);max-height:80vh;overflow:auto;border:1px solid #a855f766;border-radius:20px;padding:24px;background:radial-gradient(circle at 50% 0%,#35164f,#130c20 62%);box-shadow:0 25px 100px #000b;text-align:left}
.memory-card h2{margin:8px 0;font-size:23px}
.memory-card p{color:#aa9bb9;font-size:13px;line-height:1.6}
.memory-list{display:grid;gap:8px;margin:16px 0}
.memory-item{display:flex;align-items:flex-start;justify-content:space-between;gap:12px;padding:11px 12px;border:1px solid #ffffff18;background:#0c0714;border-radius:10px;color:#e9e0f2;font-size:12px;line-height:1.5}
.memory-item button{border:1px solid #ffffff22;background:#24142f;color:#e9d5ff;border-radius:7px;padding:4px 8px;cursor:pointer;flex:0 0 auto}
.memory-empty{padding:16px;border:1px dashed #ffffff25;border-radius:10px;color:#9688a7;font-size:12px;text-align:center}
.memory-footer{display:flex;justify-content:space-between;gap:10px;flex-wrap:wrap;margin-top:16px}
.memory-close{position:sticky;float:right;top:0;border:1px solid #ffffff33;background:#160e21;color:white;border-radius:50%;width:34px;height:34px;font-size:19px;cursor:pointer}
.memory-clear{border:1px solid #ff718d66;background:#321322;color:#ffdce4;border-radius:9px;padding:9px 12px;cursor:pointer}
.memory-done{border:1px solid #a855f766;background:#28143d;color:#f4eaff;border-radius:9px;padding:9px 14px;cursor:pointer}
/* VOICE ASSISTANT PANEL */
.voice-panel{display:none;position:fixed;inset:0;z-index:20;background:#05030bd9;backdrop-filter:blur(12px);align-items:center;justify-content:center;padding:20px}
.voice-panel.open{display:flex}
.voice-card{width:min(520px,100%);border:1px solid #a855f766;border-radius:22px;padding:25px;background:radial-gradient(circle at 50% 0%,#35164f,#130c20 62%);box-shadow:0 25px 100px #000b,0 0 45px #9333ea22;text-align:center}
.voice-card h2{margin:8px 0;font-size:24px}
.voice-card p{color:#aa9bb9;font-size:13px;line-height:1.6}
.voice-orb{width:94px;height:94px;margin:8px auto 18px;border-radius:50%;background:radial-gradient(circle at 35% 28%,#fff,#d8b4fe 12%,#9333ea 42%,#240b3c 76%);box-shadow:0 0 24px #c084fcaa,0 0 60px #9333ea77;animation:voiceBreathe 2.4s ease-in-out infinite}
.voice-orb.listening{animation:voiceListen .8s ease-in-out infinite alternate}
@keyframes voiceBreathe{50%{transform:scale(1.07);box-shadow:0 0 36px #e9d5ff,0 0 78px #9333ea}}
@keyframes voiceListen{to{transform:scale(1.15);filter:hue-rotate(25deg);box-shadow:0 0 48px #e9d5ff,0 0 95px #a855f7}}
.voice-actions{display:flex;justify-content:center;gap:10px;flex-wrap:wrap;margin:18px 0}
.voice-btn{border:1px solid #a855f766;background:#28143d;color:#f4eaff;border-radius:11px;padding:11px 16px;cursor:pointer}
.voice-btn.primary{background:linear-gradient(120deg,#9333ea,#6d28d9);border:0}
.voice-btn:disabled{opacity:.45;cursor:not-allowed}
.voice-transcript{min-height:42px;padding:11px;border:1px solid #ffffff16;background:#0c0714;border-radius:10px;color:#d9c9e8;font-size:12px;text-align:left;white-space:pre-wrap}
.voice-close{position:absolute;top:18px;right:18px;border:1px solid #ffffff33;background:#160e21;color:white;border-radius:50%;width:38px;height:38px;font-size:20px;cursor:pointer}
.hero-orb-wrap{cursor:pointer}
.hero-orb-wrap:focus-visible{outline:2px solid #d8b4fe;outline-offset:8px;border-radius:50%}
.voice-note{font-size:10px!important;color:#81738f!important}

</style>
</head>
<body>
<div class="app">
  <aside class="sidebar" id="sidebar">
    <div class="brand"><div class="logo">N</div><div><div class="brand-name">NOVA</div><div class="brand-sub">NEURAL AI SYSTEM</div></div></div>
    <button class="new-chat" id="newChat">＋ &nbsp; New conversation</button>
    <div class="nav-label">WORKSPACE</div>
    <nav class="nav">
      <button class="active" id="navDashboard"><span>◈</span> Dashboard</button>
      <button id="navChat"><span>⌘</span> AI Chat</button>
      <button id="navCoding"><span>⌁</span> Coding assistant</button>
      <button id="navGames"><span>◇</span> 3D game lab</button>
      <button id="navImages"><span>✧</span> Image studio</button>
    </nav>
    <div class="nav-label">SYSTEM</div>
    <nav class="nav">
      <button id="navSettings"><span>⚙</span> Settings</button>
    </nav>
    <div class="sidebar-bottom"><div class="status-line"><i class="dot" id="statusDot"></i><b id="statusText">Checking AI connection…</b></div><div class="status-detail" id="statusDetail">Local AI system</div></div>
  </aside>

  <main>
    <header class="topbar">
      <div style="display:flex;align-items:center;gap:12px">
        <button class="mobile-menu" id="mobileMenu">☰</button>
        <div><div class="eyebrow">NOVA / COMMAND CENTER</div><div class="top-title">Your personal intelligence workspace</div></div>
      </div>
      <div class="avatar">N</div>
    </header>

    <section class="hero">
      <div><div class="eyebrow">✦ SYSTEM ONLINE · READY WHEN YOU ARE</div><h1>Welcome back to <span class="gradient">NOVA.</span></h1><div class="subtitle">Your ideas. Your intelligence. One command center.<br>What would you like to create today?</div></div>
      <div class="hero-orb-wrap" id="novaOrb" role="button" tabindex="0" aria-label="Open NOVA voice assistant" title="Open voice assistant">
        <div class="orb-ring"></div><div class="orb-ring ring-two"></div><div class="orb-ring ring-three"></div>
        <div class="nova-orb"></div><div class="orb-spark"></div>
        <div class="orb-core-label" id="orbLabel">NOVA CORE · ONLINE</div>
      </div>
    </section>

    <div class="grid">
      <article class="tool-card"><div class="tool-icon">⌘</div><h3>Coding assistant</h3><p>Build, debug and understand code with NOVA.</p><small>OPEN CODING MODE ↗</small></article>
      <article class="tool-card"><div class="tool-icon">◇</div><h3>3D game lab</h3><p>Turn game ideas into playable prototypes.</p><small>OPEN GAME MODE ↗</small></article>
      <article class="tool-card"><div class="tool-icon">✧</div><h3>Image studio</h3><p>Creative image tools. Generation setup coming next.</p><small>COMING SOON</small></article>
    </div>

    <div class="section-head"><h2>AI workspace</h2><span>SECURE LOCAL SESSION</span></div>
    <section class="chat-shell" id="chatSection">
      <div class="chat-head"><div class="chat-head-left"><div class="mini-logo">N</div><div>NOVA Assistant</div></div><div class="model-tag">QWEN 2.5 · 3B</div></div>
      <div class="messages" id="messages">
        <div class="message"><div class="msg-icon">N</div><div class="bubble">Hello! I'm NOVA, your personal AI assistant. What are we building today?</div></div>
      </div>
      <div class="composer">
        <div class="composer-tools">
          <button class="tool-chip active" data-mode="chat">✦ General</button>
          <button class="tool-chip" data-mode="coding">⌘ Coding</button>
          <button class="tool-chip" data-mode="game">◇ 3D Games</button>
        </div>
        <div class="input-row"><textarea id="prompt" rows="1" placeholder="Message NOVA… (Enter to send, Shift + Enter for new line)"></textarea><button class="send" id="send" title="Send message">➤</button></div>
        <div class="hint">NOVA runs on your local Ollama AI. Responses may take a moment.</div>
      </div>
    </section>
  </main>
</div>

<div class="voice-panel" id="voicePanel" role="dialog" aria-modal="true" aria-labelledby="voiceTitle">
  <button class="voice-close" id="voiceClose" aria-label="Close voice assistant">×</button>
  <div class="voice-card">
    <div class="eyebrow">NOVA / VOICE INTERFACE</div>
    <div class="voice-orb" id="voiceOrb"></div>
    <h2 id="voiceTitle">Talk to NOVA</h2>
    <p id="voiceStatus">Start a hands-free conversation. NOVA listens, answers aloud, then listens again.</p>
    <div class="voice-transcript" id="voiceTranscript">Your speech transcript will appear here.</div>
    <div class="voice-actions">
      <button class="voice-btn primary" id="voiceStart">🎙 Start live conversation</button>
      <button class="voice-btn" id="voiceStop" disabled>Stop conversation</button>
      <button class="voice-btn" id="voiceSpeak" disabled>🔊 Speak last reply</button>
    </div>
    <p class="voice-note">Hands-free voice uses Chrome speech recognition and your device's available speech voice. It is inspired by live AI voice chats, not Google's actual voice service.</p>
  </div>
</div>

<script>
const $ = id => document.getElementById(id);
const messagesEl = $("messages"), promptEl = $("prompt"), sendBtn = $("send");
const CHAT_KEY = "nova_chat_history_v1";
const CHAT_ARCHIVE_KEY = "nova_chat_archive_v1";
function loadChatArchives() {
  try {
    const saved = JSON.parse(localStorage.getItem(CHAT_ARCHIVE_KEY) || "[]");
    return Array.isArray(saved) ? saved.filter(x => x && Array.isArray(x.messages)).slice(-10) : [];
  } catch { return []; }
}
let chatArchives = loadChatArchives();
function saveChatArchives() {
  try { localStorage.setItem(CHAT_ARCHIVE_KEY, JSON.stringify(chatArchives.slice(-10))); }
  catch (error) { console.warn("NOVA could not save archived chats:", error); }
}
function loadChatHistory() {
  try {
    const saved = JSON.parse(localStorage.getItem(CHAT_KEY) || "[]");
    return Array.isArray(saved)
      ? saved.filter(m => m && (m.role === "user" || m.role === "assistant") && typeof m.content === "string").slice(-300)
      : [];
  } catch { return []; }
}
let history = loadChatHistory(), mode = "chat", busy = false, lastAssistantReply = "";
let liveVoice = false;
function saveChatHistory() {
  try { localStorage.setItem(CHAT_KEY, JSON.stringify(history.slice(-300))); }
  catch (error) { console.warn("NOVA could not save chat history:", error); }
}
const MEMORY_KEY = "nova_personal_memories_v1";

function loadMemories() {
  try {
    const saved = JSON.parse(localStorage.getItem(MEMORY_KEY) || "[]");
    return Array.isArray(saved) ? saved.filter(x => typeof x === "string") : [];
  } catch { return []; }
}
let memories = loadMemories();

function saveMemories() {
  try { localStorage.setItem(MEMORY_KEY, JSON.stringify(memories)); }
  catch (error) { console.warn("NOVA could not save memories:", error); }
}

function handleMemoryCommand(text) {
  const remember = text.match(/^\\s*(?:please\\s+)?remember that\\s+(.+)\\s*$/i);
  if (remember) {
    const fact = remember[1].trim().replace(/[.!?]+$/, "");
    if (fact && !memories.some(m => m.toLowerCase() === fact.toLowerCase())) {
      memories.push(fact);
      saveMemories();
    }
    return "Got it — I'll remember: " + fact;
  }

  if (/^\\s*(?:what do you remember about me|show my memories|view memories)\\s*[?!.]*\\s*$/i.test(text)) {
    return memories.length
      ? "Here are the things I remember:\\n" + memories.map((m, i) => (i + 1) + ". " + m).join("\\n")
      : "I don't have any saved memories yet. Tell me “Remember that…” followed by something you'd like me to keep in mind.";
  }

  if (/^\\s*(?:forget everything|forget all memories|clear all memories)\\s*[.!]*\\s*$/i.test(text)) {
    memories = [];
    saveMemories();
    return "I've cleared NOVA's saved memories in this browser.";
  }

  const forget = text.match(/^\\s*forget that\\s+(.+)\\s*$/i);
  if (forget) {
    const target = forget[1].trim().replace(/[.!?]+$/, "").toLowerCase();
    const before = memories.length;
    memories = memories.filter(m => !m.toLowerCase().includes(target));
    saveMemories();
    return memories.length < before ? "Okay — I removed the matching memory." : "I couldn't find a saved memory matching that.";
  }
  return null;
}

// Speak NOVA's replies automatically, using the same browser voice
// and settings as the existing "Speak last reply" button.
function speakReply(text, onFinished) {
  if (!text || !("speechSynthesis" in window)) {
    if (typeof onFinished === "function") onFinished();
    return;
  }
  window.speechSynthesis.cancel();
  const utterance = new SpeechSynthesisUtterance(text);
  utterance.lang = navigator.language || "en-IN";
  const availableVoices = window.speechSynthesis.getVoices();
  const preferredVoice = availableVoices.find(v => /google/i.test(v.name) && /^en(-IN|-US)?$/i.test(v.lang))
    || availableVoices.find(v => /^en-IN$/i.test(v.lang))
    || availableVoices.find(v => /^en/i.test(v.lang));
  if (preferredVoice) utterance.voice = preferredVoice;
  utterance.rate = 1;
  utterance.pitch = 1;
  utterance.onend = () => { if (typeof onFinished === "function") onFinished(); };
  utterance.onerror = () => { if (typeof onFinished === "function") onFinished(); };
  window.speechSynthesis.speak(utterance);
}

function addMessage(role, text) {
  const wrap = document.createElement("div");
  wrap.className = "message " + (role === "user" ? "user" : "");
  const icon = document.createElement("div");
  icon.className = "msg-icon";
  icon.textContent = role === "user" ? "Y" : "N";
  const bubble = document.createElement("div");
  bubble.className = "bubble";
  bubble.textContent = text;
  wrap.append(icon, bubble);
  messagesEl.appendChild(wrap);
  messagesEl.scrollTop = messagesEl.scrollHeight;
  return bubble;
}
function restoreChatHistory() {
  if (history.length) {
    messagesEl.innerHTML = "";
    history.forEach(message => addMessage(message.role, message.content));
    const last = [...history].reverse().find(message => message.role === "assistant");
    if (last) {
      lastAssistantReply = last.content;
      $("voiceSpeak").disabled = false;
    }
  }
}
restoreChatHistory();

function setMode(nextMode) {
  mode = nextMode;
  document.querySelectorAll(".tool-chip").forEach(b => b.classList.toggle("active", b.dataset.mode === mode));
  const names = {chat:"Message NOVA…",coding:"Ask NOVA to write or debug code…",game:"Describe the 3D game you want to create…"};
  promptEl.placeholder = names[mode];
}
async function sendMessage() {
  const text = promptEl.value.trim();
  if (!text || busy) return;
  promptEl.value = "";
  addMessage("user", text);
  history.push({role:"user", content:text});
  saveChatHistory();

  const memoryReply = handleMemoryCommand(text);
  if (memoryReply) {
    addMessage("assistant", memoryReply);
    history.push({role:"assistant", content:memoryReply});
    saveChatHistory();
    lastAssistantReply = memoryReply;
    $("voiceSpeak").disabled = false;
    speakReply(memoryReply, () => {
      if (liveVoice) startLiveListening();
    });
    promptEl.focus();
    return;
  }

  busy = true; sendBtn.disabled = true; $("novaOrb").classList.add("thinking"); $("orbLabel").textContent = "NOVA CORE · THINKING";
  const replyBubble = addMessage("assistant", "NOVA is thinking…");
  try {
    const response = await fetch("/api/chat", {
      method:"POST",
      headers:{"Content-Type":"application/json"},
      body:JSON.stringify({
        messages: [
          {
            role:"system",
            content:
              "You are NOVA, a friendly and capable personal AI assistant. Use the saved personal details and recent conversation history to maintain continuity. Do not claim to know anything that is not present in the supplied context. " +
              (memories.length ? "Saved personal details:\\n- " + memories.join("\\n- ") : "No separate personal details have been saved yet.") +
              (chatArchives.length
                ? "\\n\\nEarlier conversations (use these when relevant):\\n" +
                  chatArchives.slice(-3).map((session, index) =>
                    "Earlier chat " + (index + 1) + ":\\n" +
                    session.messages.slice(-20).map(m => m.role + ": " + m.content).join("\\n")
                  ).join("\\n\\n")
                : "")
          },
          ...history.slice(-30)
        ],
        mode, webSearch:false
      })
    });
    const data = await response.json();
    if (!response.ok) throw new Error(data.error || "Request failed.");
    const reply = data.reply || "NOVA couldn't create a response. Please try again.";
    replyBubble.textContent = reply;
    lastAssistantReply = reply;
    $("voiceSpeak").disabled = false;
    history.push({role:"assistant", content:reply});
    saveChatHistory();
    speakReply(reply, () => {
      if (liveVoice) startLiveListening();
    });
  } catch (error) {
    replyBubble.textContent = "Connection error: " + error.message + "\n\nMake sure the NOVA server and Ollama are running.";
    history.pop();
    saveChatHistory();
  } finally {
    busy = false; sendBtn.disabled = false; $("novaOrb").classList.remove("thinking"); $("orbLabel").textContent = "NOVA CORE · ONLINE"; promptEl.focus();
  }
}
sendBtn.addEventListener("click", sendMessage);
promptEl.addEventListener("keydown", e => { if(e.key === "Enter" && !e.shiftKey){e.preventDefault();sendMessage();} });
document.querySelectorAll(".tool-chip").forEach(b => b.addEventListener("click", () => setMode(b.dataset.mode)));
$("newChat").addEventListener("click", () => {
  if (history.length && !confirm("Start a new conversation? NOVA will archive this chat so it can refer to it later.")) return;
  if (history.length) {
    chatArchives.push({savedAt:new Date().toISOString(), messages:history.slice(-200)});
    chatArchives = chatArchives.slice(-10);
    saveChatArchives();
  }
  history = [];
  saveChatHistory();
  messagesEl.innerHTML = "";
  addMessage("assistant", "A fresh session is ready. What would you like to explore?");
  setMode("chat"); $("sidebar").classList.remove("open");
});
$("mobileMenu").addEventListener("click", () => $("sidebar").classList.toggle("open"));
$("navDashboard").addEventListener("click", () => $("sidebar").classList.remove("open"));
$("navChat").addEventListener("click", () => { $("chatSection").scrollIntoView({behavior:"smooth"}); $("sidebar").classList.remove("open"); promptEl.focus(); });
$("navCoding").addEventListener("click", () => { setMode("coding"); $("chatSection").scrollIntoView({behavior:"smooth"}); $("sidebar").classList.remove("open"); promptEl.focus(); });
$("navGames").addEventListener("click", () => { setMode("game"); $("chatSection").scrollIntoView({behavior:"smooth"}); $("sidebar").classList.remove("open"); promptEl.focus(); });
$("navImages").addEventListener("click", () => alert("Image generation is not configured in the current server yet. We'll add it in a later step."));
$("navSettings").addEventListener("click", () => alert("NOVA settings will be added in a future update."));
async function checkHealth(){
  try{
    const r = await fetch("/api/health");
    if(!r.ok) throw new Error("Offline");
    const d = await r.json();
    $("statusText").textContent = d.ok ? "AI system ready" : "AI system offline";
    $("statusDetail").textContent = d.provider || "Local AI system";
    $("statusDot").style.background = d.ok ? "var(--good)" : "var(--bad)";
  }catch{
    $("statusText").textContent = "Server unavailable";
    $("statusDetail").textContent = "Start NOVA server to connect";
    $("statusDot").style.background = "var(--bad)";
  }
}
checkHealth();

// Decorative ambient stars; purely visual and independent of the AI backend.
(function(){
  const field=document.createElement("div");
  field.setAttribute("aria-hidden","true");
  Object.assign(field.style,{position:"fixed",inset:"0",pointerEvents:"none",zIndex:"0",overflow:"hidden"});
  for(let i=0;i<34;i++){
    const star=document.createElement("i");
    const size=(Math.random()*2+1).toFixed(1)+"px";
    Object.assign(star.style,{
      position:"absolute",left:(Math.random()*100)+"%",top:(Math.random()*100)+"%",
      width:size,height:size,borderRadius:"50%",background:"#d8b4fe",
      opacity:(Math.random()*.42+.12).toFixed(2),
      boxShadow:"0 0 8px #a855f7",
      animation:`starBlink ${(Math.random()*3+2).toFixed(1)}s ease-in-out ${(-Math.random()*4).toFixed(1)}s infinite alternate`
    });
    field.appendChild(star);
  }
  document.body.prepend(field);
  const style=document.createElement("style");
  style.textContent="@keyframes starBlink{from{opacity:.12;transform:scale(.7)}to{opacity:.75;transform:scale(1.35)}}";
  document.head.appendChild(style);
})();


// Hands-free NOVA voice conversation: listen -> ask the existing AI -> speak -> listen again.
(function(){
  const panel=$("voicePanel"), orb=$("novaOrb"), voiceOrb=$("voiceOrb");
  const status=$("voiceStatus"), transcript=$("voiceTranscript");
  const SpeechRecognition=window.SpeechRecognition||window.webkitSpeechRecognition;
  let recognition=null, listening=false, restarting=false;

  function updateVoiceButtons(){
    $("voiceStart").disabled = liveVoice || !SpeechRecognition;
    $("voiceStop").disabled = !liveVoice;
  }
  function openVoice(){
    panel.classList.add("open");
    status.textContent=SpeechRecognition
      ? "Press Start live conversation. Speak naturally; NOVA will answer and listen again."
      : "Speech recognition is not supported in this browser. Try the latest Google Chrome.";
    updateVoiceButtons();
  }
  function stopLiveVoice(){
    liveVoice=false; restarting=false;
    if(recognition && listening){try{recognition.stop()}catch(e){}}
    if("speechSynthesis" in window) window.speechSynthesis.cancel();
    listening=false; voiceOrb.classList.remove("listening");
    status.textContent="Live conversation stopped.";
    updateVoiceButtons();
  }
  function closeVoice(){
    stopLiveVoice();
    panel.classList.remove("open");
  }
  function startLiveListening(){
    if(!liveVoice || !panel.classList.contains("open") || busy || listening || restarting) return;
    if(!SpeechRecognition){
      status.textContent="Speech recognition is unavailable. Use Google Chrome and allow microphone access.";
      liveVoice=false; updateVoiceButtons(); return;
    }
    restarting=true;
    recognition=new SpeechRecognition();
    recognition.lang=navigator.language||"en-IN";
    recognition.interimResults=true;
    recognition.continuous=false;
    let finalTranscript="";

    recognition.onstart=()=>{
      restarting=false; listening=true;
      $("voiceStart").disabled=true; $("voiceStop").disabled=false;
      voiceOrb.classList.add("listening");
      status.textContent="Listening… speak naturally.";
      transcript.textContent="I'm listening…";
    };
    recognition.onresult=event=>{
      let interim="";
      for(let i=event.resultIndex;i<event.results.length;i++){
        const part=event.results[i][0].transcript;
        if(event.results[i].isFinal) finalTranscript+=part;
        else interim+=part;
      }
      transcript.textContent=finalTranscript||interim||"Listening…";
    };
    recognition.onerror=event=>{
      restarting=false;
      if(event.error==="not-allowed" || event.error==="service-not-allowed"){
        status.textContent="Microphone permission was blocked. Allow microphone access in Chrome site settings.";
        liveVoice=false; updateVoiceButtons();
      } else if(event.error!=="no-speech" && liveVoice){
        status.textContent="Voice recognition issue: "+event.error+". Trying again…";
      }
    };
    recognition.onend=()=>{
      listening=false; voiceOrb.classList.remove("listening");
      if(!liveVoice){updateVoiceButtons();return;}
      if(finalTranscript.trim()){
        const spoken=finalTranscript.trim();
        transcript.textContent="You: "+spoken;
        promptEl.value=spoken;
        status.textContent="NOVA is thinking…";
        sendMessage();
      } else {
        status.textContent="I didn't catch that. Listening again…";
        setTimeout(startLiveListening,700);
      }
    };
    try{recognition.start();}
    catch(error){restarting=false;status.textContent="Could not start the microphone. Please try again.";}
  }

  if(orb){
    orb.addEventListener("click",openVoice);
    orb.addEventListener("keydown",e=>{
      if(e.key==="Enter"||e.key===" "){e.preventDefault();openVoice();}
    });
  }
  $("voiceClose").addEventListener("click",closeVoice);
  panel.addEventListener("click",e=>{if(e.target===panel)closeVoice();});
  $("voiceStart").addEventListener("click",()=>{
    if(!SpeechRecognition){
      status.textContent="Speech recognition is unavailable here. Use Google Chrome and allow microphone access.";
      return;
    }
    liveVoice=true; status.textContent="Starting live conversation…";
    updateVoiceButtons(); startLiveListening();
  });
  $("voiceStop").addEventListener("click",stopLiveVoice);
  $("voiceSpeak").addEventListener("click",()=>{
    if(!lastAssistantReply)return;
    if(!("speechSynthesis" in window)){
      status.textContent="Speech playback is not supported in this browser.";return;
    }
    speakReply(lastAssistantReply);
    status.textContent="NOVA is speaking its last reply.";
  });
  updateVoiceButtons();
})();

</script>
</body>
</html>
