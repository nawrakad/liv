<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>ATOMIC — Student Athlete OS</title>
<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
<style>
  :root {
    --neon: #00f5d4;
    --neon2: #7b2ff7;
    --neon3: #ff4d6d;
    --neon4: #ffd60a;
    --bg: #060912;
    --bg2: #0d1117;
    --bg3: #131a24;
    --bg4: #1a2332;
    --border: rgba(0,245,212,0.15);
    --text: #e2e8f0;
    --muted: #64748b;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
    background: var(--bg);
    color: var(--text);
    min-height: 100vh;
    overflow-x: hidden;
  }
  ::-webkit-scrollbar { width: 4px; }
  ::-webkit-scrollbar-track { background: var(--bg2); }
  ::-webkit-scrollbar-thumb { background: var(--neon2); border-radius: 4px; }

  /* GRID NOISE BACKGROUND */
  body::before {
    content: '';
    position: fixed;
    inset: 0;
    background-image:
      linear-gradient(rgba(0,245,212,0.03) 1px, transparent 1px),
      linear-gradient(90deg, rgba(0,245,212,0.03) 1px, transparent 1px);
    background-size: 40px 40px;
    pointer-events: none;
    z-index: 0;
  }

  /* NEON GLOW UTILITIES */
  .glow-cyan { text-shadow: 0 0 12px var(--neon), 0 0 30px rgba(0,245,212,0.4); }
  .glow-purple { text-shadow: 0 0 12px var(--neon2), 0 0 30px rgba(123,47,247,0.4); }
  .glow-red { text-shadow: 0 0 12px var(--neon3), 0 0 30px rgba(255,77,109,0.4); }
  .glow-yellow { text-shadow: 0 0 12px var(--neon4), 0 0 30px rgba(255,214,10,0.4); }
  .border-glow { box-shadow: 0 0 0 1px var(--border), 0 0 20px rgba(0,245,212,0.05); }
  .border-glow-active { box-shadow: 0 0 0 1px rgba(0,245,212,0.5), 0 0 25px rgba(0,245,212,0.15); }

  /* CARD */
  .card {
    background: var(--bg2);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 24px;
    position: relative;
    overflow: hidden;
    transition: all 0.3s ease;
  }
  .card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 1px;
    background: linear-gradient(90deg, transparent, var(--neon), transparent);
    opacity: 0.4;
  }
  .card:hover { border-color: rgba(0,245,212,0.3); transform: translateY(-2px); }
  .card.no-hover:hover { transform: none; }

  /* SECTION LABELS */
  .section-tag {
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--neon);
    margin-bottom: 6px;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .section-tag::after {
    content: '';
    flex: 1;
    height: 1px;
    background: linear-gradient(90deg, var(--border), transparent);
  }

  /* BUTTONS */
  .btn {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 8px 18px;
    border-radius: 8px;
    font-size: 13px;
    font-weight: 600;
    cursor: pointer;
    border: none;
    transition: all 0.25s ease;
    letter-spacing: 0.5px;
  }
  .btn-neon {
    background: linear-gradient(135deg, var(--neon), #00b4d8);
    color: #000;
  }
  .btn-neon:hover { box-shadow: 0 0 20px rgba(0,245,212,0.5); transform: translateY(-1px); }
  .btn-ghost {
    background: transparent;
    border: 1px solid var(--border);
    color: var(--text);
  }
  .btn-ghost:hover { border-color: var(--neon); color: var(--neon); }
  .btn-danger {
    background: rgba(255,77,109,0.1);
    border: 1px solid rgba(255,77,109,0.3);
    color: var(--neon3);
  }
  .btn-danger:hover { background: rgba(255,77,109,0.2); }

  /* PROGRESS BAR */
  .progress-wrap {
    width: 100%;
    height: 6px;
    background: var(--bg4);
    border-radius: 99px;
    overflow: hidden;
  }
  .progress-fill {
    height: 100%;
    border-radius: 99px;
    transition: width 0.8s cubic-bezier(0.4,0,0.2,1);
    position: relative;
  }
  .progress-fill::after {
    content: '';
    position: absolute;
    right: 0; top: 0; bottom: 0;
    width: 20px;
    background: rgba(255,255,255,0.3);
    border-radius: 99px;
    filter: blur(4px);
  }
  .progress-cyan { background: linear-gradient(90deg, #00b4d8, var(--neon)); }
  .progress-purple { background: linear-gradient(90deg, #5a00c8, var(--neon2)); }
  .progress-red { background: linear-gradient(90deg, #c0004a, var(--neon3)); }

  /* COUNTDOWN */
  .countdown-digit {
    background: var(--bg3);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 12px 18px;
    font-size: clamp(22px, 4vw, 36px);
    font-weight: 800;
    color: var(--neon);
    font-variant-numeric: tabular-nums;
    min-width: 70px;
    text-align: center;
    letter-spacing: 2px;
    position: relative;
    overflow: hidden;
  }
  .countdown-digit::before {
    content: '';
    position: absolute;
    inset: 0;
    background: linear-gradient(180deg, rgba(0,245,212,0.05) 0%, transparent 50%);
  }

  /* HABIT ITEM */
  .habit-item {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 14px 16px;
    background: var(--bg3);
    border: 1px solid var(--border);
    border-radius: 12px;
    transition: all 0.25s ease;
    cursor: default;
  }
  .habit-item:hover { border-color: rgba(0,245,212,0.25); background: var(--bg4); }
  .habit-check {
    width: 22px;
    height: 22px;
    border-radius: 6px;
    border: 2px solid var(--muted);
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    transition: all 0.2s ease;
    flex-shrink: 0;
  }
  .habit-check.checked {
    background: var(--neon);
    border-color: var(--neon);
    box-shadow: 0 0 12px rgba(0,245,212,0.4);
  }
  .habit-check svg { display: none; }
  .habit-check.checked svg { display: block; }
  .streak-badge {
    margin-left: auto;
    display: flex;
    align-items: center;
    gap: 4px;
    background: rgba(255,214,10,0.1);
    border: 1px solid rgba(255,214,10,0.2);
    border-radius: 20px;
    padding: 3px 10px;
    font-size: 12px;
    font-weight: 700;
    color: var(--neon4);
    white-space: nowrap;
    flex-shrink: 0;
  }

  /* TIME BLOCK */
  .time-block {
    display: flex;
    gap: 12px;
    align-items: flex-start;
    padding: 8px 0;
    border-bottom: 1px solid rgba(255,255,255,0.04);
  }
  .time-block:last-child { border-bottom: none; }
  .time-label {
    font-size: 11px;
    color: var(--muted);
    font-weight: 600;
    min-width: 44px;
    padding-top: 8px;
    letter-spacing: 0.5px;
  }
  .time-input {
    flex: 1;
    background: var(--bg3);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 7px 12px;
    font-size: 13px;
    color: var(--text);
    outline: none;
    transition: all 0.2s ease;
    resize: none;
    font-family: inherit;
    min-height: 36px;
    line-height: 1.4;
  }
  .time-input:focus { border-color: var(--neon); box-shadow: 0 0 10px rgba(0,245,212,0.1); }
  .time-input.prefilled { color: var(--neon); font-weight: 600; }
  .time-input.workout { color: var(--neon3); font-weight: 600; }
  .time-input.fast { color: var(--neon4); font-weight: 600; }

  /* INPUT FIELDS */
  input[type="text"], input[type="number"], input[type="time"], input[type="email"], textarea, select {
    background: var(--bg3);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 10px 14px;
    font-size: 14px;
    color: var(--text);
    outline: none;
    transition: border-color 0.2s ease, box-shadow 0.2s ease;
    font-family: inherit;
    width: 100%;
  }
  input:focus, textarea:focus, select:focus {
    border-color: var(--neon);
    box-shadow: 0 0 12px rgba(0,245,212,0.1);
  }
  input::placeholder, textarea::placeholder { color: var(--muted); }
  select option { background: var(--bg3); }

  /* QUOTE TICKER */
  @keyframes fadeSlide {
    0% { opacity: 0; transform: translateY(10px); }
    10% { opacity: 1; transform: translateY(0); }
    85% { opacity: 1; transform: translateY(0); }
    100% { opacity: 0; transform: translateY(-10px); }
  }
  .quote-animate { animation: fadeSlide 8s ease-in-out infinite; }

  /* DAY PROGRESS ARC */
  .day-arc-wrap { position: relative; display: inline-block; }
  .day-arc-wrap svg { transform: rotate(-90deg); }
  .arc-text {
    position: absolute;
    inset: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-weight: 800;
  }

  /* NAV */
  .nav-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 3px;
    padding: 8px 12px;
    border-radius: 12px;
    cursor: pointer;
    transition: all 0.2s ease;
    font-size: 10px;
    font-weight: 600;
    color: var(--muted);
    letter-spacing: 0.5px;
    text-transform: uppercase;
    border: 1px solid transparent;
    white-space: nowrap;
  }
  .nav-item.active {
    color: var(--neon);
    background: rgba(0,245,212,0.08);
    border-color: rgba(0,245,212,0.2);
  }
  .nav-item:hover:not(.active) { color: var(--text); background: var(--bg3); }

  /* SECTION PANELS */
  .panel { display: none; }
  .panel.active { display: block; }

  /* IDENTITY GOAL */
  .identity-card {
    background: linear-gradient(135deg, rgba(123,47,247,0.1), rgba(0,245,212,0.05));
    border: 1px solid rgba(123,47,247,0.3);
  }

  /* PROTOCOL ITEM */
  .protocol-item {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 12px 14px;
    background: var(--bg3);
    border: 1px solid var(--border);
    border-radius: 10px;
    transition: all 0.2s;
  }
  .protocol-item:hover { border-color: rgba(0,245,212,0.2); }
  .protocol-check {
    width: 18px;
    height: 18px;
    border-radius: 50%;
    border: 2px solid var(--muted);
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    transition: all 0.2s;
    flex-shrink: 0;
  }
  .protocol-check.done {
    background: var(--neon);
    border-color: var(--neon);
    box-shadow: 0 0 10px rgba(0,245,212,0.35);
  }
  .protocol-check.done::after { content: '✓'; font-size: 10px; color: #000; font-weight: 900; }

  /* STAT BADGE */
  .stat-box {
    background: var(--bg3);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 14px;
    text-align: center;
    transition: all 0.3s;
  }
  .stat-box:hover { border-color: rgba(0,245,212,0.3); }

  /* MODAL */
  .modal-overlay {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.75);
    backdrop-filter: blur(6px);
    z-index: 100;
    align-items: center;
    justify-content: center;
    padding: 20px;
  }
  .modal-overlay.open { display: flex; }
  .modal-box {
    background: var(--bg2);
    border: 1px solid rgba(0,245,212,0.2);
    border-radius: 20px;
    padding: 28px;
    width: 100%;
    max-width: 440px;
    position: relative;
    box-shadow: 0 0 60px rgba(0,245,212,0.1);
  }

  /* RING */
  @keyframes ring-pulse { 0%,100%{opacity:1} 50%{opacity:0.5} }
  .ring-pulse { animation: ring-pulse 2s ease-in-out infinite; }

  /* TOAST */
  .toast {
    position: fixed;
    bottom: 80px;
    right: 20px;
    background: var(--bg3);
    border: 1px solid var(--neon);
    border-radius: 10px;
    padding: 12px 18px;
    font-size: 13px;
    font-weight: 600;
    color: var(--neon);
    z-index: 999;
    transform: translateX(200px);
    opacity: 0;
    transition: all 0.3s ease;
    box-shadow: 0 0 20px rgba(0,245,212,0.2);
    max-width: 280px;
  }
  .toast.show { transform: translateX(0); opacity: 1; }

  /* MOBILE NAV */
  @media (max-width: 640px) {
    .nav-bar { overflow-x: auto; }
    .nav-bar::-webkit-scrollbar { display: none; }
    .card { padding: 18px; }
    .countdown-digit { min-width: 56px; padding: 10px 12px; }
  }

  /* SHIMMER on load */
  @keyframes shimmer {
    0% { background-position: -200% center; }
    100% { background-position: 200% center; }
  }
  .shimmer-text {
    background: linear-gradient(90deg, var(--neon), #fff, var(--neon2), var(--neon));
    background-size: 200% auto;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: shimmer 4s linear infinite;
  }

  /* WEIGHT HISTORY */
  .weight-dot {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: var(--neon);
    border: 2px solid var(--bg2);
    box-shadow: 0 0 8px rgba(0,245,212,0.4);
  }

  /* FASTING STATE */
  .fasting-active { border-color: rgba(255,214,10,0.4) !important; }
  .fasting-active::before { background: linear-gradient(90deg, transparent, var(--neon4), transparent) !important; }

  @keyframes pulse-border {
    0%,100% { box-shadow: 0 0 0 0 rgba(0,245,212,0.4); }
    50% { box-shadow: 0 0 0 8px rgba(0,245,212,0); }
  }
  .pulse-anim { animation: pulse-border 2s ease-in-out infinite; }

  /* MEAL TRACKER */
  .macro-ring-wrap { position: relative; display: inline-flex; align-items: center; justify-content: center; }
  .macro-ring-wrap svg { transform: rotate(-90deg); }
  .macro-ring-center {
    position: absolute;
    inset: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .meal-card {
    background: var(--bg3);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 14px 16px;
    transition: all 0.25s ease;
  }
  .meal-card:hover { border-color: rgba(0,245,212,0.25); background: var(--bg4); }
  .macro-pill {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    padding: 2px 8px;
    border-radius: 20px;
    font-size: 10px;
    font-weight: 700;
  }
  .macro-pill.protein { background: rgba(255,77,109,0.12); color: var(--neon3); border: 1px solid rgba(255,77,109,0.2); }
  .macro-pill.carbs { background: rgba(255,214,10,0.12); color: var(--neon4); border: 1px solid rgba(255,214,10,0.2); }
  .macro-pill.fat { background: rgba(123,47,247,0.12); color: var(--neon2); border: 1px solid rgba(123,47,247,0.2); }
  .macro-pill.cal { background: rgba(0,245,212,0.12); color: var(--neon); border: 1px solid rgba(0,245,212,0.2); }
  .preset-chip {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    padding: 6px 12px;
    border-radius: 20px;
    font-size: 11px;
    font-weight: 600;
    cursor: pointer;
    border: 1px solid var(--border);
    background: var(--bg3);
    color: var(--text);
    transition: all 0.2s ease;
    white-space: nowrap;
  }
  .preset-chip:hover { border-color: var(--neon); color: var(--neon); background: rgba(0,245,212,0.06); transform: translateY(-1px); }
  .meal-type-badge {
    font-size: 9px;
    font-weight: 700;
    letter-spacing: 1px;
    text-transform: uppercase;
    padding: 2px 8px;
    border-radius: 4px;
    display: inline-block;
  }
  .meal-type-badge.breakfast { background: rgba(255,214,10,0.15); color: var(--neon4); }
  .meal-type-badge.lunch { background: rgba(0,245,212,0.15); color: var(--neon); }
  .meal-type-badge.dinner { background: rgba(123,47,247,0.15); color: var(--neon2); }
  .meal-type-badge.snack { background: rgba(255,77,109,0.15); color: var(--neon3); }
  .meal-type-badge.pre-workout { background: rgba(0,180,216,0.15); color: #00b4d8; }
  .meal-type-badge.post-workout { background: rgba(0,245,212,0.15); color: var(--neon); }
  .meal-type-badge.suhoor { background: rgba(255,214,10,0.2); color: var(--neon4); }
  .meal-type-badge.iftar { background: rgba(255,214,10,0.2); color: var(--neon4); }
  @keyframes countUp {
    from { opacity: 0; transform: translateY(8px); }
    to { opacity: 1; transform: translateY(0); }
  }
  .count-up-anim { animation: countUp 0.4s ease-out; }
</style>
</head>
<body>

<!-- TOAST -->
<div class="toast" id="toast"></div>

<!-- MODAL: Add Habit -->
<div class="modal-overlay" id="habitModal">
  <div class="modal-box">
    <div class="section-tag mb-4">Add New Habit</div>
    <h3 class="text-lg font-bold mb-4 text-white">Define Your Habit</h3>
    <div class="flex flex-col gap-4">
      <div>
        <label class="text-xs text-slate-400 mb-1 block uppercase tracking-widest">Habit Name</label>
        <input type="text" id="habitNameInput" placeholder="e.g. Gym, Read 10 pages, Cold shower..." />
      </div>
      <div>
        <label class="text-xs text-slate-400 mb-1 block uppercase tracking-widest">Category</label>
        <select id="habitCatInput">
          <option value="🏋️ Fitness">🏋️ Fitness</option>
          <option value="📖 Mind">📖 Mind</option>
          <option value="🕌 Spirit">🕌 Spirit</option>
          <option value="🥗 Nutrition">🥗 Nutrition</option>
          <option value="😴 Recovery">😴 Recovery</option>
          <option value="💼 Grind">💼 Grind</option>
        </select>
      </div>
      <div class="flex gap-3 mt-2">
        <button class="btn btn-ghost flex-1" onclick="closeModal('habitModal')">Cancel</button>
        <button class="btn btn-neon flex-1" onclick="addHabit()">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3"><path d="M12 5v14M5 12h14"/></svg>
          Add Habit
        </button>
      </div>
    </div>
  </div>
</div>

<!-- MODAL: Weight Entry -->
<div class="modal-overlay" id="weightModal">
  <div class="modal-box">
    <div class="section-tag mb-4">Log Weight</div>
    <h3 class="text-lg font-bold mb-4 text-white">Today's Weigh-In</h3>
    <div class="flex flex-col gap-4">
      <div>
        <label class="text-xs text-slate-400 mb-1 block uppercase tracking-widest">Weight (kg)</label>
        <input type="number" id="weightInput" step="0.1" placeholder="e.g. 91.5" min="30" max="300" />
      </div>
      <div class="flex gap-3 mt-2">
        <button class="btn btn-ghost flex-1" onclick="closeModal('weightModal')">Cancel</button>
        <button class="btn btn-neon flex-1" onclick="logWeight()">Log It</button>
      </div>
    </div>
  </div>
</div>

<!-- MODAL: Add Meal -->
<div class="modal-overlay" id="mealModal">
  <div class="modal-box" style="max-width:480px">
    <div class="section-tag mb-4">Log Meal</div>
    <h3 class="text-lg font-bold mb-4 text-white">🍽️ What Did You Eat?</h3>
    <div class="flex flex-col gap-3">
      <div>
        <label class="text-[10px] text-slate-400 mb-1 block uppercase tracking-widest">Meal Name</label>
        <input type="text" id="mealNameInput" placeholder="e.g. Grilled chicken + rice..." />
      </div>
      <div class="grid grid-cols-2 gap-3">
        <div>
          <label class="text-[10px] text-slate-400 mb-1 block uppercase tracking-widest">Meal Type</label>
          <select id="mealTypeInput">
            <option value="breakfast">☀️ Breakfast</option>
            <option value="lunch">🌤️ Lunch</option>
            <option value="dinner">🌙 Dinner</option>
            <option value="snack">🍎 Snack</option>
            <option value="pre-workout">⚡ Pre-Workout</option>
            <option value="post-workout">💪 Post-Workout</option>
            <option value="suhoor">🌅 Suhoor</option>
            <option value="iftar">🌙 Iftar</option>
          </select>
        </div>
        <div>
          <label class="text-[10px] text-slate-400 mb-1 block uppercase tracking-widest">Calories (kcal)</label>
          <input type="number" id="mealCalInput" placeholder="500" min="0" step="1" />
        </div>
      </div>
      <div class="grid grid-cols-3 gap-3">
        <div>
          <label class="text-[10px] text-slate-400 mb-1 block uppercase tracking-widest">Protein (g)</label>
          <input type="number" id="mealProteinInput" placeholder="40" min="0" step="1" />
        </div>
        <div>
          <label class="text-[10px] text-slate-400 mb-1 block uppercase tracking-widest">Carbs (g)</label>
          <input type="number" id="mealCarbsInput" placeholder="60" min="0" step="1" />
        </div>
        <div>
          <label class="text-[10px] text-slate-400 mb-1 block uppercase tracking-widest">Fat (g)</label>
          <input type="number" id="mealFatInput" placeholder="15" min="0" step="1" />
        </div>
      </div>
      <div class="flex gap-3 mt-2">
        <button class="btn btn-ghost flex-1" onclick="closeModal('mealModal')">Cancel</button>
        <button class="btn btn-neon flex-1" onclick="addMeal()">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3"><path d="M12 5v14M5 12h14"/></svg>
          Log Meal
        </button>
      </div>
    </div>
  </div>
</div>

<!-- WRAPPER -->
<div class="relative z-10 max-w-2xl mx-auto px-4 pb-28 pt-6">

  <!-- ======= HEADER ======= -->
  <div class="flex items-center justify-between mb-6">
    <div>
      <p class="text-xs text-slate-500 uppercase tracking-widest font-semibold" id="dateDisplay">—</p>
      <h1 class="text-2xl font-black shimmer-text mt-1 leading-none">ATOMIC OS</h1>
      <p class="text-xs text-slate-500 mt-0.5">Student × Athlete Protocol</p>
    </div>
    <div class="day-arc-wrap">
      <svg width="72" height="72" viewBox="0 0 72 72">
        <circle cx="36" cy="36" r="30" fill="none" stroke="rgba(255,255,255,0.05)" stroke-width="5"/>
        <circle id="dayArc" cx="36" cy="36" r="30" fill="none" stroke="url(#arcGrad)" stroke-width="5"
          stroke-linecap="round" stroke-dasharray="188.5" stroke-dashoffset="188.5" transition="stroke-dashoffset 1s ease"/>
        <defs>
          <linearGradient id="arcGrad" x1="0%" y1="0%" x2="100%" y2="0%">
            <stop offset="0%" stop-color="#00b4d8"/>
            <stop offset="100%" stop-color="#00f5d4"/>
          </linearGradient>
        </defs>
      </svg>
      <div class="arc-text">
        <span class="text-xs font-black glow-cyan" id="arcPct">0%</span>
        <span class="text-[8px] text-slate-500 uppercase tracking-wider">Day</span>
      </div>
    </div>
  </div>

  <!-- ======= CLOCK + QUOTE ======= -->
  <div class="card no-hover mb-4">
    <div class="flex items-center justify-between gap-4">
      <div>
        <div class="text-4xl font-black glow-cyan tracking-tighter" id="clockDisplay">00:00:00</div>
        <div id="quoteWrap" class="mt-3 max-w-sm">
          <p class="text-xs text-slate-400 italic leading-relaxed quote-animate" id="quoteText">"Stay hard."</p>
          <p class="text-[10px] text-slate-600 mt-1 font-semibold tracking-widest uppercase" id="quoteAuthor">— David Goggins</p>
        </div>
      </div>
      <div class="text-right flex-shrink-0">
        <div class="text-[10px] text-slate-500 uppercase tracking-widest mb-1">1% Better</div>
        <div class="w-24">
          <div class="progress-wrap mb-1" style="height:8px">
            <div class="progress-fill progress-cyan" id="dayProgressBar" style="width:0%"></div>
          </div>
          <div class="text-right text-[10px] text-slate-500" id="dayProgressText">0%</div>
        </div>
        <button class="btn btn-ghost mt-2 text-[10px] px-2 py-1" onclick="nextQuote()">
          <svg width="10" height="10" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path d="M17 1l4 4-4 4"/><path d="M3 11V9a4 4 0 014-4h14M7 23l-4-4 4-4"/><path d="M21 13v2a4 4 0 01-4 4H3"/></svg>
          Inspire
        </button>
      </div>
    </div>
  </div>

  <!-- ======= NAVIGATION ======= -->
  <div class="nav-bar flex gap-2 mb-6 pb-1">
    <div class="nav-item active" onclick="showPanel('dashboard')" data-panel="dashboard">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="7" height="7" rx="1"/><rect x="14" y="3" width="7" height="7" rx="1"/><rect x="3" y="14" width="7" height="7" rx="1"/><rect x="14" y="14" width="7" height="7" rx="1"/></svg>
      Dash
    </div>
    <div class="nav-item" onclick="showPanel('habits')" data-panel="habits">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 11l3 3L22 4"/><path d="M21 12v7a2 2 0 01-2 2H5a2 2 0 01-2-2V5a2 2 0 012-2h11"/></svg>
      Habits
    </div>
    <div class="nav-item" onclick="showPanel('planner')" data-panel="planner">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
      Planner
    </div>
    <div class="nav-item" onclick="showPanel('identity')" data-panel="identity">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 20h9"/><path d="M16.5 3.5a2.121 2.121 0 013 3L7 19l-4 1 1-4L16.5 3.5z"/></svg>
      Identity
    </div>
    <div class="nav-item" onclick="showPanel('fasting')" data-panel="fasting">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
      Fasting
    </div>
    <div class="nav-item" onclick="showPanel('meals')" data-panel="meals">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 8h1a4 4 0 010 8h-1"/><path d="M2 8h16v9a4 4 0 01-4 4H6a4 4 0 01-4-4V8z"/><line x1="6" y1="1" x2="6" y2="4"/><line x1="10" y1="1" x2="10" y2="4"/><line x1="14" y1="1" x2="14" y2="4"/></svg>
      Meals
    </div>
    <div class="nav-item" onclick="showPanel('protocol')" data-panel="protocol">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 3H5a2 2 0 00-2 2v4m6-6h10a2 2 0 012 2v4M9 3v18m0 0h10a2 2 0 002-2V9M9 21H5a2 2 0 01-2-2V9m0 0h18"/></svg>
      Protocol
    </div>
  </div>

  <!-- ============================================ -->
  <!-- PANEL: DASHBOARD                             -->
  <!-- ============================================ -->
  <div class="panel active" id="panel-dashboard">

    <!-- Stats Row -->
    <div class="grid grid-cols-4 gap-3 mb-4">
      <div class="stat-box">
        <div class="text-2xl font-black glow-cyan" id="statHabits">0/0</div>
        <div class="text-[10px] text-slate-500 uppercase tracking-widest mt-1">Habits</div>
      </div>
      <div class="stat-box">
        <div class="text-2xl font-black" style="color:var(--neon4)" id="statStreak">🔥 0</div>
        <div class="text-[10px] text-slate-500 uppercase tracking-widest mt-1">Streak</div>
      </div>
      <div class="stat-box">
        <div class="text-2xl font-black" style="color:var(--neon3)" id="statWeight">— kg</div>
        <div class="text-[10px] text-slate-500 uppercase tracking-widest mt-1">Weight</div>
      </div>
      <div class="stat-box">
        <div class="text-xl font-black" style="color:#00b4d8" id="statCalories">0 kcal</div>
        <div class="text-[10px] text-slate-500 uppercase tracking-widest mt-1">Calories</div>
      </div>
    </div>

    <!-- Fasting Status Card -->
    <div class="card no-hover mb-4" id="dashFastCard">
      <div class="section-tag">Ramadan / Fasting</div>
      <div class="flex items-center justify-between mt-2">
        <div>
          <div class="text-xs text-slate-400 mb-1" id="dashFastLabel">Next: Iftar</div>
          <div class="text-2xl font-black" style="color:var(--neon4)" id="dashFastTime">--:--:--</div>
          <div class="text-[10px] text-slate-500 mt-1">Go to Fasting tab to set times →</div>
        </div>
        <div class="text-5xl ring-pulse" id="dashFastEmoji">🌙</div>
      </div>
      <div class="progress-wrap mt-3">
        <div class="progress-fill" style="background:linear-gradient(90deg,#b45309,var(--neon4)); width:0%" id="dashFastBar"></div>
      </div>
    </div>

    <!-- Today's Habits Quick View -->
    <div class="card no-hover mb-4">
      <div class="section-tag">Today's Habits</div>
      <div id="dashHabitsPreview" class="flex flex-col gap-2 mt-3">
        <p class="text-xs text-slate-500 text-center py-4">No habits yet. Go to Habits tab →</p>
      </div>
    </div>

    <!-- Habit Completion Progress -->
    <div class="card no-hover">
      <div class="flex justify-between items-center mb-3">
        <div class="section-tag" style="margin-bottom:0">Daily Completion</div>
        <span class="text-xs font-bold glow-cyan" id="completionPct">0%</span>
      </div>
      <div class="progress-wrap" style="height:10px">
        <div class="progress-fill progress-cyan" id="completionBar" style="width:0%"></div>
      </div>
      <div class="mt-3 text-xs text-slate-400 italic" id="motiveLine">"Every action is a vote for the person you wish to become."</div>
    </div>
  </div>

  <!-- ============================================ -->
  <!-- PANEL: HABITS                                -->
  <!-- ============================================ -->
  <div class="panel" id="panel-habits">
    <div class="flex items-center justify-between mb-4">
      <div>
        <div class="section-tag" style="margin-bottom:2px">Atomic Habits</div>
        <h2 class="text-lg font-black text-white">Build The System</h2>
      </div>
      <button class="btn btn-neon" onclick="openModal('habitModal')">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3"><path d="M12 5v14M5 12h14"/></svg>
        New Habit
      </button>
    </div>

    <!-- Habit list -->
    <div id="habitList" class="flex flex-col gap-3 mb-6"></div>

    <!-- Weekly Heatmap -->
    <div class="card no-hover">
      <div class="section-tag">7-Day Completion Map</div>
      <div id="weekHeatmap" class="grid grid-cols-7 gap-2 mt-3"></div>
      <div class="flex justify-between mt-2">
        <span class="text-[10px] text-slate-600">7 days ago</span>
        <span class="text-[10px] text-slate-600">Today</span>
      </div>
    </div>
  </div>

  <!-- ============================================ -->
  <!-- PANEL: PLANNER                               -->
  <!-- ============================================ -->
  <div class="panel" id="panel-planner">
    <div class="flex items-center justify-between mb-4">
      <div>
        <div class="section-tag" style="margin-bottom:2px">Time Boxing</div>
        <h2 class="text-lg font-black text-white">Daily Planner</h2>
      </div>
      <button class="btn btn-ghost text-xs" onclick="savePlanner()">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path d="M19 21H5a2 2 0 01-2-2V5a2 2 0 012-2h11l5 5v11a2 2 0 01-2 2z"/><polyline points="17 21 17 13 7 13 7 21"/><polyline points="7 3 7 8 15 8"/></svg>
        Save
      </button>
    </div>
    <div class="card no-hover" id="plannerGrid">
      <!-- JS fills this -->
    </div>
  </div>

  <!-- ============================================ -->
  <!-- PANEL: IDENTITY                              -->
  <!-- ============================================ -->
  <div class="panel" id="panel-identity">
    <div class="section-tag mb-2">The Identity</div>
    <h2 class="text-lg font-black text-white mb-4">Who Are You Becoming?</h2>

    <!-- Main Goal -->
    <div class="card identity-card no-hover mb-4">
      <div class="text-[10px] text-slate-400 uppercase tracking-widest mb-1 font-semibold">Current Identity Statement</div>
      <textarea id="identityStatement" rows="2" placeholder='e.g. "I am a disciplined athlete who trains every day and eats clean."'
        class="bg-transparent border-none outline-none text-white text-sm font-semibold resize-none w-full mt-1 p-0 focus:ring-0"
        oninput="saveIdentity()" style="border:none!important; box-shadow:none!important; background:transparent!important; padding:0!important"></textarea>
      <div class="w-full h-px bg-gradient-to-r from-transparent via-purple-500 to-transparent opacity-30 mt-2"></div>
    </div>

    <!-- Weight Goal -->
    <div class="card no-hover mb-4">
      <div class="section-tag">Weight Goal</div>
      <div class="grid grid-cols-2 gap-3 mt-3 mb-4">
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-1">Start Weight (kg)</label>
          <input type="number" id="startWeight" step="0.1" placeholder="95" oninput="saveIdentity()" />
        </div>
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-1">Goal Weight (kg)</label>
          <input type="number" id="goalWeight" step="0.1" placeholder="85" oninput="saveIdentity()" />
        </div>
      </div>
      <div class="flex justify-between text-xs mb-2">
        <span class="text-slate-400">Progress</span>
        <span class="font-bold glow-cyan" id="weightProgressPct">—</span>
      </div>
      <div class="progress-wrap" style="height:10px">
        <div class="progress-fill progress-red" id="weightProgressBar" style="width:0%"></div>
      </div>
      <div class="flex justify-between mt-2 text-[10px] text-slate-500">
        <span id="weightStartLabel">Start: —</span>
        <span id="weightCurrentLabel">Current: —</span>
        <span id="weightGoalLabel">Goal: —</span>
      </div>
    </div>

    <!-- Weight Log -->
    <div class="card no-hover mb-4">
      <div class="flex justify-between items-center mb-3">
        <div class="section-tag" style="margin-bottom:0">Weight History</div>
        <button class="btn btn-neon text-xs py-1 px-3" onclick="openModal('weightModal')">+ Log</button>
      </div>
      <div id="weightHistory" class="flex flex-col gap-2"></div>
    </div>

    <!-- Milestone Box -->
    <div class="card no-hover">
      <div class="section-tag">Milestones</div>
      <div id="milestones" class="flex flex-col gap-2 mt-3"></div>
    </div>
  </div>

  <!-- ============================================ -->
  <!-- PANEL: FASTING                               -->
  <!-- ============================================ -->
  <div class="panel" id="panel-fasting">
    <div class="section-tag mb-2">Ramadan / Fasting Tracker</div>
    <h2 class="text-lg font-black text-white mb-4">Fast With Intention</h2>

    <!-- Time Input -->
    <div class="card no-hover mb-4">
      <div class="grid grid-cols-2 gap-4">
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-2">Suhoor (End of pre-dawn)</label>
          <input type="time" id="suhoorTime" value="05:00" oninput="saveFastingTimes()" />
        </div>
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-2">Iftar (Break fast)</label>
          <input type="time" id="iftarTime" value="19:30" oninput="saveFastingTimes()" />
        </div>
      </div>
      <div class="flex gap-3 mt-4">
        <button class="btn btn-ghost flex-1 text-xs" onclick="toggleFasting()">
          <span id="fastToggleIcon">▶</span>
          <span id="fastToggleText">Start Fasting</span>
        </button>
      </div>
    </div>

    <!-- Main Countdown -->
    <div class="card no-hover fasting-active mb-4">
      <div class="text-center">
        <div class="text-[10px] text-yellow-400 uppercase tracking-widest font-bold mb-1" id="fastStateLabel">Next Event</div>
        <div class="text-5xl mb-2" id="fastEmoji">🌙</div>
        <div class="text-xl font-bold text-white mb-3" id="fastEventName">Iftar</div>
        <div class="flex justify-center gap-3 mb-4">
          <div class="countdown-digit"><span id="cd-h">00</span></div>
          <div class="flex items-center text-2xl font-black" style="color:var(--neon4)">:</div>
          <div class="countdown-digit"><span id="cd-m">00</span></div>
          <div class="flex items-center text-2xl font-black" style="color:var(--neon4)">:</div>
          <div class="countdown-digit"><span id="cd-s">00</span></div>
        </div>
        <div class="flex justify-center gap-4 text-[10px] text-slate-500">
          <span>HR</span><span>MIN</span><span>SEC</span>
        </div>

        <!-- Fasting Arc Progress -->
        <div class="mt-4">
          <div class="flex justify-between text-xs mb-1">
            <span class="text-slate-400" id="fastingFromLabel">Suhoor: 05:00</span>
            <span class="text-yellow-400 font-bold" id="fastingPctLabel">0%</span>
            <span class="text-slate-400" id="fastingToLabel">Iftar: 19:30</span>
          </div>
          <div class="progress-wrap" style="height:10px">
            <div class="progress-fill" style="background:linear-gradient(90deg,#b45309,#ffd60a);width:0%" id="fastingProgressBar"></div>
          </div>
        </div>
      </div>
    </div>

    <!-- Fasting Tips -->
    <div class="card no-hover">
      <div class="section-tag">Ramadan Protocol</div>
      <div class="flex flex-col gap-2 mt-3">
        <div class="protocol-item">
          <div class="protocol-check" id="ftp-0" onclick="toggleFastProtocol(0)"></div>
          <span class="text-sm">💧 Drink 1L of water at Suhoor</span>
        </div>
        <div class="protocol-item">
          <div class="protocol-check" id="ftp-1" onclick="toggleFastProtocol(1)"></div>
          <span class="text-sm">🥚 High-protein Suhoor meal</span>
        </div>
        <div class="protocol-item">
          <div class="protocol-check" id="ftp-2" onclick="toggleFastProtocol(2)"></div>
          <span class="text-sm">🧘 Dhuhr + Asr prayers done</span>
        </div>
        <div class="protocol-item">
          <div class="protocol-check" id="ftp-3" onclick="toggleFastProtocol(3)"></div>
          <span class="text-sm">🏋️ Workout scheduled post-Iftar</span>
        </div>
        <div class="protocol-item">
          <div class="protocol-check" id="ftp-4" onclick="toggleFastProtocol(4)"></div>
          <span class="text-sm">🍝 Break fast with dates + water first</span>
        </div>
      </div>
    </div>
  </div>

  <!-- ============================================ -->
  <!-- PANEL: MEALS                                 -->
  <!-- ============================================ -->
  <div class="panel" id="panel-meals">
    <div class="flex items-center justify-between mb-4">
      <div>
        <div class="section-tag" style="margin-bottom:2px">Gym Meal Tracker</div>
        <h2 class="text-lg font-black text-white">Fuel The Machine</h2>
      </div>
      <button class="btn btn-neon" onclick="openModal('mealModal')">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3"><path d="M12 5v14M5 12h14"/></svg>
        Log Meal
      </button>
    </div>

    <!-- Calorie Ring + Macro Summary -->
    <div class="card no-hover mb-4">
      <div class="section-tag">Daily Macro Overview</div>
      <div class="flex items-center justify-center gap-6 mt-4 mb-2 flex-wrap">
        <!-- Calorie Ring -->
        <div class="macro-ring-wrap">
          <svg width="130" height="130" viewBox="0 0 130 130">
            <circle cx="65" cy="65" r="54" fill="none" stroke="rgba(255,255,255,0.05)" stroke-width="10"/>
            <circle id="calRing" cx="65" cy="65" r="54" fill="none" stroke="url(#calRingGrad)" stroke-width="10"
              stroke-linecap="round" stroke-dasharray="339.3" stroke-dashoffset="339.3"/>
            <defs>
              <linearGradient id="calRingGrad" x1="0%" y1="0%" x2="100%" y2="0%">
                <stop offset="0%" stop-color="#00b4d8"/>
                <stop offset="100%" stop-color="#00f5d4"/>
              </linearGradient>
            </defs>
          </svg>
          <div class="macro-ring-center">
            <span class="text-2xl font-black glow-cyan" id="calRingVal">0</span>
            <span class="text-[9px] text-slate-500 uppercase tracking-widest">kcal</span>
            <span class="text-[10px] text-slate-400 mt-0.5" id="calRingTarget">/ 2500</span>
          </div>
        </div>
        <!-- Macro Bars -->
        <div class="flex flex-col gap-3 flex-1 min-w-[140px]">
          <div>
            <div class="flex justify-between text-xs mb-1">
              <span class="text-slate-400">🥩 Protein</span>
              <span class="font-bold" style="color:var(--neon3)" id="mealProteinStat">0g / 160g</span>
            </div>
            <div class="progress-wrap" style="height:8px">
              <div class="progress-fill progress-red" id="mealProteinBar" style="width:0%"></div>
            </div>
          </div>
          <div>
            <div class="flex justify-between text-xs mb-1">
              <span class="text-slate-400">🍚 Carbs</span>
              <span class="font-bold" style="color:var(--neon4)" id="mealCarbsStat">0g / 300g</span>
            </div>
            <div class="progress-wrap" style="height:8px">
              <div class="progress-fill" style="background:linear-gradient(90deg,#b45309,var(--neon4));width:0%" id="mealCarbsBar"></div>
            </div>
          </div>
          <div>
            <div class="flex justify-between text-xs mb-1">
              <span class="text-slate-400">🥑 Fat</span>
              <span class="font-bold" style="color:var(--neon2)" id="mealFatStat">0g / 80g</span>
            </div>
            <div class="progress-wrap" style="height:8px">
              <div class="progress-fill progress-purple" id="mealFatBar" style="width:0%"></div>
            </div>
          </div>
        </div>
      </div>
      <!-- Remaining calories -->
      <div class="mt-3 text-center">
        <span class="text-xs text-slate-400">Remaining: </span>
        <span class="text-sm font-bold glow-cyan" id="calRemaining">2500 kcal</span>
      </div>
    </div>

    <!-- Macro Targets Settings -->
    <div class="card no-hover mb-4">
      <div class="section-tag">Daily Targets</div>
      <div class="grid grid-cols-4 gap-2 mt-3">
        <div>
          <label class="text-[9px] text-slate-400 uppercase tracking-widest block mb-1">Calories</label>
          <input type="number" id="mealCalGoal" placeholder="2500" min="0" step="50" oninput="saveMealTargets()" style="padding:8px 10px;font-size:12px" />
        </div>
        <div>
          <label class="text-[9px] text-slate-400 uppercase tracking-widest block mb-1">Protein (g)</label>
          <input type="number" id="mealProteinGoal" placeholder="160" min="0" step="5" oninput="saveMealTargets()" style="padding:8px 10px;font-size:12px" />
        </div>
        <div>
          <label class="text-[9px] text-slate-400 uppercase tracking-widest block mb-1">Carbs (g)</label>
          <input type="number" id="mealCarbsGoal" placeholder="300" min="0" step="5" oninput="saveMealTargets()" style="padding:8px 10px;font-size:12px" />
        </div>
        <div>
          <label class="text-[9px] text-slate-400 uppercase tracking-widest block mb-1">Fat (g)</label>
          <input type="number" id="mealFatGoal" placeholder="80" min="0" step="5" oninput="saveMealTargets()" style="padding:8px 10px;font-size:12px" />
        </div>
      </div>
    </div>

    <!-- Quick Add Presets -->
    <div class="card no-hover mb-4">
      <div class="section-tag">Quick Add — Gym Meals</div>
      <div class="flex flex-wrap gap-2 mt-3" id="presetChips">
        <!-- JS fills -->
      </div>
    </div>

    <!-- Today's Meals Log -->
    <div class="card no-hover mb-4">
      <div class="flex justify-between items-center mb-3">
        <div class="section-tag" style="margin-bottom:0">Today's Meals</div>
        <button class="btn btn-danger text-[10px] py-1 px-2" onclick="clearTodayMeals()">Clear All</button>
      </div>
      <div id="mealLog" class="flex flex-col gap-3">
        <p class="text-xs text-slate-500 text-center py-4">No meals logged yet. Start fueling up! 💪</p>
      </div>
    </div>

    <!-- Meal History (past 7 days summary) -->
    <div class="card no-hover">
      <div class="section-tag">7-Day Calorie History</div>
      <div id="mealHistory7d" class="mt-3">
        <!-- JS fills -->
      </div>
    </div>
  </div>

  <!-- ============================================ -->
  <!-- PANEL: PROTOCOL                              -->
  <!-- ============================================ -->
  <div class="panel" id="panel-protocol">
    <div class="section-tag mb-2">The Protocol</div>
    <h2 class="text-lg font-black text-white mb-4">Non-Negotiables</h2>

    <!-- Macros / Intake -->
    <div class="card no-hover mb-4">
      <div class="section-tag">Nutrition Targets</div>
      <div class="grid grid-cols-2 gap-3 mt-3">
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-1">Water Goal (L)</label>
          <input type="number" id="waterGoal" step="0.1" placeholder="3.0" oninput="saveProtocol()" />
        </div>
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-1">Protein Goal (g)</label>
          <input type="number" id="proteinGoal" step="1" placeholder="160" oninput="saveProtocol()" />
        </div>
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-1">Water Today (L)</label>
          <input type="number" id="waterToday" step="0.1" placeholder="0.0" oninput="saveProtocol()" />
        </div>
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-1">Protein Today (g)</label>
          <input type="number" id="proteinToday" step="1" placeholder="0" oninput="saveProtocol()" />
        </div>
      </div>
      <div class="flex flex-col gap-3 mt-4">
        <div>
          <div class="flex justify-between text-xs mb-1">
            <span class="text-slate-400">💧 Water</span>
            <span class="font-bold" style="color:#00b4d8" id="waterPct">0%</span>
          </div>
          <div class="progress-wrap">
            <div class="progress-fill" style="background:linear-gradient(90deg,#0077b6,#00b4d8);width:0%" id="waterBar"></div>
          </div>
        </div>
        <div>
          <div class="flex justify-between text-xs mb-1">
            <span class="text-slate-400">🥩 Protein</span>
            <span class="font-bold" style="color:#ff4d6d" id="proteinPct">0%</span>
          </div>
          <div class="progress-wrap">
            <div class="progress-fill progress-red" style="width:0%" id="proteinBar"></div>
          </div>
        </div>
      </div>
    </div>

    <!-- Daily Non-Negotiables Checklist -->
    <div class="card no-hover mb-4">
      <div class="section-tag">Daily Non-Negotiables</div>
      <div id="nonNegList" class="flex flex-col gap-2 mt-3">
        <!-- JS fills this -->
      </div>
      <div class="flex gap-2 mt-4">
        <input type="text" id="nonNegInput" placeholder="Add a non-negotiable..." style="flex:1" />
        <button class="btn btn-neon" onclick="addNonNeg()">+</button>
      </div>
    </div>

    <!-- Mindset Notes -->
    <div class="card no-hover">
      <div class="section-tag">Daily Reflection</div>
      <div class="flex flex-col gap-3 mt-3">
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-1">Win of the Day</label>
          <textarea id="winOfDay" rows="2" placeholder="What did you crush today?" oninput="saveProtocol()"></textarea>
        </div>
        <div>
          <label class="text-[10px] text-slate-400 uppercase tracking-widest block mb-1">Tomorrow's Focus</label>
          <textarea id="tomorrowFocus" rows="2" placeholder="One key priority for tomorrow..." oninput="saveProtocol()"></textarea>
        </div>
      </div>
    </div>
  </div>

</div><!-- end wrapper -->

<!-- ======= BOTTOM NAV (mobile-friendly repeat) ======= -->
<div style="position:fixed;bottom:0;left:0;right:0;background:rgba(6,9,18,0.95);backdrop-filter:blur(16px);border-top:1px solid var(--border);z-index:50;padding:8px 16px 12px">
  <div class="flex justify-around max-w-2xl mx-auto">
    <div class="nav-item active" onclick="showPanel('dashboard')" data-panel-bottom="dashboard">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="7" height="7" rx="1"/><rect x="14" y="3" width="7" height="7" rx="1"/><rect x="3" y="14" width="7" height="7" rx="1"/><rect x="14" y="14" width="7" height="7" rx="1"/></svg>
      Dash
    </div>
    <div class="nav-item" onclick="showPanel('habits')" data-panel-bottom="habits">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 11l3 3L22 4"/><path d="M21 12v7a2 2 0 01-2 2H5a2 2 0 01-2-2V5a2 2 0 012-2h11"/></svg>
      Habits
    </div>
    <div class="nav-item" onclick="showPanel('planner')" data-panel-bottom="planner">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
      Plan
    </div>
    <div class="nav-item" onclick="showPanel('identity')" data-panel-bottom="identity">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 20h9"/><path d="M16.5 3.5a2.121 2.121 0 013 3L7 19l-4 1 1-4L16.5 3.5z"/></svg>
      Identity
    </div>
    <div class="nav-item" onclick="showPanel('fasting')" data-panel-bottom="fasting">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
      Fast
    </div>
    <div class="nav-item" onclick="showPanel('meals')" data-panel-bottom="meals">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 8h1a4 4 0 010 8h-1"/><path d="M2 8h16v9a4 4 0 01-4 4H6a4 4 0 01-4-4V8z"/><line x1="6" y1="1" x2="6" y2="4"/><line x1="10" y1="1" x2="10" y2="4"/><line x1="14" y1="1" x2="14" y2="4"/></svg>
      Meals
    </div>
    <div class="nav-item" onclick="showPanel('protocol')" data-panel-bottom="protocol">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 3H5a2 2 0 00-2 2v4m6-6h10a2 2 0 012 2v4M9 3v18m0 0h10a2 2 0 002-2V9M9 21H5a2 2 0 01-2-2V9m0 0h18"/></svg>
      Protocol
    </div>
  </div>
</div>

<script>
// ============================================================
// DATA & STATE
// ============================================================
const QUOTES = [
  { text: "Stay hard. The only way to know you're going to do something is to do it.", author: "— David Goggins" },
  { text: "You are not your feelings. You are what you do.", author: "— David Goggins" },
  { text: "Suffer now and live the rest of your life as a champion.", author: "— Muhammad Ali" },
  { text: "Every action you take is a vote for the type of person you wish to become.", author: "— James Clear, Atomic Habits" },
  { text: "You do not rise to the level of your goals. You fall to the level of your systems.", author: "— James Clear, Atomic Habits" },
  { text: "The man who is disciplined in food, recreation, sleep, and wakefulness — for him, Yoga destroys all pain.", author: "— Bhagavad Gita" },
  { text: "Waste no more time arguing what a good man should be. Be one.", author: "— Marcus Aurelius" },
  { text: "It never gets easier, you just get stronger.", author: "— Unknown" },
  { text: "Habits are the compound interest of self-improvement.", author: "— James Clear, Atomic Habits" },
  { text: "The impediment to action advances action. What stands in the way becomes the way.", author: "— Marcus Aurelius" },
  { text: "Don't tell me what you value. Show me your schedule and I'll tell you what you value.", author: "— Anonymous" },
  { text: "The secret of getting ahead is getting started.", author: "— Mark Twain" },
  { text: "Callus your mind. Make your mind work for you, not against you.", author: "— David Goggins" },
  { text: "Small habits don't add up, they compound.", author: "— James Clear, Atomic Habits" },
  { text: "The first step toward change is awareness. The second step is acceptance.", author: "— Nathaniel Branden" },
];

let quoteIndex = Math.floor(Math.random() * QUOTES.length);
let fastingActive = false;
let fastProtocolState = JSON.parse(localStorage.getItem('fastProtocol') || '[false,false,false,false,false]');

// ============================================================
// INIT
// ============================================================
window.addEventListener('DOMContentLoaded', () => {
  loadHabits();
  loadPlanner();
  loadIdentity();
  loadFasting();
  loadProtocol();
  loadMealTargets();
  renderNonNegs();
  renderWeightHistory();
  renderMilestones();
  updateHeatmap();
  updateDashboard();
  updateProtocolBars();
  renderFastProtocol();
  renderMealLog();
  renderPresetChips();
  updateMealDashboard();
  setInterval(tick, 1000);
  tick();
  rotateQuote();
  setInterval(rotateQuote, 9000);
  checkDayReset();
});

// ============================================================
// CLOCK & DAY PROGRESS
// ============================================================
function tick() {
  const now = new Date();
  const h = String(now.getHours()).padStart(2,'0');
  const m = String(now.getMinutes()).padStart(2,'0');
  const s = String(now.getSeconds()).padStart(2,'0');
  document.getElementById('clockDisplay').textContent = `${h}:${m}:${s}`;

  const days = ['Sunday','Monday','Tuesday','Wednesday','Thursday','Friday','Saturday'];
  const months = ['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];
  document.getElementById('dateDisplay').textContent =
    `${days[now.getDay()]}, ${now.getDate()} ${months[now.getMonth()]} ${now.getFullYear()}`;

  // Day progress arc (06:00 = start, 00:00 = end = 18h window)
  const startH = 6, totalH = 18;
  const elapsed = (now.getHours() - startH) * 3600 + now.getMinutes() * 60 + now.getSeconds();
  const total = totalH * 3600;
  const pct = Math.min(100, Math.max(0, (elapsed / total) * 100));
  const circumference = 188.5;
  const offset = circumference - (pct / 100) * circumference;
  document.getElementById('dayArc').style.strokeDashoffset = offset;
  document.getElementById('arcPct').textContent = Math.round(pct) + '%';
  document.getElementById('dayProgressBar').style.width = pct + '%';
  document.getElementById('dayProgressText').textContent = Math.round(pct) + '%';

  // Fasting countdown
  updateFastingCountdown();
}

// ============================================================
// QUOTES
// ============================================================
function rotateQuote() {
  quoteIndex = (quoteIndex + 1) % QUOTES.length;
  const q = QUOTES[quoteIndex];
  const el = document.getElementById('quoteText');
  const ea = document.getElementById('quoteAuthor');
  el.style.animation = 'none';
  void el.offsetWidth;
  el.style.animation = '';
  el.textContent = `"${q.text}"`;
  ea.textContent = q.author;
}
function nextQuote() { rotateQuote(); }

// ============================================================
// NAVIGATION
// ============================================================
function showPanel(name) {
  document.querySelectorAll('.panel').forEach(p => p.classList.remove('active'));
  document.querySelectorAll('.nav-item').forEach(n => n.classList.remove('active'));
  document.getElementById('panel-' + name).classList.add('active');
  document.querySelectorAll(`[data-panel="${name}"], [data-panel-bottom="${name}"]`).forEach(n => n.classList.add('active'));
  if (name === 'habits') { renderHabits(); updateHeatmap(); }
  if (name === 'dashboard') { updateDashboard(); }
  if (name === 'identity') { renderWeightHistory(); renderMilestones(); updateWeightProgress(); }
  if (name === 'protocol') { updateProtocolBars(); renderNonNegs(); }
  if (name === 'meals') { renderMealLog(); renderPresetChips(); updateMealDashboard(); }
}

function openModal(id) { document.getElementById(id).classList.add('open'); }
function closeModal(id) { document.getElementById(id).classList.remove('open'); }

// ============================================================
// HABITS
// ============================================================
function getHabits() { return JSON.parse(localStorage.getItem('habits') || '[]'); }
function saveHabits(h) { localStorage.setItem('habits', JSON.stringify(h)); }
function getTodayKey() { return new Date().toISOString().split('T')[0]; }

function loadHabits() { renderHabits(); }

function addHabit() {
  const name = document.getElementById('habitNameInput').value.trim();
  const cat = document.getElementById('habitCatInput').value;
  if (!name) { showToast('Enter a habit name!'); return; }
  const habits = getHabits();
  habits.push({ id: Date.now(), name, cat, streak: 0, completedDays: {}, created: getTodayKey() });
  saveHabits(habits);
  document.getElementById('habitNameInput').value = '';
  closeModal('habitModal');
  renderHabits();
  updateDashboard();
  showToast('✅ Habit added!');
}

function renderHabits() {
  const habits = getHabits();
  const today = getTodayKey();
  const list = document.getElementById('habitList');
  if (!list) return;
  if (habits.length === 0) {
    list.innerHTML = `<div class="card no-hover text-center py-8">
      <div class="text-4xl mb-3">🎯</div>
      <div class="text-sm text-slate-400">No habits yet. Start building your system.</div>
    </div>`;
    return;
  }
  list.innerHTML = habits.map((h, i) => {
    const done = h.completedDays && h.completedDays[today];
    const streak = calcStreak(h);
    return `<div class="habit-item" id="habit-${h.id}">
      <div class="habit-check ${done ? 'checked' : ''}" onclick="toggleHabit(${h.id})">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="#000" stroke-width="4"><polyline points="20 6 9 17 4 12"/></svg>
      </div>
      <div class="flex-1 min-w-0">
        <div class="text-sm font-semibold ${done ? 'line-through text-slate-500' : 'text-white'}">${h.name}</div>
        <div class="text-[10px] text-slate-500 mt-0.5">${h.cat}</div>
      </div>
      <div class="streak-badge">🔥 ${streak}</div>
      <button class="btn btn-danger py-1 px-2 text-[10px]" onclick="deleteHabit(${h.id})">✕</button>
    </div>`;
  }).join('');
}

function toggleHabit(id) {
  const habits = getHabits();
  const today = getTodayKey();
  const h = habits.find(x => x.id === id);
  if (!h) return;
  if (!h.completedDays) h.completedDays = {};
  if (h.completedDays[today]) {
    delete h.completedDays[today];
  } else {
    h.completedDays[today] = true;
    showToast('🔥 Habit logged!');
  }
  saveHabits(habits);
  renderHabits();
  updateDashboard();
  updateHeatmap();
}

function calcStreak(h) {
  if (!h.completedDays) return 0;
  let streak = 0;
  const today = new Date();
  for (let i = 0; i < 365; i++) {
    const d = new Date(today);
    d.setDate(d.getDate() - i);
    const key = d.toISOString().split('T')[0];
    if (h.completedDays[key]) streak++;
    else if (i > 0) break;
  }
  return streak;
}

function deleteHabit(id) {
  let habits = getHabits();
  habits = habits.filter(h => h.id !== id);
  saveHabits(habits);
  renderHabits();
  updateDashboard();
  showToast('Habit removed.');
}

function updateHeatmap() {
  const habits = getHabits();
  const el = document.getElementById('weekHeatmap');
  if (!el) return;
  const days = [];
  for (let i = 6; i >= 0; i--) {
    const d = new Date();
    d.setDate(d.getDate() - i);
    days.push(d.toISOString().split('T')[0]);
  }
  el.innerHTML = days.map(day => {
    const total = habits.length;
    const done = total === 0 ? 0 : habits.filter(h => h.completedDays && h.completedDays[day]).length;
    const pct = total === 0 ? 0 : done / total;
    const opacity = pct === 0 ? 0.08 : 0.2 + pct * 0.8;
    const isToday = day === getTodayKey();
    return `<div title="${day}: ${done}/${total}" style="
      background:rgba(0,245,212,${opacity});
      border:1px solid ${isToday ? 'rgba(0,245,212,0.6)' : 'rgba(0,245,212,0.1)'};
      border-radius:6px;height:36px;
      display:flex;align-items:center;justify-content:center;
      font-size:10px;font-weight:700;color:rgba(0,245,212,${Math.max(0.4,opacity)});
      cursor:default;transition:all 0.2s;
    ">${done}</div>`;
  }).join('');
}

// ============================================================
// DASHBOARD UPDATE
// ============================================================
function updateDashboard() {
  const habits = getHabits();
  const today = getTodayKey();
  const total = habits.length;
  const done = habits.filter(h => h.completedDays && h.completedDays[today]).length;
  const pct = total === 0 ? 0 : Math.round((done / total) * 100);
  const bestStreak = total === 0 ? 0 : Math.max(...habits.map(h => calcStreak(h)));

  document.getElementById('statHabits').textContent = `${done}/${total}`;
  document.getElementById('statStreak').textContent = `🔥 ${bestStreak}`;
  document.getElementById('completionPct').textContent = pct + '%';
  document.getElementById('completionBar').style.width = pct + '%';

  // Identity weight
  const identity = JSON.parse(localStorage.getItem('identity') || '{}');
  const weightLog = JSON.parse(localStorage.getItem('weightLog') || '[]');
  const currentW = weightLog.length > 0 ? weightLog[weightLog.length - 1].w : null;
  document.getElementById('statWeight').textContent = currentW ? currentW + ' kg' : '— kg';

  // Calories stat
  const todayMeals = getMeals().filter(m => m.date === today);
  const totalCal = todayMeals.reduce((s, m) => s + m.cal, 0);
  document.getElementById('statCalories').textContent = totalCal + ' kcal';

  // Motivational line
  const lines = [
    '"Every action is a vote for the person you wish to become."',
    '"Small habits, compounded over time, create extraordinary results."',
    '"The man who moves a mountain begins by carrying away small stones."',
    '"Discipline equals freedom." — Jocko Willink',
    '"Stay hard." — David Goggins',
  ];
  document.getElementById('motiveLine').textContent = lines[Math.floor(Math.random() * lines.length)];

  // Dashboard habits preview
  const preview = document.getElementById('dashHabitsPreview');
  if (preview) {
    if (total === 0) {
      preview.innerHTML = `<p class="text-xs text-slate-500 text-center py-4">No habits yet. Go to Habits tab →</p>`;
    } else {
      preview.innerHTML = habits.slice(0, 4).map(h => {
        const isDone = h.completedDays && h.completedDays[today];
        return `<div class="flex items-center gap-2 py-1">
          <div style="width:8px;height:8px;border-radius:50%;background:${isDone ? 'var(--neon)' : 'var(--bg4)'}; border:1px solid ${isDone ? 'var(--neon)' : 'var(--muted)'}; box-shadow:${isDone ? '0 0 8px rgba(0,245,212,0.5)' : 'none'}"></div>
          <span class="text-xs ${isDone ? 'text-slate-400 line-through' : 'text-white'}">${h.name}</span>
          <span class="text-[10px] text-slate-600 ml-auto">${h.cat}</span>
        </div>`;
      }).join('') + (total > 4 ? `<div class="text-[10px] text-slate-500 text-right">+${total - 4} more</div>` : '');
    }
  }
}

// ============================================================
// PLANNER
// ============================================================
const DEFAULT_PLANNER = {
  "06:00": "", "06:30": "🌅 Fajr Prayer + Wudu",
  "07:00": "☀️ Morning Routine / Stretch", "07:30": "",
  "08:00": "🏫 School / University", "08:30": "",
  "09:00": "📚 School", "09:30": "",
  "10:00": "📚 School", "10:30": "",
  "11:00": "📚 School", "11:30": "",
  "12:00": "🕐 Dhuhr Prayer + Break", "12:30": "",
  "13:00": "📚 School", "13:30": "",
  "14:00": "📚 School / Study", "14:30": "",
  "15:00": "🕒 Asr Prayer", "15:30": "📖 Self-Study / Reading",
  "16:00": "", "16:30": "",
  "17:00": "🏋️ Workout", "17:30": "🏋️ Workout (continued)",
  "18:00": "", "18:30": "",
  "19:00": "🌙 Prepare for Iftar", "19:30": "🍽️ Iftar",
  "20:00": "🕖 Maghrib Prayer", "20:30": "",
  "21:00": "🕘 Isha Prayer", "21:30": "📖 Read / Study",
  "22:00": "", "22:30": "",
  "23:00": "😴 Wind Down / Sleep Prep", "23:30": "",
  "00:00": "🌙 Sleep"
};

function loadPlanner() {
  const saved = JSON.parse(localStorage.getItem('planner') || 'null') || DEFAULT_PLANNER;
  renderPlanner(saved);
}

function renderPlanner(data) {
  const grid = document.getElementById('plannerGrid');
  if (!grid) return;
  grid.innerHTML = Object.entries(data).map(([time, val]) => {
    const h = parseInt(time.split(':')[0]);
    let cls = '';
    if (val.includes('School') || val.includes('Study') || val.includes('📚')) cls = 'prefilled';
    else if (val.includes('Workout') || val.includes('🏋')) cls = 'workout';
    else if (val.includes('Iftar') || val.includes('Suhoor') || val.includes('🌙') || val.includes('Prayer')) cls = 'fast';
    const isNowHour = new Date().getHours() === h;
    return `<div class="time-block ${isNowHour ? 'border-glow-active' : ''}" style="${isNowHour ? 'background:rgba(0,245,212,0.03);border-radius:8px;padding:4px 0 8px;' : ''}">
      <div class="time-label">${time}</div>
      <textarea class="time-input ${cls}" rows="1" data-time="${time}" onchange="savePlanner()" onfocus="this.rows=2" onblur="this.rows=1">${val}</textarea>
    </div>`;
  }).join('');
}

function savePlanner() {
  const inputs = document.querySelectorAll('.time-input[data-time]');
  const data = {};
  inputs.forEach(inp => { data[inp.dataset.time] = inp.value; });
  localStorage.setItem('planner', JSON.stringify(data));
  showToast('📅 Planner saved!');
}

// ============================================================
// IDENTITY / WEIGHT
// ============================================================
function loadIdentity() {
  const d = JSON.parse(localStorage.getItem('identity') || '{}');
  if (d.statement) document.getElementById('identityStatement').value = d.statement;
  if (d.startWeight) document.getElementById('startWeight').value = d.startWeight;
  if (d.goalWeight) document.getElementById('goalWeight').value = d.goalWeight;
  updateWeightProgress();
}

function saveIdentity() {
  const d = {
    statement: document.getElementById('identityStatement').value,
    startWeight: document.getElementById('startWeight').value,
    goalWeight: document.getElementById('goalWeight').value,
  };
  localStorage.setItem('identity', JSON.stringify(d));
  updateWeightProgress();
}

function updateWeightProgress() {
  const d = JSON.parse(localStorage.getItem('identity') || '{}');
  const weightLog = JSON.parse(localStorage.getItem('weightLog') || '[]');
  const start = parseFloat(d.startWeight);
  const goal = parseFloat(d.goalWeight);
  const current = weightLog.length > 0 ? parseFloat(weightLog[weightLog.length - 1].w) : start;

  document.getElementById('weightStartLabel').textContent = `Start: ${start || '—'}kg`;
  document.getElementById('weightCurrentLabel').textContent = `Now: ${current || '—'}kg`;
  document.getElementById('weightGoalLabel').textContent = `Goal: ${goal || '—'}kg`;

  if (start && goal && current) {
    const totalToLose = start - goal;
    const lost = start - current;
    const pct = totalToLose > 0 ? Math.min(100, Math.max(0, (lost / totalToLose) * 100)) : 0;
    document.getElementById('weightProgressBar').style.width = pct + '%';
    document.getElementById('weightProgressPct').textContent = Math.round(pct) + '%';
  }
}

function logWeight() {
  const val = document.getElementById('weightInput').value;
  if (!val || isNaN(val)) { showToast('Enter valid weight!'); return; }
  const log = JSON.parse(localStorage.getItem('weightLog') || '[]');
  log.push({ date: getTodayKey(), w: parseFloat(val) });
  localStorage.setItem('weightLog', JSON.stringify(log));
  document.getElementById('weightInput').value = '';
  closeModal('weightModal');
  renderWeightHistory();
  updateWeightProgress();
  updateDashboard();
  showToast('⚖️ Weight logged!');
}

function renderWeightHistory() {
  const log = JSON.parse(localStorage.getItem('weightLog') || '[]');
  const el = document.getElementById('weightHistory');
  if (!el) return;
  if (log.length === 0) {
    el.innerHTML = `<p class="text-xs text-slate-500 text-center py-3">No weight logs yet.</p>`;
    return;
  }
  el.innerHTML = log.slice(-7).reverse().map((entry, i) => `
    <div class="flex items-center gap-3 py-2 border-b border-white/5 last:border-0">
      <div class="weight-dot"></div>
      <span class="text-xs text-slate-400">${entry.date}</span>
      <span class="ml-auto font-bold text-white text-sm">${entry.w} kg</span>
      ${i === 0 ? '<span class="text-[10px] bg-cyan-500/10 text-cyan-400 border border-cyan-500/20 rounded-full px-2 py-0.5">Latest</span>' : ''}
    </div>
  `).join('');
}

function renderMilestones() {
  const log = JSON.parse(localStorage.getItem('weightLog') || '[]');
  const d = JSON.parse(localStorage.getItem('identity') || '{}');
  const el = document.getElementById('milestones');
  if (!el) return;
  const start = parseFloat(d.startWeight);
  const goal = parseFloat(d.goalWeight);
  if (!start || !goal || log.length === 0) {
    el.innerHTML = `<p class="text-xs text-slate-500 text-center py-2">Set weight goals and log weights to track milestones.</p>`;
    return;
  }
  const current = parseFloat(log[log.length - 1].w);
  const intervals = [25, 50, 75, 100];
  const total = start - goal;
  el.innerHTML = intervals.map(pct => {
    const target = start - (total * pct / 100);
    const reached = current <= target;
    return `<div class="flex items-center gap-3 py-2">
      <div style="width:24px;height:24px;border-radius:50%;background:${reached ? 'var(--neon)' : 'var(--bg4)'};border:1px solid ${reached ? 'var(--neon)' : 'var(--muted)'};display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:900;color:${reached ? '#000' : 'var(--muted)'};">${reached ? '✓' : pct + '%'}</div>
      <div>
        <div class="text-xs font-semibold text-white">${pct}% Progress</div>
        <div class="text-[10px] text-slate-500">Target: ${target.toFixed(1)} kg</div>
      </div>
      ${reached ? '<span class="ml-auto text-[10px] glow-cyan font-bold">ACHIEVED 🏆</span>' : ''}
    </div>`;
  }).join('');
}

// ============================================================
// FASTING
// ============================================================
function loadFasting() {
  const d = JSON.parse(localStorage.getItem('fasting') || '{}');
  if (d.suhoor) document.getElementById('suhoorTime').value = d.suhoor;
  if (d.iftar) document.getElementById('iftarTime').value = d.iftar;
  fastingActive = d.active || false;
  updateFastToggleUI();
}

function saveFastingTimes() {
  const d = JSON.parse(localStorage.getItem('fasting') || '{}');
  d.suhoor = document.getElementById('suhoorTime').value;
  d.iftar = document.getElementById('iftarTime').value;
  localStorage.setItem('fasting', JSON.stringify(d));
}

function toggleFasting() {
  fastingActive = !fastingActive;
  const d = JSON.parse(localStorage.getItem('fasting') || '{}');
  d.active = fastingActive;
  localStorage.setItem('fasting', JSON.stringify(d));
  updateFastToggleUI();
  showToast(fastingActive ? '🌙 Fasting started. Stay strong!' : '🍽️ Fasting ended.');
}

function updateFastToggleUI() {
  const icon = document.getElementById('fastToggleIcon');
  const text = document.getElementById('fastToggleText');
  if (icon) icon.textContent = fastingActive ? '⏸' : '▶';
  if (text) text.textContent = fastingActive ? 'Fasting Active (End)' : 'Start Fasting';
}

function timeToMinutes(t) {
  const [h, m] = t.split(':').map(Number);
  return h * 60 + m;
}

function updateFastingCountdown() {
  const suhoorVal = document.getElementById('suhoorTime')?.value || '05:00';
  const iftarVal = document.getElementById('iftarTime')?.value || '19:30';
  const now = new Date();
  const nowMin = now.getHours() * 60 + now.getMinutes();
  const suhoorMin = timeToMinutes(suhoorVal);
  const iftarMin = timeToMinutes(iftarVal);

  let targetMin, label, emoji, eventName;
  const isFasting = nowMin >= suhoorMin && nowMin < iftarMin;

  if (nowMin < suhoorMin) {
    targetMin = suhoorMin; label = 'Until Suhoor'; emoji = '🌃'; eventName = 'Suhoor';
  } else if (isFasting) {
    targetMin = iftarMin; label = 'Until Iftar'; emoji = '🌙'; eventName = 'Iftar';
  } else {
    // After iftar, next suhoor is tomorrow
    targetMin = suhoorMin + 1440; label = 'Until Suhoor (Tomorrow)'; emoji = '🌃'; eventName = 'Suhoor';
  }

  let diffMin = targetMin - nowMin;
  if (diffMin < 0) diffMin += 1440;
  const diffSec = diffMin * 60 - now.getSeconds();
  const dh = Math.floor(diffSec / 3600);
  const dm = Math.floor((diffSec % 3600) / 60);
  const ds = diffSec % 60;

  const fmtH = String(Math.max(0, dh)).padStart(2, '0');
  const fmtM = String(Math.max(0, dm)).padStart(2, '0');
  const fmtS = String(Math.max(0, ds)).padStart(2, '0');

  ['cd-h','cd-m','cd-s'].forEach((id, i) => {
    const el = document.getElementById(id);
    if (el) el.textContent = [fmtH, fmtM, fmtS][i];
  });

  const setEl = (id, val) => { const e = document.getElementById(id); if (e) e.textContent = val; };
  setEl('fastStateLabel', label);
  setEl('fastEventName', eventName);
  setEl('fastEmoji', emoji);
  setEl('dashFastLabel', `Next: ${eventName}`);
  setEl('dashFastTime', `${fmtH}:${fmtM}:${fmtS}`);
  setEl('dashFastEmoji', emoji);

  // Fasting progress bar (time elapsed through fast)
  const fastingDuration = iftarMin - suhoorMin;
  const elapsed = nowMin - suhoorMin;
  const fpct = isFasting && fastingDuration > 0 ? Math.min(100, Math.max(0, (elapsed / fastingDuration) * 100)) : 0;
  const fpctEl = document.getElementById('fastingProgressBar');
  if (fpctEl) fpctEl.style.width = fpct + '%';
  const fpctLbl = document.getElementById('fastingPctLabel');
  if (fpctLbl) fpctLbl.textContent = Math.round(fpct) + '%';
  const dashFastBar = document.getElementById('dashFastBar');
  if (dashFastBar) dashFastBar.style.width = fpct + '%';

  setEl('fastingFromLabel', `Suhoor: ${suhoorVal}`);
  setEl('fastingToLabel', `Iftar: ${iftarVal}`);
}

function renderFastProtocol() {
  for (let i = 0; i < 5; i++) {
    const el = document.getElementById(`ftp-${i}`);
    if (el) {
      el.classList.toggle('done', fastProtocolState[i]);
    }
  }
}

function toggleFastProtocol(i) {
  fastProtocolState[i] = !fastProtocolState[i];
  localStorage.setItem('fastProtocol', JSON.stringify(fastProtocolState));
  renderFastProtocol();
  showToast(fastProtocolState[i] ? '✅ Done!' : 'Unchecked.');
}

// ============================================================
// PROTOCOL
// ============================================================
function loadProtocol() {
  const d = JSON.parse(localStorage.getItem('protocol') || '{}');
  if (d.waterGoal) document.getElementById('waterGoal').value = d.waterGoal;
  if (d.proteinGoal) document.getElementById('proteinGoal').value = d.proteinGoal;
  if (d.waterToday) document.getElementById('waterToday').value = d.waterToday;
  if (d.proteinToday) document.getElementById('proteinToday').value = d.proteinToday;
  if (d.winOfDay) document.getElementById('winOfDay').value = d.winOfDay;
  if (d.tomorrowFocus) document.getElementById('tomorrowFocus').value = d.tomorrowFocus;
}

function saveProtocol() {
  const d = {
    waterGoal: document.getElementById('waterGoal').value,
    proteinGoal: document.getElementById('proteinGoal').value,
    waterToday: document.getElementById('waterToday').value,
    proteinToday: document.getElementById('proteinToday').value,
    winOfDay: document.getElementById('winOfDay').value,
    tomorrowFocus: document.getElementById('tomorrowFocus').value,
  };
  localStorage.setItem('protocol', JSON.stringify(d));
  updateProtocolBars();
}

function updateProtocolBars() {
  const d = JSON.parse(localStorage.getItem('protocol') || '{}');
  const wg = parseFloat(d.waterGoal) || 3;
  const wt = parseFloat(d.waterToday) || 0;
  const pg = parseFloat(d.proteinGoal) || 160;
  const pt = parseFloat(d.proteinToday) || 0;
  const wp = Math.min(100, Math.round((wt / wg) * 100));
  const pp = Math.min(100, Math.round((pt / pg) * 100));
  const wb = document.getElementById('waterBar');
  const pb = document.getElementById('proteinBar');
  const wpl = document.getElementById('waterPct');
  const ppl = document.getElementById('proteinPct');
  if (wb) wb.style.width = wp + '%';
  if (pb) pb.style.width = pp + '%';
  if (wpl) wpl.textContent = wp + '%';
  if (ppl) ppl.textContent = pp + '%';
}

// Non-Negotiables
const DEFAULT_NON_NEGS = [
  { id: 1, text: '💧 3L Water intake', done: false },
  { id: 2, text: '🥩 Hit protein target', done: false },
  { id: 3, text: '🧘 Morning intention / Niyyah', done: false },
  { id: 4, text: '📵 No social media before 10am', done: false },
  { id: 5, text: '📖 Read 10 pages', done: false },
];

function getNonNegs() {
  return JSON.parse(localStorage.getItem('nonNegs') || JSON.stringify(DEFAULT_NON_NEGS));
}
function saveNonNegs(list) { localStorage.setItem('nonNegs', JSON.stringify(list)); }

function renderNonNegs() {
  const list = getNonNegs();
  const el = document.getElementById('nonNegList');
  if (!el) return;
  el.innerHTML = list.map(item => `
    <div class="protocol-item">
      <div class="protocol-check ${item.done ? 'done' : ''}" onclick="toggleNonNeg(${item.id})"></div>
      <span class="text-sm flex-1 ${item.done ? 'line-through text-slate-500' : 'text-white'}">${item.text}</span>
      <button onclick="deleteNonNeg(${item.id})" class="text-slate-600 hover:text-red-400 text-xs ml-2 transition-colors">✕</button>
    </div>
  `).join('');
}

function toggleNonNeg(id) {
  const list = getNonNegs();
  const item = list.find(x => x.id === id);
  if (item) item.done = !item.done;
  saveNonNegs(list);
  renderNonNegs();
  if (item && item.done) showToast('✅ Done!');
}

function deleteNonNeg(id) {
  const list = getNonNegs().filter(x => x.id !== id);
  saveNonNegs(list);
  renderNonNegs();
}

function addNonNeg() {
  const input = document.getElementById('nonNegInput');
  const text = input.value.trim();
  if (!text) return;
  const list = getNonNegs();
  list.push({ id: Date.now(), text, done: false });
  saveNonNegs(list);
  input.value = '';
  renderNonNegs();
  showToast('📌 Non-negotiable added!');
}

// ============================================================
// MEAL TRACKER
// ============================================================
const MEAL_PRESETS = [
  { name: '🍗 Grilled Chicken Breast', cal: 280, protein: 53, carbs: 0, fat: 6, type: 'lunch' },
  { name: '🍚 White Rice (200g)', cal: 260, protein: 5, carbs: 58, fat: 0.5, type: 'lunch' },
  { name: '🥚 4 Boiled Eggs', cal: 312, protein: 25, carbs: 1.5, fat: 21, type: 'breakfast' },
  { name: '🥤 Whey Protein Shake', cal: 120, protein: 25, carbs: 3, fat: 1.5, type: 'post-workout' },
  { name: '🥜 Peanut Butter Toast', cal: 320, protein: 12, carbs: 30, fat: 18, type: 'breakfast' },
  { name: '🥗 Tuna Salad', cal: 350, protein: 35, carbs: 12, fat: 18, type: 'lunch' },
  { name: '🍌 Banana + Oats', cal: 310, protein: 8, carbs: 58, fat: 5, type: 'suhoor' },
  { name: '🍳 Omelette (3 eggs)', cal: 270, protein: 21, carbs: 2, fat: 20, type: 'breakfast' },
  { name: '🥩 Steak (200g)', cal: 500, protein: 50, carbs: 0, fat: 32, type: 'dinner' },
  { name: '🐟 Salmon Fillet', cal: 367, protein: 34, carbs: 0, fat: 22, type: 'dinner' },
  { name: '🫘 Lentil Soup', cal: 230, protein: 18, carbs: 40, fat: 1, type: 'iftar' },
  { name: '🍗 Chicken + Rice Bowl', cal: 550, protein: 45, carbs: 60, fat: 10, type: 'lunch' },
  { name: '🥛 Greek Yogurt + Honey', cal: 200, protein: 15, carbs: 22, fat: 6, type: 'snack' },
  { name: '🥤 Mass Gainer Shake', cal: 650, protein: 40, carbs: 85, fat: 12, type: 'post-workout' },
  { name: '🥙 Chicken Wrap', cal: 420, protein: 32, carbs: 38, fat: 14, type: 'lunch' },
  { name: '🍎 Apple + Almonds', cal: 190, protein: 5, carbs: 22, fat: 10, type: 'snack' },
  { name: '🥣 Overnight Oats', cal: 380, protein: 15, carbs: 52, fat: 12, type: 'suhoor' },
  { name: '🧆 Falafel Plate', cal: 480, protein: 18, carbs: 50, fat: 22, type: 'iftar' },
  { name: '🍠 Sweet Potato (200g)', cal: 172, protein: 3, carbs: 40, fat: 0, type: 'dinner' },
  { name: '🫐 Protein Smoothie Bowl', cal: 340, protein: 30, carbs: 40, fat: 6, type: 'breakfast' },
];

function getMealTargets() {
  return JSON.parse(localStorage.getItem('mealTargets') || '{"cal":2500,"protein":160,"carbs":300,"fat":80}');
}

function saveMealTargets() {
  const t = {
    cal: parseInt(document.getElementById('mealCalGoal').value) || 2500,
    protein: parseInt(document.getElementById('mealProteinGoal').value) || 160,
    carbs: parseInt(document.getElementById('mealCarbsGoal').value) || 300,
    fat: parseInt(document.getElementById('mealFatGoal').value) || 80,
  };
  localStorage.setItem('mealTargets', JSON.stringify(t));
  updateMealDashboard();
}

function loadMealTargets() {
  const t = getMealTargets();
  document.getElementById('mealCalGoal').value = t.cal;
  document.getElementById('mealProteinGoal').value = t.protein;
  document.getElementById('mealCarbsGoal').value = t.carbs;
  document.getElementById('mealFatGoal').value = t.fat;
}

function getMeals() {
  return JSON.parse(localStorage.getItem('mealLog') || '[]');
}

function saveMeals(meals) {
  localStorage.setItem('mealLog', JSON.stringify(meals));
}

function getTodayMeals() {
  const today = getTodayKey();
  return getMeals().filter(m => m.date === today);
}

function addMeal() {
  const name = document.getElementById('mealNameInput').value.trim();
  const type = document.getElementById('mealTypeInput').value;
  const cal = parseInt(document.getElementById('mealCalInput').value) || 0;
  const protein = parseInt(document.getElementById('mealProteinInput').value) || 0;
  const carbs = parseInt(document.getElementById('mealCarbsInput').value) || 0;
  const fat = parseInt(document.getElementById('mealFatInput').value) || 0;
  if (!name) { showToast('Enter a meal name!'); return; }
  if (cal === 0 && protein === 0 && carbs === 0 && fat === 0) { showToast('Add some macros!'); return; }

  const meals = getMeals();
  meals.push({
    id: Date.now(),
    date: getTodayKey(),
    time: new Date().toTimeString().slice(0, 5),
    name, type, cal, protein, carbs, fat
  });
  saveMeals(meals);

  document.getElementById('mealNameInput').value = '';
  document.getElementById('mealCalInput').value = '';
  document.getElementById('mealProteinInput').value = '';
  document.getElementById('mealCarbsInput').value = '';
  document.getElementById('mealFatInput').value = '';
  closeModal('mealModal');
  renderMealLog();
  updateMealDashboard();
  updateDashboard();
  showToast('🍽️ Meal logged! Keep fueling up!');
}

function addPresetMeal(index) {
  const p = MEAL_PRESETS[index];
  const meals = getMeals();
  meals.push({
    id: Date.now(),
    date: getTodayKey(),
    time: new Date().toTimeString().slice(0, 5),
    name: p.name, type: p.type,
    cal: p.cal, protein: p.protein, carbs: p.carbs, fat: p.fat
  });
  saveMeals(meals);
  renderMealLog();
  updateMealDashboard();
  updateDashboard();
  showToast(`✅ ${p.name} added!`);
}

function deleteMeal(id) {
  const meals = getMeals().filter(m => m.id !== id);
  saveMeals(meals);
  renderMealLog();
  updateMealDashboard();
  updateDashboard();
  showToast('Meal removed.');
}

function clearTodayMeals() {
  const today = getTodayKey();
  const meals = getMeals().filter(m => m.date !== today);
  saveMeals(meals);
  renderMealLog();
  updateMealDashboard();
  updateDashboard();
  showToast('🗑️ Today\'s meals cleared.');
}

function renderMealLog() {
  const todayMeals = getTodayMeals();
  const el = document.getElementById('mealLog');
  if (!el) return;
  if (todayMeals.length === 0) {
    el.innerHTML = '<p class="text-xs text-slate-500 text-center py-4">No meals logged yet. Start fueling up! 💪</p>';
    return;
  }

  // Group by meal type
  const typeOrder = ['suhoor','breakfast','snack','pre-workout','lunch','post-workout','dinner','iftar'];
  const typeLabels = {
    'breakfast': '☀️ Breakfast', 'lunch': '🌤️ Lunch', 'dinner': '🌙 Dinner',
    'snack': '🍎 Snack', 'pre-workout': '⚡ Pre-Workout', 'post-workout': '💪 Post-Workout',
    'suhoor': '🌅 Suhoor', 'iftar': '🌙 Iftar'
  };

  const sorted = [...todayMeals].sort((a, b) => {
    const ai = typeOrder.indexOf(a.type);
    const bi = typeOrder.indexOf(b.type);
    return ai - bi;
  });

  el.innerHTML = sorted.map(m => `
    <div class="meal-card count-up-anim">
      <div class="flex items-start justify-between gap-3">
        <div class="flex-1 min-w-0">
          <div class="flex items-center gap-2 mb-1.5">
            <span class="meal-type-badge ${m.type}">${typeLabels[m.type] || m.type}</span>
            <span class="text-[10px] text-slate-500">${m.time}</span>
          </div>
          <div class="text-sm font-semibold text-white mb-2">${m.name}</div>
          <div class="flex flex-wrap gap-1.5">
            <span class="macro-pill cal">🔥 ${m.cal} kcal</span>
            <span class="macro-pill protein">P: ${m.protein}g</span>
            <span class="macro-pill carbs">C: ${m.carbs}g</span>
            <span class="macro-pill fat">F: ${m.fat}g</span>
          </div>
        </div>
        <button class="btn btn-danger py-1 px-2 text-[10px] flex-shrink-0" onclick="deleteMeal(${m.id})">✕</button>
      </div>
    </div>
  `).join('');
}

function renderPresetChips() {
  const el = document.getElementById('presetChips');
  if (!el) return;
  el.innerHTML = MEAL_PRESETS.map((p, i) => `
    <div class="preset-chip" onclick="addPresetMeal(${i})" title="${p.cal}kcal | P:${p.protein}g C:${p.carbs}g F:${p.fat}g">
      ${p.name.split(' ').slice(0, 2).join(' ')}
      <span class="text-[9px] text-slate-500">${p.cal}</span>
    </div>
  `).join('');
}

function updateMealDashboard() {
  const todayMeals = getTodayMeals();
  const targets = getMealTargets();

  const totalCal = todayMeals.reduce((s, m) => s + m.cal, 0);
  const totalProtein = todayMeals.reduce((s, m) => s + m.protein, 0);
  const totalCarbs = todayMeals.reduce((s, m) => s + m.carbs, 0);
  const totalFat = todayMeals.reduce((s, m) => s + m.fat, 0);

  const calPct = Math.min(100, Math.round((totalCal / targets.cal) * 100));
  const protPct = Math.min(100, Math.round((totalProtein / targets.protein) * 100));
  const carbPct = Math.min(100, Math.round((totalCarbs / targets.carbs) * 100));
  const fatPct = Math.min(100, Math.round((totalFat / targets.fat) * 100));

  // Calorie ring
  const ring = document.getElementById('calRing');
  if (ring) {
    const circumference = 339.3;
    const offset = circumference - (calPct / 100) * circumference;
    ring.style.strokeDashoffset = offset;
    ring.style.transition = 'stroke-dashoffset 0.8s ease';
  }
  const setT = (id, v) => { const e = document.getElementById(id); if (e) e.textContent = v; };
  setT('calRingVal', totalCal);
  setT('calRingTarget', '/ ' + targets.cal);
  setT('calRemaining', Math.max(0, targets.cal - totalCal) + ' kcal');

  // Macro bars
  setT('mealProteinStat', totalProtein + 'g / ' + targets.protein + 'g');
  setT('mealCarbsStat', totalCarbs + 'g / ' + targets.carbs + 'g');
  setT('mealFatStat', totalFat + 'g / ' + targets.fat + 'g');

  const setBar = (id, pct) => { const e = document.getElementById(id); if (e) e.style.width = pct + '%'; };
  setBar('mealProteinBar', protPct);
  setBar('mealCarbsBar', carbPct);
  setBar('mealFatBar', fatPct);

  // 7-day calorie history
  render7DayMealHistory();

  // Update dashboard stats card with today's calories
  const dashCalEl = document.getElementById('statCalories');
  if (dashCalEl) dashCalEl.textContent = totalCal + ' kcal';
}

function render7DayMealHistory() {
  const el = document.getElementById('mealHistory7d');
  if (!el) return;
  const meals = getMeals();
  const targets = getMealTargets();
  const days = [];
  for (let i = 6; i >= 0; i--) {
    const d = new Date();
    d.setDate(d.getDate() - i);
    days.push(d.toISOString().split('T')[0]);
  }
  const dayNames = ['Sun','Mon','Tue','Wed','Thu','Fri','Sat'];

  const maxCal = targets.cal * 1.3; // scale bar to 130% of goal
  el.innerHTML = days.map(day => {
    const dayMeals = meals.filter(m => m.date === day);
    const totalCal = dayMeals.reduce((s, m) => s + m.cal, 0);
    const totalProt = dayMeals.reduce((s, m) => s + m.protein, 0);
    const barPct = Math.min(100, (totalCal / maxCal) * 100);
    const isToday = day === getTodayKey();
    const dt = new Date(day);
    const dayLabel = dayNames[dt.getDay()];
    const overTarget = totalCal > targets.cal;

    return `<div class="flex items-center gap-3 py-2 ${isToday ? '' : 'opacity-70'}" style="border-bottom:1px solid rgba(255,255,255,0.04)">
      <span class="text-[10px] text-slate-500 font-semibold min-w-[28px]">${dayLabel}</span>
      <div class="flex-1">
        <div class="progress-wrap" style="height:14px;border-radius:4px;position:relative">
          <div class="progress-fill" style="width:${barPct}%;border-radius:4px;background:${overTarget ? 'linear-gradient(90deg,#c0004a,#ff4d6d)' : 'linear-gradient(90deg,#00b4d8,#00f5d4)'};display:flex;align-items:center;justify-content:flex-end;padding-right:6px">
            <span style="font-size:9px;font-weight:700;color:${overTarget ? '#fff' : '#000'}">${totalCal > 0 ? totalCal : ''}</span>
          </div>
          ${isToday ? '<div style="position:absolute;right:4px;top:50%;transform:translateY(-50%);font-size:8px;color:var(--muted)">◀ Goal: ' + targets.cal + '</div>' : ''}
        </div>
      </div>
      <span class="text-[10px] text-slate-500 min-w-[32px] text-right">${totalProt}g P</span>
    </div>`;
  }).join('');
}

// ============================================================
// DAY RESET
// ============================================================
function checkDayReset() {
  const lastDay = localStorage.getItem('lastDay');
  const today = getTodayKey();
  if (lastDay && lastDay !== today) {
    // Reset daily completions but keep streaks
    const habits = getHabits();
    // Don't delete completedDays — we keep history
    // Reset fasting protocol
    localStorage.setItem('fastProtocol', '[false,false,false,false,false]');
    fastProtocolState = [false, false, false, false, false];
    // Reset protocol daily fields
    const p = JSON.parse(localStorage.getItem('protocol') || '{}');
    p.waterToday = '0';
    p.proteinToday = '0';
    p.winOfDay = '';
    p.tomorrowFocus = '';
    localStorage.setItem('protocol', JSON.stringify(p));
    // Reset nonNegs done
    const nn = getNonNegs().map(x => ({ ...x, done: false }));
    saveNonNegs(nn);
    showToast('🌅 New day reset! Stay atomic.');
  }
  localStorage.setItem('lastDay', today);
}

// ============================================================
// TOAST
// ============================================================
function showToast(msg) {
  const el = document.getElementById('toast');
  el.textContent = msg;
  el.classList.add('show');
  setTimeout(() => el.classList.remove('show'), 2500);
}

// ============================================================
// CLOSE MODALS ON OVERLAY CLICK
// ============================================================
document.querySelectorAll('.modal-overlay').forEach(overlay => {
  overlay.addEventListener('click', function(e) {
    if (e.target === this) this.classList.remove('open');
  });
});

// Keyboard: Enter on habit input
document.getElementById('habitNameInput').addEventListener('keydown', e => {
  if (e.key === 'Enter') addHabit();
});
document.getElementById('nonNegInput').addEventListener('keydown', e => {
  if (e.key === 'Enter') addNonNeg();
});
</script>
</body>
</html>
