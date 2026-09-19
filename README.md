# trading-web
 <!doctype html>
<html lang="en"><head><script>window["__codeletBootstrap__"]=JSON.parse('{"A":"A","B":"20260901-05-1a916a1","C":{"Abril Fatface":"YACgEZbkUVE,0","Alfa Slab One":"YACgEYS9sJU,0","Anton":"YACgEcYqQ-A,0","Archivo":"YAHO2-t-jNE,0","Arial":"YAGyDvJ_4Ts,0","Bebas Neue":"YACgESME5ew,0","Bricolage Grotesque":"YAFyMcdwzpc,0","Canva Sans":"YAFLd8sKbwc,2","Caveat":"YALBs2ploWQ,0","Comic Sans MS":"YAHO2VMiyZo,0","Cormorant Garamond":"YAFdJhX-538,0","Courier New":"YAGzXiGs0_8,0","DM Sans":"YAD1aU3sLnI,0","DM Serif Display":"YAD1aYG82rc,0","Forum":"YACgEcnnqB4,0","Fraunces":"YAEul-FRQw4,0","Georgia":"YAGzXkO0pEM,0","Helvetica Neue":"YAFcf6CtJfI,0","Impact":"YAFcfnjI7Vk,0","Inter":"YAFdJvSyp_k,3","Iowan Old Style":"YAGNIFa8j9o,0","Jacques Francois":"YAHO2a5g66Q,0","JetBrains Mono":"YAFdJksXcAk,0","Libre Baskerville":"YACgEUFdPdA,0","Manrope":"YAHO2b2feC4,0","Merriweather":"YACgEXvHxxs,0","Montserrat":"YADLjI9qxTA,0","Nunito":"YACgEX8C5Gg,0","Oleo Script":"YACgEQQ14jI,0","Phantom Sans":"YAHO2E8Pb88,0","Playfair Display":"YACgEYmuCJE,0","Poppins":"YAFdJjbTu24,1","Press Start 2P":"YAFyGr-8pmQ,0","Quicksand":"YADWjpfPmdk,0","Raleway":"YACgEVg3xZg,0","Segoe UI":"YAHNdRD1Klw,0","Source Sans 3":"YAG4lO1Mj10,0","Spectral":"YAHO2rVUHIM,0","Times New Roman":"YAGzXW3gftg,0","Times":"YAGzXW3gftg,0","Ubuntu":"YACgERDU--Q,0","Work Sans":"YAGXhLOKv44,0","Yellowtail":"YACgEYG4kG4,0","ui-monospace":"YADlN8CFZ8Q,0","ui-sans-serif":"YACkoN-xg4g,0"}}');</script><script src="/_sdk/50d846425a1e5082.telemetry_sdk.js" integrity="sha512-Otbex+ztlVbcEGql0rXGd/3E3ee/hqAntg6DeuUEMG6pIPbXGOSvZbFZVzknAXi1tH/itQ+ijEhOTr2aWj6CXg=="></script>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prediction Market Arbitrage Tracker</title>
  <script src="https://cdn.tailwindcss.com/3.4.17"></script>
  <script src="https://cdn.jsdelivr.net/npm/lucide@0.263.0/dist/umd/lucide.min.js"></script>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&amp;display=swap" rel="stylesheet">
  <style>
    :root { --navy:#14213d; --blue:#2563eb; --teal:#0f766e; --green:#16803c; --amber:#b45309; --red:#c43232; --line:#e3e8f0; --canvas:#f6f8fb; }
    * { box-sizing:border-box; }
    body { font-family:"DM Sans",sans-serif; color:var(--navy); }
    button,input,select { font:inherit; }
    button:focus-visible,input:focus-visible,select:focus-visible { outline:3px solid #93c5fd; outline-offset:2px; }
    .app-shell { min-height:calc(100 * min(var(--vh, 1vh), 1vh)); }
    .sidebar { width:248px; }
    .nav-item { transition:background .16s ease,color .16s ease,transform .16s ease; }
    .nav-item:hover { transform:translateX(2px); }
    .nav-item.is-active { background:#eff6ff; color:var(--blue); font-weight:700; }
    .metric-card,.panel-card { border:1px solid var(--line); box-shadow:0 4px 18px rgba(20,33,61,.035); }
    .opportunity-row { cursor:pointer; transition:background .15s ease; }
    .opportunity-row:hover,.opportunity-row.is-selected { background:#f5f9ff; }
    .sort-button.is-sorted { color:var(--blue); }
    .range-button.is-selected { background:#eff6ff; color:var(--blue); }
    .modal-backdrop { background:rgba(15,23,42,.52); }
    .mobile-menu-open .mobile-navigation { display:block; }
    .drawer-sticky { position:sticky; top:80px; }
    @media (max-width:1023px) { .sidebar { display:none; } .dashboard-layout { grid-template-columns:1fr !important; } .drawer-sticky { position:static; } }
    @media (max-width:640px) { .top-search { display:none; } .metrics-grid { grid-template-columns:1fr 1fr !important; } .metrics-grid article:last-child { grid-column:span 2; } }
  </style>
  <script src="/_sdk/b3bf9e8ac58e6ad6.data_sdk.js" type="text/javascript" integrity="sha512-otc1u9NYq9Ms5Jt//7vmhrrqR5CLPr8Jdgs6741gqniClfLMcfmC+jK/cKuQdhLv6G0esJ/FzaMS9tv0T/vj/Q=="></script>
  <script src="/_sdk/2cfae6c35b9820dc.resizing_sdk.js" type="text/javascript" integrity="sha512-Oy+wKa9tloayelgS18tBfR707QfWMdeA8unVpm1M0/W/edVyjcRCNO6/jCvDwt/HpUta1v7sfMHiF1mAVr5RIA=="></script>
 </head>
 <body data-template-id="__page-root" class="w-full bg-[#f6f8fb]" style="background: rgb(246, 248, 251);">
  <div class="app-shell w-full flex">
   <aside class="sidebar fixed inset-y-0 left-0 z-30 flex flex-col border-r border-slate-200 bg-white px-4 py-5" aria-label="Primary navigation">
    <div class="mb-8 flex items-center gap-3 px-2">
     <div class="flex h-9 w-9 items-center justify-center rounded-xl bg-blue-600 text-white">
      <i data-lucide="scan-line" class="h-5 w-5"></i>
     </div>
     <div>
      <p data-template-id="brand-name" class="canva-text font-bold tracking-tight" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 15px;">Signal Ledger</p>
      <p data-template-id="brand-caption" class="canva-text text-xs text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 12px;">Simulation workspace</p>
     </div>
    </div>
    <nav class="space-y-1"><button type="button" class="nav-item is-active canva-button flex w-full items-center gap-3 rounded-xl px-3 py-2.5 text-left text-slate-600" data-section="Overview" data-template-id="nav-overview" aria-current="page" style="color: rgb(37, 99, 235); font-weight: 700; font-style: normal; font-size: 15px;">Overview</button> <button type="button" class="nav-item canva-button flex w-full items-center gap-3 rounded-xl px-3 py-2.5 text-left text-slate-600" data-section="Opportunities" data-template-id="nav-opportunities" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Opportunities</button> <button type="button" class="nav-item canva-button flex w-full items-center gap-3 rounded-xl px-3 py-2.5 text-left text-slate-600" data-section="Markets" data-template-id="nav-markets" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Markets</button> <button type="button" class="nav-item canva-button flex w-full items-center gap-3 rounded-xl px-3 py-2.5 text-left text-slate-600" data-section="Watchlist" data-template-id="nav-watchlist" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Watchlist</button> <button type="button" class="nav-item canva-button flex w-full items-center gap-3 rounded-xl px-3 py-2.5 text-left text-slate-600" data-section="Positions" data-template-id="nav-positions" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Positions</button> <button type="button" class="nav-item canva-button flex w-full items-center gap-3 rounded-xl px-3 py-2.5 text-left text-slate-600" data-section="Alerts" data-template-id="nav-alerts" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Alerts</button>
    </nav>
    <div class="mt-auto border-t border-slate-100 pt-4"><button type="button" class="nav-item canva-button flex w-full items-center gap-3 rounded-xl px-3 py-2.5 text-left text-slate-600" data-section="Settings" data-template-id="nav-settings" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Settings</button>
     <div data-template-id="sidebar-simulated-badge" class="canva-tag mt-5 rounded-xl px-3 py-2 text-xs font-bold" style="background: rgb(239, 246, 255); color: rgb(29, 78, 216); font-weight: 700; font-style: normal; font-size: 15px;">SIMULATED DATA</div>
    </div>
   </aside>
   <div class="w-full lg:pl-[248px]">
    <header class="sticky top-0 z-20 border-b border-slate-200 bg-white/95 px-4 py-3 backdrop-blur sm:px-6">
     <div class="mx-auto flex max-w-[1600px] items-center gap-3"><button id="mobile-menu-button" type="button" class="rounded-lg p-2 text-slate-600 hover:bg-slate-100 lg:hidden" aria-label="Open navigation" aria-expanded="false"><i data-lucide="menu" class="h-5 w-5"></i></button>
      <div class="min-w-0">
       <h1 data-template-id="header-title" class="canva-text whitespace-nowrap font-bold tracking-tight" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 20px;">Prediction Market Arbitrage Tracker</h1>
      </div>
      <div class="top-search relative ml-3 hidden max-w-md flex-1 md:block"><label class="sr-only" for="market-search">Search simulated markets</label> <i data-lucide="search" class="absolute left-3 top-1/2 h-4 w-4 -translate-y-1/2 text-slate-400"></i> <input id="market-search" data-template-id="market-search-input" class="canva-input w-full rounded-xl border border-slate-200 bg-slate-50 py-2.5 pl-9 pr-3 text-sm text-slate-800" type="search" placeholder="Search simulated markets" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 14px;">
      </div>
      <div class="ml-auto flex items-center gap-2 sm:gap-3">
       <div data-template-id="header-simulated-badge" class="canva-tag hidden rounded-full px-3 py-1.5 text-xs font-bold sm:block" style="background: rgb(239, 246, 255); color: rgb(29, 78, 216); font-weight: 700; font-style: normal; font-size: 15px;">SIMULATED DATA</div>
       <p data-template-id="last-updated" class="canva-text hidden text-xs text-slate-500 lg:block" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 12px;">Sample update: Sep 1, 2026 · 13:55 UTC</p><button type="button" class="relative rounded-lg p-2 text-slate-500 hover:bg-slate-100" aria-label="Notifications"><i data-lucide="bell" class="h-5 w-5"></i><span class="absolute right-2 top-2 h-1.5 w-1.5 rounded-full bg-blue-600"></span></button> <button data-template-id="user-menu" type="button" class="canva-button flex items-center gap-2 rounded-xl border border-slate-200 px-2 py-1.5 text-sm font-medium text-slate-700 hover:bg-slate-50" style="background: rgb(255, 255, 255); color: rgb(51, 65, 85); font-weight: 600; font-style: normal; font-size: 15px;">Jordan P.</button>
      </div>
     </div>
     <nav class="mobile-navigation mt-3 hidden border-t border-slate-100 pt-3 lg:hidden" aria-label="Mobile navigation">
      <div class="grid grid-cols-4 gap-2"><button class="nav-item is-active canva-button rounded-lg px-2 py-2 text-xs" type="button" data-section="Overview" data-template-id="mobile-nav-overview" style="background: rgb(239, 246, 255); color: rgb(37, 99, 235); font-weight: 700; font-style: normal; font-size: 15px;">Overview</button> <button class="nav-item canva-button rounded-lg px-2 py-2 text-xs" type="button" data-section="Opportunities" data-template-id="mobile-nav-opportunities" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Opportunities</button> <button class="nav-item canva-button rounded-lg px-2 py-2 text-xs" type="button" data-section="Markets" data-template-id="mobile-nav-markets" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Markets</button> <button class="nav-item canva-button rounded-lg px-2 py-2 text-xs" type="button" data-section="Watchlist" data-template-id="mobile-nav-watchlist" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Watchlist</button> <button class="nav-item canva-button rounded-lg px-2 py-2 text-xs" type="button" data-section="Positions" data-template-id="mobile-nav-positions" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Positions</button> <button class="nav-item canva-button rounded-lg px-2 py-2 text-xs" type="button" data-section="Alerts" data-template-id="mobile-nav-alerts" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Alerts</button> <button class="nav-item canva-button rounded-lg px-2 py-2 text-xs" type="button" data-section="Settings" data-template-id="mobile-nav-settings" style="color: rgb(71, 85, 105); font-weight: 500; font-style: normal; font-size: 15px;">Settings</button>
      </div>
     </nav>
    </header>
    <main class="mx-auto max-w-[1600px] p-4 sm:p-6">
     <div class="mb-6 flex flex-wrap items-end justify-between gap-3">
      <div>
       <p data-template-id="section-eyebrow" class="canva-text mb-1 text-sm font-medium text-slate-500" style="color: rgb(100, 116, 139); font-weight: 500; font-style: normal; font-size: 14px;">Educational analytics · simulated venues and quotes</p>
       <h2 id="section-title" class="text-2xl font-bold tracking-tight text-[#14213d] sm:text-3xl">Opportunity overview</h2>
      </div>
      <p data-template-id="data-disclosure" class="canva-text rounded-lg border px-3 py-2 text-xs font-medium" style="background: rgb(255, 251, 235); color: rgb(146, 64, 14); font-weight: 600; font-style: normal; font-size: 12px;">View-only simulation · no live execution</p>
     </div>
     <section class="metrics-grid grid gap-4 md:grid-cols-4" aria-label="Opportunity summary">
      <article data-template-id="open-opportunities-card" class="metric-card canva-card rounded-2xl bg-white p-5" style="background: rgb(255, 255, 255);">
       <p data-template-id="open-opportunities-label" class="canva-text text-sm font-medium text-slate-500" style="color: rgb(100, 116, 139); font-weight: 500; font-style: normal; font-size: 14px;">Open opportunities</p>
       <p id="open-count" class="mt-3 text-2xl font-bold tracking-tight">4</p>
       <p data-template-id="open-opportunities-caption" class="canva-text mt-2 text-xs text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 12px;">Matching current sample filters</p>
      </article>
      <article data-template-id="best-edge-card" class="metric-card canva-card rounded-2xl bg-white p-5" style="background: rgb(255, 255, 255);">
       <p data-template-id="best-edge-label" class="canva-text text-sm font-medium text-slate-500" style="color: rgb(100, 116, 139); font-weight: 500; font-style: normal; font-size: 14px;">Best net edge</p>
       <p id="best-edge" class="mt-3 text-2xl font-bold tracking-tight text-[#16803c]">4.8%</p>
       <p data-template-id="best-edge-caption" class="canva-text mt-2 text-xs text-slate-500" style="color: rgb(22, 128, 60); font-weight: 400; font-style: normal; font-size: 12px;">After sample fees and buffers</p>
      </article>
      <article data-template-id="capital-card" class="metric-card canva-card rounded-2xl bg-white p-5" style="background: rgb(255, 255, 255);">
       <p data-template-id="capital-label" class="canva-text text-sm font-medium text-slate-500" style="color: rgb(100, 116, 139); font-weight: 500; font-style: normal; font-size: 14px;">Estimated capital required</p>
       <p id="capital-required" class="mt-3 text-2xl font-bold tracking-tight">$1,240</p>
       <p data-template-id="capital-caption" class="canva-text mt-2 text-xs text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 12px;">Illustrative, not an account balance</p>
      </article>
      <article data-template-id="quality-card" class="metric-card canva-card rounded-2xl bg-white p-5" style="background: rgb(255, 255, 255);">
       <p data-template-id="quality-label" class="canva-text text-sm font-medium text-slate-500" style="color: rgb(100, 116, 139); font-weight: 500; font-style: normal; font-size: 14px;">Data quality</p>
       <p class="mt-3 text-2xl font-bold tracking-tight text-[#0f766e]">Good</p>
       <p data-template-id="quality-caption" class="canva-text mt-2 text-xs text-slate-500" style="color: rgb(15, 118, 110); font-weight: 400; font-style: normal; font-size: 12px;">3 fresh sample quotes · 1 stale</p>
      </article>
     </section>
     <section class="dashboard-layout mt-5 grid gap-5 xl:grid-cols-[minmax(0,1fr)_380px]">
      <div class="space-y-5">
       <section data-template-id="opportunities-panel" class="panel-card canva-panel rounded-2xl bg-white p-5 sm:p-6" aria-labelledby="opportunities-heading" style="background: rgb(255, 255, 255);">
        <div class="flex flex-wrap items-start justify-between gap-4">
         <div>
          <h2 id="opportunities-heading" data-template-id="opportunities-heading-text" class="canva-text font-bold" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 23px;">Simulated opportunities</h2>
          <p data-template-id="opportunities-subtext" class="canva-text mt-1 text-sm text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 14px;">Compare fictional venue quotes after estimated costs.</p>
         </div>
         <div data-template-id="table-status-badge" class="canva-tag rounded-full px-3 py-1.5 text-xs font-semibold" style="background: rgb(236, 253, 245); color: rgb(22, 128, 60); font-weight: 700; font-style: normal; font-size: 15px;">4 SAMPLE QUOTES</div>
        </div>
        <div class="mt-5 grid gap-3 rounded-xl border border-slate-100 bg-slate-50 p-3 md:grid-cols-[1fr_1fr_1.3fr_auto]">
         <div><label for="venue-filter" data-template-id="venue-filter-label" class="canva-text mb-1 block text-xs font-semibold text-slate-600" style="color: rgb(71, 85, 105); font-weight: 600; font-style: normal; font-size: 12px;">Venue filter</label> <select id="venue-filter" class="w-full rounded-lg border border-slate-200 bg-white px-3 py-2 text-sm"> <option value="all">All fictional venues</option> <option value="SignalBay">SignalBay</option> <option value="ForecastX">ForecastX</option> <option value="CivicOdds">CivicOdds</option> </select>
         </div>
         <div><label for="edge-filter" data-template-id="edge-filter-label" class="canva-text mb-1 block text-xs font-semibold text-slate-600" style="color: rgb(71, 85, 105); font-weight: 600; font-style: normal; font-size: 12px;">Minimum net edge</label>
          <div class="flex items-center gap-2">
           <input id="edge-filter" class="w-full accent-blue-600" type="range" min="0" max="6" value="0" step="0.5"><output id="edge-output" class="w-10 text-sm font-bold text-blue-700">0%</output>
          </div>
         </div>
         <div><label for="table-search" data-template-id="table-search-label" class="canva-text mb-1 block text-xs font-semibold text-slate-600" style="color: rgb(71, 85, 105); font-weight: 600; font-style: normal; font-size: 12px;">Filter opportunities</label> <input id="table-search" class="w-full rounded-lg border border-slate-200 bg-white px-3 py-2 text-sm" type="search" placeholder="Filter event or outcome">
         </div><label class="mt-5 flex cursor-pointer items-center gap-2 text-xs font-semibold text-slate-600"><input id="liquidity-toggle" class="h-4 w-4 accent-blue-600" type="checkbox"><span data-template-id="liquidity-toggle-label" class="canva-text" style="color: rgb(71, 85, 105); font-weight: 600; font-style: normal; font-size: 12px;">Actionable liquidity only</span></label>
        </div>
        <div class="mt-5 overflow-x-auto">
         <table class="w-full min-w-[1240px] text-left text-xs">
          <thead class="border-b border-slate-200 text-[11px] uppercase tracking-wide text-slate-400">
           <tr>
            <th class="pb-3 pr-3">Event</th>
            <th class="pb-3 pr-3">Market / outcome</th>
            <th class="pb-3 pr-3">Venue A</th>
            <th class="pb-3 pr-3">Venue B</th>
            <th class="pb-3 pr-3">Yes / buy</th>
            <th class="pb-3 pr-3">No / sell</th>
            <th class="pb-3 pr-3">Gross</th>
            <th class="pb-3 pr-3">Fees</th>
            <th class="pb-3 pr-3">Slip.</th>
            <th class="pb-3 pr-3"><button class="sort-button is-sorted font-medium" type="button" data-sort="net">Net edge ↕</button></th>
            <th class="pb-3 pr-3">Liquidity</th>
            <th class="pb-3 pr-3">Expiry</th>
            <th class="pb-3 pr-3">Confidence</th>
            <th class="pb-3">Status</th>
           </tr>
          </thead>
          <tbody id="opportunity-table" class="divide-y divide-slate-100 text-slate-700"></tbody>
         </table>
        </div>
        <p id="table-empty" data-template-id="table-empty-state" class="canva-text hidden py-8 text-center text-sm text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 14px;">No simulated opportunities match these filters.</p>
        <div class="mt-4 flex items-center justify-between">
         <p id="page-info" class="text-xs text-slate-500">Showing 1–4 of 4 simulated opportunities</p>
         <div class="flex gap-2">
          <button id="previous-page" type="button" class="rounded-lg border border-slate-200 px-3 py-1.5 text-xs font-semibold text-slate-600 disabled:opacity-40">Previous</button><button id="next-page" type="button" class="rounded-lg border border-slate-200 px-3 py-1.5 text-xs font-semibold text-slate-600 disabled:opacity-40">Next</button>
         </div>
        </div>
       </section>
       <section class="grid gap-5 lg:grid-cols-2">
        <section data-template-id="edge-chart-panel" class="panel-card canva-panel rounded-2xl bg-white p-5" aria-labelledby="edge-chart-heading" style="background: rgb(255, 255, 255);">
         <div class="flex items-start justify-between gap-3">
          <div>
           <h2 id="edge-chart-heading" data-template-id="edge-chart-heading-text" class="canva-text font-bold" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 18px;">Net edge over time</h2>
           <p data-template-id="edge-chart-subtext" class="canva-text mt-1 text-xs text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 12px;">Illustrative history for selected sample conditions.</p>
          </div>
          <div class="flex rounded-lg bg-slate-100 p-1" role="group" aria-label="Chart range"><button class="range-button is-selected rounded-md px-2 py-1 text-xs font-semibold" type="button" data-range="6H">6H</button><button class="range-button rounded-md px-2 py-1 text-xs font-semibold" type="button" data-range="1D">1D</button><button class="range-button rounded-md px-2 py-1 text-xs font-semibold" type="button" data-range="1W">1W</button>
          </div>
         </div>
         <div id="chart-loading" class="hidden py-16 text-center text-sm text-slate-500">
          Loading simulated quote history…
         </div>
         <div id="edge-chart-wrap" class="mt-4 h-48">
          <svg class="h-full w-full" viewBox="0 0 560 180" role="img" aria-label="Simulated net edge history"><path d="M0 42H560M0 90H560M0 138H560" stroke="#edf1f5"></path> <path id="edge-area" d="M0,140 C50,129 72,114 112,121 S180,78 220,92 S281,104 321,66 S390,86 432,54 S500,65 560,29 L560,180 L0,180 Z" fill="#dbeafe"></path> <path id="edge-path" d="M0,140 C50,129 72,114 112,121 S180,78 220,92 S281,104 321,66 S390,86 432,54 S500,65 560,29" fill="none" stroke="#2563eb" stroke-width="3.5" stroke-linecap="round"></path>
          </svg>
          <div class="flex justify-between text-xs text-slate-400">
           <span id="chart-start">08:00</span><span id="chart-end">Now</span>
          </div>
         </div>
         <p data-template-id="chart-stale-note" class="canva-text mt-3 rounded-lg border px-3 py-2 text-xs" style="background: rgb(255, 247, 237); color: rgb(154, 52, 18); font-weight: 400; font-style: normal; font-size: 12px;">Stale-data state: refresh frequency and quote timing can materially affect this chart.</p>
        </section>
        <section data-template-id="venue-chart-panel" class="panel-card canva-panel rounded-2xl bg-white p-5" aria-labelledby="venue-heading" style="background: rgb(255, 255, 255);">
         <h2 id="venue-heading" data-template-id="venue-heading-text" class="canva-text font-bold" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 18px;">Venue comparison</h2>
         <p data-template-id="venue-subtext" class="canva-text mt-1 text-xs text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 12px;">Sample implied probability comparison.</p>
         <div class="mt-6 space-y-5 text-sm">
          <div>
           <div class="mb-1 flex justify-between">
            <span class="font-semibold">SignalBay</span><span class="text-slate-500">46¢ implied</span>
           </div>
           <div class="h-3 rounded-full bg-slate-100">
            <div class="h-3 w-[46%] rounded-full bg-blue-600"></div>
           </div>
          </div>
          <div>
           <div class="mb-1 flex justify-between">
            <span class="font-semibold">ForecastX</span><span class="text-slate-500">51¢ implied</span>
           </div>
           <div class="h-3 rounded-full bg-slate-100">
            <div class="h-3 w-[51%] rounded-full bg-teal-600"></div>
           </div>
          </div>
          <div>
           <div class="mb-1 flex justify-between">
            <span class="font-semibold">CivicOdds</span><span class="text-slate-500">49¢ implied</span>
           </div>
           <div class="h-3 rounded-full bg-slate-100">
            <div class="h-3 w-[49%] rounded-full bg-slate-500"></div>
           </div>
          </div>
         </div>
        </section>
       </section>
       <section data-template-id="market-monitor-panel" class="panel-card canva-panel rounded-2xl bg-white p-5 sm:p-6" aria-labelledby="monitor-heading" style="background: rgb(255, 255, 255);">
        <div class="flex items-center justify-between">
         <div>
          <h2 id="monitor-heading" data-template-id="monitor-heading-text" class="canva-text font-bold" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 20px;">Market monitor</h2>
          <p data-template-id="monitor-subtext" class="canva-text mt-1 text-sm text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 14px;">Fictional markets, quote spreads, expiry windows, and liquidity health.</p>
         </div><i data-lucide="radar" class="h-5 w-5 text-teal-600"></i>
        </div>
        <div class="mt-5 grid gap-3 md:grid-cols-3">
         <article class="rounded-xl border border-slate-100 bg-slate-50 p-4">
          <p class="text-xs font-semibold text-slate-500">Will Metro City host Expo 2027?</p>
          <p class="mt-3 text-sm font-bold">46¢ / 51¢ across venues</p>
          <p class="mt-2 text-xs text-slate-500">Volume $84k · 2d 14h · <span class="font-semibold text-emerald-700">Healthy liquidity</span></p>
         </article>
         <article class="rounded-xl border border-slate-100 bg-slate-50 p-4">
          <p class="text-xs font-semibold text-slate-500">Will River FC win the cup final?</p>
          <p class="mt-3 text-sm font-bold">61¢ / 65¢ across venues</p>
          <p class="mt-2 text-xs text-slate-500">Volume $31k · 18h · <span class="font-semibold text-amber-700">Thin liquidity</span></p>
         </article>
         <article class="rounded-xl border border-slate-100 bg-slate-50 p-4">
          <p class="text-xs font-semibold text-slate-500">Will Aurora launch by October?</p>
          <p class="mt-3 text-sm font-bold">33¢ / 37¢ across venues</p>
          <p class="mt-2 text-xs text-slate-500">Volume $57k · 6d · <span class="font-semibold text-red-700">Quote stale</span></p>
         </article>
        </div>
       </section>
       <section data-template-id="activity-panel" class="panel-card canva-panel rounded-2xl bg-white p-5 sm:p-6" aria-labelledby="activity-heading" style="background: rgb(255, 255, 255);">
        <div>
         <h2 id="activity-heading" data-template-id="activity-heading-text" class="canva-text font-bold" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 20px;">Recent simulated activity</h2>
         <p data-template-id="activity-subtext" class="canva-text mt-1 text-sm text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 14px;">Watched markets, triggered alerts, and dismissed sample opportunities.</p>
        </div>
        <ul class="mt-4 divide-y divide-slate-100 text-sm">
         <li class="flex items-center justify-between gap-4 py-3"><span><span class="font-semibold">Metro City Expo 2027</span><span class="ml-2 text-slate-500">added to simulated watchlist</span></span><span class="text-xs text-slate-400">Sample 13:42</span></li>
         <li class="flex items-center justify-between gap-4 py-3"><span><span class="font-semibold">River FC final</span><span class="ml-2 text-slate-500">simulated liquidity alert triggered</span></span><span class="text-xs text-slate-400">Sample 13:18</span></li>
         <li class="flex items-center justify-between gap-4 py-3"><span><span class="font-semibold">Aurora launch</span><span class="ml-2 text-slate-500">dismissed due to stale quote</span></span><span class="text-xs text-slate-400">Sample 12:54</span></li>
        </ul>
       </section>
      </div>
      <aside class="space-y-5" aria-label="Selected opportunity details">
       <section data-template-id="detail-panel" class="drawer-sticky panel-card canva-panel rounded-2xl bg-white p-5" aria-labelledby="detail-heading" style="background: rgb(255, 255, 255);">
        <div class="flex items-start justify-between gap-3">
         <div>
          <p data-template-id="detail-eyebrow" class="canva-text text-xs font-bold uppercase tracking-wide" style="color: rgb(37, 99, 235); font-weight: 700; font-style: normal; font-size: 12px;">Selected opportunity</p>
          <h2 id="detail-heading" class="mt-1 text-lg font-bold">Metro City Expo 2027</h2>
         </div><span data-template-id="view-only-label" class="canva-tag rounded-full px-2 py-1 text-[10px] font-bold uppercase" style="background: rgb(241, 245, 249); color: rgb(71, 85, 105); font-weight: 700; font-style: normal; font-size: 15px;">View only</span>
        </div>
        <p id="detail-question" class="mt-4 text-sm leading-relaxed text-slate-600">Will Metro City host Expo 2027?</p>
        <div class="mt-4 grid grid-cols-2 gap-3">
         <div class="rounded-xl bg-blue-50 p-3">
          <p class="text-[11px] font-semibold uppercase text-blue-700">Venue A implied</p>
          <p id="prob-a" class="mt-1 text-xl font-bold text-blue-800">46%</p>
         </div>
         <div class="rounded-xl bg-teal-50 p-3">
          <p class="text-[11px] font-semibold uppercase text-teal-700">Venue B implied</p>
          <p id="prob-b" class="mt-1 text-xl font-bold text-teal-800">51%</p>
         </div>
        </div>
        <div class="mt-4 rounded-xl border border-slate-100 p-3">
         <div class="flex justify-between text-xs">
          <span class="text-slate-500">Simulated payout illustration</span><span id="payout-value" class="font-bold text-emerald-700">+$48 / $1,000</span>
         </div>
         <div class="mt-2 flex h-3 overflow-hidden rounded-full bg-slate-100">
          <span id="payout-buy" class="bg-blue-600" style="width:46%"></span><span class="bg-teal-500" style="width:54%"></span>
         </div>
        </div>
        <div class="mt-4">
         <p data-template-id="calculation-label" class="canva-text text-xs font-bold uppercase tracking-wide text-slate-500" style="color: rgb(100, 116, 139); font-weight: 700; font-style: normal; font-size: 11px;">Sample calculation</p>
         <dl class="mt-2 space-y-2 text-sm">
          <div class="flex justify-between">
           <dt class="text-slate-500">
            Gross edge
           </dt>
           <dd id="detail-gross" class="font-semibold">
            6.2%
           </dd>
          </div>
          <div class="flex justify-between">
           <dt class="text-slate-500">
            Fees
           </dt>
           <dd id="detail-fees" class="font-semibold text-amber-700">
            −0.8%
           </dd>
          </div>
          <div class="flex justify-between">
           <dt class="text-slate-500">
            Slippage buffer
           </dt>
           <dd id="detail-slippage" class="font-semibold text-amber-700">
            −0.6%
           </dd>
          </div>
          <div class="flex justify-between border-t border-slate-100 pt-2">
           <dt class="font-bold">
            Simulated net edge
           </dt>
           <dd id="detail-net" class="font-bold text-emerald-700">
            4.8%
           </dd>
          </div>
         </dl>
        </div>
        <div class="mt-4 grid grid-cols-2 gap-3">
         <div>
          <label for="fee-input" data-template-id="fee-input-label" class="canva-text mb-1 block text-xs font-semibold text-slate-600" style="color: rgb(71, 85, 105); font-weight: 600; font-style: normal; font-size: 12px;">Fees (%)</label><input id="fee-input" class="w-full rounded-lg border border-slate-200 px-2 py-2 text-sm" type="number" value="0.8" min="0" max="10" step="0.1">
         </div>
         <div>
          <label for="slippage-input" data-template-id="slippage-input-label" class="canva-text mb-1 block text-xs font-semibold text-slate-600" style="color: rgb(71, 85, 105); font-weight: 600; font-style: normal; font-size: 12px;">Slippage (%)</label><input id="slippage-input" class="w-full rounded-lg border border-slate-200 px-2 py-2 text-sm" type="number" value="0.6" min="0" max="10" step="0.1">
         </div>
        </div>
        <p id="liquidity-warning" class="mt-4 rounded-lg border border-amber-200 bg-amber-50 px-3 py-2 text-xs text-amber-800">Liquidity can change before a simulated quote is reviewed.</p>
        <div class="mt-4 grid grid-cols-2 gap-2"><button id="watch-button" data-template-id="watch-button" type="button" class="canva-button rounded-xl border px-3 py-2.5 text-sm font-bold" style="background: rgb(255, 255, 255); color: rgb(37, 99, 235); font-weight: 700; font-style: normal; font-size: 14px;">Add to watchlist</button> <button id="add-alert-button" data-template-id="add-alert-button" type="button" class="canva-button rounded-xl bg-blue-600 px-3 py-2.5 text-sm font-bold text-white hover:bg-blue-700" style="background: rgb(37, 99, 235); color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 14px;">Add alert</button>
        </div><button id="review-button" data-template-id="review-button" type="button" class="canva-button mt-2 w-full rounded-xl border border-slate-200 bg-white px-3 py-2.5 text-sm font-bold text-slate-700 hover:bg-slate-50" style="background: rgb(255, 255, 255); color: rgb(51, 65, 85); font-weight: 700; font-style: normal; font-size: 14px;">Review strategy assumptions</button>
       </section>
       <section data-template-id="insights-panel" class="panel-card canva-panel rounded-2xl bg-white p-5" aria-labelledby="insights-heading" style="background: rgb(255, 255, 255);">
        <div class="flex items-center justify-between">
         <h2 id="insights-heading" data-template-id="insights-heading-text" class="canva-text font-bold" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 18px;">AI insights</h2><i data-lucide="sparkles" class="h-4 w-4 text-teal-600"></i>
        </div>
        <p data-template-id="insights-badge" class="canva-tag mt-3 inline-block rounded-full px-2 py-1 text-[10px] font-bold uppercase" style="background: rgb(240, 253, 250); color: rgb(15, 118, 110); font-weight: 700; font-style: normal; font-size: 15px;">Simulated analysis</p>
        <p id="insight-text" class="mt-3 text-sm leading-relaxed text-slate-600">The simulated spread is flagged because Venue A's Yes price is lower than Venue B's complementary price after the selected buffers.</p>
        <ul class="mt-3 space-y-2 text-xs leading-relaxed text-slate-500">
         <li>• Assumes both fictional quotes can be accessed at the shown size.</li>
         <li>• Fees, resolution rules, liquidity, and timing can erase a displayed edge.</li>
         <li>• This is not certainty, a recommendation, or financial advice.</li>
        </ul>
       </section>
       <section data-template-id="alerts-panel" class="panel-card canva-panel rounded-2xl bg-white p-5" aria-labelledby="alerts-heading" style="background: rgb(255, 255, 255);">
        <div class="flex items-center justify-between">
         <div>
          <h2 id="alerts-heading" data-template-id="alerts-heading-text" class="canva-text font-bold" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 18px;">Simulated alerts</h2>
          <p data-template-id="alerts-subtext" class="canva-text mt-1 text-xs text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 12px;">Create, pause, or remove session-only sample alerts.</p>
         </div><i data-lucide="bell-ring" class="h-4 w-4 text-blue-600"></i>
        </div>
        <form id="alert-form" class="mt-4 hidden rounded-xl bg-slate-50 p-3"><label for="alert-type" data-template-id="alert-type-label" class="canva-text mb-1 block text-xs font-semibold text-slate-600" style="color: rgb(71, 85, 105); font-weight: 600; font-style: normal; font-size: 12px;">Alert condition</label> <select id="alert-type" class="w-full rounded-lg border border-slate-200 bg-white px-2 py-2 text-sm"><option>Net edge threshold</option><option>Liquidity change</option><option>Approaching expiry</option><option>Stale quote</option><option>Price divergence</option></select> <label for="alert-threshold" data-template-id="alert-threshold-label" class="canva-text mb-1 mt-3 block text-xs font-semibold text-slate-600" style="color: rgb(71, 85, 105); font-weight: 600; font-style: normal; font-size: 12px;">Sample threshold</label> <input id="alert-threshold" class="w-full accent-blue-600" type="range" min="1" max="8" value="3" step="0.5">
         <div class="mt-3 flex gap-2">
          <button data-template-id="save-alert-button" type="submit" class="canva-button flex-1 rounded-lg bg-blue-600 px-3 py-2 text-xs font-bold text-white" style="background: rgb(37, 99, 235); color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 12px;">Save simulated alert</button><button id="cancel-alert-button" data-template-id="cancel-alert-button" type="button" class="canva-button rounded-lg border border-slate-200 px-3 py-2 text-xs font-bold text-slate-600" style="background: rgb(255, 255, 255); color: rgb(71, 85, 105); font-weight: 700; font-style: normal; font-size: 12px;">Cancel</button>
         </div>
        </form>
        <div id="alerts-list" class="mt-4 space-y-2"></div>
       </section>
      </aside>
     </section>
     <footer class="mt-6 pb-2">
      <p data-template-id="footer-disclaimer" class="canva-text text-center text-xs leading-relaxed text-slate-500" style="color: rgb(100, 116, 139); font-weight: 400; font-style: normal; font-size: 12px; line-height: 1.5;">This dashboard uses fictional, simulated sample data for educational analytics only. Opportunities can disappear quickly; fees, liquidity, settlement rules, timing, and stale quotes matter. Nothing shown is financial advice, a guarantee, or an instruction to trade. No orders can be placed from this page.</p>
     </footer>
    </main>
   </div>
  </div>
  <div id="strategy-modal" class="modal-backdrop fixed inset-0 z-50 hidden items-center justify-center p-4" role="dialog" aria-modal="true" aria-labelledby="modal-heading">
   <section data-template-id="strategy-modal-card" class="canva-card w-full max-w-lg rounded-2xl bg-white p-6 shadow-2xl" style="background: rgb(255, 255, 255);">
    <div class="flex items-start justify-between gap-4">
     <div>
      <p data-template-id="modal-eyebrow" class="canva-text text-xs font-bold uppercase tracking-wider" style="color: rgb(37, 99, 235); font-weight: 700; font-style: normal; font-size: 12px;">View-only explanation</p>
      <h2 id="modal-heading" data-template-id="modal-heading-text" class="canva-text mt-1 font-bold" style="color: rgb(20, 33, 61); font-weight: 700; font-style: normal; font-size: 23px;">Risk and assumptions review</h2>
     </div><button id="close-modal" type="button" class="rounded-lg p-1.5 text-slate-500 hover:bg-slate-100" aria-label="Close explanation"><i data-lucide="x" class="h-5 w-5"></i></button>
    </div>
    <div class="mt-5 rounded-xl bg-slate-50 p-4 text-sm leading-relaxed text-slate-600">
     <p>This is a view-only educational review. No order is created, routed, or sent anywhere.</p>
     <ul class="mt-3 list-disc space-y-2 pl-5">
      <li>Displayed quotes and venue names are fictional samples.</li>
      <li>Price movement, fees, available liquidity, settlement timing, and differing market rules may invalidate the simulated calculation.</li>
      <li>A positive historical or displayed edge does not mean a profit is available.</li>
     </ul>
    </div><button id="modal-close-button" data-template-id="modal-close-button" type="button" class="canva-button mt-5 w-full rounded-xl border border-slate-200 bg-white px-4 py-2.5 text-sm font-bold text-slate-700" style="background: rgb(255, 255, 255); color: rgb(51, 65, 85); font-weight: 700; font-style: normal; font-size: 14px;">Close review</button>
   </section>
  </div>
  <script src="/_sdk/0aac212797dcb9a6.editing_sdk.js" integrity="sha512-U1Z5TGB/MTX0fFSADhP7rVM3+UzJJjKTapiY1vm1cxcbcyWo4eBuCJNJO6zARJ5kHopP9UvWNtPszOqzRc1ICA=="></script>
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      lucide.createIcons();
      const opportunities = [
        { id:1, event:"Metro City Expo 2027", market:"Hosts Expo 2027 · YES", a:"SignalBay", b:"ForecastX", buy:46, sell:48, gross:6.2, fees:.8, slip:.6, net:4.8, liquidity:84, expiry:"2d 14h", confidence:"High", status:"Fresh", actionable:true, question:"Will Metro City host Expo 2027?" },
        { id:2, event:"River FC Cup Final", market:"Wins final · YES", a:"ForecastX", b:"CivicOdds", buy:61, sell:63, gross:4.9, fees:.9, slip:.7, net:3.3, liquidity:31, expiry:"18h", confidence:"Medium", status:"Fresh", actionable:false, question:"Will River FC win the cup final?" },
        { id:3, event:"Aurora Launch", market:"Launches by October · YES", a:"CivicOdds", b:"SignalBay", buy:33, sell:35, gross:5.6, fees:1.0, slip:.8, net:3.8, liquidity:57, expiry:"6d", confidence:"Medium", status:"Stale", actionable:true, question:"Will Aurora launch by October?" },
        { id:4, event:"Coastal Transit Vote", market:"Measure passes · YES", a:"SignalBay", b:"CivicOdds", buy:52, sell:54, gross:3.8, fees:.7, slip:.5, net:2.6, liquidity:102, expiry:"9d", confidence:"High", status:"Fresh", actionable:true, question:"Will the Coastal Transit measure pass?" }
      ];
      let selected = opportunities[0], sortDescending = true, currentPage = 1, watched = false, alerts = [{ id:1, text:"Net edge ≥ 3.0%", paused:false }];

      const $ = id => document.getElementById(id);
      function renderTable() {
        const venue = $("venue-filter").value, min = Number($("edge-filter").value), query = $("table-search").value.toLowerCase(), actionable = $("liquidity-toggle").checked;
        let rows = opportunities.filter(o => (venue === "all" || o.a === venue || o.b === venue) && o.net >= min && (!actionable || o.actionable) && (o.event + o.market).toLowerCase().includes(query));
        rows.sort((a,b) => sortDescending ? b.net-a.net : a.net-b.net);
        $("opportunity-table").innerHTML = rows.map(o => `<tr class="opportunity-row ${selected.id===o.id?"is-selected":""}" data-id="${o.id}" tabindex="0">
          <td class="py-3 pr-3 font-semibold text-slate-800">${o.event}<span class="ml-1 rounded bg-slate-100 px-1 py-0.5 text-[9px] font-bold text-slate-500">SIM</span></td><td class="py-3 pr-3">${o.market}</td><td class="py-3 pr-3">${o.a}</td><td class="py-3 pr-3">${o.b}</td><td class="py-3 pr-3">${o.buy}¢</td><td class="py-3 pr-3">${o.sell}¢</td><td class="py-3 pr-3">${o.gross.toFixed(1)}%</td><td class="py-3 pr-3">${o.fees.toFixed(1)}%</td><td class="py-3 pr-3">${o.slip.toFixed(1)}%</td><td class="py-3 pr-3 font-bold text-emerald-700">${o.net.toFixed(1)}%</td><td class="py-3 pr-3">$${o.liquidity}k</td><td class="py-3 pr-3">${o.expiry}</td><td class="py-3 pr-3">${o.confidence}</td><td class="py-3"><span class="rounded-full px-2 py-1 text-[10px] font-bold ${o.status==="Stale"?"bg-red-50 text-red-700":"bg-emerald-50 text-emerald-700"}">${o.status}</span></td>
        </tr>`).join("");
        $("table-empty").classList.toggle("hidden", rows.length !== 0);
        $("page-info").textContent = rows.length ? `Showing 1–${rows.length} of ${rows.length} simulated opportunities` : "No simulated opportunities match these filters";
        $("open-count").textContent = rows.length;
        $("best-edge").textContent = rows.length ? Math.max(...rows.map(o=>o.net)).toFixed(1)+"%" : "—";
        $("capital-required").textContent = rows.length ? "$"+(Math.min(...rows.map(o=>o.liquidity))*20).toLocaleString() : "—";
        document.querySelectorAll(".opportunity-row").forEach(row => {
          const choose = () => { selected = opportunities.find(o => o.id === Number(row.dataset.id)); renderDetail(); renderTable(); };
          row.addEventListener("click", choose); row.addEventListener("keydown", e => { if(e.key==="Enter" || e.key===" ") { e.preventDefault(); choose(); } });
        });
      }
      function renderDetail() {
        $("detail-heading").textContent = selected.event; $("detail-question").textContent = selected.question;
        $("prob-a").textContent = selected.buy+"%"; $("prob-b").textContent = (100-selected.sell)+"%";
        $("detail-gross").textContent = selected.gross.toFixed(1)+"%"; $("fee-input").value = selected.fees; $("slippage-input").value = selected.slip;
        $("liquidity-warning").textContent = selected.actionable ? `Sample liquidity estimate: $${selected.liquidity}k. Quotes can change before review.` : `Sample liquidity is thin at $${selected.liquidity}k. This displayed edge may not support the shown size.`;
        $("insight-text").textContent = `Simulated analysis: ${selected.a}'s ${selected.buy}¢ quote differs from ${selected.b}'s complementary ${selected.sell}¢ quote. The indicator remains sensitive to fees, liquidity, and quote freshness.`;
        updateCalculation();
      }
      function updateCalculation() {
        const fee = Number($("fee-input").value)||0, slip = Number($("slippage-input").value)||0, net = Math.max(0, selected.gross-fee-slip);
        $("detail-fees").textContent = "−"+fee.toFixed(1)+"%"; $("detail-slippage").textContent = "−"+slip.toFixed(1)+"%"; $("detail-net").textContent = net.toFixed(1)+"%";
        $("payout-value").textContent = "+$"+Math.round(net*10)+" / $1,000";
      }
      function renderAlerts() {
        $("alerts-list").innerHTML = alerts.length ? alerts.map(a => `<div class="flex items-center justify-between gap-2 rounded-lg border border-slate-100 p-2 text-xs"><span class="${a.paused?"text-slate-400 line-through":"font-semibold text-slate-700"}">${a.text}</span><span class="flex gap-1"><button class="pause-alert rounded px-2 py-1 text-blue-700 hover:bg-blue-50" data-id="${a.id}">${a.paused?"Resume":"Pause"}</button><button class="delete-alert rounded px-2 py-1 text-red-700 hover:bg-red-50" data-id="${a.id}">Delete</button></span></div>`).join("") : `<p class="text-center text-xs text-slate-500">No simulated alerts yet.</p>`;
        document.querySelectorAll(".pause-alert").forEach(b=>b.addEventListener("click",()=>{ const a=alerts.find(x=>x.id===Number(b.dataset.id)); a.paused=!a.paused; renderAlerts(); }));
        document.querySelectorAll(".delete-alert").forEach(b=>b.addEventListener("click",()=>{ alerts=alerts.filter(x=>x.id!==Number(b.dataset.id)); renderAlerts(); }));
      }
      ["venue-filter","edge-filter","table-search","liquidity-toggle"].forEach(id => $(id).addEventListener(id==="edge-filter"?"input":"input", () => { $("edge-output").textContent = $("edge-filter").value+"%"; renderTable(); }));
      $("edge-filter").addEventListener("change", renderTable);
      document.querySelector("[data-sort='net']").addEventListener("click", () => { sortDescending=!sortDescending; document.querySelector("[data-sort='net']").textContent=sortDescending?"Net edge ↓":"Net edge ↑"; renderTable(); });
      ["fee-input","slippage-input"].forEach(id => $(id).addEventListener("input", updateCalculation));
      $("market-search").addEventListener("input", e => { $("table-search").value=e.target.value; renderTable(); });
      $("watch-button").addEventListener("click", () => { watched=!watched; $("watch-button").textContent=watched?"Watching market":"Add to watchlist"; });
      $("add-alert-button").addEventListener("click",()=>{ $("alert-form").classList.remove("hidden"); $("alert-type").focus(); });
      $("cancel-alert-button").addEventListener("click",()=> $("alert-form").classList.add("hidden"));
      $("alert-form").addEventListener("submit",e=>{ e.preventDefault(); alerts.push({id:Date.now(), text:$("alert-type").value+" · "+$("alert-threshold").value+"% sample threshold",paused:false}); $("alert-form").classList.add("hidden"); renderAlerts(); });
      const modal=$("strategy-modal");
      function closeModal(){ modal.classList.add("hidden"); modal.classList.remove("flex"); $("review-button").focus(); }
      $("review-button").addEventListener("click",()=>{ modal.classList.remove("hidden"); modal.classList.add("flex"); $("close-modal").focus(); });
      $("close-modal").addEventListener("click",closeModal); $("modal-close-button").addEventListener("click",closeModal); modal.addEventListener("click",e=>{if(e.target===modal)closeModal();});
      document.addEventListener("keydown",e=>{if(e.key==="Escape"&&!modal.classList.contains("hidden"))closeModal();});
      const paths={ "6H":["M0,140 C50,129 72,114 112,121 S180,78 220,92 S281,104 321,66 S390,86 432,54 S500,65 560,29","08:00","Now"], "1D":["M0,135 C52,96 77,124 118,105 S182,143 225,91 S284,111 330,79 S387,101 430,56 S503,79 560,38","Yesterday","Now"], "1W":["M0,145 C49,135 78,102 116,119 S176,88 222,107 S282,59 330,82 S391,48 432,74 S502,53 560,30","Mon","Today"] };
      document.querySelectorAll(".range-button").forEach(b=>b.addEventListener("click",()=>{ document.querySelectorAll(".range-button").forEach(x=>x.classList.toggle("is-selected",x===b)); const s=paths[b.dataset.range]; $("edge-path").setAttribute("d",s[0]); $("edge-area").setAttribute("d",s[0]+" L560,180 L0,180 Z"); $("chart-start").textContent=s[1]; $("chart-end").textContent=s[2]; }));
      document.querySelectorAll(".nav-item").forEach(b=>b.addEventListener("click",()=>{ const section=b.dataset.section; document.querySelectorAll(".nav-item").forEach(x=>{const on=x.dataset.section===section;x.classList.toggle("is-active",on);if(on)x.setAttribute("aria-current","page");else x.removeAttribute("aria-current");}); $("section-title").textContent=section==="Overview"?"Opportunity overview":section; document.body.classList.remove("mobile-menu-open"); $("mobile-menu-button").setAttribute("aria-expanded","false"); }));
      $("mobile-menu-button").addEventListener("click",()=>{document.body.classList.toggle("mobile-menu-open");$("mobile-menu-button").setAttribute("aria-expanded",document.body.classList.contains("mobile-menu-open"));});
      $("previous-page").disabled=true; $("next-page").disabled=true;
      $("watch-button").textContent="Add to watchlist";
      renderTable(); renderDetail(); renderAlerts();
    });
  </script>
 
</body></html>
