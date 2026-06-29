<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MindJournal — Awaremind Indonesia</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400;1,600&family=Nunito:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.min.js"></script>
<style>
/* =====================================================
   RESET & VARIABLES
===================================================== */
*, *::before, *::after { margin:0; padding:0; box-sizing:border-box; }

:root {
  --bg:        #EDE8E0;
  --bg2:       #F7F3EE;
  --card:      #FDFBF8;
  --pri:       #27470E;
  --pri-m:     #356115;
  --pri-l:     #6FA046;
  --acc:       #B8623A;
  --acc-l:     #D4845A;
  --sand:      #DDD4C6;
  --sand-l:    #EDE6DA;
  --text:      #1A1610;
  --text2:     #4E4537;
  --text3:     #9A8D7E;
  --border:    #CEC6B8;

  --dopa:      #F4A261;
  --sero:      #45B585;
  --oxy:       #E07A5F;
  --cort:      #9B8DEA;

  --r:         14px;
  --rl:        22px;
  --sh:        0 2px 16px rgba(26,22,16,.07);
  --shl:       0 10px 40px rgba(26,22,16,.13);
  --trans:     .22s cubic-bezier(.4,0,.2,1);
}

html, body { height:100%; background:var(--bg); color:var(--text); font-family:'Nunito',sans-serif; font-size:15px; line-height:1.6; }

/* =====================================================
   LAYOUT
===================================================== */
#app { display:flex; height:100vh; overflow:hidden; }

/* =====================================================
   SIDEBAR
===================================================== */
#sidebar {
  width:248px; min-width:248px;
  background:var(--pri);
  display:flex; flex-direction:column;
  position:relative; overflow:hidden;
}
#sidebar::before {
  content:''; position:absolute;
  width:220px; height:220px; border-radius:50%;
  background:rgba(255,255,255,.035);
  bottom:-70px; right:-70px;
}
#sidebar::after {
  content:''; position:absolute;
  width:140px; height:140px; border-radius:50%;
  background:rgba(255,255,255,.025);
  top:-50px; left:-50px;
}

.sb-logo { padding:26px 22px 18px; border-bottom:1px solid rgba(255,255,255,.1); }
.sb-logo .brand { font-family:'Cormorant Garamond',serif; font-size:21px; font-weight:600; color:#fff; letter-spacing:.02em; display:flex; align-items:center; gap:8px; }
.sb-logo .sub { font-size:10.5px; color:rgba(255,255,255,.42); letter-spacing:.1em; text-transform:uppercase; margin-top:3px; }

.sb-user { padding:14px 22px; display:flex; align-items:center; gap:10px; border-bottom:1px solid rgba(255,255,255,.1); }
.u-avatar { width:38px; height:38px; border-radius:50%; background:linear-gradient(135deg,var(--acc-l),var(--dopa)); display:flex; align-items:center; justify-content:center; font-size:15px; color:#fff; font-weight:700; flex-shrink:0; }
.u-name { font-size:13px; font-weight:700; color:#fff; }
.u-plan { font-size:10px; color:rgba(255,255,255,.45); text-transform:uppercase; letter-spacing:.07em; }
.plan-badge { display:inline-block; padding:1px 7px; border-radius:4px; font-size:9.5px; font-weight:800; text-transform:uppercase; letter-spacing:.06em; margin-left:4px; vertical-align:middle; }
.plan-badge.free { background:rgba(255,255,255,.18); color:rgba(255,255,255,.75); }
.plan-badge.premium { background:var(--acc); color:#fff; }

.sb-nav { flex:1; padding:14px 10px; display:flex; flex-direction:column; gap:2px; overflow-y:auto; }
.nav-section { font-size:9.5px; font-weight:800; text-transform:uppercase; letter-spacing:.13em; color:rgba(255,255,255,.28); padding:10px 12px 4px; }
.nav-item { display:flex; align-items:center; gap:9px; padding:10px 12px; border-radius:10px; cursor:pointer; transition:all var(--trans); color:rgba(255,255,255,.58); font-size:13.5px; font-weight:600; position:relative; z-index:1; }
.nav-item:hover { background:rgba(255,255,255,.09); color:rgba(255,255,255,.9); }
.nav-item.active { background:rgba(255,255,255,.16); color:#fff; }
.nav-item .ni-icon { font-size:16px; width:20px; text-align:center; }
.nav-item .ni-lock { margin-left:auto; font-size:11px; opacity:.45; }

.sb-footer { padding:14px 18px; border-top:1px solid rgba(255,255,255,.1); }
.upgrade-card { background:rgba(255,255,255,.07); border:1px solid rgba(255,255,255,.12); border-radius:14px; padding:14px 16px; text-align:center; cursor:pointer; transition:all var(--trans); }
.upgrade-card:hover { background:rgba(255,255,255,.11); }
.upgrade-card .uc-emoji { font-size:24px; display:block; margin-bottom:5px; }
.upgrade-card .uc-title { color:#fff; font-size:12.5px; font-weight:700; }
.upgrade-card .uc-sub { color:rgba(255,255,255,.42); font-size:10.5px; margin-top:1px; }
.upgrade-btn { display:block; width:100%; margin-top:10px; background:var(--acc); color:#fff; border:none; border-radius:8px; padding:8px; font-family:'Nunito',sans-serif; font-size:12px; font-weight:800; cursor:pointer; letter-spacing:.02em; transition:background var(--trans); }
.upgrade-btn:hover { background:var(--acc-l); }

/* =====================================================
   MAIN CONTENT
===================================================== */
#main { flex:1; overflow-y:auto; background:var(--bg2); }

.page { display:none; padding:34px 38px 60px; min-height:100%; animation:fadeUp .35s ease; }
.page.active { display:block; }
@keyframes fadeUp { from { opacity:0; transform:translateY(10px); } to { opacity:1; transform:translateY(0); } }

.ph { margin-bottom:28px; }
.ph h1 { font-family:'Cormorant Garamond',serif; font-size:36px; font-weight:500; color:var(--text); line-height:1.15; }
.ph p { color:var(--text3); font-size:13.5px; margin-top:4px; }

/* =====================================================
   CARDS
===================================================== */
.card { background:var(--card); border-radius:var(--rl); padding:24px; box-shadow:var(--sh); border:1px solid var(--border); }
.card-title { font-family:'Cormorant Garamond',serif; font-size:19px; font-weight:600; color:var(--text); margin-bottom:16px; }

/* =====================================================
   GRIDS
===================================================== */
.g2 { display:grid; grid-template-columns:1fr 1fr; gap:20px; }
.g3 { display:grid; grid-template-columns:1fr 1fr 1fr; gap:16px; }
.g4h { display:grid; grid-template-columns:1fr 1fr; gap:18px; }

/* =====================================================
   STATS
===================================================== */
.stat-card { background:var(--card); border:1px solid var(--border); border-radius:var(--r); padding:18px 16px; text-align:center; box-shadow:var(--sh); }
.stat-val { font-family:'Cormorant Garamond',serif; font-size:30px; font-weight:600; color:var(--pri); line-height:1; }
.stat-lbl { font-size:11.5px; color:var(--text3); margin-top:4px; font-weight:600; }

/* =====================================================
   MOOD RING
===================================================== */
.ring-wrap { display:flex; flex-direction:column; align-items:center; gap:14px; }
.ring-canvas-wrap { position:relative; width:190px; height:190px; }
.ring-canvas-wrap canvas { position:absolute; top:0; left:0; }
.ring-center { position:absolute; top:50%; left:50%; transform:translate(-50%,-50%); text-align:center; }
.ring-score { font-family:'Cormorant Garamond',serif; font-size:38px; font-weight:600; color:var(--text); line-height:1; }
.ring-label { font-size:10px; color:var(--text3); text-transform:uppercase; letter-spacing:.1em; margin-top:2px; }
.ring-legend { display:flex; flex-wrap:wrap; gap:10px; justify-content:center; }
.legend-dot { display:flex; align-items:center; gap:5px; font-size:11px; color:var(--text2); font-weight:600; }
.legend-dot span { width:9px; height:9px; border-radius:50%; display:block; }

/* =====================================================
   HORMONE SLIDERS
===================================================== */
.horm-grid { display:grid; grid-template-columns:1fr 1fr; gap:18px; }
.horm-item { background:var(--bg2); border-radius:14px; padding:18px; border:1px solid var(--border); transition:box-shadow var(--trans); }
.horm-item:hover { box-shadow:var(--sh); }
.horm-hdr { display:flex; align-items:center; gap:8px; margin-bottom:14px; }
.horm-dot { width:11px; height:11px; border-radius:50%; flex-shrink:0; }
.horm-name { font-size:13px; font-weight:800; color:var(--text); }
.horm-desc { font-size:10.5px; color:var(--text3); margin-top:1px; }
.horm-val { margin-left:auto; font-family:'Cormorant Garamond',serif; font-size:28px; font-weight:600; line-height:1; }
.horm-bar { position:relative; }
input[type="range"] { -webkit-appearance:none; appearance:none; width:100%; height:6px; border-radius:10px; outline:none; cursor:pointer; }
input[type="range"]::-webkit-slider-thumb { -webkit-appearance:none; appearance:none; width:20px; height:20px; border-radius:50%; background:#fff; border:2.5px solid currentColor; box-shadow:0 2px 8px rgba(0,0,0,.15); cursor:pointer; transition:transform .15s; }
input[type="range"]::-webkit-slider-thumb:hover { transform:scale(1.2); }
.horm-lbls { display:flex; justify-content:space-between; font-size:10px; color:var(--text3); margin-top:5px; }
.horm-insight-box { background:var(--bg); border:1px solid var(--border); border-radius:12px; padding:14px 16px; margin-top:18px; }
.horm-insight-txt { font-size:12.5px; color:var(--text2); font-style:italic; line-height:1.6; }

/* =====================================================
   GRATITUDE
===================================================== */
.grat-row { display:flex; align-items:center; gap:12px; margin-bottom:10px; }
.grat-num { width:30px; height:30px; border-radius:50%; background:linear-gradient(135deg,var(--dopa),var(--acc)); color:#fff; font-size:12px; font-weight:800; display:flex; align-items:center; justify-content:center; flex-shrink:0; }
.grat-input { flex:1; border:1px solid var(--border); border-radius:9px; padding:10px 14px; font-family:'Nunito',sans-serif; font-size:13.5px; color:var(--text); background:var(--bg2); outline:none; transition:border-color var(--trans),background var(--trans); }
.grat-input:focus { border-color:var(--dopa); background:#fff; }
.grat-input::placeholder { color:var(--text3); }

/* =====================================================
   FLOW SCALE
===================================================== */
.flow-scale { display:flex; gap:6px; margin-top:10px; }
.flow-btn { flex:1; aspect-ratio:1; border:2px solid var(--border); border-radius:9px; background:var(--bg2); cursor:pointer; font-size:13px; font-weight:800; color:var(--text3); transition:all .15s; display:flex; align-items:center; justify-content:center; font-family:'Nunito',sans-serif; }
.flow-btn:hover { border-color:var(--sero); color:var(--sero); }
.flow-btn.sel { background:var(--sero); border-color:var(--sero); color:#fff; }
.flow-fb { background:linear-gradient(135deg,#dff3eb,#cdeadf); border:1px solid #a6d9c1; border-radius:12px; padding:13px 16px; font-size:13px; color:#1a6040; line-height:1.6; margin-top:12px; min-height:48px; }

/* =====================================================
   TEXTAREA & INPUTS
===================================================== */
textarea { width:100%; border:1px solid var(--border); border-radius:10px; padding:14px; font-family:'Nunito',sans-serif; font-size:14px; color:var(--text); background:var(--bg2); resize:vertical; outline:none; transition:border-color var(--trans),background var(--trans); line-height:1.7; }
textarea:focus { border-color:var(--pri-l); background:#fff; }
textarea::placeholder { color:var(--text3); }
.text-input { width:100%; border:1px solid var(--border); border-radius:9px; padding:10px 14px; font-family:'Nunito',sans-serif; font-size:13.5px; color:var(--text); background:var(--bg2); outline:none; transition:border-color var(--trans),background var(--trans); }
.text-input:focus { border-color:var(--pri-l); background:#fff; }
.text-input::placeholder { color:var(--text3); }

/* =====================================================
   PROMPTS
===================================================== */
.prompt-card { background:linear-gradient(135deg,#edf7e5,#dff0d4); border:1px solid #b8d9a0; border-radius:14px; padding:20px; margin-bottom:14px; }
.prompt-lbl { font-size:10px; color:var(--pri); text-transform:uppercase; letter-spacing:.13em; font-weight:800; margin-bottom:7px; }
.prompt-q { font-family:'Cormorant Garamond',serif; font-size:18px; color:var(--pri-m); font-style:italic; margin-bottom:12px; line-height:1.45; }

/* =====================================================
   BUTTONS
===================================================== */
.btn { display:inline-flex; align-items:center; gap:8px; padding:11px 22px; border-radius:10px; font-family:'Nunito',sans-serif; font-size:14px; font-weight:800; cursor:pointer; border:none; transition:all var(--trans); line-height:1; }
.btn:disabled { opacity:.5; cursor:not-allowed; }
.btn-pri { background:var(--pri); color:#fff; }
.btn-pri:hover { background:var(--pri-m); transform:translateY(-1px); box-shadow:0 5px 16px rgba(39,71,14,.3); }
.btn-acc { background:var(--acc); color:#fff; }
.btn-acc:hover { background:var(--acc-l); transform:translateY(-1px); box-shadow:0 5px 16px rgba(184,98,58,.3); }
.btn-out { background:transparent; color:var(--pri); border:2px solid var(--pri); }
.btn-out:hover { background:var(--pri); color:#fff; }
.btn-ghost { background:var(--sand-l); color:var(--text2); border:1px solid var(--border); }
.btn-ghost:hover { background:var(--sand); }
.btn-lg { padding:14px 28px; font-size:15px; border-radius:13px; }
.btn-full { width:100%; justify-content:center; }

/* =====================================================
   STEP PROGRESS
===================================================== */
.step-bar { display:flex; gap:6px; margin-bottom:26px; }
.step-seg { flex:1; height:4px; border-radius:3px; background:var(--sand); transition:background .4s; }
.step-seg.done { background:var(--pri-l); }
.step-seg.active { background:var(--pri); }

/* =====================================================
   TAGS & BADGES
===================================================== */
.tag { display:inline-block; padding:3px 10px; border-radius:20px; font-size:11px; font-weight:700; }
.tag-g { background:#e8f5e0; color:var(--pri); }
.tag-a { background:#fef3e2; color:#B45309; }
.tag-r { background:#fde8e4; color:#C0392B; }
.tag-b { background:#e8effe; color:#2563EB; }
.section-lbl { font-size:10px; font-weight:800; text-transform:uppercase; letter-spacing:.13em; color:var(--text3); margin-bottom:10px; }

/* =====================================================
   ENTRY CARDS (HISTORY)
===================================================== */
.entry-card { background:var(--card); border:1px solid var(--border); border-radius:var(--r); padding:18px 20px; margin-bottom:12px; cursor:pointer; transition:all var(--trans); }
.entry-card:hover { box-shadow:var(--sh); transform:translateY(-1px); }
.entry-date { font-size:11px; color:var(--text3); text-transform:uppercase; letter-spacing:.1em; margin-bottom:5px; font-weight:600; }
.entry-preview { font-size:13.5px; color:var(--text2); line-height:1.55; display:-webkit-box; -webkit-line-clamp:2; -webkit-box-orient:vertical; overflow:hidden; }
.entry-pills { display:flex; gap:7px; margin-top:10px; flex-wrap:wrap; }
.h-pill { display:flex; align-items:center; gap:4px; background:var(--bg); border-radius:20px; padding:3px 10px; font-size:11px; font-weight:700; border:1px solid var(--border); }
.h-pill-dot { width:7px; height:7px; border-radius:50%; }

/* =====================================================
   STREAK CALENDAR
===================================================== */
.s-grid { display:grid; grid-template-columns:repeat(7,1fr); gap:4px; }
.s-cell { aspect-ratio:1; border-radius:5px; background:var(--sand); transition:background .2s; }
.s-cell.filled { background:var(--pri-l); }
.s-cell.today { background:var(--pri); box-shadow:0 0 0 2px #fff,0 0 0 4px var(--pri); }

/* =====================================================
   CHART AREA
===================================================== */
.chart-wrap { position:relative; height:230px; }

/* =====================================================
   PREMIUM LOCK / MODAL
===================================================== */
#premium-modal { position:fixed; inset:0; background:rgba(26,22,16,.55); backdrop-filter:blur(5px); z-index:200; display:none; align-items:center; justify-content:center; }
#premium-modal.open { display:flex; }
.modal-box { background:#fff; border-radius:26px; padding:38px; max-width:460px; width:90%; box-shadow:0 20px 70px rgba(26,22,16,.22); animation:mIn .32s cubic-bezier(.34,1.56,.64,1); position:relative; }
@keyframes mIn { from { opacity:0; transform:scale(.88) translateY(20px); } to { opacity:1; transform:scale(1) translateY(0); } }
.modal-badge { display:inline-block; background:linear-gradient(135deg,var(--dopa),var(--acc)); color:#fff; font-size:11px; font-weight:800; padding:4px 12px; border-radius:20px; text-transform:uppercase; letter-spacing:.08em; margin-bottom:14px; }
.modal-title { font-family:'Cormorant Garamond',serif; font-size:30px; font-weight:600; margin-bottom:7px; color:var(--text); }
.modal-sub { color:var(--text3); font-size:13.5px; margin-bottom:22px; line-height:1.65; }
.modal-close { position:absolute; top:16px; right:16px; width:34px; height:34px; border-radius:50%; background:var(--bg2); border:1px solid var(--border); cursor:pointer; font-size:16px; display:flex; align-items:center; justify-content:center; color:var(--text3); transition:all var(--trans); }
.modal-close:hover { background:var(--sand); }
.feat-list { list-style:none; margin-bottom:22px; }
.feat-list li { display:flex; align-items:center; gap:10px; padding:8px 0; font-size:13.5px; color:var(--text2); border-bottom:1px solid var(--sand-l); }
.feat-list li:last-child { border-bottom:none; }
.feat-list .chk { color:var(--sero); font-size:16px; }
.price-row { display:flex; align-items:baseline; gap:6px; margin-bottom:20px; }
.price-amt { font-family:'Cormorant Garamond',serif; font-size:44px; font-weight:600; color:var(--pri); }
.price-per { color:var(--text3); font-size:13px; }

/* =====================================================
   EXPORT PREVIEW
===================================================== */
.exp-preview { background:#fff; border:1px solid var(--border); border-radius:18px; overflow:hidden; }
.exp-hdr { background:var(--pri); padding:22px 26px; color:#fff; }
.exp-body { padding:24px; }

/* =====================================================
   TOAST
===================================================== */
#toast { position:fixed; bottom:28px; right:28px; background:var(--text); color:#fff; padding:14px 20px; border-radius:13px; font-size:13px; font-weight:700; opacity:0; transform:translateY(10px); transition:all .3s; z-index:500; pointer-events:none; max-width:300px; box-shadow:var(--shl); }
#toast.show { opacity:1; transform:translateY(0); }

/* =====================================================
   DIVIDER
===================================================== */
.div { height:1px; background:var(--sand); margin:22px 0; }

/* =====================================================
   EMPTY STATE
===================================================== */
.empty { text-align:center; padding:50px 20px; color:var(--text3); }
.empty .e-icon { font-size:40px; margin-bottom:10px; }
.empty .e-title { font-family:'Cormorant Garamond',serif; font-size:21px; color:var(--text2); margin-bottom:5px; }
.empty .e-sub { font-size:13px; }

/* =====================================================
   PREMIUM GATE OVERLAY
===================================================== */
.prem-gate { position:relative; }
.prem-gate-content { pointer-events:none; filter:blur(5px); user-select:none; }
.prem-gate-overlay { position:absolute; inset:0; display:flex; align-items:center; justify-content:center; z-index:10; padding:20px; }
.prem-gate-box { background:#fff; border-radius:24px; padding:38px; max-width:460px; width:100%; text-align:center; box-shadow:var(--shl); }
.prem-gate-icon { font-size:48px; margin-bottom:12px; }
.prem-gate-title { font-family:'Cormorant Garamond',serif; font-size:27px; font-weight:600; margin-bottom:8px; }
.prem-gate-sub { font-size:13.5px; color:var(--text2); line-height:1.7; margin-bottom:22px; }
.prem-feat-grid { text-align:left; margin-bottom:22px; }
.prem-feat-grid div { display:flex; align-items:center; gap:8px; padding:7px 0; font-size:13px; color:var(--text2); border-bottom:1px solid var(--sand-l); }
.prem-feat-grid div:last-child { border-bottom:none; }

/* =====================================================
   DAILY PROMPT CARD
===================================================== */
.daily-prompt-card { background:var(--bg2); border:1px solid var(--border); border-radius:14px; padding:16px 18px; }
.dpc-lbl { font-size:10px; font-weight:800; text-transform:uppercase; letter-spacing:.12em; color:var(--text3); margin-bottom:6px; }
.dpc-q { font-family:'Cormorant Garamond',serif; font-size:17px; color:var(--text2); font-style:italic; line-height:1.5; margin-bottom:10px; }

/* =====================================================
   LOCKED PROMPT CARD
===================================================== */
.locked-card { background:linear-gradient(135deg,#fef3e2,#fde8d4); border:1px solid #F4A261; border-radius:14px; padding:16px 18px; cursor:pointer; transition:all var(--trans); }
.locked-card:hover { box-shadow:0 4px 16px rgba(244,162,97,.25); }

/* =====================================================
   RESPONSIVE
===================================================== */
@media (max-width: 860px) {
  #sidebar { display:none; }
  .page { padding:20px 16px 60px; }
  .g2,.g3,.g4h,.horm-grid { grid-template-columns:1fr; }
}

/* =====================================================
   ANIMATION HELPERS
===================================================== */
.fade-in { animation:fadeUp .3s ease; }
@keyframes spin { from { transform:rotate(0deg); } to { transform:rotate(360deg); } }
</style>
</head>
<body>

<div id="app">
<!-- ================================ SIDEBAR ================================ -->
<aside id="sidebar">
  <div class="sb-logo">
    <div class="brand">🌿 MindJournal</div>
    <div class="sub">by Awaremind Indonesia</div>
  </div>
  <div class="sb-user">
    <div class="u-avatar" id="avatar-letter">F</div>
    <div>
      <div class="u-name" id="sb-name">Pengguna <span class="plan-badge free" id="plan-badge">Free</span></div>
      <div class="u-plan">Akun Pribadi</div>
    </div>
  </div>
  <nav class="sb-nav">
    <div class="nav-section">Menu Utama</div>
    <div class="nav-item active" data-page="dashboard"><span class="ni-icon">🏡</span>Dashboard</div>
    <div class="nav-item" data-page="journal"><span class="ni-icon">✍️</span>Jurnal Hari Ini</div>
    <div class="nav-item" data-page="history"><span class="ni-icon">📅</span>Riwayat Jurnal</div>
    <div class="nav-section" style="margin-top:10px;">Premium</div>
    <div class="nav-item" data-page="analytics"><span class="ni-icon">📊</span>Analitik Mood<span class="ni-lock" id="lock-analytics">🔒</span></div>
    <div class="nav-item" data-page="export"><span class="ni-icon">🔗</span>Ekspor ke HealMind<span class="ni-lock" id="lock-export">🔒</span></div>
    <div class="nav-section" style="margin-top:10px;">Tentang</div>
    <div class="nav-item" data-page="blueprint"><span class="ni-icon">📐</span>Blueprint Produk</div>
  </nav>
  <div class="sb-footer">
    <div class="upgrade-card" onclick="openModal()" id="upgrade-card-wrap">
      <span class="uc-emoji">⭐</span>
      <div class="uc-title">Upgrade ke Premium</div>
      <div class="uc-sub">Buka semua fitur psikologi</div>
      <button class="upgrade-btn">Coba Gratis 7 Hari</button>
    </div>
  </div>
</aside>

<!-- ================================ MAIN ================================ -->
<main id="main">

<!-- ===================== PAGE: DASHBOARD ===================== -->
<div id="page-dashboard" class="page active">
  <div class="ph">
    <h1 id="greeting">Selamat Datang 🌿</h1>
    <p id="today-date">Memuat tanggal...</p>
  </div>

  <!-- STATS ROW -->
  <div class="g3" style="margin-bottom:20px;">
    <div class="stat-card"><div class="stat-val" id="d-streak">0</div><div class="stat-lbl">🔥 Hari Berturut</div></div>
    <div class="stat-card"><div class="stat-val" id="d-total">0</div><div class="stat-lbl">📝 Total Entri</div></div>
    <div class="stat-card"><div class="stat-val" id="d-avgmood">—</div><div class="stat-lbl">😊 Rata-rata Wellbeing</div></div>
  </div>

  <!-- MOOD RING + QUICK START -->
  <div class="g2" style="margin-bottom:20px;">

    <div class="card">
      <div class="card-title">Kondisi Hormonal Hari Ini</div>
      <div class="ring-wrap">
        <div class="ring-canvas-wrap">
          <canvas id="moodRing" width="190" height="190"></canvas>
          <div class="ring-center">
            <div class="ring-score" id="ring-score">—</div>
            <div class="ring-label">Wellbeing</div>
          </div>
        </div>
        <div class="ring-legend">
          <div class="legend-dot"><span style="background:var(--dopa)"></span>Dopamine</div>
          <div class="legend-dot"><span style="background:var(--sero)"></span>Serotonin</div>
          <div class="legend-dot"><span style="background:var(--oxy)"></span>Oksitosin</div>
          <div class="legend-dot"><span style="background:var(--cort)"></span>Kortisol</div>
        </div>
      </div>
    </div>

    <div class="card" style="display:flex;flex-direction:column;gap:13px;">
      <div class="card-title">Mulai Hari Ini</div>
      <button class="btn btn-pri btn-lg btn-full" onclick="nav('journal')">✍️ Buka Jurnal Hari Ini</button>
      
      <div class="daily-prompt-card">
        <div class="dpc-lbl">💭 Prompt Hari Ini</div>
        <div class="dpc-q" id="daily-prompt-txt">"Apa satu hal kecil yang membuatmu tersenyum hari ini?"</div>
        <span class="tag tag-g" id="daily-prompt-tag">Mindfulness</span>
      </div>
      
      <div class="locked-card" onclick="openModal()">
        <div style="display:flex;align-items:center;justify-content:space-between;">
          <div>
            <div style="font-size:10.5px;font-weight:800;color:#B45309;text-transform:uppercase;letter-spacing:.08em;">🔒 Premium</div>
            <div style="font-size:13px;color:var(--text2);margin-top:2px;">+12 Guided Prompts Tematik</div>
          </div>
          <span style="color:#B45309;font-size:18px;font-weight:800;">→</span>
        </div>
      </div>
    </div>

  </div>

  <!-- STREAK CALENDAR -->
  <div class="card" style="margin-bottom:20px;">
    <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:16px;">
      <div class="card-title" style="margin-bottom:0">Kalender Konsistensi (28 Hari)</div>
      <span class="tag tag-g" id="streak-tag">0 hari streak</span>
    </div>
    <div class="s-grid" id="streak-cal"></div>
    <div style="display:flex;gap:14px;margin-top:12px;">
      <div style="display:flex;align-items:center;gap:5px;font-size:11px;color:var(--text3);font-weight:600;"><div style="width:13px;height:13px;border-radius:4px;background:var(--sand)"></div>Belum</div>
      <div style="display:flex;align-items:center;gap:5px;font-size:11px;color:var(--text3);font-weight:600;"><div style="width:13px;height:13px;border-radius:4px;background:var(--pri-l)"></div>Sudah</div>
      <div style="display:flex;align-items:center;gap:5px;font-size:11px;color:var(--text3);font-weight:600;"><div style="width:13px;height:13px;border-radius:4px;background:var(--pri)"></div>Hari ini</div>
    </div>
  </div>

  <!-- RECENT ENTRIES -->
  <div class="card-title" style="margin-bottom:12px;">Entri Terbaru</div>
  <div id="recent-entries">
    <div class="empty"><div class="e-icon">🌱</div><div class="e-title">Belum Ada Entri</div><div class="e-sub">Mulai perjalanan refleksi dirimu hari ini!</div></div>
  </div>
</div>

<!-- ===================== PAGE: JOURNAL ===================== -->
<div id="page-journal" class="page">
  <div class="ph">
    <h1>Jurnal Hari Ini ✍️</h1>
    <p id="journal-date-lbl">Isi refleksi harianmu di sini — ruang ini hanya untukmu.</p>
  </div>

  <div class="step-bar">
    <div class="step-seg active" id="seg1"></div>
    <div class="step-seg" id="seg2"></div>
    <div class="step-seg" id="seg3"></div>
    <div class="step-seg" id="seg4"></div>
  </div>

  <!-- STEP 1: HORMONE MOOD CHECK-IN -->
  <div id="jstep-1">
    <div class="card">
      <div style="margin-bottom:22px;">
        <div class="section-lbl">Langkah 1 dari 4</div>
        <div style="font-family:'Cormorant Garamond',serif;font-size:24px;font-weight:600;">Cek-in Hormonal Hari Ini 🧪</div>
        <div style="font-size:13px;color:var(--text3);margin-top:4px;">Geser slider untuk merepresentasikan kondisi neurokimiamu saat ini. Tidak ada jawaban yang salah.</div>
      </div>
      
      <div class="horm-grid" id="horm-grid-journal">

        <div class="horm-item">
          <div class="horm-hdr">
            <div class="horm-dot" style="background:var(--dopa)"></div>
            <div><div class="horm-name">Dopamine</div><div class="horm-desc">Motivasi & Produktivitas</div></div>
            <div class="horm-val" style="color:var(--dopa)" id="vd">50</div>
          </div>
          <input type="range" min="0" max="100" value="50" id="sl-dopa" style="color:var(--dopa)" oninput="onSlide('dopa',this.value)">
          <div class="horm-lbls"><span>Lesu 😔</span><span>Berenergi 🚀</span></div>
        </div>

        <div class="horm-item">
          <div class="horm-hdr">
            <div class="horm-dot" style="background:var(--sero)"></div>
            <div><div class="horm-name">Serotonin</div><div class="horm-desc">Ketenangan & Stabilitas</div></div>
            <div class="horm-val" style="color:var(--sero)" id="vs">50</div>
          </div>
          <input type="range" min="0" max="100" value="50" id="sl-sero" style="color:var(--sero)" oninput="onSlide('sero',this.value)">
          <div class="horm-lbls"><span>Cemas 😰</span><span>Tenang 😌</span></div>
        </div>

        <div class="horm-item">
          <div class="horm-hdr">
            <div class="horm-dot" style="background:var(--oxy)"></div>
            <div><div class="horm-name">Oksitosin</div><div class="horm-desc">Koneksi Sosial & Kasih Sayang</div></div>
            <div class="horm-val" style="color:var(--oxy)" id="vo">50</div>
          </div>
          <input type="range" min="0" max="100" value="50" id="sl-oxy" style="color:var(--oxy)" oninput="onSlide('oxy',this.value)">
          <div class="horm-lbls"><span>Terisolasi 😶</span><span>Terhubung 🤝</span></div>
        </div>

        <div class="horm-item">
          <div class="horm-hdr">
            <div class="horm-dot" style="background:var(--cort)"></div>
            <div><div class="horm-name">Kortisol</div><div class="horm-desc">Level Stres & Tekanan</div></div>
            <div class="horm-val" style="color:var(--cort)" id="vc">50</div>
          </div>
          <input type="range" min="0" max="100" value="50" id="sl-cort" style="color:var(--cort)" oninput="onSlide('cort',this.value)">
          <div class="horm-lbls"><span>Sangat Stres 😤</span><span>Rileks Total 🧘</span></div>
        </div>

      </div>

      <div class="horm-insight-box">
        <div class="horm-insight-txt" id="insight-txt">💡 Geser slider untuk mendapatkan pembacaan kondisi hormonalmu...</div>
      </div>

      <div style="margin-top:18px;text-align:right;">
        <button class="btn btn-pri" onclick="gotoStep(2)">Lanjut → Log Syukur</button>
      </div>
    </div>
  </div>

  <!-- STEP 2: GRATITUDE LOG -->
  <div id="jstep-2" style="display:none">
    <div class="card">
      <div style="margin-bottom:20px;">
        <div class="section-lbl">Langkah 2 dari 4</div>
        <div style="font-family:'Cormorant Garamond',serif;font-size:24px;font-weight:600;">Gratitude Log 🙏</div>
        <div style="font-size:13px;color:var(--text3);margin-top:4px;">Penelitian Emmons & McCullough (2003) membuktikan 3 hal syukur per hari secara konsisten meningkatkan wellbeing.</div>
      </div>
      <div class="grat-row"><div class="grat-num">1</div><input class="grat-input" type="text" id="g1" placeholder="Hari ini aku bersyukur karena..."></div>
      <div class="grat-row"><div class="grat-num">2</div><input class="grat-input" type="text" id="g2" placeholder="Seseorang yang aku apresiasi hari ini..."></div>
      <div class="grat-row"><div class="grat-num">3</div><input class="grat-input" type="text" id="g3" placeholder="Hal kecil yang membuatku tersenyum..."></div>
      <div class="div"></div>
      <div style="display:flex;justify-content:space-between;">
        <button class="btn btn-ghost" onclick="gotoStep(1)">← Kembali</button>
        <button class="btn btn-pri" onclick="gotoStep(3)">Lanjut → Flow State →</button>
      </div>
    </div>
  </div>

  <!-- STEP 3: FLOW TRACKER -->
  <div id="jstep-3" style="display:none">
    <div class="card">
      <div style="margin-bottom:20px;">
        <div class="section-lbl">Langkah 3 dari 4</div>
        <div style="font-family:'Cormorant Garamond',serif;font-size:24px;font-weight:600;">Flow State Tracker 🌊</div>
        <div style="font-size:13px;color:var(--text3);margin-top:4px;">Konsep Flow dari Csikszentmihalyi — seberapa dalam kamu "tenggelam" secara positif dalam aktivitasmu hari ini?</div>
      </div>
      
      <div style="font-size:13px;font-weight:600;color:var(--text2);margin-bottom:8px;">Pilih angka yang paling merepresentasikan tingkat fokus & engagement-mu hari ini:</div>
      <div class="flow-scale" id="flow-scale"></div>
      <div style="display:flex;justify-content:space-between;font-size:10.5px;color:var(--text3);margin-top:6px;font-weight:600;">
        <span>1 = Sangat Terdistraksi</span><span>10 = Flow Penuh ⚡</span>
      </div>
      <div class="flow-fb" id="flow-fb">Pilih angka untuk mendapatkan refleksi kondisi flow-mu...</div>

      <div style="margin-top:18px;">
        <div style="font-size:13px;font-weight:700;color:var(--text);margin-bottom:8px;">Aktivitas apa yang paling terasa seperti flow hari ini?</div>
        <input type="text" id="flow-act" class="text-input" placeholder="Misalnya: menulis, coding, memasak, membaca...">
      </div>

      <div class="div"></div>
      <div style="display:flex;justify-content:space-between;">
        <button class="btn btn-ghost" onclick="gotoStep(2)">← Kembali</button>
        <button class="btn btn-pri" onclick="gotoStep(4)">Lanjut → Refleksi →</button>
      </div>
    </div>
  </div>

  <!-- STEP 4: FREE JOURNAL + GUIDED PROMPTS (PREMIUM) -->
  <div id="jstep-4" style="display:none">
    <div class="card" style="margin-bottom:16px;">
      <div style="margin-bottom:18px;">
        <div class="section-lbl">Langkah 4 dari 4</div>
        <div style="font-family:'Cormorant Garamond',serif;font-size:24px;font-weight:600;">Jurnal Bebas 📝</div>
        <div style="font-size:13px;color:var(--text3);margin-top:4px;">Ceritakan harimu dengan caramu sendiri. Ruang ini aman dan hanya untukmu.</div>
      </div>
      <textarea id="free-journal" rows="7" placeholder="Hari ini terasa seperti... Aku memikirkan... Yang paling membekas dari hari ini adalah... Tidak ada yang menghakimi di sini."></textarea>
    </div>

    <!-- GUIDED PROMPTS — PREMIUM LOCKED -->
    <div class="card" style="margin-bottom:16px;position:relative;overflow:hidden;padding-bottom:0;">
      <div class="card-title">Guided Prompts Tematik</div>
      
      <div style="filter:blur(5px);pointer-events:none;padding-bottom:24px;">
        <div class="prompt-card">
          <div class="prompt-lbl">🧘 Mindfulness</div>
          <div class="prompt-q">"Di mana tubuhmu berada sekarang, dan di mana pikiranmu? Apakah keduanya hadir di saat yang sama?"</div>
          <textarea rows="3" placeholder="Tuliskan refleksimu..."></textarea>
        </div>
        <div class="prompt-card">
          <div class="prompt-lbl">💪 Kekuatan Karakter (VIA)</div>
          <div class="prompt-q">"Kekuatan karakter apa yang kamu gunakan hari ini tanpa kamu sadari sepenuhnya?"</div>
          <textarea rows="3" placeholder="Tuliskan refleksimu..."></textarea>
        </div>
        <div class="prompt-card">
          <div class="prompt-lbl">🌸 Self-Compassion</div>
          <div class="prompt-q">"Apa yang akan kamu katakan kepada sahabat terbaikmu jika dia sedang merasakan apa yang kamu rasakan hari ini?"</div>
          <textarea rows="3" placeholder="Tuliskan refleksimu..."></textarea>
        </div>
      </div>

      <div style="position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:12px;padding:24px;text-align:center;background:rgba(247,243,238,.94);backdrop-filter:blur(3px);">
        <div style="font-size:34px;">🔒</div>
        <div style="font-family:'Cormorant Garamond',serif;font-size:22px;font-weight:600;color:var(--text);">Guided Prompts Premium</div>
        <div style="font-size:13px;color:var(--text2);max-width:300px;line-height:1.65;">12+ prompt tematik berbasis Positive Psychology, Mindfulness, CBT, dan Self-Compassion — dikurasi oleh tim psikolog Awaremind.</div>
        <button class="btn btn-acc" onclick="openModal()">🌟 Aktifkan Premium — Gratis 7 Hari</button>
      </div>
    </div>

    <div style="display:flex;justify-content:space-between;align-items:center;gap:14px;">
      <button class="btn btn-ghost" onclick="gotoStep(3)">← Kembali</button>
      <button class="btn btn-pri btn-lg" onclick="saveEntry()">💾 Simpan Entri Hari Ini</button>
    </div>
  </div>
</div>

<!-- ===================== PAGE: HISTORY ===================== -->
<div id="page-history" class="page">
  <div class="ph">
    <h1>Riwayat Jurnal 📅</h1>
    <p>Semua catatan refleksi harianmu tersimpan di sini.</p>
  </div>
  <div id="history-list">
    <div class="empty"><div class="e-icon">📚</div><div class="e-title">Belum Ada Riwayat</div><div class="e-sub">Buat jurnal pertamamu untuk mulai melacak perjalananmu.</div><button class="btn btn-pri" style="margin-top:18px" onclick="nav('journal')">✍️ Buat Jurnal Pertama</button></div>
  </div>
</div>

<!-- ===================== PAGE: ANALYTICS (PREMIUM) ===================== -->
<div id="page-analytics" class="page">
  <div class="ph">
    <h1>Analitik Mood 📊</h1>
    <p>Visualisasi tren kondisi hormonal & wellbeing-mu</p>
  </div>
  <div class="prem-gate">
    <div class="prem-gate-content" id="analytics-inner">
      <div class="g2" style="margin-bottom:20px;">
        <div class="card">
          <div class="card-title">Tren Hormon — 7 Hari Terakhir</div>
          <div class="chart-wrap"><canvas id="trendChart"></canvas></div>
        </div>
        <div class="card">
          <div class="card-title">Radar Keseimbangan Hormonal</div>
          <div class="chart-wrap"><canvas id="radarChart"></canvas></div>
        </div>
      </div>
      <div class="card" style="margin-bottom:20px;">
        <div class="card-title">Distribusi Level per Hormon (30 Hari)</div>
        <div class="chart-wrap"><canvas id="barChart"></canvas></div>
      </div>
      <div class="g2">
        <div class="card">
          <div class="card-title">Keyword Emosi Dominan</div>
          <div style="display:flex;flex-wrap:wrap;gap:8px;margin-top:4px;">
            <span class="tag tag-g">bersyukur (15×)</span><span class="tag tag-g">semangat (12×)</span>
            <span class="tag tag-g">fokus (9×)</span><span class="tag tag-a">deadline (6×)</span>
            <span class="tag tag-g">capek (8×)</span><span class="tag tag-r">cemas (4×)</span>
            <span class="tag tag-b">belajar (11×)</span><span class="tag tag-g">tenang (7×)</span>
          </div>
        </div>
        <div class="card">
          <div class="card-title">Wellbeing Score Rata-rata</div>
          <div style="font-family:'Cormorant Garamond',serif;font-size:58px;font-weight:600;color:var(--pri);line-height:1;">72</div>
          <div style="font-size:12px;color:var(--text3);">dari 100 · 7 hari terakhir</div>
          <div style="margin-top:12px;font-size:13px;color:var(--text2);line-height:1.6;background:var(--bg2);padding:10px;border-radius:8px;border-left:3px solid var(--pri-l);">
            Tren positif terdeteksi. Serotonin-mu meningkat 8 poin dibanding minggu lalu 📈
          </div>
        </div>
      </div>
    </div>
    <div class="prem-gate-overlay" id="analytics-overlay">
      <div class="prem-gate-box">
        <div class="prem-gate-icon">📊</div>
        <div class="prem-gate-title">Analitik Mood Premium</div>
        <div class="prem-gate-sub">Lihat pola hormonal mingguan, radar keseimbangan, dan identifikasi trigger mood dengan analitik visual yang mendalam berbasis data jurnalmu.</div>
        <div class="prem-feat-grid">
          <div>✅ Grafik tren hormon 7 & 30 hari</div>
          <div>✅ Radar chart keseimbangan hormonal</div>
          <div>✅ Deteksi keyword & pola emosi</div>
          <div>✅ Wellbeing score historis</div>
        </div>
        <button class="btn btn-acc btn-lg btn-full" onclick="openModal()">🌟 Aktifkan Premium — Rp 49.000/bln</button>
        <div style="font-size:11px;color:var(--text3);margin-top:10px;">7 hari coba gratis · Batal kapan saja</div>
      </div>
    </div>
  </div>
</div>

<!-- ===================== PAGE: EXPORT TO HEALMIND ===================== -->
<div id="page-export" class="page">
  <div class="ph">
    <h1>Ekspor ke HealMind 🔗</h1>
    <p>Kirimkan ringkasan kondisi mentalmu ke konselor sebelum sesi dimulai — agar sesimu lebih efektif dan tepat sasaran.</p>
  </div>
  <div class="prem-gate">
    <div class="prem-gate-content" id="export-inner">
      <div class="exp-preview" style="margin-bottom:20px;">
        <div class="exp-hdr">
          <div style="display:flex;justify-content:space-between;align-items:center;">
            <div>
              <div style="font-family:'Cormorant Garamond',serif;font-size:21px;font-weight:600;">Laporan Wellbeing — MindJournal</div>
              <div style="font-size:11.5px;opacity:.65;margin-top:3px;">Awaremind Indonesia · Digenerate otomatis · Periode: 30 Hari Terakhir</div>
            </div>
            <div style="background:rgba(255,255,255,.13);border-radius:8px;padding:7px 13px;font-size:11.5px;">🔒 Konten Privat</div>
          </div>
        </div>
        <div class="exp-body">
          <div class="g3" style="margin-bottom:20px;">
            <div style="text-align:center;padding:16px;background:var(--bg2);border-radius:10px;">
              <div style="font-family:'Cormorant Garamond',serif;font-size:30px;font-weight:600;color:var(--dopa);">72</div>
              <div style="font-size:11px;color:var(--text3)">Rata-rata Dopamine</div>
            </div>
            <div style="text-align:center;padding:16px;background:var(--bg2);border-radius:10px;">
              <div style="font-family:'Cormorant Garamond',serif;font-size:30px;font-weight:600;color:var(--sero);">65</div>
              <div style="font-size:11px;color:var(--text3)">Rata-rata Serotonin</div>
            </div>
            <div style="text-align:center;padding:16px;background:var(--bg2);border-radius:10px;">
              <div style="font-family:'Cormorant Garamond',serif;font-size:30px;font-weight:600;color:var(--pri);">7.2</div>
              <div style="font-size:11px;color:var(--text3)">Avg. Flow Score</div>
            </div>
          </div>
          <div style="margin-bottom:16px;">
            <div style="font-size:11px;font-weight:800;text-transform:uppercase;letter-spacing:.1em;color:var(--text3);margin-bottom:8px;">Keyword Emosi Dominan</div>
            <div style="display:flex;flex-wrap:wrap;gap:7px;">
              <span class="tag tag-g">capek (8×)</span><span class="tag tag-g">semangat (12×)</span><span class="tag tag-a">deadline (6×)</span><span class="tag tag-g">bersyukur (15×)</span><span class="tag tag-r">cemas (4×)</span><span class="tag tag-g">fokus (9×)</span>
            </div>
          </div>
          <div>
            <div style="font-size:11px;font-weight:800;text-transform:uppercase;letter-spacing:.1em;color:var(--text3);margin-bottom:8px;">Catatan Otomatis untuk Konselor</div>
            <div style="font-size:13px;color:var(--text2);background:var(--bg2);border-radius:10px;padding:14px;line-height:1.7;border-left:3px solid var(--pri-l);">Klien menunjukkan pola dopamine tinggi pada Senin–Rabu, dengan penurunan signifikan akhir pekan. Kortisol sempat melonjak minggu ke-2. Tema syukur dominan dengan 15 entri positif. Direkomendasikan untuk mendiskusikan manajemen energi dan transisi akhir pekan dalam sesi.</div>
          </div>
        </div>
      </div>
      <div class="g2">
        <div class="card">
          <div class="card-title">Opsi Konten Ekspor</div>
          <div style="display:flex;flex-direction:column;gap:11px;">
            <label style="display:flex;align-items:center;gap:10px;cursor:pointer;font-size:13.5px;"><input type="checkbox" checked style="width:16px;height:16px;accent-color:var(--pri)"> Grafik hormon 30 hari</label>
            <label style="display:flex;align-items:center;gap:10px;cursor:pointer;font-size:13.5px;"><input type="checkbox" checked style="width:16px;height:16px;accent-color:var(--pri)"> Analisis keyword emosi</label>
            <label style="display:flex;align-items:center;gap:10px;cursor:pointer;font-size:13.5px;"><input type="checkbox" checked style="width:16px;height:16px;accent-color:var(--pri)"> Rata-rata flow state</label>
            <label style="display:flex;align-items:center;gap:10px;cursor:pointer;font-size:13.5px;"><input type="checkbox" style="width:16px;height:16px;accent-color:var(--pri)"> Isi jurnal lengkap (opsional)</label>
            <label style="display:flex;align-items:center;gap:10px;cursor:pointer;font-size:13.5px;"><input type="checkbox" checked style="width:16px;height:16px;accent-color:var(--pri)"> Gratitude log ringkasan</label>
          </div>
        </div>
        <div class="card">
          <div class="card-title">Kirim ke Konselor</div>
          <div style="font-size:13px;color:var(--text2);margin-bottom:16px;line-height:1.65;">Laporan akan dikirim langsung ke dashboard admin HealMind. Konselormu dapat membacanya sebelum sesi dimulai untuk percakapan yang lebih terarah.</div>
          <button class="btn btn-pri btn-full" style="margin-bottom:10px" id="export-send-btn" onclick="doExport()">📤 Ekspor & Kirim ke HealMind</button>
          <button class="btn btn-ghost btn-full" id="export-pdf-btn" onclick="downloadPDF()">📄 Unduh Laporan PDF</button>
          <div style="font-size:11px;color:var(--text3);margin-top:12px;text-align:center">🔒 End-to-end encrypted · HIPAA-aware</div>
        </div>
      </div>
    </div>
    <div class="prem-gate-overlay" id="export-overlay">
      <div class="prem-gate-box">
        <div class="prem-gate-icon">🔗</div>
        <div class="prem-gate-title">Integrasi HealMind</div>
        <div class="prem-gate-sub">Kirimkan ringkasan kondisi mentalmu secara otomatis ke konselor HealMind — agar setiap sesi konseling lebih efektif, berbasis data, dan tepat sasaran.</div>
        <div class="prem-feat-grid">
          <div>✅ Ekspor PDF laporan wellbeing</div>
          <div>✅ Kirim otomatis ke dashboard konselor</div>
          <div>✅ Ringkasan keyword & pola emosi</div>
          <div>✅ Kontrol penuh data yang dikirim</div>
        </div>
        <button class="btn btn-acc btn-lg btn-full" onclick="openModal()">🌟 Aktifkan Fitur Ini</button>
        <div style="font-size:11px;color:var(--text3);margin-top:10px">7 hari coba gratis · Tidak perlu kartu kredit</div>
      </div>
    </div>
  </div>
</div>

<!-- ===================== PAGE: BLUEPRINT ===================== -->
<div id="page-blueprint" class="page">
  <div class="ph">
    <h1>Blueprint Produk 📐</h1>
    <p>Arsitektur lengkap: User Flow, Database Schema, Tech Stack, dan Logika Integrasi</p>
  </div>

  <!-- USER FLOW -->
  <div class="card" style="margin-bottom:20px;">
    <div class="card-title">1. User Flow — Perjalanan Pengguna</div>
    <div style="font-size:13px;color:var(--text3);margin-bottom:16px;">Diagram perjalanan dari onboarding hingga ekspor ke konselor</div>
    <div style="display:flex;flex-direction:column;gap:0;">
      <!-- Flow steps -->
      <div id="flow-diagram"></div>
    </div>
  </div>

  <!-- DB SCHEMA -->
  <div class="card" style="margin-bottom:20px;">
    <div class="card-title">2. Database Schema</div>
    <div style="font-size:13px;color:var(--text3);margin-bottom:18px;">Struktur tabel utama dengan relasi — direkomendasikan menggunakan PostgreSQL / Supabase.</div>
    <div id="db-schema"></div>
  </div>

  <!-- TECH STACK -->
  <div class="card" style="margin-bottom:20px;">
    <div class="card-title">3. Tech Stack Rekomendasi</div>
    <div id="tech-stack"></div>
  </div>

  <!-- INTEGRATION LOGIC -->
  <div class="card">
    <div class="card-title">4. Logika Integrasi dengan HealMind (Google Apps Script)</div>
    <div id="integration-logic"></div>
  </div>
</div>

</main>
</div>

<!-- ===================== PREMIUM MODAL ===================== -->
<div id="premium-modal">
  <div class="modal-box">
    <button class="modal-close" onclick="closeModal()">✕</button>
    <div class="modal-badge">⭐ MindJournal Premium</div>
    <div class="modal-title">Buka Potensi Penuh Jurnalmu</div>
    <div class="modal-sub">Dapatkan akses ke semua fitur psikologi berbasis riset yang dikurasi tim Awaremind Indonesia.</div>
    <ul class="feat-list">
      <li><span class="chk">✅</span> 12+ Guided Prompts (Mindfulness, CBT, Strengths-Based)</li>
      <li><span class="chk">✅</span> Analitik mood visual 7 & 30 hari</li>
      <li><span class="chk">✅</span> Radar chart keseimbangan hormonal</li>
      <li><span class="chk">✅</span> Deteksi keyword & pola emosi dari jurnal</li>
      <li><span class="chk">✅</span> Ekspor laporan otomatis ke konselor HealMind</li>
      <li><span class="chk">✅</span> Unduh PDF laporan wellbeing pribadi</li>
    </ul>
    <div class="price-row"><div class="price-amt">Rp 49.000</div><div class="price-per">/ bulan</div></div>
    <button class="btn btn-acc btn-lg btn-full" onclick="activatePremium()">🌟 Mulai Trial 7 Hari — GRATIS</button>
    <div style="font-size:11px;color:var(--text3);margin-top:10px;text-align:center">Tidak ada biaya selama 7 hari · Batal kapan saja</div>
  </div>
</div>

<!-- TOAST -->
<div id="toast"></div>

<script>
// ================================================================
// CONSTANTS & STATE
// ================================================================
const PROMPTS = [
  { q: '"Apa satu hal kecil yang membuatmu tersenyum hari ini?"', tag: 'Mindfulness' },
  { q: '"Siapa yang paling kamu syukuri kehadirannya dalam hidupmu?"', tag: 'Gratitude' },
  { q: '"Di mana kamu merasa paling hidup hari ini?"', tag: 'Flow State' },
  { q: '"Kekuatan apa dalam dirimu yang baru kamu sadari belakangan ini?"', tag: 'Strengths' },
  { q: '"Apa yang ingin kamu katakan kepada dirimu sendiri di masa lalu?"', tag: 'Self-Compassion' },
  { q: '"Apa satu langkah kecil yang bisa kamu ambil besok untuk merasa lebih baik?"', tag: 'Positive Action' },
  { q: '"Momen apa hari ini yang ingin kamu kenang 5 tahun ke depan?"', tag: 'Savoring' },
];

const FLOW_MSG = {
  1:'😵 Pikiranmu tersebar ke mana-mana hari ini. Itu wajar — kenali dan hadapi dengan lembut.',
  2:'😟 Banyak distraksi. Coba break 5 menit dan fokus ulang pada satu hal.',
  3:'😕 Agak sulit fokus, tapi kamu tetap berusaha. Itu sudah cukup.',
  4:'😐 Cukup untuk menyelesaikan beberapa hal. Kamu bertahan dengan baik.',
  5:'🙂 Fokus moderat. Separuh harimu berjalan cukup produktif.',
  6:'😊 Cukup engaged. Kamu hadir dalam sebagian besar aktivitasmu.',
  7:'😌 Fokus yang baik. Pikiranmu lebih jernih dari biasanya.',
  8:'🎯 Sangat fokus. Kamu merasakan kedalaman dalam aktivitasmu.',
  9:'🌊 Hampir flow! Kamu nyaris lupa waktu — momen yang langka dan berharga.',
  10:'⚡ Flow Penuh! Kamu sepenuhnya tenggelam. Simpan energi dan momen ini dalam ingatanmu.',
};

const COLORS = { dopa:'#F4A261', sero:'#45B585', oxy:'#E07A5F', cort:'#9B8DEA' };
const DAYS_ID = ['Min','Sen','Sel','Rab','Kam','Jum','Sab'];
const MONTHS_ID = ['Januari','Februari','Maret','April','Mei','Juni','Juli','Agustus','September','Oktober','November','Desember'];

let state = {
  isPremium: false,
  hormones: { dopa:50, sero:50, oxy:50, cort:50 },
  flowScore: null,
  entries: JSON.parse(localStorage.getItem('mj_entries')||'[]'),
};

let moodRingChart = null;
let chartsReady = false;

// ================================================================
// INIT
// ================================================================
function init() {
  loadProfile();
  setDates();
  buildFlowScale();
  buildStreakCal();
  buildMoodRing();
  renderDashboard();
  buildBlueprintPage();
  syncSliders();
}

function setDates() {
  const d = new Date();
  const str = `${DAYS_ID[d.getDay()]}, ${d.getDate()} ${MONTHS_ID[d.getMonth()]} ${d.getFullYear()}`;
  document.getElementById('today-date').textContent = str;
  document.getElementById('journal-date-lbl').textContent = `${str} — Isi refleksi harianmu di sini.`;
  
  const idx = d.getDay() % PROMPTS.length;
  document.getElementById('daily-prompt-txt').textContent = PROMPTS[idx].q;
  document.getElementById('daily-prompt-tag').textContent = PROMPTS[idx].tag;
}

// ================================================================
// NAVIGATION
// ================================================================
function nav(page) {
  document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
  document.querySelectorAll('.nav-item').forEach(n => n.classList.remove('active'));
  document.getElementById('page-'+page).classList.add('active');
  document.querySelector('[data-page="'+page+'"]').classList.add('active');
  document.getElementById('main').scrollTop = 0;
  if (page === 'analytics' && state.isPremium) initCharts();
  if (page === 'journal') { gotoStep(1); resetJournalForm(); }
}

document.querySelectorAll('.nav-item').forEach(el => {
  el.addEventListener('click', () => nav(el.dataset.page));
});

// ================================================================
// JOURNAL STEPS
// ================================================================
function gotoStep(n) {
  for (let i=1;i<=4;i++) {
    const el = document.getElementById('jstep-'+i);
    if (el) el.style.display = i===n?'block':'none';
    const seg = document.getElementById('seg'+i);
    if (seg) {
      seg.className = 'step-seg';
      if (i<n) seg.classList.add('done');
      if (i===n) seg.classList.add('active');
    }
  }
}

function resetJournalForm() {
  ['sl-dopa','sl-sero','sl-oxy','sl-cort'].forEach(id => { const el=document.getElementById(id); if(el) el.value=50; });
  state.hormones = {dopa:50,sero:50,oxy:50,cort:50};
  syncSliders();
  ['g1','g2','g3','flow-act'].forEach(id=>{const el=document.getElementById(id);if(el)el.value='';});
  const fj = document.getElementById('free-journal'); if(fj) fj.value='';
  state.flowScore = null;
  document.querySelectorAll('.flow-btn').forEach(b=>b.classList.remove('sel'));
  const ff = document.getElementById('flow-fb'); if(ff) ff.textContent='Pilih angka untuk mendapatkan refleksi kondisi flow-mu...';
  document.getElementById('insight-txt').textContent='💡 Geser slider untuk mendapatkan pembacaan kondisi hormonalmu...';
}

// ================================================================
// HORMONE SLIDERS
// ================================================================
function onSlide(h, v) {
  state.hormones[h] = parseInt(v);
  const ids = {dopa:'vd',sero:'vs',oxy:'vo',cort:'vc'};
  document.getElementById(ids[h]).textContent = v;
  updateSliderBg(h, v);
  document.getElementById('insight-txt').textContent = getInsight();
  updateMoodRing();
}

function updateSliderBg(h, v) {
  const el = document.getElementById('sl-'+h);
  if (!el) return;
  const c = COLORS[h];
  el.style.background = `linear-gradient(to right,${c} ${v}%,#DDD4C6 ${v}%)`;
}

function syncSliders() {
  Object.keys(state.hormones).forEach(h => {
    updateSliderBg(h, state.hormones[h]);
    const el = document.getElementById('sl-'+h); if(el) el.value=state.hormones[h];
    const ids={dopa:'vd',sero:'vs',oxy:'vo',cort:'vc'};
    const vEl=document.getElementById(ids[h]);if(vEl)vEl.textContent=state.hormones[h];
  });
}

function getInsight() {
  const {dopa,sero,oxy,cort} = state.hormones;
  const inv = 100-cort;
  const avg = (dopa+sero+oxy+inv)/4;
  if (avg>=78) return '💚 Kondisi hormonal yang luar biasa hari ini! Manfaatkan energi ini untuk hal-hal yang bermakna.';
  if (cort>70) return '🔴 Kortisol tinggi terdeteksi. Coba teknik pernapasan 4-7-8 atau jalan singkat 10 menit sekarang.';
  if (dopa<35) return '🟠 Motivasi sedang rendah. Mulai dengan satu tugas kecil yang bisa diselesaikan dalam 5 menit.';
  if (sero<35) return '🟡 Suasana hati sedikit kurang stabil. Journaling ini sendiri sudah membantu — teruslah menulis.';
  if (oxy<35) return '🩷 Rasa koneksi sosial sedang rendah. Mungkin ini saatnya menghubungi seseorang yang kamu sayangi.';
  if (avg>=60) return '💛 Kondisi cukup seimbang. Ada satu atau dua area yang bisa ditingkatkan — dan itu progres yang bagus!';
  return '💙 Hari yang netral, dan itu sangat valid untuk dirasakan. Kamu sudah hadir — itu cukup.';
}

// ================================================================
// MOOD RING (DOUGHNUT CHART)
// ================================================================
function buildMoodRing() {
  const ctx = document.getElementById('moodRing');
  if (!ctx) return;
  moodRingChart = new Chart(ctx, {
    type: 'doughnut',
    data: {
      datasets: [{
        data: [25,25,25,25],
        backgroundColor: [COLORS.dopa,COLORS.sero,COLORS.oxy,COLORS.cort],
        borderWidth: 0,
      }]
    },
    options: {
      cutout: '72%',
      plugins: { legend:{display:false}, tooltip:{enabled:false} },
      animation: { duration:700 },
    }
  });
  updateMoodRing();
}

function updateMoodRing() {
  if (!moodRingChart) return;
  const {dopa,sero,oxy,cort} = state.hormones;
  const inv = 100-cort;
  const wb = Math.round((dopa+sero+oxy+inv)/4);
  moodRingChart.data.datasets[0].data = [dopa,sero,oxy,inv];
  moodRingChart.update('none');
  const el = document.getElementById('ring-score');
  if (el) el.textContent = wb;
}

// ================================================================
// FLOW SCALE
// ================================================================
function buildFlowScale() {
  const c = document.getElementById('flow-scale');
  if (!c) return;
  c.innerHTML = '';
  for (let i=1;i<=10;i++) {
    const b = document.createElement('button');
    b.className = 'flow-btn';
    b.textContent = i;
    b.type = 'button';
    b.onclick = ()=>selectFlow(i);
    c.appendChild(b);
  }
}

function selectFlow(n) {
  state.flowScore = n;
  document.querySelectorAll('.flow-btn').forEach((b,i)=>b.classList.toggle('sel',i<n));
  const fb=document.getElementById('flow-fb');
  if(fb) fb.textContent = FLOW_MSG[n]||'';
}

// ================================================================
// SAVE ENTRY
// ================================================================
function saveEntry() {
  const entry = {
    id: Date.now(),
    date: new Date().toISOString(),
    hormones: {...state.hormones},
    flowScore: state.flowScore||5,
    flowActivity: document.getElementById('flow-act')?.value||'',
    gratitude: [
      document.getElementById('g1')?.value||'',
      document.getElementById('g2')?.value||'',
      document.getElementById('g3')?.value||'',
    ],
    journal: document.getElementById('free-journal')?.value||'',
  };
  
  // Prevent duplicate for same day
  const today = new Date().toDateString();
  state.entries = state.entries.filter(e => new Date(e.date).toDateString() !== today);
  state.entries.unshift(entry);
  
  localStorage.setItem('mj_entries', JSON.stringify(state.entries));
  showToast('✅ Entri berhasil disimpan!');
  renderDashboard();
  buildStreakCal();
  nav('dashboard');
}

// ================================================================
// DASHBOARD RENDER
// ================================================================
function renderDashboard() {
  const entries = state.entries;
  document.getElementById('d-total').textContent = entries.length;

  // Streak
  let streak=0;
  const today = new Date();
  let check = new Date(today);
  const dateset = new Set(entries.map(e=>new Date(e.date).toDateString()));
  while(dateset.has(check.toDateString())) {
    streak++;
    check.setDate(check.getDate()-1);
  }
  document.getElementById('d-streak').textContent = streak;
  document.getElementById('streak-tag').textContent = `${streak} hari streak`;

  // Avg mood
  if (entries.length>0) {
    const slice = entries.slice(0,7);
    const avg = slice.reduce((s,e)=>{
      const {dopa,sero,oxy,cort}=e.hormones;
      return s+(dopa+sero+oxy+(100-cort))/4;
    },0)/slice.length;
    document.getElementById('d-avgmood').textContent = Math.round(avg);
  }

  // Mood ring: load today's entry if exists
  const todayEntry = entries.find(e=>new Date(e.date).toDateString()===today.toDateString());
  if (todayEntry) {
    state.hormones = {...todayEntry.hormones};
    updateMoodRing();
  }

  renderEntries();
}

function renderEntries() {
  const entries = state.entries;
  const makeCard = (e) => {
    const d = new Date(e.date);
    const ds = `${DAYS_ID[d.getDay()]}, ${d.getDate()} ${MONTHS_ID[d.getMonth()]} ${d.getFullYear()}`;
    const wb = Math.round((e.hormones.dopa+e.hormones.sero+e.hormones.oxy+(100-e.hormones.cort))/4);
    const prev = e.journal ? e.journal.substring(0,200) : '<span style="font-style:italic;color:var(--text3)">Tidak ada catatan jurnal bebas.</span>';
    return `
      <div class="entry-card">
        <div class="entry-date">📅 ${ds}</div>
        <div style="display:flex;align-items:center;gap:12px;margin-bottom:7px;">
          <span style="font-family:'Cormorant Garamond',serif;font-size:16px;font-weight:600;">Wellbeing: <span style="color:var(--pri)">${wb}/100</span></span>
          <span style="font-size:12px;color:var(--text3);">Flow: ${e.flowScore}/10</span>
          ${e.flowActivity?`<span class="tag tag-g" style="font-size:10px">${e.flowActivity}</span>`:''}
        </div>
        <div class="entry-preview">${prev}</div>
        ${e.gratitude.some(g=>g) ? `<div style="font-size:11.5px;color:var(--text3);margin-top:6px;font-style:italic">🙏 ${e.gratitude.filter(g=>g).join(' · ')}</div>`:''}
        <div class="entry-pills">
          <div class="h-pill"><div class="h-pill-dot" style="background:var(--dopa)"></div>${e.hormones.dopa}</div>
          <div class="h-pill"><div class="h-pill-dot" style="background:var(--sero)"></div>${e.hormones.sero}</div>
          <div class="h-pill"><div class="h-pill-dot" style="background:var(--oxy)"></div>${e.hormones.oxy}</div>
          <div class="h-pill"><div class="h-pill-dot" style="background:var(--cort)"></div>${e.hormones.cort}</div>
        </div>
      </div>`;
  };

  if (!entries.length) {
    const emp = '<div class="empty"><div class="e-icon">🌱</div><div class="e-title">Belum Ada Entri</div><div class="e-sub">Mulai perjalanan refleksi dirimu hari ini!</div></div>';
    document.getElementById('recent-entries').innerHTML = emp;
    document.getElementById('history-list').innerHTML = '<div class="empty"><div class="e-icon">📚</div><div class="e-title">Belum Ada Riwayat</div><div class="e-sub">Buat jurnal pertamamu untuk mulai melacak perjalananmu.</div><button class="btn btn-pri" style="margin-top:18px" onclick="nav(\'journal\')">✍️ Buat Jurnal Pertama</button></div>';
    return;
  }
  document.getElementById('recent-entries').innerHTML = entries.slice(0,3).map(makeCard).join('');
  document.getElementById('history-list').innerHTML = entries.map(makeCard).join('');
}

// ================================================================
// STREAK CALENDAR
// ================================================================
function buildStreakCal() {
  const c = document.getElementById('streak-cal');
  if (!c) return;
  const dateset = new Set(state.entries.map(e=>new Date(e.date).toDateString()));
  const today = new Date();
  let html='';
  for(let i=27;i>=0;i--){
    const d=new Date(today); d.setDate(today.getDate()-i);
    const isToday=d.toDateString()===today.toDateString();
    const filled=dateset.has(d.toDateString());
    html+=`<div class="s-cell ${isToday?'today':filled?'filled':''}" title="${d.toLocaleDateString('id-ID')}"></div>`;
  }
  c.innerHTML=html;
}

// ================================================================
// ANALYTICS CHARTS
// ================================================================
function initCharts() {
  if (chartsReady) return;
  chartsReady = true;

  const entries = state.entries;
  const days = ['Sen','Sel','Rab','Kam','Jum','Sab','Min'];
  const rnd = (b,v)=>Math.round(b+(Math.random()-.5)*v*2);
  
  const getArr = key => entries.length>=7
    ? entries.slice(0,7).reverse().map(e=>e.hormones[key])
    : days.map(()=>rnd(key==='cort'?45:65,20));

  const dopaArr=getArr('dopa'), seroArr=getArr('sero'), oxyArr=getArr('oxy'), cortArr=getArr('cort');

  const baseOpts = {
    responsive:true, maintainAspectRatio:false,
    plugins:{legend:{labels:{font:{family:'Nunito',size:11},color:'#4E4537'}}},
  };

  new Chart(document.getElementById('trendChart'),{
    type:'line',
    data:{
      labels:days,
      datasets:[
        {label:'Dopamine',data:dopaArr,borderColor:COLORS.dopa,backgroundColor:'rgba(244,162,97,.1)',tension:.4,fill:true,borderWidth:2.5,pointRadius:4,pointBackgroundColor:COLORS.dopa},
        {label:'Serotonin',data:seroArr,borderColor:COLORS.sero,backgroundColor:'rgba(69,181,133,.1)',tension:.4,fill:true,borderWidth:2.5,pointRadius:4,pointBackgroundColor:COLORS.sero},
        {label:'Oksitosin',data:oxyArr,borderColor:COLORS.oxy,backgroundColor:'rgba(224,122,95,.1)',tension:.4,fill:true,borderWidth:2.5,pointRadius:4,pointBackgroundColor:COLORS.oxy},
        {label:'Kortisol',data:cortArr,borderColor:COLORS.cort,backgroundColor:'rgba(155,141,234,.1)',tension:.4,fill:true,borderWidth:2.5,pointRadius:4,pointBackgroundColor:COLORS.cort},
      ]
    },
    options:{...baseOpts,scales:{y:{min:0,max:100,grid:{color:'rgba(0,0,0,.05)'},ticks:{font:{family:'Nunito',size:10}}}}}
  });

  const avg=arr=>Math.round(arr.reduce((a,b)=>a+b,0)/arr.length);
  new Chart(document.getElementById('radarChart'),{
    type:'radar',
    data:{
      labels:['Dopamine','Serotonin','Oksitosin','Anti-Kortisol','Flow'],
      datasets:[{
        label:'Profil Hormonal',
        data:[avg(dopaArr),avg(seroArr),avg(oxyArr),100-avg(cortArr),(state.entries[0]?.flowScore||6)*10],
        backgroundColor:'rgba(39,71,14,.1)',borderColor:'#27470E',pointBackgroundColor:'#6FA046',pointRadius:5,borderWidth:2,
      }]
    },
    options:{...baseOpts,scales:{r:{min:0,max:100,grid:{color:'rgba(0,0,0,.06)'},ticks:{display:false},pointLabels:{font:{family:'Nunito',size:10.5},color:'#4E4537'}}},plugins:{legend:{display:false}}}
  });

  new Chart(document.getElementById('barChart'),{
    type:'bar',
    data:{
      labels:['Dopamine','Serotonin','Oksitosin','Anti-Kortisol'],
      datasets:[
        {label:'Rendah (<40)',data:[15,20,25,10],backgroundColor:'rgba(224,122,95,.45)',borderRadius:4},
        {label:'Sedang (40–70)',data:[45,50,40,55],backgroundColor:'rgba(244,162,97,.45)',borderRadius:4},
        {label:'Tinggi (>70)',data:[40,30,35,35],backgroundColor:'rgba(69,181,133,.45)',borderRadius:4},
      ]
    },
    options:{...baseOpts,scales:{x:{stacked:true,grid:{display:false},ticks:{font:{family:'Nunito',size:11}}},y:{stacked:true,grid:{color:'rgba(0,0,0,.05)'},ticks:{font:{family:'Nunito',size:10}}}}}
  });
}

// ================================================================
// PREMIUM
// ================================================================
function openModal() { document.getElementById('premium-modal').classList.add('open'); }
function closeModal() { document.getElementById('premium-modal').classList.remove('open'); }

document.getElementById('premium-modal').addEventListener('click', e=>{
  if(e.target===document.getElementById('premium-modal')) closeModal();
});

function activatePremium() {
  state.isPremium = true;
  closeModal();

  // Update badge
  const badge=document.getElementById('plan-badge');
  badge.textContent='Premium'; badge.classList.remove('free'); badge.classList.add('premium');

  // Remove locks
  document.querySelectorAll('.ni-lock').forEach(l=>l.remove());

  // Unlock analytics page
  const ao=document.getElementById('analytics-overlay');
  const ai=document.getElementById('analytics-inner');
  if(ao){ao.style.display='none';}
  if(ai){ai.style.filter='none';ai.style.pointerEvents='auto';}

  // Unlock export page
  const eo=document.getElementById('export-overlay');
  const ei=document.getElementById('export-inner');
  if(eo){eo.style.display='none';}
  if(ei){ei.style.filter='none';ei.style.pointerEvents='auto';}

  // Unlock guided prompts in journal — remove blur overlay
  const guidedLock = document.querySelector('#jstep-4 [style*="position:absolute"]');
  if (guidedLock) guidedLock.style.display = 'none';
  const guidedBlur = document.querySelector('#jstep-4 [style*="filter:blur"]');
  if (guidedBlur) { guidedBlur.style.filter = 'none'; guidedBlur.style.pointerEvents = 'auto'; }

  // Upgrade card
  const uw=document.getElementById('upgrade-card-wrap');
  if(uw) uw.innerHTML=`<div style="background:rgba(255,255,255,.1);border:1px solid rgba(255,255,255,.18);border-radius:14px;padding:14px 16px;text-align:center;"><span style="font-size:20px">✨</span><div style="color:#fff;font-size:12.5px;font-weight:700;margin-top:5px;">Premium Aktif</div><div style="color:rgba(255,255,255,.5);font-size:10.5px;margin-top:2px;">Semua fitur terbuka</div></div>`;

  showToast('🎉 Premium aktif! Selamat menikmati semua fitur.');
  initCharts();
}

// ================================================================
// TOAST
// ================================================================
function showToast(msg) {
  const el=document.getElementById('toast');
  el.textContent=msg; el.classList.add('show');
  setTimeout(()=>el.classList.remove('show'),3200);
}

// ================================================================
// BLUEPRINT PAGE
// ================================================================
function buildBlueprintPage() {
  // FLOW DIAGRAM
  const fd = document.getElementById('flow-diagram');
  if (fd) {
    const steps = [
      {icon:'👤', title:'Landing Page / Registrasi', desc:'User membuka landing page Awaremind → Klik "Mulai Gratis" → Isi nama & email → Verifikasi (opsional via Google OAuth)'},
      {icon:'🏠', title:'Dashboard Pertama Kali', desc:'Disambut greeting + prompt onboarding → Ditampilkan kalender streak kosong + CTA "Mulai Jurnal Hari Ini"'},
      {icon:'🧪', title:'Cek-in Hormonal (Step 1)', desc:'Geser 4 slider hormon (Dopamine, Serotonin, Oksitosin, Kortisol) → Real-time insight muncul → Mood Ring terupdate secara live'},
      {icon:'🙏', title:'Gratitude Log (Step 2)', desc:'Isi 3 hal syukur dengan placeholder yang memandu → Data disimpan ke state sementara'},
      {icon:'🌊', title:'Flow State Tracker (Step 3)', desc:'Pilih skor 1–10 dengan feedback kontekstual → Input aktivitas flow → Dapat referensi teori Csikszentmihalyi'},
      {icon:'✍️', title:'Jurnal Bebas + Guided Prompts (Step 4)', desc:'FREE: Jurnal teks bebas tanpa batas karakter | PREMIUM: 12+ guided prompts tematik terkuak (Mindfulness, CBT, Strengths)'},
      {icon:'💾', title:'Simpan Entri', desc:'Klik "Simpan" → Data disimpan ke localStorage (demo) / database (produksi) → Mood ring dashboard terupdate → Streak +1'},
      {icon:'📊', title:'Analitik (Premium)', desc:'Dashboard visual: line chart tren 7/30 hari, radar hormonal, bar distribusi, keyword cloud emosi dari NLP jurnal'},
      {icon:'🔗', title:'Ekspor ke HealMind (Premium)', desc:'Pilih konten yang akan diekspor → Klik "Kirim ke HealMind" → API call ke Google Apps Script HealMind → Konselor menerima notifikasi & dashboard update sebelum sesi'},
    ];
    fd.innerHTML = steps.map((s,i)=>`
      <div style="display:flex;gap:16px;padding:16px 0;${i<steps.length-1?'border-bottom:1px solid var(--sand-l);':''}">
        <div style="width:44px;height:44px;border-radius:12px;background:${i%3===0?'var(--bg2)':i%3===1?'#edf7e5':'#fef3e2'};border:1px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:20px;flex-shrink:0;">${s.icon}</div>
        <div>
          <div style="font-weight:800;font-size:13.5px;color:var(--text);margin-bottom:3px;">${i+1}. ${s.title}</div>
          <div style="font-size:12.5px;color:var(--text2);line-height:1.6;">${s.desc}</div>
        </div>
      </div>`).join('');
  }

  // DB SCHEMA
  const db = document.getElementById('db-schema');
  if (db) {
    const tables = [
      {
        name:'users',color:'#27470E',
        cols:[
          {n:'id',t:'UUID PRIMARY KEY',d:'Identifier unik'},
          {n:'name',t:'VARCHAR(100)',d:'Nama pengguna'},
          {n:'email',t:'VARCHAR(255) UNIQUE',d:'Email login'},
          {n:'password_hash',t:'TEXT',d:'Bcrypt hash'},
          {n:'plan',t:"ENUM('free','premium')",d:'Status berlangganan'},
          {n:'premium_until',t:'TIMESTAMP',d:'Tanggal expiry premium'},
          {n:'healmind_user_id',t:'VARCHAR',d:'ID user di sistem HealMind (opsional)'},
          {n:'created_at',t:'TIMESTAMP',d:'Waktu registrasi'},
        ]
      },
      {
        name:'journal_entries',color:'#45B585',
        cols:[
          {n:'id',t:'UUID PRIMARY KEY',d:'ID entri'},
          {n:'user_id',t:'UUID → FK users.id',d:'Relasi ke pengguna'},
          {n:'created_at',t:'TIMESTAMP',d:'Tanggal entri'},
          {n:'journal_text',t:'TEXT',d:'Isi jurnal bebas'},
          {n:'flow_score',t:'SMALLINT (1-10)',d:'Skor flow state'},
          {n:'flow_activity',t:'VARCHAR(200)',d:'Aktivitas yang terasa flow'},
          {n:'gratitude_1',t:'TEXT',d:'Syukur pertama'},
          {n:'gratitude_2',t:'TEXT',d:'Syukur kedua'},
          {n:'gratitude_3',t:'TEXT',d:'Syukur ketiga'},
        ]
      },
      {
        name:'hormone_logs',color:'#F4A261',
        cols:[
          {n:'id',t:'UUID PRIMARY KEY',d:'ID log'},
          {n:'entry_id',t:'UUID → FK journal_entries.id',d:'Relasi ke entri'},
          {n:'user_id',t:'UUID → FK users.id',d:'Relasi ke pengguna'},
          {n:'logged_at',t:'TIMESTAMP',d:'Waktu pencatatan'},
          {n:'dopamine',t:'SMALLINT (0-100)',d:'Level dopamine'},
          {n:'serotonin',t:'SMALLINT (0-100)',d:'Level serotonin'},
          {n:'oxytocin',t:'SMALLINT (0-100)',d:'Level oksitosin'},
          {n:'cortisol',t:'SMALLINT (0-100)',d:'Level kortisol'},
          {n:'wellbeing_score',t:'DECIMAL(5,2)',d:'Skor wellbeing dihitung otomatis'},
        ]
      },
      {
        name:'subscriptions',color:'#9B8DEA',
        cols:[
          {n:'id',t:'UUID PRIMARY KEY',d:'ID langganan'},
          {n:'user_id',t:'UUID → FK users.id',d:'Relasi ke pengguna'},
          {n:'plan',t:"ENUM('free','premium')",d:'Tipe plan'},
          {n:'started_at',t:'TIMESTAMP',d:'Mulai berlangganan'},
          {n:'expires_at',t:'TIMESTAMP',d:'Expiry date'},
          {n:'payment_gateway',t:"VARCHAR",d:'midtrans / stripe'},
          {n:'status',t:"ENUM('active','expired','cancelled')",d:'Status'},
          {n:'transaction_id',t:'VARCHAR',d:'Referensi transaksi'},
        ]
      },
    ];

    db.innerHTML = tables.map(t=>`
      <div style="margin-bottom:22px;">
        <div style="display:inline-flex;align-items:center;gap:8px;background:${t.color};color:#fff;padding:5px 14px;border-radius:8px 8px 0 0;font-size:12px;font-weight:800;font-family:monospace;letter-spacing:.04em;">TABLE: ${t.name}</div>
        <div style="border:1.5px solid ${t.color};border-radius:0 10px 10px 10px;overflow:hidden;">
          <table style="width:100%;border-collapse:collapse;font-size:12.5px;">
            <thead><tr style="background:${t.color}18;">
              <th style="text-align:left;padding:8px 12px;color:var(--text2);font-weight:800;border-bottom:1px solid ${t.color}40;width:28%">Column</th>
              <th style="text-align:left;padding:8px 12px;color:var(--text2);font-weight:800;border-bottom:1px solid ${t.color}40;width:34%">Type</th>
              <th style="text-align:left;padding:8px 12px;color:var(--text2);font-weight:800;border-bottom:1px solid ${t.color}40">Keterangan</th>
            </tr></thead>
            <tbody>${t.cols.map((c,i)=>`<tr style="background:${i%2?'transparent':'rgba(0,0,0,.015)'};">
              <td style="padding:7px 12px;font-family:monospace;color:${t.color};font-weight:700;">${c.n}</td>
              <td style="padding:7px 12px;font-family:monospace;color:var(--text2);font-size:11.5px;">${c.t}</td>
              <td style="padding:7px 12px;color:var(--text3);font-size:12px;">${c.d}</td>
            </tr>`).join('')}</tbody>
          </table>
        </div>
      </div>`).join('');
  }

  // TECH STACK
  const ts = document.getElementById('tech-stack');
  if (ts) {
    const stack = [
      {cat:'Frontend',color:'#45B585',items:[
        {name:'React.js + Vite','role':'SPA framework utama — komponen reusable, routing, state management'},
        {name:'TailwindCSS','role':'Utility-first styling yang konsisten dan scalable'},
        {name:'Chart.js / Recharts','role':'Visualisasi mood chart, radar, dan bar analytics'},
        {name:'React Hook Form + Zod','role':'Validasi form jurnal yang ringan dan type-safe'},
      ]},
      {cat:'Backend',color:'#27470E',items:[
        {name:'Node.js + Express / FastAPI (Python)','role':'REST API untuk auth, CRUD entries, analytics processing'},
        {name:'Supabase (PostgreSQL)','role':'Database utama + Auth + Real-time subscriptions'},
        {name:'Supabase Storage','role':'Menyimpan ekspor PDF yang digenerate'},
        {name:'JWT (JSON Web Tokens)','role':'Autentikasi stateless yang aman'},
      ]},
      {cat:'Premium & Payment',color:'#F4A261',items:[
        {name:'Midtrans (Snap)','role':'Payment gateway Indonesia — kartu kredit, transfer bank, e-wallet'},
        {name:'Webhook Midtrans','role':'Update status premium otomatis setelah pembayaran sukses'},
      ]},
      {cat:'Analytics & NLP',color:'#9B8DEA',items:[
        {name:'Node NLP / compromise.js','role':'Keyword extraction dari teks jurnal untuk mood pattern detection'},
        {name:'PDFKit / jsPDF','role':'Generasi PDF laporan wellbeing untuk ekspor'},
      ]},
      {cat:'Integrasi HealMind',color:'#B8623A',items:[
        {name:'Google Apps Script (HealMind)','role':'Menerima POST request dari MindJournal API → update sheet admin'},
        {name:'Webhook API Endpoint', role:'Endpoint khusus di GAS: doPost() → parsing JSON laporan → tulis ke Google Sheets'},
        {name:'Google Sheets','role':'Database admin HealMind — kolom: nama klien, summary mood, tanggal sesi'},
      ]},
    ];
    ts.innerHTML = stack.map(s=>`
      <div style="margin-bottom:18px;">
        <div style="font-size:11px;font-weight:800;text-transform:uppercase;letter-spacing:.12em;color:${s.color};margin-bottom:8px;display:flex;align-items:center;gap:6px;"><div style="width:10px;height:10px;border-radius:50%;background:${s.color}"></div>${s.cat}</div>
        <div style="display:flex;flex-direction:column;gap:6px;">
          ${s.items.map(i=>`<div style="display:flex;align-items:flex-start;gap:10px;background:var(--bg2);border:1px solid var(--border);border-radius:9px;padding:10px 13px;">
            <div style="font-size:13px;font-weight:700;color:var(--text);min-width:180px;flex-shrink:0;">${i.name}</div>
            <div style="font-size:12.5px;color:var(--text3);line-height:1.5;">${i.role}</div>
          </div>`).join('')}
        </div>
      </div>`).join('');
  }

  // INTEGRATION LOGIC
  const il = document.getElementById('integration-logic');
  if (il) {
    il.innerHTML = `
      <div style="font-size:13px;color:var(--text2);line-height:1.75;margin-bottom:16px;">Saat pengguna Premium menekan <strong>"Ekspor & Kirim ke HealMind"</strong>, sistem bekerja melalui alur berikut:</div>
      
      <div style="display:flex;flex-direction:column;gap:10px;margin-bottom:20px;">
        ${[
          {n:1, t:'Frontend mengirim POST ke backend MindJournal API', d:'Payload: { userId, periodDays: 30, includeOptions: {...} }'},
          {n:2, t:'Backend query Supabase', d:'Ambil hormone_logs + journal_entries 30 hari terakhir → Hitung averages, run NLP → Buat JSON laporan terstruktur'},
          {n:3, t:'Backend buat PDF via PDFKit', d:'Render laporan hormonal, grafik (base64), keyword cloud → Simpan ke Supabase Storage → Dapatkan signed URL'},
          {n:4, t:'Backend kirim POST ke HealMind GAS Webhook', d:`URL: https://script.google.com/macros/s/[DEPLOYMENT_ID]/exec\nBody: { clientName, clientEmail, wbAvg, dopaAvg, seroAvg, keywords[], pdfUrl, sessionId }`},
          {n:5, t:'Google Apps Script (doPost) memproses request', d:'Parse JSON → Tulis baris baru ke Google Sheets admin HealMind (kolom: Tanggal, Klien, Wellbeing, Mood Summary, PDF URL) → Kirim email notifikasi ke konselor'},
          {n:6, t:'Konselor menerima notifikasi', d:'Email: "Laporan baru dari [Klien] tersedia sebelum sesi [Tanggal]" + link PDF → Konselor buka dashboard HealMind → lihat ringkasan klien'},
          {n:7, t:'Response ke frontend', d:'{ success: true, pdfUrl, sentAt } → Tampilkan toast konfirmasi + countdown sebelum sesi'},
        ].map(s=>`
          <div style="display:flex;gap:12px;">
            <div style="width:28px;height:28px;border-radius:50%;background:var(--pri);color:#fff;font-size:12px;font-weight:800;display:flex;align-items:center;justify-content:center;flex-shrink:0;">${s.n}</div>
            <div style="background:var(--bg2);border:1px solid var(--border);border-radius:10px;padding:11px 14px;flex:1;">
              <div style="font-size:13px;font-weight:700;color:var(--text);margin-bottom:3px;">${s.t}</div>
              <div style="font-size:12px;color:var(--text3);line-height:1.6;font-family:${s.d.includes('https://')?'monospace':'inherit'}">${s.d}</div>
            </div>
          </div>`).join('')}
      </div>
      
      <div style="background:#edf7e5;border:1px solid #b8d9a0;border-radius:12px;padding:16px 18px;">
        <div style="font-size:11px;font-weight:800;text-transform:uppercase;letter-spacing:.1em;color:var(--pri);margin-bottom:8px;">📌 Catatan Penting untuk Integrasi GAS</div>
        <div style="font-size:12.5px;color:var(--pri-m);line-height:1.75;">
          • Set <code style="background:rgba(39,71,14,.1);padding:1px 5px;border-radius:4px">doPost(e)</code> di Apps Script dan deploy sebagai "Web App — siapa pun dapat mengakses"<br>
          • Gunakan <code style="background:rgba(39,71,14,.1);padding:1px 5px;border-radius:4px">LockService</code> untuk menghindari concurrent write ke Google Sheets<br>
          • Simpan DEPLOYMENT_ID di environment variable backend MindJournal (bukan di frontend)<br>
          • Tambahkan shared secret token di header untuk validasi request
        </div>
      </div>

      <div style="margin-top:18px;">
        <div style="font-size:11px;font-weight:800;text-transform:uppercase;letter-spacing:.1em;color:var(--text3);margin-bottom:10px;">💻 Contoh Google Apps Script — HealMind Webhook Receiver</div>
        <div style="background:#1e1e2e;border-radius:12px;padding:20px;overflow-x:auto;">
          <pre style="font-family:'Courier New',monospace;font-size:12px;line-height:1.75;color:#cdd6f4;white-space:pre-wrap;margin:0;"><span style="color:#89b4fa">// HealMind Admin — Google Apps Script Webhook</span>
<span style="color:#89b4fa">// Deploy sebagai: Web App → Anyone can access</span>

<span style="color:#cba6f7">const</span> <span style="color:#f38ba8">SHEET_NAME</span> = <span style="color:#a6e3a1">'Laporan Klien'</span>;
<span style="color:#cba6f7">const</span> <span style="color:#f38ba8">SECRET_TOKEN</span> = <span style="color:#a6e3a1">'mj_secret_xxxx'</span>; <span style="color:#89b4fa">// Samakan dgn backend MindJournal</span>

<span style="color:#cba6f7">function</span> <span style="color:#89dceb">doPost</span>(e) {
  <span style="color:#cba6f7">const</span> lock = LockService.<span style="color:#89dceb">getScriptLock</span>();
  lock.<span style="color:#89dceb">waitLock</span>(10000);

  <span style="color:#cba6f7">try</span> {
    <span style="color:#cba6f7">const</span> body = JSON.<span style="color:#89dceb">parse</span>(e.postData.contents);

    <span style="color:#89b4fa">// Validasi secret token</span>
    <span style="color:#cba6f7">if</span> (body.secretToken !== SECRET_TOKEN) {
      <span style="color:#cba6f7">return</span> ContentService
        .<span style="color:#89dceb">createTextOutput</span>(JSON.<span style="color:#89dceb">stringify</span>({error:<span style="color:#a6e3a1">'Unauthorized'</span>}))
        .<span style="color:#89dceb">setMimeType</span>(ContentService.MimeType.JSON);
    }

    <span style="color:#cba6f7">const</span> sheet = SpreadsheetApp
      .<span style="color:#89dceb">getActiveSpreadsheet</span>()
      .<span style="color:#89dceb">getSheetByName</span>(SHEET_NAME);

    <span style="color:#89b4fa">// Tulis data ke baris baru</span>
    sheet.<span style="color:#89dceb">appendRow</span>([
      <span style="color:#cba6f7">new</span> <span style="color:#89dceb">Date</span>(),                       <span style="color:#89b4fa">// Timestamp</span>
      body.clientName,                   <span style="color:#89b4fa">// Nama klien</span>
      body.clientEmail,                  <span style="color:#89b4fa">// Email klien</span>
      body.wellbeingAvg,                 <span style="color:#89b4fa">// Wellbeing score rata-rata</span>
      body.dopamineAvg,                  <span style="color:#89b4fa">// Rata-rata Dopamine</span>
      body.serotoninAvg,                 <span style="color:#89b4fa">// Rata-rata Serotonin</span>
      body.oxytocinAvg,                  <span style="color:#89b4fa">// Rata-rata Oksitosin</span>
      body.cortisol_inv_avg,             <span style="color:#89b4fa">// Anti-kortisol avg</span>
      body.flowAvg,                      <span style="color:#89b4fa">// Flow score rata-rata</span>
      body.topKeywords.<span style="color:#89dceb">join</span>(<span style="color:#a6e3a1">', '</span>),    <span style="color:#89b4fa">// Keyword emosi dominan</span>
      body.autoNote,                     <span style="color:#89b4fa">// Catatan otomatis untuk konselor</span>
      body.pdfUrl,                       <span style="color:#89b4fa">// URL PDF laporan (Supabase Storage)</span>
      body.periodDays,                   <span style="color:#89b4fa">// Periode data (30 hari)</span>
      <span style="color:#a6e3a1">'Menunggu Sesi'</span>                    <span style="color:#89b4fa">// Status sesi</span>
    ]);

    <span style="color:#89b4fa">// Kirim email notifikasi ke konselor</span>
    <span style="color:#cba6f7">const</span> konselorEmail = <span style="color:#a6e3a1">'konselor@awaremind.id'</span>;
    MailApp.<span style="color:#89dceb">sendEmail</span>({
      to: konselorEmail,
      subject: <span style="color:#a6e3a1">&#96;📋 Laporan Baru: ${body.clientName} — MindJournal&#96;</span>,
      htmlBody: <span style="color:#a6e3a1">&#96;&lt;h3&gt;Laporan Wellbeing Baru&lt;/h3&gt;
        &lt;p&gt;Klien &lt;strong&gt;${body.clientName}&lt;/strong&gt; telah mengirim laporan
        kondisi mental mereka sebelum sesi konseling.&lt;/p&gt;
        &lt;ul&gt;
          &lt;li&gt;Wellbeing Score: &lt;strong&gt;${body.wellbeingAvg}/100&lt;/strong&gt;&lt;/li&gt;
          &lt;li&gt;Flow Rata-rata: ${body.flowAvg}/10&lt;/li&gt;
          &lt;li&gt;Keyword Dominan: ${body.topKeywords.join(', ')}&lt;/li&gt;
        &lt;/ul&gt;
        &lt;p&gt;&lt;a href="${body.pdfUrl}"&gt;📄 Buka Laporan PDF&lt;/a&gt;&lt;/p&gt;&#96;</span>
    });

    <span style="color:#cba6f7">return</span> ContentService
      .<span style="color:#89dceb">createTextOutput</span>(JSON.<span style="color:#89dceb">stringify</span>({
        success: <span style="color:#fab387">true</span>,
        message: <span style="color:#a6e3a1">'Laporan berhasil diterima dan konselor telah dinotifikasi.'</span>
      }))
      .<span style="color:#89dceb">setMimeType</span>(ContentService.MimeType.JSON);

  } <span style="color:#cba6f7">catch</span>(err) {
    <span style="color:#cba6f7">return</span> ContentService
      .<span style="color:#89dceb">createTextOutput</span>(JSON.<span style="color:#89dceb">stringify</span>({error: err.message}))
      .<span style="color:#89dceb">setMimeType</span>(ContentService.MimeType.JSON);
  } <span style="color:#cba6f7">finally</span> {
    lock.<span style="color:#89dceb">releaseLock</span>();
  }
}</pre>
        </div>
      </div>
  `;
  }
}

// ================================================================
// USER PROFILE (name from localStorage)
// ================================================================
function loadProfile() {
  let name = localStorage.getItem('mj_username');
  if (!name) {
    name = prompt('Halo! Siapa nama panggilanmu?') || 'Sahabat';
    localStorage.setItem('mj_username', name);
  }
  document.getElementById('sb-name').innerHTML = name + ' <span class="plan-badge free" id="plan-badge">Free</span>';
  document.getElementById('avatar-letter').textContent = name.charAt(0).toUpperCase();

  const h = new Date().getHours();
  const g = h<12?'Selamat Pagi 🌅':h<17?'Selamat Siang ☀️':h<20?'Selamat Sore 🌤️':'Selamat Malam 🌙';
  document.getElementById('greeting').textContent = g + ', ' + name + '!';
}

// ================================================================
// EXPORT TO HEALMIND SIMULATION
// ================================================================
function doExport() {
  if (!state.isPremium) { openModal(); return; }
  const btn = document.getElementById('export-send-btn');
  if (!btn) return;

  // Loading state
  btn.disabled = true;
  btn.innerHTML = '<span id="exp-spinner" style="display:inline-block;animation:spin .7s linear infinite;">⏳</span> Mengirim laporan...';

  // Simulate multi-step async process
  const steps = [
    {delay:600, msg:'⚙️ Menganalisis data jurnal...'},
    {delay:1300, msg:'📊 Membuat ringkasan hormonal...'},
    {delay:2100, msg:'📄 Menyusun laporan PDF...'},
    {delay:2900, msg:'🔗 Menghubungkan ke HealMind...'},
    {delay:3700, msg:'✅ Laporan terkirim!'},
  ];

  steps.forEach(s => {
    setTimeout(() => {
      if (btn) btn.innerHTML = s.msg;
    }, s.delay);
  });

  setTimeout(() => {
    btn.disabled = false;
    btn.innerHTML = '✅ Laporan Sudah Dikirim ke Konselor';
    btn.style.background = 'var(--sero)';
    showToast('🎉 Laporan wellbeing-mu berhasil dikirim ke dashboard konselor HealMind!');

    // Show confirmation box
    const card = btn.closest('.card');
    if (card) {
      const conf = document.createElement('div');
      conf.style.cssText = 'background:#edf7e5;border:1px solid #a6d9c1;border-radius:10px;padding:14px 16px;margin-top:12px;font-size:13px;color:#1a6040;line-height:1.7;';
      conf.innerHTML = `<strong>📬 Terkirim pada ${new Date().toLocaleTimeString('id-ID', {hour:'2-digit',minute:'2-digit'})}</strong><br>Konselormu akan menerima notifikasi email beserta laporan PDF. Data mencakup: grafik hormon 30 hari, keyword emosi dominan, rata-rata flow state, dan catatan wellbeing otomatis.<br><br><span style="font-size:11px;opacity:.7;">🔒 Enkripsi end-to-end · Hanya konselor yang ditunjuk yang dapat mengakses.</span>`;
      card.appendChild(conf);
    }
  }, 4100);
}

function downloadPDF() {
  if (!state.isPremium) { openModal(); return; }
  const btn = document.getElementById('export-pdf-btn');
  if (!btn) return;
  const orig = btn.innerHTML;
  btn.disabled = true;
  btn.innerHTML = '⏳ Menyiapkan PDF...';
  setTimeout(() => {
    btn.disabled = false;
    btn.innerHTML = orig;
    showToast('📄 Laporan PDF siap! (Dalam produksi: file akan otomatis terunduh)');
  }, 1800);
}

// ================================================================
// START
// ================================================================
init();
</script>
</body>
</html>
