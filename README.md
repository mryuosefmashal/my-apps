<!doctype html><html><head><meta charset=utf8><meta name=viewport content="width=device-width,initial-scale=1,viewport-fit=cover"><style>:root{color-scheme:light;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}html{scroll-padding-top:env(safe-area-inset-top,0px)}body{margin:0;padding:0;font:14px -apple-system,BlinkMacSystemFont,sans-serif;background:#fff;color:#000}img{max-width:100%}[hidden]:not([hidden=until-found i]){display:none!important}</style></head><body>
<title>القراءة في البيت</title>
<meta name="claude:viewport-fit-sides" content="cover">
<script>document.documentElement.lang="ar";document.documentElement.dir="rtl";</script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Noto+Naskh+Arabic:wght@400;500;600;700&display=swap">
<style>
/* Layout: classroom board — school header, step strip, one big reading stage. Sizes are in rem and the root size grows with the screen, so the page scales up on interactive boards and down on phones. */
:root{
  --bg:#EAF6FF; --bg2:#D4ECFF; --card:#FFFFFF; --ink:#1D2A4D; --muted:#5A6B8F; --line:#C9E0F5;
  --a:#FF5F6D; --b:#FFB21E; --c:#22B573; --d:#8B5CF6; --sky:#2F86F6; --orange:#FF8A3D;
  --a-soft:#FFE3E6; --b-soft:#FFF1CF; --c-soft:#D8F5E7; --d-soft:#ECE3FF; --sky-soft:#DCEBFF; --o-soft:#FFE6D4;
  --on-b:#3A2500; --white:#FFFFFF; --hl:#FFE27A;
  --shadow:0 .375rem 0 rgba(29,42,77,.13); --shadow-sm:0 .2rem 0 rgba(29,42,77,.12);
  --font:"Noto Naskh Arabic","Amiri","Traditional Arabic","Simplified Arabic",serif;
  font-size:clamp(15px, .7vw + 8.5px, 28px);
}
@media (prefers-color-scheme: dark){:root:not([data-theme="light"]){
  --bg:#0E1931; --bg2:#14254A; --card:#1A2C55; --ink:#F1F5FF; --muted:#A8B7DA; --line:#2B3F6E;
  --a-soft:#4A2131; --b-soft:#4A3712; --c-soft:#143F33; --d-soft:#33275E; --sky-soft:#1B3768; --o-soft:#4A2C17; --hl:#7A6420;
  --shadow:0 .375rem 0 rgba(0,0,0,.35); --shadow-sm:0 .2rem 0 rgba(0,0,0,.3); color-scheme:dark}}
:root[data-theme="dark"]{
  --bg:#0E1931; --bg2:#14254A; --card:#1A2C55; --ink:#F1F5FF; --muted:#A8B7DA; --line:#2B3F6E;
  --a-soft:#4A2131; --b-soft:#4A3712; --c-soft:#143F33; --d-soft:#33275E; --sky-soft:#1B3768; --o-soft:#4A2C17; --hl:#7A6420;
  --shadow:0 .375rem 0 rgba(0,0,0,.35); --shadow-sm:0 .2rem 0 rgba(0,0,0,.3); color-scheme:dark}

*{box-sizing:border-box}
html,body{min-height:100%}
body{direction:rtl;margin:0;background:var(--bg);color:var(--ink);font-family:var(--font);font-size:1.125rem;line-height:1.7;
  background-image:radial-gradient(circle at 12% 18%,var(--bg2) 0 4.5rem,transparent 4.55rem),
  radial-gradient(circle at 88% 70%,var(--bg2) 0 7rem,transparent 7.05rem),
  radial-gradient(circle at 70% 8%,var(--bg2) 0 2.5rem,transparent 2.55rem);
  background-attachment:fixed}
button,input,textarea,select{font-family:var(--font);font-size:inherit;color:inherit}
button{cursor:pointer;touch-action:manipulation}
:focus-visible{outline:3px solid var(--sky);outline-offset:3px}
.wrap{max-width:72rem;margin:0 auto;padding-left:max(16px,env(safe-area-inset-left,0px));padding-right:max(16px,env(safe-area-inset-right,0px));padding-block:.9rem 2.5rem}

/* avatars */
.ava{display:inline-grid;place-items:center;width:1.25em;height:1.25em;line-height:1;flex:none}
.ava svg{width:100%;height:100%;display:block}

/* header */
.top{display:flex;align-items:center;gap:1rem;flex-wrap:wrap;background:var(--card);border:3px solid var(--line);border-radius:1.6rem;padding:.6rem 1.1rem;box-shadow:var(--shadow)}
.logo{width:5.6rem;height:6.8rem;flex:none;display:block;object-fit:contain;filter:drop-shadow(0 .2rem 0 rgba(29,42,77,.15))}
.brand{flex:1;min-width:12rem}
.brand h1{margin:0;font-size:clamp(1.4rem,3.2vw,2.1rem);font-weight:700;line-height:1.4;text-wrap:balance}
.brand p{margin:0;color:var(--muted);font-size:1.1rem;font-weight:600}
.brand p b{color:var(--a)}
.tools{display:flex;gap:.5rem;flex-wrap:wrap;align-items:flex-end}
.lessonpick{display:flex;flex-direction:column;gap:2px}
.lessonpick label{font-size:.8rem;color:var(--muted);font-weight:600}
select{background:var(--bg);border:2px solid var(--line);border-radius:.9rem;padding:.25rem .75rem;max-width:15rem;font-weight:600;min-height:2.6rem}
.iconbtn{border:2px solid var(--line);background:var(--bg);border-radius:.9rem;padding:.3rem .8rem;font-weight:700;display:inline-flex;gap:.4rem;align-items:center;box-shadow:var(--shadow-sm);transition:transform .12s;min-height:2.6rem;font-size:1rem}
.iconbtn:hover{transform:translateY(-2px)}
.iconbtn:active{transform:translateY(2px);box-shadow:none}

/* steps strip */
.steps{display:flex;gap:.6rem;justify-content:center;flex-wrap:wrap;margin:1.1rem 0 .9rem}
.step{display:flex;align-items:center;gap:.5rem;border:2px solid var(--line);background:var(--card);border-radius:999px;padding:.25rem 1rem .25rem .5rem;font-weight:700;color:var(--muted);font-size:1.05rem;min-height:2.8rem}
.step .n{width:1.9rem;height:1.9rem;border-radius:50%;display:grid;place-items:center;background:var(--bg2);color:var(--ink)}
.step.on{border-color:var(--sky);color:var(--ink)}
.step.on .n{background:var(--sky);color:var(--white)}
.step.done .n{background:var(--c);color:var(--white)}
.step:disabled{opacity:.55;cursor:default}
.step.res{border-color:var(--d);color:var(--ink);background:var(--d-soft)}
.step.res .n{background:var(--d);color:var(--white)}
.step.res.on{box-shadow:0 0 0 3px var(--d)}

.view{animation:pop .35s ease}
@keyframes pop{from{transform:translateY(10px) scale(.98);opacity:.4}to{transform:none;opacity:1}}
.h2{text-align:center;font-size:clamp(1.5rem,3.6vw,2.2rem);margin:.4rem 0 .2rem;font-weight:700}
.sub{text-align:center;color:var(--muted);margin:0 0 1.1rem;font-weight:500}

/* section cards */
.secgrid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:1.4rem;max-width:48rem;margin:0 auto}
.seccard{border:none;border-radius:2rem;padding:1.6rem 1rem 1.25rem;color:var(--white);box-shadow:var(--shadow);display:flex;flex-direction:column;align-items:center;gap:.25rem;transition:transform .15s;position:relative;overflow:hidden}
.seccard:hover{transform:translateY(-4px) rotate(-1deg)}
.seccard:active{transform:translateY(3px)}
.seccard.sa{background:var(--a)}
.seccard.sb{background:var(--sky)}
.seccard .big{font-size:clamp(4.4rem,12vw,7rem);font-weight:700;line-height:1.2;text-shadow:0 .3rem 0 rgba(0,0,0,.15)}
.seccard .lbl{font-size:1.5rem;font-weight:700}
.seccard .cnt{font-size:1rem;background:rgba(255,255,255,.25);border-radius:999px;padding:0 .9rem}
.seccard .emo{position:absolute;font-size:2.4rem;top:.7rem;inset-inline-start:1rem}
.listenCard{max-width:48rem;margin:1.4rem auto 0;display:flex;align-items:center;gap:1rem;background:var(--d);color:var(--white);border:none;border-radius:1.6rem;padding:.9rem 1.4rem;box-shadow:var(--shadow);width:100%;text-align:start;transition:transform .15s}
.listenCard:hover{transform:translateY(-3px)}
.listenCard .big{font-size:2.6rem;line-height:1}
.listenCard b{font-size:1.4rem;display:block}
.listenCard span.s{font-size:1rem;opacity:.9}

/* picker */
.pickbox{background:var(--card);border:3px solid var(--line);border-radius:2rem;padding:1.4rem 1.1rem;box-shadow:var(--shadow);text-align:center;max-width:46rem;margin:0 auto}
.slot{margin:.4rem auto 1rem;min-height:8rem;border-radius:1.5rem;background:var(--b-soft);border:3px dashed var(--b);display:grid;place-items:center;padding:.6rem .9rem}
.slot .nm{font-size:clamp(1.75rem,5vw,2.9rem);font-weight:700;line-height:1.5}
.slot .av{font-size:3rem;line-height:1}
.slot.spin .nm{color:var(--muted)}
.slot.got{background:var(--c-soft);border-color:var(--c);border-style:solid;animation:bounce .5s}
@keyframes bounce{0%{transform:scale(.9)}60%{transform:scale(1.05)}100%{transform:scale(1)}}
.row{display:flex;gap:.75rem;justify-content:center;flex-wrap:wrap;align-items:center}
.btn{border:none;border-radius:1.25rem;padding:.6rem 1.6rem;font-size:1.3rem;font-weight:700;box-shadow:var(--shadow);transition:transform .12s;display:inline-flex;align-items:center;gap:.5rem;min-height:3.2rem}
.btn:hover{transform:translateY(-2px)}
.btn:active{transform:translateY(4px);box-shadow:none}
.btn:disabled{opacity:.5;cursor:default;transform:none}
.btn.go{background:var(--b);color:var(--on-b)}
.btn.ok{background:var(--c);color:var(--white)}
.btn.no{background:var(--orange);color:var(--white)}
.btn.blue{background:var(--sky);color:var(--white)}
.btn.purple{background:var(--d);color:var(--white)}
.btn.ghost{background:var(--card);color:var(--ink);border:3px solid var(--line)}
.btn.huge{font-size:1.55rem;padding:.8rem 2rem}
.pulse{animation:pulse 1.2s infinite}
@keyframes pulse{0%,100%{transform:scale(1)}50%{transform:scale(1.06)}}
.namesHead{display:flex;justify-content:space-between;align-items:center;gap:.6rem;flex-wrap:wrap;margin:1.6rem auto .6rem;max-width:64rem}
.namesHead h3{margin:0;font-size:1.4rem}
.namesHead small{color:var(--muted);font-size:.95rem}
.names{display:grid;grid-template-columns:repeat(auto-fill,minmax(14rem,1fr));gap:.6rem;max-width:64rem;margin:0 auto}
.nameBtn{display:flex;align-items:center;gap:.5rem;text-align:start;background:var(--card);border:2px solid var(--line);border-radius:1rem;padding:.4rem .65rem;font-weight:600;font-size:1.05rem;line-height:1.5;transition:transform .12s;min-height:3rem}
.nameBtn:hover{transform:translateY(-2px);border-color:var(--sky)}
.nameBtn .ava{font-size:1.6rem}
.nameBtn .t{flex:1;min-width:0}
.nameBtn.picked{background:var(--bg2);opacity:.7}
.dots{display:flex;gap:3px}
.dots i{width:.6rem;height:.6rem;border-radius:50%;background:var(--line);display:block}
.dots i.pa{background:var(--a)}.dots i.pb{background:var(--b)}.dots i.pc{background:var(--c)}.dots i.pd{background:var(--d)}
.dots i.f{background:transparent;box-shadow:inset 0 0 0 2px var(--orange)}

/* reading */
.reader{display:flex;flex-direction:column;gap:.9rem}
.who{display:flex;align-items:center;gap:.75rem;flex-wrap:wrap;background:var(--card);border:3px solid var(--line);border-radius:1.5rem;padding:.5rem .9rem;box-shadow:var(--shadow-sm)}
.who .avbox{display:flex;flex-direction:column;align-items:center;line-height:1.2}
.who .avbox .ava{font-size:2.8rem}
.who .avbox small{font-size:.8rem;color:var(--muted);font-weight:700}
.who .nm{font-size:clamp(1.4rem,3vw,1.9rem);font-weight:700;line-height:1.4}
.who .meta{color:var(--muted);font-size:.95rem;font-weight:600}
.who .grow{flex:1;min-width:10rem}
.tabs{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:.75rem}
.tab{border:3px solid transparent;border-radius:1.4rem;padding:.5rem .4rem;background:var(--card);box-shadow:var(--shadow-sm);display:flex;flex-direction:column;align-items:center;font-weight:700;position:relative;transition:transform .12s}
.tab:hover{transform:translateY(-3px)}
.tab .L{width:2.9rem;height:2.9rem;border-radius:50%;display:grid;place-items:center;font-size:1.75rem;color:var(--white);line-height:1}
.tab .nmx{font-size:1.05rem}
.tab .ic{font-size:1.25rem;position:absolute;top:.25rem;inset-inline-end:.5rem}
.tab .chk{position:absolute;top:-.5rem;inset-inline-start:-.4rem;color:var(--white);border-radius:50%;width:1.75rem;height:1.75rem;display:grid;place-items:center;font-size:1rem;box-shadow:var(--shadow-sm)}
.tab .chk.ok{background:var(--c)} .tab .chk.no{background:var(--orange)}
.tab[data-k="a"] .L{background:var(--a)} .tab[data-k="b"] .L{background:var(--b);color:var(--on-b)} .tab[data-k="c"] .L{background:var(--c)} .tab[data-k="d"] .L{background:var(--d)}
.tab.on[data-k="a"]{border-color:var(--a);background:var(--a-soft)}
.tab.on[data-k="b"]{border-color:var(--b);background:var(--b-soft)}
.tab.on[data-k="c"]{border-color:var(--c);background:var(--c-soft)}
.tab.on[data-k="d"]{border-color:var(--d);background:var(--d-soft)}
.stage{background:var(--card);border:3px solid var(--line);border-radius:1.9rem;padding:1.1rem clamp(.9rem,3vw,1.9rem) 1.4rem;box-shadow:var(--shadow)}
.stage[data-k="a"]{border-color:var(--a)} .stage[data-k="b"]{border-color:var(--b)} .stage[data-k="c"]{border-color:var(--c)} .stage[data-k="d"]{border-color:var(--d)}
.stHead{display:flex;align-items:center;gap:.6rem;flex-wrap:wrap;margin-bottom:.4rem}
.stHead h2{margin:0;font-size:clamp(1.4rem,3vw,1.9rem)}
.stHead .hint{color:var(--muted);font-size:1rem;flex:1;min-width:12rem}
.tog{display:inline-flex;align-items:center;gap:.4rem;font-size:1rem;font-weight:600;background:var(--bg);border:2px solid var(--line);border-radius:999px;padding:.15rem .75rem;min-height:2.6rem}
.tog input{width:1.2rem;height:1.2rem}
.items{display:flex;flex-wrap:wrap;gap:1rem;justify-content:center;margin:.9rem 0 1.25rem}
.item{border:3px solid var(--line);background:var(--bg);border-radius:1.5rem;font-weight:600;position:relative;transition:transform .15s,background .2s,border-color .2s;line-height:2.1;color:var(--ink)}
.item:hover{transform:translateY(-3px)}
.item .st{position:absolute;top:-.75rem;inset-inline-end:-.5rem;font-size:1.6rem;opacity:0;transform:scale(.3);transition:.25s}
.item.read .st{opacity:1;transform:scale(1)}
.item .tag{position:absolute;bottom:-.75rem;left:50%;transform:translateX(-50%);font-size:.8rem;line-height:1.6;background:var(--card);border:2px solid var(--line);border-radius:999px;padding:0 .6rem;white-space:nowrap;color:var(--muted);font-weight:700}
.items.sent{flex-direction:column;align-items:stretch}
.items.sent .item{font-size:clamp(1.55rem,3.8vw,2.4rem);padding:.6rem 1.4rem .6rem 3.4rem;text-align:right}
.items.sent .item .num{position:absolute;left:.75rem;top:50%;transform:translateY(-50%);width:2.1rem;height:2.1rem;border-radius:50%;background:var(--a);color:var(--white);display:grid;place-items:center;font-size:1.1rem;line-height:1}
.stage[data-k="a"] .item.read{background:var(--a-soft);border-color:var(--a)}
.items.word .item{font-size:clamp(2rem,5vw,3.1rem);padding:.6rem 1.9rem .9rem;min-width:9.5rem}
.stage[data-k="b"] .item.read{background:var(--b-soft);border-color:var(--b)}
.lv{display:inline-flex;gap:3px;vertical-align:middle}
.lv i{width:.5rem;height:.5rem;border-radius:50%;background:var(--line);display:block}
.lv i.f{background:var(--b)}
.items.syl .item{font-size:clamp(2.4rem,6vw,3.75rem);min-width:7.5rem;height:8.1rem;display:grid;place-items:center;padding:0 1.4rem}
.items.syl .item.short{border-radius:50%;width:8.1rem;min-width:0;padding:0}
.items.syl .item.long{border-radius:2.5rem;min-width:11rem;border-color:var(--c)}
.stage[data-k="c"] .item.read{background:var(--c-soft);border-color:var(--c)}
.items.let .item{font-size:clamp(3.4rem,9vw,5.25rem);width:8.1rem;height:8.75rem;display:grid;place-items:center;border-radius:1.75rem;line-height:1.4}
.stage[data-k="d"] .item.read{background:var(--d-soft);border-color:var(--d)}
.actions{display:flex;justify-content:space-between;align-items:center;gap:.75rem;flex-wrap:wrap;border-top:3px dotted var(--line);padding-top:1rem}
.progressTxt{color:var(--muted);font-weight:600;font-size:1rem}
.empty{text-align:center;color:var(--muted);padding:1.9rem}

/* results */
.resBar{display:flex;justify-content:space-between;align-items:center;gap:.75rem;flex-wrap:wrap;margin-bottom:.8rem}
.segs{display:flex;gap:.4rem;background:var(--card);border:3px solid var(--line);border-radius:999px;padding:.25rem}
.seg{border:none;background:none;border-radius:999px;padding:.3rem 1.2rem;font-weight:700;font-size:1.1rem;color:var(--muted);min-height:2.6rem}
.seg.on{background:var(--sky);color:var(--white)}
.sumrow{display:flex;gap:.6rem;flex-wrap:wrap;margin-bottom:.8rem}
.chip{background:var(--card);border:2px solid var(--line);border-radius:999px;padding:.2rem .9rem;font-weight:700;font-size:1rem}
.chip b{font-variant-numeric:tabular-nums}
.chip.g{border-color:var(--c);background:var(--c-soft)} .chip.o{border-color:var(--orange);background:var(--o-soft)}
.tblwrap{overflow-x:auto;background:var(--card);border:3px solid var(--line);border-radius:1.5rem;box-shadow:var(--shadow-sm)}
table.res{width:100%;border-collapse:collapse;font-size:1.05rem}
table.res th,table.res td{padding:.35rem .5rem;border-bottom:2px solid var(--line);text-align:center;vertical-align:middle}
table.res th{background:var(--bg2);font-size:1rem;line-height:1.4;white-space:nowrap}
table.res th small{display:block;font-weight:600;color:var(--muted);font-size:.8rem}
table.res td.num{color:var(--muted);font-variant-numeric:tabular-nums}
table.res td.nm{text-align:right;white-space:nowrap;font-weight:600}
table.res td.nm .ava{font-size:1.4rem;vertical-align:middle;margin-inline-end:.3rem}
table.res tr:last-child td{border-bottom:none}
.cell{width:2.6rem;height:2.6rem;border-radius:50%;border:2px dashed var(--line);background:var(--bg);font-size:1.2rem;font-weight:700;color:var(--muted)}
.cell.pass{background:var(--c);border:2px solid var(--c);color:var(--white)}
.cell.fail{background:var(--orange);border:2px solid var(--orange);color:var(--white)}
.badge{display:inline-block;border-radius:999px;padding:.05rem .7rem;font-weight:700;font-size:.95rem;white-space:nowrap}
.badge.full{background:var(--c-soft);color:var(--ink);border:2px solid var(--c)}
.badge.follow{background:var(--o-soft);color:var(--ink);border:2px solid var(--orange)}
.badge.part{background:var(--sky-soft);color:var(--ink);border:2px solid var(--sky)}
.badge.none{color:var(--muted)}
.sync{font-size:.95rem;font-weight:700}
.sync.ok{color:var(--c)} .sync.local{color:var(--orange)}

/* modals */
.overlay{position:fixed;inset:0;background:rgba(10,20,45,.55);z-index:50;display:grid;place-items:center;padding:16px max(16px,env(safe-area-inset-right,0px)) 16px max(16px,env(safe-area-inset-left,0px));overflow:auto}
.modal{background:var(--card);border-radius:1.75rem;border:3px solid var(--line);width:min(52rem,100%);max-height:calc(100vh - 32px);overflow:auto;padding:1.25rem clamp(.9rem,3vw,1.75rem);box-shadow:var(--shadow);animation:pop .3s}
.modal h2{margin:0 0 .25rem;font-size:1.75rem}
.field{display:flex;flex-direction:column;gap:.25rem;margin:.6rem 0}
.field label{font-weight:700}
.field input,.field textarea{background:var(--bg);border:2px solid var(--line);border-radius:1rem;padding:.5rem .9rem;line-height:2;width:100%}
.field textarea{min-height:12rem;resize:vertical;font-size:1.25rem}
.prev{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:.6rem;margin:.75rem 0}
.pv{border-radius:1.1rem;padding:.5rem .9rem;border:2px solid var(--line);min-width:0}
.pv h4{margin:0;font-size:1.05rem;display:flex;justify-content:space-between;gap:.5rem}
.pv p{margin:2px 0 0;font-size:1.05rem;color:var(--muted);overflow-wrap:anywhere;line-height:1.9}
.pv.a{background:var(--a-soft)}.pv.b{background:var(--b-soft)}.pv.c{background:var(--c-soft)}.pv.d{background:var(--d-soft)}
.lessonList{display:flex;flex-direction:column;gap:.4rem;margin-top:.5rem}
.lessonList div{display:flex;justify-content:space-between;align-items:center;gap:.5rem;background:var(--bg);border-radius:.9rem;padding:.25rem .75rem;font-weight:600}
.small{font-size:.95rem;color:var(--muted)}
.err{color:var(--a);font-weight:700}
.toast{position:fixed;bottom:calc(20px + env(safe-area-inset-bottom,0px));left:50%;transform:translateX(-50%);background:var(--ink);color:var(--bg);padding:.5rem 1.4rem;border-radius:999px;font-weight:700;z-index:80;box-shadow:var(--shadow);max-width:calc(100% - 32px);text-align:center}

/* celebration / retry */
.cele{position:fixed;inset:0;z-index:60;display:grid;place-items:center;background:radial-gradient(circle,rgba(255,178,30,.35),rgba(10,20,45,.7));padding:16px;overflow:auto}
.cele.retry{background:radial-gradient(circle,rgba(255,138,61,.3),rgba(10,20,45,.7))}
.celeCard{background:var(--card);border-radius:2.25rem;border:5px solid var(--b);padding:1.5rem 1.6rem;text-align:center;width:min(36rem,100%);box-shadow:0 .6rem 0 rgba(0,0,0,.2);animation:zoom .6s cubic-bezier(.2,1.6,.4,1)}
.retry .celeCard{border-color:var(--orange)}
@keyframes zoom{from{transform:scale(.3) rotate(-8deg);opacity:0}to{transform:none;opacity:1}}
.celeCard .trophy{font-size:6rem;line-height:1.1;animation:wig 1s ease-in-out infinite}
.retry .celeCard .trophy{animation:float 2s ease-in-out infinite}
@keyframes wig{0%,100%{transform:rotate(-8deg)}50%{transform:rotate(8deg) scale(1.08)}}
@keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-.5rem)}}
.celeCard h2{margin:.25rem 0;font-size:clamp(1.9rem,6vw,2.75rem);color:var(--a)}
.retry .celeCard h2{color:var(--orange)}
.celeCard .nm{font-size:clamp(1.5rem,4.5vw,2.1rem);font-weight:700;display:flex;justify-content:center;align-items:center;gap:.4rem;flex-wrap:wrap}
.celeCard .what{color:var(--muted);font-weight:600;margin:.25rem 0 .4rem}
.stars{font-size:2.5rem;letter-spacing:.4rem;margin-bottom:.75rem}
.stars span{display:inline-block;animation:starIn .5s both}
.stars span:nth-child(2){animation-delay:.15s}.stars span:nth-child(3){animation-delay:.3s}
@keyframes starIn{from{transform:scale(0) rotate(-90deg)}to{transform:none}}
#confetti{position:fixed;inset:0;pointer-events:none;z-index:70;width:100%;height:100%}

@media (max-width:700px){
  .tabs{grid-template-columns:repeat(2,minmax(0,1fr))}
  .secgrid{gap:.75rem}
  .prev{grid-template-columns:1fr}
  .logo{width:4.2rem;height:5.1rem}
  .top{gap:.6rem}
  .tools{width:100%}
  .items{gap:.75rem}
  .items.syl .item.short{width:6.4rem}
  .items.syl .item{height:6.4rem;min-width:6.4rem}
  .items.syl .item.long{min-width:8.5rem}
  .items.let .item{width:5.6rem;height:6.4rem}
  .items.word .item{min-width:7rem;padding:.5rem 1.2rem .8rem}
  .items.sent .item{padding:.5rem 1rem .5rem 3rem}
  .btn{font-size:1.15rem;padding:.5rem 1.1rem}
  .btn.huge{font-size:1.3rem;padding:.6rem 1.3rem}
  .actions{justify-content:center}
  .names{grid-template-columns:1fr}
  .resBar{justify-content:center}
}
@media (prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}}

/* parents' guide */
.guide{display:grid;gap:1rem}
.welcome{background:var(--sky);color:var(--white);border-radius:1.9rem;padding:1.2rem 1.6rem;box-shadow:var(--shadow);display:flex;gap:1rem;align-items:center;flex-wrap:wrap}
.welcome .big{font-size:3.4rem;line-height:1}
.welcome h2{margin:0;font-size:clamp(1.5rem,3.4vw,2.1rem)}
.welcome p{margin:.2rem 0 0;font-size:1.1rem;max-width:46rem;opacity:.95}
.welcome .grow{flex:1;min-width:14rem}
.panel{background:var(--card);border:3px solid var(--line);border-radius:1.7rem;padding:1.1rem clamp(.9rem,3vw,1.7rem);box-shadow:var(--shadow-sm)}
.panel h3{margin:0 0 .6rem;font-size:1.45rem}
.howto{list-style:none;margin:0;padding:0;display:grid;gap:.6rem;counter-reset:s}
.howto li{display:flex;gap:.75rem;align-items:flex-start;font-size:1.1rem;line-height:1.8;counter-increment:s}
.howto li::before{content:counter(s, arabic-indic);flex:none;width:2.1rem;height:2.1rem;border-radius:50%;background:var(--b);color:var(--on-b);display:grid;place-items:center;font-weight:700;margin-top:.15rem}
.howto b{color:var(--ink)}
.stagecards{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:.75rem}
.sc{border-radius:1.3rem;padding:.8rem .9rem;border:3px solid var(--line);min-width:0}
.sc .L{width:2.6rem;height:2.6rem;border-radius:50%;display:grid;place-items:center;font-size:1.5rem;font-weight:700;color:var(--white);margin-bottom:.3rem}
.sc h4{margin:0;font-size:1.15rem}
.sc p{margin:.2rem 0 0;font-size:1rem;color:var(--muted);line-height:1.8}
.sc.a{background:var(--a-soft);border-color:var(--a)} .sc.a .L{background:var(--a)}
.sc.b{background:var(--b-soft);border-color:var(--b)} .sc.b .L{background:var(--b);color:var(--on-b)}
.sc.c{background:var(--c-soft);border-color:var(--c)} .sc.c .L{background:var(--c)}
.sc.d{background:var(--d-soft);border-color:var(--d)} .sc.d .L{background:var(--d)}
.tips{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:.6rem;margin:0;padding:0;list-style:none}
.tips li{display:flex;gap:.6rem;align-items:flex-start;background:var(--bg);border-radius:1rem;padding:.6rem .8rem;font-size:1.05rem;line-height:1.8}
.tips li span{font-size:1.5rem;line-height:1.2;flex:none}
.startRow{display:flex;justify-content:center;padding:.4rem 0 .2rem}
.note{display:flex;gap:.6rem;align-items:flex-start;background:var(--b-soft);border:2px dashed var(--b);border-radius:1.1rem;padding:.55rem .9rem;margin:.2rem 0 .4rem;font-size:1.02rem;line-height:1.8}
.note span{font-size:1.4rem;line-height:1.3;flex:none}
.lessonBanner{display:flex;align-items:center;gap:.75rem;flex-wrap:wrap;background:var(--card);border:3px solid var(--line);border-radius:1.5rem;padding:.5rem 1rem;box-shadow:var(--shadow-sm)}
.lessonBanner .big{font-size:2.4rem;line-height:1}
.lessonBanner .grow{flex:1;min-width:10rem}
.lessonBanner .nm{font-size:clamp(1.4rem,3vw,1.9rem);font-weight:700;line-height:1.5}
.lessonBanner .meta{color:var(--muted);font-size:.95rem;font-weight:600}
.celeCard .tip{background:var(--o-soft);border-radius:1rem;padding:.5rem .8rem;margin:.2rem 0 .8rem;font-size:1rem;line-height:1.8;text-align:right}
@media (max-width:900px){.stagecards{grid-template-columns:repeat(2,minmax(0,1fr))}}
@media (max-width:700px){.tips{grid-template-columns:1fr}.stagecards{grid-template-columns:1fr}}
</style>

<div class="wrap">
  <header class="top">
    <img class="logo" src="data:image/webp;base64,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" alt="شعار المعلم يوسف مشعل">
    <div class="brand">
      <h1>مدرسة ذكور كوبر الأساسية</h1>
      <p>المعلم: <b>يوسف مشعل</b> · القراءة في البيت مع أولياء الأمور</p>
    </div>
    <div class="tools">
      <div class="lessonpick">
        <label for="lessonSel">الدرس</label>
        <select id="lessonSel"></select>
      </div>
      <button class="iconbtn" id="soundBtn" aria-pressed="true">🔊 الأصوات</button>
      <button class="iconbtn" id="fsBtn">⛶ ملء الشاشة</button>
    </div>
  </header>

  <nav class="steps" aria-label="أقسام المنصة">
    <button class="step" id="stG"><span class="n">١</span>إرشادات لولي الأمر</button>
    <button class="step" id="stT"><span class="n">٢</span>التدريب على القراءة</button>
  </nav>

  <main id="main"></main>
</div>
<canvas id="confetti" hidden></canvas>
<script>
const $=s=>document.querySelector(s);
const DEFAULT_LESSON={id:'crow',title:'الْغُرَابُ وَالْجَرَّةُ',builtin:true,text:`فِي يَوْمٍ صَيْفِيٍّ حارٍّ، عَطِشَ الْغُرابُ كَثيراً، فَأَخَذَ يَبْحَثُ عَنِ الْمَاءِ. وَبَعْدَ الْبَحْثِ الطَّوِيلِ، وَجَدَ جَرَّةً فيها ماءٌ. حَاوَلَ أَنْ يَصِلَ إِلى الْمَاءِ بِمِنْقارِهِ، فَلَمْ يَقْدِرْ.
فَكَّرَ طَوِيلاً كَيْفَ يُمْكِنُ أَنْ يَصِلَ إِلى الْمَاءِ. نَظَرَ حَوْلَهُ، فَوَجَدَ حِجارَةً صَغِيرَةً. أَخَذَ الْغُرابُ يُلْقِي الْحِجارَةَ فِي الْجَرَّةِ. ارْتَفَعَ الْمَاءُ إِلَى أَعْلَى. فَرِحَ الْغُرابُ، وَشَرِبَ حَتَّى ارْتَوى.`};
const MORE_LESSONS=[{"id": "dairy", "title": "مَصْنَعُ الْأَلْبانِ", "text": "ذَهَبْتُ مَعَ صَديقَتي عَفافَ في زِيارَةٍ إِلى مَصْنَعِ أَلْبانٍ. عِنْدَما وَصَلْنا إِلى الْمَصْنَعِ، وَجَدْنا مَزْرَعَةَ أَبْقارٍ بِجانِبِهِ، وَكانَتِ الْأَبْقارُ تَرْعى الْعُشْبَ.\nأَخْبَرَنا صاحِبُ الْمَصْنَعِ أَنَّهُم يَحْصُلونَ عَلى الْحَليبِ مِنَ الْأَبْقارِ، وَيَبيعونَ جُزْءاً مِنْهُ، وَيَسْتَخْدِمونَ الْباقِيَ لِصِناعَةِ اللَّبَنِ، وَاللَّبَنَةِ، وَالْجُبْنِ، وَالْقِشْطَةِ.\nأَهْدانا صاحِبُ الْمَصْنَعِ بَعْضَ هَذِهِ الْمُنْتَجاتِ، وَفَرِحْتُ بِها كَثيراً. شَكَرْتُهُ، وَقُلْتُ لَهُ: أُحِبُّ مُنْتَجاتِ بِلادي؛ لِأَنَّها صِناعاتٌ وَطَنِيَّةٌ.", "builtin": true}, {"id": "juha", "title": "جُحا وَحَميرُهُ الْعَشَرَةُ", "text": "ذَهَبَ جُحا إِلى السّوقِ، واشْتَرى عَشَرَةَ حَميرٍ. رَكِبَ جُحا واحِداً مِنْها، وَساقَ بَقِيَّةَ الْحَميرِ أَمامَهُ، وفي الطَّريقِ، عَدَّ جُحا الْحَميرَ الَّتي أَمامَهُ، فَوَجَدَها تِسْعَةً.\nنَزَلَ عَنِ الْحِمارِ، وَعَدَّها مَرَّةً ثانِيَةً، فَوَجَدَها عَشَرَةَ حَميرٍ، فَقالَ جُحا: أَمْشي، وَأَكْسِبُ حِماراً، أَفْضَلُ لي مِنْ أَنْ أَرْكَبَ، وَأَخْسَرَ حِماراً.", "builtin": true}, {"id": "traffic", "title": "يَوْمُ الْمُرورِ", "text": "صَحِبَ الْمُعَلِّمونَ وَالْمُعَلِّماتُ مَجْموعَةً مِنْ طَلَبَةِ الْمَدْرَسَةِ إِلى الشّارِعِ في يَوْمِ الْمُرورِ، وَوَزَّعوا الْأَطْفالَ الصِّغارَ في الشَّوارِعِ. وَقَفَ الْأَطْفالُ بِجانِبِ شُرْطَةِ السَّيْرِ، وَقَدَّموا لَهُم الْوُرودَ.\nشارَكَ الْأَطْفالُ الشُّرْطَةَ في تَنْظيمِ السَّيْرِ، فَوَقَفَ فادي وَلَيْلى مَعَ الشُّرْطِيِّ في أَحَدِ الْمُفْتَرَقاتِ، وَنَظَّما حَرَكَةَ السَّيْرِ وَعُبورَ الشّارِعِ، وَساعَدا التَّلاميذَ الصِّغارَ وَكِبارَ السِّنِّ في الْوُصولِ بِأَمانٍ إِلى الرَّصيفِ الْمُقابِلِ. فَرِحَ الْأَطْفالُ؛ لِأَنَّهُم ساعَدوا في تَنْظيمِ حَرَكَةِ الْمُرورِ في الشَّوارِعِ.", "builtin": true}, {"id": "sheep", "title": "الْخَروفُ وَالذِّئْبُ", "text": "بَيْنَما كانَ الرّاعي يَرْعى غَنَمَهُ في الْبَرِّيَّةِ، ابْتَعَدَ خَروفٌ عَنِ الْقَطيعِ؛ فَهَجَمَ عَلَيْهِ ذِئْبٌ؛ لِيَأْكُلَهُ. فَقالَ لَهُ الْخَروفُ: إِنَّ الرّاعِيَ أَرْسَلَني إِلَيْكَ؛ لِتَأْكُلَني، وَلكِنَّهُ أَمَرَني أَنْ أُغَنِّيَ لَكَ قَبْلَ أَنْ تَأْكُلَني، فَقالَ الذِّئْبُ: هَلْ صَوْتُكَ حَسَنٌ؟ قالَ: نَعَمْ، إِنَّ صَوْتِيَ جَميلٌ جِدّاً، فَقالَ لَهُ الذِّئْبُ: غَنِّ، وَارْفَعْ صَوْتَكَ.\nرَفَعَ الْخَروفُ صَوْتَهُ، فَسَمِعَهُ الرّاعي، وَأَقْبَلَ وَفي يَدِهِ عَصًا طَويلَةٌ. رَآهُ الذِّئْبُ مُقْبِلاً، فَفَرَّ هارِباً، وَنَجا الْخَروفُ مِنَ الذِّئْبِ.", "builtin": true}, {"id": "doctor", "title": "طَبيبَةُ الْقَرْيَةِ", "text": "سَميرَةُ طالِبَةٌ مُجْتَهِدَةٌ، تَسْكُنُ في قَرْيَةٍ صَغيرَةٍ. كانَتْ تُحِبُّ أَهْلَ قَرْيَتِها وَخاصَّةً الْأَطْفالَ، وَعِنْدَما كَبُرَتْ سافَرَتْ؛ لِتَدْرُسَ طِبَّ الْأَطْفالِ، وَبَعْدَ أَنْ أَنْهَتْ دِراسَتَها، عادَتْ إِلى الْقَرْيَةِ؛ لِتُساعِدَ أَهْلَ قَرْيَتِها.\nفي أَوَّلِ أَيّامِ عَمَلِها، زارَتْ سَميرَةُ مَدْرَسَةَ الْقَرْيَةِ، وَتَحَدَّثَتْ إِلى الْأَطْفالِ عَنِ النَّظافَةِ وَأَهَمِّيَّتِها في الْمُحافَظَةِ عَلى صِحَّتِهِم. فَرِحَ الْأَطْفالُ مِنْ حَديثِها، وَقَدَّموا لَها بِطاقاتِ شُكْرٍ، وَعادوا إِلى أَهْلِهِم يُحَدِّثونَهُم عَنْ أَهَمِّيَّةِ النَّظافَةِ.", "builtin": true}, {"id": "lion", "title": "الْأَسَدُ وَالْفَأْرُ", "text": "في يَوْمٍ مِنَ الْأَيّامِ، مَرَّ فَأْرٌ صَغيرٌ قُرْبَ أَسَدٍ نائِمٍ، وَأَزْعَجَهُ، فَغَضِبَ الْأَسَدُ، وَهَمَّ بِأَكْلِهِ. فَقالَ لَهُ الْفَأْرُ: أَنا حَيَوانٌ ضَعيفٌ وَصَغيرٌ، وَلا أَكْفيكَ إِذا أَكَلْتَني. اتْرُكْني، فَقَدْ تَحْتاجُ لِمُساعَدَتي يَوْماً ما، فَتَرَكَهُ الْأَسَدُ، وَعادَ لِنَوْمِهِ.\nوَذاتَ يَوْمٍ، وَقَعَ الْأَسَدُ في شَبَكَةِ صَيّادٍ، فَرَآهُ الْفَأْرُ، فَقالَ الْأَسَدُ: ساعِدْني أَيُّها الْفَأْرُ، فَقَطَعَ الْفَأْرُ الشَّبَكَةَ بِأَسْنانِهِ؛ حَتّى أَخْرَجَ الْأَسَدَ. سُرَّ الْأَسَدُ مِنَ الْفَأْرِ، وَشَكَرَهُ.", "builtin": true}, {"id": "fisher", "title": "الصَّيّادُ", "text": "رَكِبَ الصَّيّادُ قارِبَهُ، وَدَخَلَ بِهِ إِلى الْبَحْرِ، قَطَعَ مَسافَةً مُبْتَعِداً عَنِ الشّاطِئِ، ثُمَّ أَلْقى شِباكَهُ في الْبَحْرِ، وَانْتَظَرَ طَويلاً؛ حَتّى تَتَجَمَّعَ الْأَسْماكُ في الشَّبَكَةِ، وَعِنْدَما امْتَلَأَتْ، شَدَّها الصَّيّادُ إِلى أَعْلى، وَوَضَعَ الشَّبَكَةَ بِأَسْماكِها الْمُتَنَوِّعَةِ في الْقارِبِ، ثُمَّ عادَ إِلى الشّاطِئِ، وَحَمَلَ السَّمَكَ إِلى السّوقِ؛ لِيَبيعَهُ، وَيُنْفِقَ عَلى نَفْسِهِ وَعِيالِهِ.", "builtin": true}, {"id": "researchers", "title": "الْباحِثاتُ الصَّغيراتُ", "text": "طَلَبَتِ الْمُعَلِّمَةُ مِنْ طالِباتِ الصَّفِّ الثّاني كِتابَةَ مَعْلوماتٍ عَنْ مَدينَةٍ فِلَسْطينِيَّةٍ.\nقالَتْ هَلا: أَنا سَأَطْلُبُ مُساعَدَةَ أَخي لِاسْتِخْدامِ شَبَكَةِ الْإِنْتَرْنِت؛ لِأَجِدَ مَعْلوماتٍ عَنْ مَدينَةِ غَزَّةَ.\nقالَتْ صَفاءُ: أَنا سَأَذْهَبُ إِلى الْمَكْتَبَةِ الْعامَّةِ؛ لِأَقْرَأَ عَنْ مَدينَةِ الْخَليلِ.\nقالَتْ سَمَرُ: الْيَوْمَ سَيَعْرِضُ التِّلْفازُ فيلْماً عَنْ مَدينَةِ أَريحا، سَأُشاهِدُهُ، وَأَتَحَدَّثُ عَنْهُ.\nقالَتْ مَرَحُ: أَنا سَأَطْلُبُ مِنْ جَدَّتي أَنْ تَحْكِيَ لي عَنْ مَدينَةِ حَيْفا.", "builtin": true}];
const STAGES=[
 {k:'a',L:'أ',name:'قراءة الجمل',ic:'📖',hint:'اقرأ الجمل الثلاث قراءة صحيحة. اجتياز هذه المرحلة يمنح العلامة الكاملة.'},
 {k:'b',L:'ب',name:'قراءة الكلمات',ic:'🔤',hint:'خمس كلمات من الدرس، من السهلة إلى الصعبة. النقاط تبيّن درجة الصعوبة.'},
 {k:'c',L:'ج',name:'قراءة المقاطع',ic:'🧩',hint:'ستة مقاطع: الدائرة مقطع قصير، والشكل المستطيل مقطع طويل.'},
 {k:'d',L:'د',name:'قراءة الحروف',ic:'✏️',hint:'خمسة حروف من الدرس. يمكنك إظهار الحركات على الحروف.'}
];
/* ---------- storage (per-browser convenience) ---------- */
const store={get(k,d){try{const v=localStorage.getItem(k);return v?JSON.parse(v):d}catch(e){return d}},set(k,v){try{localStorage.setItem(k,JSON.stringify(v));return true}catch(e){return false}}};

/* ---------- text analysis ---------- */
const DIAC=/[ً-ْٰـ]/g;
const strip=s=>s.replace(DIAC,'');
const STOP=new Set(['في','الى','إلى','على','عن','من','أن','ان','إن','لم','لن','ما','لا','هو','هي','قد','ثم','او','أو','مع','حتى','فلم','كي','هل','يا','ذلك','هذا','هذه','التي','الذي','كان','إذا','اذا']);
const shuffle=a=>{a=[...a];for(let i=a.length-1;i>0;i--){const j=Math.floor(Math.random()*(i+1));[a[i],a[j]]=[a[j],a[i]]}return a};
const VOW={'َ':'f','ُ':'d','ِ':'k'};
const ALPH='بتثجحخدذرزسشصضطظعغفقكلمنهوي';

function analyze(text){
  text=(text||'').replace(/\r/g,'').trim();
  const clean=s=>s.replace(/^[\s،,:\-–]+|[\s،,:\-–]+$/g,'').replace(/\s+/g,' ').trim();
  const wc=s=>s.split(' ').length;
  const rough=text.split(/[.!؟?\n؛]+/).map(clean).filter(Boolean), cut=[];
  for(const s of rough){
    if(wc(s)<=9){cut.push(s);continue}
    let cur=''; for(const part of s.split(/،\s*/)){cur=cur?cur+'، '+part:part;if(wc(cur)>=4){cut.push(clean(cur));cur=''}}
    if(cur){if(wc(cur)>=3||!cut.length)cut.push(clean(cur));else cut[cut.length-1]+='، '+clean(cur)}
  }
  const sentences=[...new Set(cut.map(clean))].filter(s=>wc(s)>=3);
  const seen=new Set(),words=[];
  for(const raw of text.split(/[\s.,،!؟?:؛"«»()\[\]\-–]+/)){
    const w=raw.trim(); const b=strip(w);
    if(!w||!/^[ء-ي]+$/.test(b)||b.length<2||STOP.has(b)||seen.has(b))continue;
    seen.add(b); const len=b.length; words.push({w,lvl:len<=3?1:len<=5?2:3});
  }
  const units=[];
  for(const ch of text){
    if(/[ء-غف-ي]/.test(ch))units.push({ch,m:''});
    else if(/[ً-ْ]/.test(ch)&&units.length&&units[units.length-1])units[units.length-1].m+=ch;
    else units.push(null);
  }
  const shortS=new Set(),longS=new Set();
  for(let i=0;i<units.length;i++){
    const u=units[i]; if(!u||'اىةء'.includes(u.ch))continue;
    if(/[ً-ٍّ]/.test(u.m))continue;
    const v=[...u.m].find(c=>VOW[c]); const n=units[i+1];
    if(!v){
      if(u.m===''&&n&&n.m===''&&!'وي'.includes(u.ch)){
        if('اى'.includes(n.ch))longS.add(u.ch+'\u064E'+n.ch);
        else if(n.ch==='و')longS.add(u.ch+'\u064F'+'و');
        else if(n.ch==='ي')longS.add(u.ch+'\u0650'+'ي');
      }
      continue;
    }
    const nFree=n&&![...n.m].some(c=>VOW[c]||/[ً-ٍّ]/.test(c));
    const t=VOW[v];
    if(nFree&&((t==='f'&&(n.ch==='ا'||n.ch==='ى'))||(t==='d'&&n.ch==='و')||(t==='k'&&n.ch==='ي')))longS.add(u.ch+v+n.ch);
    else shortS.add(u.ch+v);
  }
  const letters=[...new Set([...strip(text)].map(c=>/[أإآ]/.test(c)?'ا':c).filter(c=>('ا'+ALPH+'ء').includes(c)))];
  return{sentences,words,short:[...shortS],long:[...longS],letters};
}
function genSyl(letters,kind){
  const pool=letters.filter(c=>ALPH.includes(c)&&!'وي'.includes(c)); const base=pool.length?pool:[...ALPH];
  const L=base[Math.floor(Math.random()*base.length)];
  const v=['َ','ُ','ِ'][Math.floor(Math.random()*3)];
  if(kind==='short')return L+v;
  return L+v+({'َ':'ا','ُ':'و','ِ':'ي'})[v];
}
function draw(stageK,A){
  if(stageK==='a')return shuffle(A.sentences).slice(0,3).map(t=>({t}));
  if(stageK==='b'){
    const g={1:[],2:[],3:[]}; shuffle(A.words).forEach(w=>g[w.lvl].push(w));
    let out=[...g[1].slice(0,2),...g[2].slice(0,2),...g[3].slice(0,1)];
    const rest=shuffle(A.words.filter(w=>!out.includes(w)));
    while(out.length<5&&rest.length)out.push(rest.shift());
    return out.sort((x,y)=>x.lvl-y.lvl).map(w=>({t:w.w,lvl:w.lvl}));
  }
  if(stageK==='c'){
    let s=shuffle(A.short).slice(0,3), l=shuffle(A.long).slice(0,3);
    let guard=0; while(s.length<3&&guard++<40){const x=genSyl(A.letters,'short'); if(!s.includes(x))s.push(x)}
    guard=0; while(l.length<3&&guard++<40){const x=genSyl(A.letters,'long'); if(!l.includes(x))l.push(x)}
    return shuffle([...s.map(t=>({t,kind:'short'})),...l.map(t=>({t,kind:'long'}))]);
  }
  if(stageK==='d'){
    let ls=shuffle(A.letters).slice(0,5); const extra=shuffle([...ALPH].filter(c=>!ls.includes(c)));
    while(ls.length<5)ls.push(extra.shift());
    const marks=['َ','ُ','ِ','ْ'];
    return ls.map(t=>({t,mark:t==='ا'?'':marks[Math.floor(Math.random()*4)]}));
  }
}

/* ---------- sound ---------- */
let AC=null,master=null,voiceGain=null,soundOn=store.get('rd_sound',true);
function ac(){try{if(!AC){AC=new(window.AudioContext||window.webkitAudioContext)();master=AC.createGain();master.gain.value=.8;master.connect(AC.destination);voiceGain=AC.createGain();voiceGain.gain.value=1;voiceGain.connect(AC.destination)}if(AC.state==='suspended')AC.resume();return AC}catch(e){return null}}
function tone(f,d,type='sine',vol=.2,when=0,to){
  if(!soundOn)return;const c=ac();if(!c)return;const t=c.currentTime+when;
  const o=c.createOscillator(),g=c.createGain();o.type=type;o.frequency.setValueAtTime(f,t);
  if(to)o.frequency.exponentialRampToValueAtTime(to,t+d);
  g.gain.setValueAtTime(0,t);g.gain.linearRampToValueAtTime(vol,t+.01);g.gain.exponentialRampToValueAtTime(.001,t+d);
  o.connect(g).connect(master);o.start(t);o.stop(t+d+.05);
}
let noiseBuf=null;
function noise(){const c=ac();if(!noiseBuf){noiseBuf=c.createBuffer(1,c.sampleRate*.4,c.sampleRate);const d=noiseBuf.getChannelData(0);for(let i=0;i<d.length;i++)d[i]=Math.random()*2-1}return noiseBuf}
function applause(dur=3.2){
  if(!soundOn)return;const c=ac();if(!c)return;const buf=noise();
  for(let t=0;t<dur;t+=.008+Math.random()*.025){
    const env=t<.35?t/.35:(t>dur-1?Math.max(0,(dur-t)/1):1);
    const s=c.createBufferSource();s.buffer=buf;const bp=c.createBiquadFilter();bp.type='bandpass';
    bp.frequency.value=800+Math.random()*2200;bp.Q.value=.7+Math.random()*1.2;
    const g=c.createGain();const st=c.currentTime+t;const pk=(.18+Math.random()*.32)*env;
    g.gain.setValueAtTime(0,st);g.gain.linearRampToValueAtTime(pk,st+.003);g.gain.exponentialRampToValueAtTime(.001,st+.05+Math.random()*.08);
    s.connect(bp).connect(g).connect(master);s.start(st,Math.random()*.25,.16);
  }
}
const SFX={
  click(){tone(620,.09,'triangle',.18);tone(930,.09,'triangle',.12,.05)},
  select(){[523,659,784].forEach((f,i)=>tone(f,.18,'sine',.18,i*.07))},
  tick(){tone(1300+Math.random()*300,.035,'square',.05)},
  pop(){tone(420,.14,'sine',.25,0,950)},
  unpop(){tone(760,.12,'sine',.15,0,320)},
  whoosh(){tone(300,.25,'sine',.12,0,900);tone(450,.25,'triangle',.06,.05,1300)},
  open(){tone(500,.12,'sine',.15,0,800);tone(800,.15,'sine',.12,.08,1200)},
  close(){tone(800,.12,'sine',.12,0,450)},
  got(){[660,880,1046,1318].forEach((f,i)=>tone(f,.25,'triangle',.18,i*.09))},
  shuffle(){for(let i=0;i<5;i++)tone(500+i*120,.06,'triangle',.12,i*.04)},
  retry(){[392,440,523].forEach((f,i)=>tone(f,.35,'sine',.16,i*.18));tone(659,.6,'triangle',.1,.6)},
  win(){const n=[523,659,784,1046,784,1046,1318];n.forEach((f,i)=>tone(f,i===6?.6:.18,'square',.08,i*.11));n.forEach((f,i)=>tone(f,i===6?.6:.18,'triangle',.16,i*.11));setTimeout(()=>applause(3.4),350)}
};

/* ---------- confetti ---------- */
const cv=$('#confetti'),cx=cv.getContext('2d');let parts=[],raf=null;
const COLORS=['#FF5F6D','#FFB21E','#22B573','#8B5CF6','#2F86F6','#FF8DC7'];
function confetti(n,spread){
  if(matchMedia('(prefers-reduced-motion: reduce)').matches)n=Math.min(n,30);
  cv.hidden=false;cv.width=innerWidth;cv.height=innerHeight;const k=Math.max(1,innerWidth/1200);
  for(let i=0;i<n;i++)parts.push({x:spread?Math.random()*cv.width:cv.width/2,y:spread?-20-Math.random()*cv.height*.5:cv.height*.45,vx:(Math.random()-.5)*(spread?3:14)*k,vy:(spread?2+Math.random()*3:-6-Math.random()*8)*k,s:(6+Math.random()*8)*k,r:Math.random()*6,vr:(Math.random()-.5)*.3,c:COLORS[i%COLORS.length],shape:Math.random()<.3?'c':'r',life:0,g:.18*k});
  if(!raf)loop();
}
function loop(){
  cx.clearRect(0,0,cv.width,cv.height);
  parts.forEach(p=>{p.vy+=p.g;p.vx*=.99;p.x+=p.vx;p.y+=p.vy;p.r+=p.vr;p.life++;
    cx.save();cx.translate(p.x,p.y);cx.rotate(p.r);cx.fillStyle=p.c;
    if(p.shape==='c'){cx.beginPath();cx.arc(0,0,p.s/2,0,7);cx.fill()}else cx.fillRect(-p.s/2,-p.s/4,p.s,p.s/2);cx.restore()});
  parts=parts.filter(p=>p.y<cv.height+40&&p.life<600);
  if(parts.length)raf=requestAnimationFrame(loop);else{raf=null;cv.hidden=true}
}
const bigConfetti=()=>{confetti(180,true);setTimeout(()=>confetti(130,false),300)};
const miniConfetti=()=>confetti(60,false);

/* ---------- parents' app ---------- */
const PARENT_TIP={
  a:'يقرأ طفلك ثلاث جمل من الدرس. اضغط على الجملة بعد أن يقرأها كاملة قراءة صحيحة. إذا قرأ الجمل الثلاث جيداً فهو يتقن الدرس.',
  b:'خمس كلمات من السهلة إلى الصعبة. شجّعه على قراءة الكلمة كاملة بحركاتها، وإن تعثّر فساعده على تقسيمها إلى مقاطع.',
  c:'المقطع القصير في دائرة ويُنطق بسرعة (بَ، بُ، بِ). المقطع الطويل في شكل مستطيل ويُمدّ صوته (با، بو، بي).',
  d:'حروف من الدرس. اطلب من طفلك أن يقول اسم الحرف ثم صوته. فعّل «إظهار الحركات» ليتدرّب على صوت الحرف مع الحركة.'
};
const FAIL_TIP={
  a:'تدرّبا على قراءة الدرس معاً، ثم انتقلا إلى المرحلة (ب) لمعرفة الكلمات التي تحتاج إلى تدريب.',
  b:'اقرأ الكلمة أمامه ببطء، ثم اطلب منه أن يعيدها، وجرّبا كلمات جديدة من زر «عرض جديد».',
  c:'ركّزا على الفرق بين الصوت القصير والصوت الممدود، وكرّرا المقاطع بصوت مرتفع.',
  d:'تدرّبا على أصوات الحروف مع الحركات الثلاث: الفتحة والضمة والكسرة.'
};
const PRAISE=['أحسنت!','ممتاز!','رائع جداً!','بطل القراءة!','قراءة مدهشة!','أنت نجم!'];
const RETRY=['محاولة جميلة!','لا بأس، نتدرّب أكثر','أنت تستطيع!','قريب جداً!'];

let lessonId=store.get('pr_lesson','crow');
const allLessons=()=>[DEFAULT_LESSON,...MORE_LESSONS];
const curLesson=()=>allLessons().find(l=>l.id===lessonId)||DEFAULT_LESSON;
let A=analyze(curLesson().text);
let state={stage:'a',draws:{},read:{},harakat:false};
let marks=store.get('pr_marks',{});
const markOf=()=>marks[lessonId]||{};
function setMark(k,v){const m={...markOf()};if(v==='pass'&&k==='a')STAGES.forEach(s=>m[s.k]='pass');else m[k]=v;marks[lessonId]=m;store.set('pr_marks',marks)}
const esc=s=>String(s).replace(/[&<>"]/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;'})[c]);


function renderLessonSel(){$('#lessonSel').innerHTML=allLessons().map(l=>`<option value="${l.id}" ${l.id===lessonId?'selected':''}>${esc(l.title)}</option>`).join('')}
$('#lessonSel').onchange=e=>{lessonId=e.target.value;store.set('pr_lesson',lessonId);A=analyze(curLesson().text);state={stage:'a',draws:{},read:{},harakat:state.harakat};SFX.select();toast('الدرس: '+strip(curLesson().title));render()};
function setSound(){$('#soundBtn').textContent=soundOn?'🔊 الأصوات':'🔇 بلا أصوات';$('#soundBtn').setAttribute('aria-pressed',soundOn)}
$('#soundBtn').onclick=()=>{soundOn=!soundOn;store.set('rd_sound',soundOn);setSound();SFX.click()};
$('#fsBtn').onclick=()=>{SFX.click();try{if(document.fullscreenElement)document.exitFullscreen();else{const p=document.documentElement.requestFullscreen&&document.documentElement.requestFullscreen();if(p&&p.catch)p.catch(()=>toast('ملء الشاشة غير متاح هنا'))}}catch(e){toast('ملء الشاشة غير متاح هنا')}};
$('#stG').onclick=()=>{SFX.click();go('guide')};
$('#stT').onclick=()=>{SFX.whoosh();go('train')};

let view='guide';
function go(v){view=v;render();window.scrollTo({top:0,behavior:'smooth'})}
function render(){
  $('#stG').classList.toggle('on',view==='guide');$('#stT').classList.toggle('on',view==='train');
  $('#main').innerHTML=view==='guide'?guideView():trainView();bind();
}

function guideView(){
  return `<section class="view guide">
    <div class="welcome"><span class="big">👨‍👩‍👦</span><div class="grow"><h2>أهلاً بكم أولياء الأمور الكرام</h2>
      <p>هذه المنصة تساعدكم على تدريب أبنائكم على قراءة دروس اللغة العربية في البيت، بالمراحل نفسها التي نستخدمها في الصف. لا تُسجَّل فيها أسماء ولا علامات، فهي للتدريب فقط.</p></div></div>
    <div class="panel"><h3>🧭 طريقة الاستخدام</h3>
      <ol class="howto">
        <li><span>اختر <b>الدرس</b> من القائمة في أعلى الصفحة، وهو الدرس الذي يتعلّمه طفلك في المدرسة.</span></li>
        <li><span>اجلس مع طفلك في مكان هادئ، واضغط <b>«ابدأ التدريب»</b>. يمكنك تشغيل الأصوات لأنها تشجّع الطفل.</span></li>
        <li><span>ابدأ بالمرحلة <b>(أ) قراءة الجمل</b>. اطلب من طفلك قراءة كل جملة، واضغط عليها بعد أن يقرأها صحيحة فتظهر عليها نجمة ⭐.</span></li>
        <li><span>إذا قرأ كل ما في المرحلة صحيحاً اضغط <b>«✅ أحسنت، اجتاز»</b> لتظهر شاشة الاحتفال. وإن تعثّر اضغط <b>«↻ يحتاج تدريباً»</b> لتظهر لك نصيحة.</span></li>
        <li><span>اجتياز المرحلة (أ) يعني أن طفلك يقرأ الدرس بإتقان. إن لم يجتزها فانتقل إلى <b>(ب) ثم (ج) ثم (د)</b> لتعرف أين يحتاج إلى الدعم: الكلمات أم المقاطع أم الحروف.</span></li>
        <li><span>زر <b>«🔄 عرض جديد»</b> يغيّر الجمل والكلمات في كل مرة، فيمكنكم التدرّب على الدرس نفسه أكثر من مرة.</span></li>
      </ol>
    </div>
    <div class="panel"><h3>📚 المراحل الأربع</h3>
      <div class="stagecards">
        <div class="sc a"><div class="L">أ</div><h4>قراءة الجمل</h4><p>ثلاث جمل من الدرس، تقيس قراءة الطفل للنص بطلاقة.</p></div>
        <div class="sc b"><div class="L">ب</div><h4>قراءة الكلمات</h4><p>خمس كلمات من السهلة إلى الصعبة.</p></div>
        <div class="sc c"><div class="L">ج</div><h4>قراءة المقاطع</h4><p>ستة مقاطع قصيرة وطويلة، مثل: بَ و با.</p></div>
        <div class="sc d"><div class="L">د</div><h4>قراءة الحروف</h4><p>خمسة حروف من الدرس، مع الحركات أو بدونها.</p></div>
      </div>
    </div>
    <div class="panel"><h3>💡 نصائح للتعامل مع طفلك أثناء القراءة</h3>
      <ul class="tips">
        <li><span>🌟</span>امدح محاولته وجهده، لا الإجابة الصحيحة فقط.</li>
        <li><span>⏳</span>امنحه وقتاً ليقرأ بنفسه، ولا تسارع إلى القراءة عنه.</li>
        <li><span>🧩</span>عند الخطأ ساعده على تقسيم الكلمة إلى مقاطع، ثم يقرؤها كاملة.</li>
        <li><span>⏱️</span>جلسة قصيرة كل يوم (10 إلى 15 دقيقة) أنفع من جلسة طويلة مرة في الأسبوع.</li>
        <li><span>😊</span>إذا تعب طفلك أو انزعج، توقّفا وأكملا في وقت لاحق.</li>
        <li><span>🔁</span>كرّر المرحلة التي تعثّر فيها في اليوم التالي، واحتفل معه عندما يجتازها.</li>
      </ul>
    </div>
    <div class="startRow"><button class="btn go huge" id="startBtn">🚀 ابدأ التدريب</button></div>
  </section>`;
}

function ensureDraw(k){if(!state.draws[k]){state.draws[k]=draw(k,A);state.read[k]=new Set()}}
function trainView(){
  const st=STAGES.find(s=>s.k===state.stage); ensureDraw(st.k);
  const items=state.draws[st.k], rd=state.read[st.k], mk=markOf();
  let itemsHtml='';
  if(!items.length)itemsHtml=`<div class="empty">لا يوجد محتوى كافٍ لهذه المرحلة في هذا الدرس.</div>`;
  else if(st.k==='a')itemsHtml=`<div class="items sent">${items.map((it,i)=>`<button class="item ${rd.has(i)?'read':''}" data-i="${i}"><span class="num">${i+1}</span>${esc(it.t)}<span class="st">⭐</span></button>`).join('')}</div>`;
  else if(st.k==='b')itemsHtml=`<div class="items word">${items.map((it,i)=>`<button class="item ${rd.has(i)?'read':''}" data-i="${i}">${esc(it.t)}<span class="st">⭐</span><span class="tag"><span class="lv">${[1,2,3].map(x=>`<i class="${x<=it.lvl?'f':''}"></i>`).join('')}</span> ${['','سهلة','متوسطة','صعبة'][it.lvl]}</span></button>`).join('')}</div>`;
  else if(st.k==='c')itemsHtml=`<div class="items syl">${items.map((it,i)=>`<button class="item ${it.kind} ${rd.has(i)?'read':''}" data-i="${i}">${esc(it.t)}<span class="st">⭐</span><span class="tag">${it.kind==='long'?'طويل':'قصير'}</span></button>`).join('')}</div>`;
  else itemsHtml=`<div class="items let">${items.map((it,i)=>`<button class="item ${rd.has(i)?'read':''}" data-i="${i}">${esc(it.t+(state.harakat?it.mark:''))}<span class="st">⭐</span></button>`).join('')}</div>`;
  const all=items.length&&rd.size===items.length;
  return `<section class="view reader">
    <div class="lessonBanner"><span class="big">📖</span><div class="grow"><div class="nm">${esc(curLesson().title)}</div><div class="meta">الصف الثاني الأساسي · اختر المرحلة واضغط على كل ما يقرؤه طفلك صحيحاً</div></div>
      <button class="iconbtn" id="resetMarks">↺ تدريب جديد</button></div>
    <div class="tabs" role="tablist">${STAGES.map(s=>`<button class="tab ${s.k===st.k?'on':''}" data-k="${s.k}" role="tab" aria-selected="${s.k===st.k}">
      ${mk[s.k]==='pass'?'<span class="chk ok">✓</span>':mk[s.k]==='fail'?'<span class="chk no">↻</span>':''}<span class="ic">${s.ic}</span><span class="L">${s.L}</span><span class="nmx">${s.name}</span></button>`).join('')}</div>
    <div class="stage" data-k="${st.k}">
      <div class="stHead"><h2>المرحلة (${st.L}): ${st.name} ${st.ic}</h2>
      ${st.k==='d'?`<label class="tog"><input type="checkbox" id="harakat" ${state.harakat?'checked':''}> إظهار الحركات</label>`:''}</div>
      <div class="note"><span>💡</span><div><b>لولي الأمر:</b> ${PARENT_TIP[st.k]}</div></div>
      ${itemsHtml}
      <div class="actions">
        <div class="row"><button class="btn ghost" id="redraw">🔄 عرض جديد</button><span class="progressTxt">قرأ ${rd.size} من ${items.length}</span></div>
        <div class="row"><button class="btn no" id="failBtn">↻ يحتاج تدريباً</button><button class="btn ok huge ${all?'pulse':''}" id="passBtn">✅ أحسنت، اجتاز</button></div>
      </div>
    </div>
  </section>`;
}

function bind(){
  if(view==='guide'){$('#startBtn').onclick=()=>{SFX.whoosh();go('train')};return}
  document.querySelectorAll('.tab').forEach(b=>b.onclick=()=>{state.stage=b.dataset.k;SFX.whoosh();render()});
  document.querySelectorAll('.stage .item').forEach(b=>b.onclick=()=>{
    const i=+b.dataset.i,set=state.read[state.stage];
    if(set.has(i)){set.delete(i);SFX.unpop()}else{set.add(i);SFX.pop()}
    b.classList.toggle('read');const n=state.draws[state.stage].length;
    document.querySelector('.progressTxt').textContent=`قرأ ${set.size} من ${n}`;
    $('#passBtn').classList.toggle('pulse',set.size===n);if(set.size===n)SFX.got();
  });
  $('#redraw').onclick=()=>{state.draws[state.stage]=null;SFX.shuffle();render()};
  $('#passBtn').onclick=()=>result(true);
  $('#failBtn').onclick=()=>result(false);
  $('#resetMarks').onclick=()=>{delete marks[lessonId];store.set('pr_marks',marks);state={stage:'a',draws:{},read:{},harakat:state.harakat};SFX.shuffle();toast('بدأ تدريب جديد على هذا الدرس');render()};
  const h=$('#harakat');if(h)h.onchange=()=>{state.harakat=h.checked;SFX.click();render()};
}

function result(pass){
  const st=STAGES.find(s=>s.k===state.stage);
  if(pass||markOf()[st.k]!=='pass')setMark(st.k,pass?'pass':'fail');
  const next=STAGES[STAGES.indexOf(st)+1];
  const allDone=STAGES.every(s=>markOf()[s.k]==='pass');
  const ov=document.createElement('div');ov.className='cele'+(pass?'':' retry');ov.setAttribute('role','dialog');
  ov.innerHTML=pass?`<div class="celeCard">
    <div class="trophy">${st.k==='a'||allDone?'👑':'🏆'}</div>
    <h2>${PRAISE[Math.floor(Math.random()*PRAISE.length)]}</h2>
    <div class="nm">يا بطل القراءة 🎉</div>
    <div class="what">${st.k==='a'?'قرأت جمل الدرس قراءة صحيحة، أنت قارئ ممتاز!':`اجتزت المرحلة (${st.L}): ${st.name}`}</div>
    <div class="stars"><span>⭐</span><span>⭐</span><span>⭐</span></div>
    <div class="row">${st.k!=='a'&&next?`<button class="btn blue" id="celeNext">المرحلة (${next.L}) ⬅</button>`:''}<button class="btn ghost" id="celeClose">إغلاق</button></div></div>`
  :`<div class="celeCard">
    <div class="trophy">💪</div>
    <h2>${RETRY[Math.floor(Math.random()*RETRY.length)]}</h2>
    <div class="what">نتدرّب قليلاً على المرحلة (${st.L}): ${st.name}، ثم نحاول مرة أخرى</div>
    <div class="tip">💡 <b>نصيحة لولي الأمر:</b> ${FAIL_TIP[st.k]}</div>
    <div class="row"><button class="btn go" id="celeAgain">🔄 محاولة جديدة</button>${next?`<button class="btn blue" id="celeNext">المرحلة (${next.L}) ⬅</button>`:''}<button class="btn ghost" id="celeClose">إغلاق</button></div></div>`;
  document.body.appendChild(ov);
  if(pass){SFX.win();bigConfetti()}else SFX.retry();
  const close=()=>{ov.remove();SFX.close();render()};
  ov.querySelector('#celeClose').onclick=close;
  ov.onclick=e=>{if(e.target===ov)close()};
  const nb=ov.querySelector('#celeNext');if(nb)nb.onclick=()=>{state.stage=next.k;ov.remove();SFX.whoosh();render()};
  const ag=ov.querySelector('#celeAgain');if(ag)ag.onclick=()=>{state.draws[st.k]=null;ov.remove();SFX.shuffle();render()};
  ov.querySelector('button').focus();
}

function toast(msg){const t=document.createElement('div');t.className='toast';t.textContent=msg;document.body.appendChild(t);setTimeout(()=>t.remove(),2400)}
document.addEventListener('keydown',e=>{if(e.key==='Escape'){const o=document.querySelector('.cele');if(o){o.remove();SFX.close();render()}}});
addEventListener('resize',()=>{if(!cv.hidden){cv.width=innerWidth;cv.height=innerHeight}});
renderLessonSel();setSound();render();
</script>

</body></html>
