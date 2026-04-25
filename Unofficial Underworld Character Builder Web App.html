<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>LARP Character Builder</title>
<style>
  :root {
    --color-text-primary: #1a1a1a;
    --color-text-secondary: #6b6b6b;
    --color-text-tertiary: #9b9b9b;
    --color-text-success: #2d6a2d;
    --color-text-danger: #a32d2d;
    --color-text-warning: #854f0b;
    --color-text-info: #185fa5;
    --color-background-primary: #ffffff;
    --color-background-secondary: #f5f5f3;
    --color-background-tertiary: #eeeeeb;
    --color-background-success: #eaf3de;
    --color-background-danger: #fcebeb;
    --color-background-warning: #faeeda;
    --color-background-info: #e6f1fb;
    --color-border-tertiary: rgba(0,0,0,0.1);
    --color-border-secondary: rgba(0,0,0,0.2);
    --color-border-success: #3b6d11;
    --color-border-danger: #a32d2d;
    --color-border-warning: #854f0b;
    --color-border-info: #185fa5;
    --font-sans: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    --border-radius-md: 8px;
    --border-radius-lg: 12px;
  }
  @media (prefers-color-scheme: dark) {
    :root {
      --color-text-primary: #e8e8e8;
      --color-text-secondary: #a0a0a0;
      --color-text-tertiary: #6b6b6b;
      --color-text-success: #97c459;
      --color-text-danger: #f09595;
      --color-text-warning: #ef9f27;
      --color-text-info: #85b7eb;
      --color-background-primary: #1e1e1e;
      --color-background-secondary: #2a2a2a;
      --color-background-tertiary: #333333;
      --color-background-success: #173404;
      --color-background-danger: #501313;
      --color-background-warning: #412402;
      --color-background-info: #042c53;
      --color-border-tertiary: rgba(255,255,255,0.1);
      --color-border-secondary: rgba(255,255,255,0.2);
      --color-border-success: #639922;
      --color-border-danger: #e24b4a;
      --color-border-warning: #ba7517;
      --color-border-info: #378add;
    }
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: var(--font-sans); font-size: 15px; color: var(--color-text-primary); background: var(--color-background-secondary); padding: 1.5rem; min-height: 100vh; }
  .app { max-width: 960px; margin: 0 auto; padding-bottom: 3rem; }

  /* Summary panel */
  .summary-panel { border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-lg); background: var(--color-background-primary); margin-bottom: 1.5rem; overflow: hidden; }
  .summary-top { display: grid; grid-template-columns: 1fr 1fr; }
  .summary-left { padding: 1.25rem; border-right: 0.5px solid var(--color-border-tertiary); }
  .summary-right { padding: 1.25rem; }
  .panel-label { font-size: 11px; font-weight: 500; letter-spacing: 1.5px; text-transform: uppercase; color: var(--color-text-secondary); margin-bottom: 0.875rem; }
  .fields-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 8px 16px; }
  .field-item { display: flex; flex-direction: column; gap: 3px; }
  .field-item.full { grid-column: 1 / -1; }
  .field-lbl { font-size: 11px; color: var(--color-text-secondary); }
  input[type=text], input[type=number], select { width: 100%; padding: 5px 8px; font-size: 14px; font-family: var(--font-sans); border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-md); background: var(--color-background-primary); color: var(--color-text-primary); }
  input[type=text]:focus, input[type=number]:focus, select:focus { outline: none; box-shadow: 0 0 0 2px var(--color-border-info); }

  /* Stats bar */
  .stats-bar { display: flex; flex-wrap: wrap; border-top: 0.5px solid var(--color-border-tertiary); }
  .stat-cell { flex: 1; min-width: 80px; padding: 0.75rem 1rem; border-right: 0.5px solid var(--color-border-tertiary); display: flex; flex-direction: column; gap: 3px; }
  .stat-cell:last-child { border-right: none; }
  .stat-lbl { font-size: 11px; color: var(--color-text-secondary); white-space: nowrap; }
  .stat-val { font-size: 15px; font-weight: 500; }
  .stat-val.danger { color: var(--color-text-danger); }
  .stat-sub { font-size: 10px; color: var(--color-text-danger); margin-top: 1px; }

  /* Skills acquired panel */
  .skills-right-list { display: flex; flex-direction: column; gap: 6px; max-height: 160px; overflow-y: auto; }
  .skills-group-label { font-size: 10px; font-weight: 500; letter-spacing: 1px; text-transform: uppercase; color: var(--color-text-tertiary); margin-top: 4px; }
  .skills-group-label:first-child { margin-top: 0; }
  .skill-tag { display: flex; align-items: center; justify-content: space-between; border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 3px 8px; font-size: 12px; }
  .skill-tag.granted { background: var(--color-background-success); border-color: var(--color-border-success); }
  .skill-tag.granted .stag-name { color: var(--color-text-success); }
  .skill-tag.disadvantage { background: var(--color-background-danger); border-color: var(--color-border-danger); }
  .skill-tag.disadvantage .stag-name { color: var(--color-text-danger); }
  .skill-tag.purchased { background: var(--color-background-secondary); }
  .stag-name { font-weight: 500; font-size: 12px; }
  .stag-badge { font-size: 10px; padding: 1px 5px; border-radius: 100px; background: var(--color-background-tertiary); color: var(--color-text-secondary); }
  .empty-note { font-size: 12px; color: var(--color-text-tertiary); font-style: italic; }

  /* Skills section */
  .skills-page { display: flex; flex-direction: column; gap: 0.75rem; }
  .page-title { font-size: 11px; font-weight: 500; letter-spacing: 1.5px; text-transform: uppercase; color: var(--color-text-secondary); margin-bottom: 0.75rem; }
  .skills-layout { display: flex; flex-direction: column; gap: 0.75rem; }
  .detail-panel { border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 1.25rem; background: var(--color-background-primary); }
  .skill-categories { display: flex; flex-direction: column; gap: 0.75rem; }
  .skill-category-block { border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); overflow: hidden; }
  .skill-cat-header { padding: 9px 14px; background: var(--color-background-secondary); font-size: 12px; font-weight: 500; letter-spacing: 0.5px; color: var(--color-text-secondary); cursor: pointer; display: flex; justify-content: space-between; align-items: center; user-select: none; }
  .skill-cat-header:hover { background: var(--color-background-tertiary); }
  .skill-list { display: flex; flex-direction: column; }

  /* Skill rows */
  .skill-row { display: flex; align-items: center; justify-content: space-between; padding: 8px 14px; border-top: 0.5px solid var(--color-border-tertiary); cursor: pointer; transition: background 0.1s; }
  .skill-row:hover { background: var(--color-background-secondary); }
  .skill-row.owned { background: var(--color-background-success); }
  .skill-row.locked { opacity: 0.4; cursor: default; pointer-events: none; }
  .skill-row.locked:hover { background: transparent; }
  .skill-row-left { display: flex; flex-direction: column; gap: 2px; flex: 1; min-width: 0; }
  .skill-row-name { font-size: 13px; font-weight: 500; }
  .skill-row.owned .skill-row-name { color: var(--color-text-success); }
  .tags { display: flex; gap: 4px; flex-wrap: wrap; margin-top: 2px; }
  .tag { font-size: 10px; padding: 1px 7px; border-radius: 100px; border: 0.5px solid var(--color-border-tertiary); color: var(--color-text-secondary); background: var(--color-background-primary); white-space: nowrap; }
  .tag.frag { background: var(--color-background-warning); border-color: var(--color-border-warning); color: var(--color-text-warning); }
  .tag.race-req { background: var(--color-background-warning); border-color: var(--color-border-warning); color: var(--color-text-warning); }
  .tag.lvl-req { background: var(--color-background-danger); border-color: var(--color-border-danger); color: var(--color-text-danger); }
  .tag.prereq-req { background: var(--color-background-info); border-color: var(--color-border-info); color: var(--color-text-info); }
  .skill-row-right { display: flex; align-items: center; gap: 6px; flex-shrink: 0; margin-left: 8px; }
  .cp-badge { font-size: 12px; font-weight: 500; color: var(--color-text-secondary); white-space: nowrap; }
  .count-badge { font-size: 11px; color: var(--color-text-secondary); white-space: nowrap; min-width: 28px; text-align: center; }
  .btn-sm { font-size: 13px; font-weight: 500; width: 26px; height: 26px; border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-md); background: var(--color-background-primary); color: var(--color-text-primary); cursor: pointer; display: flex; align-items: center; justify-content: center; flex-shrink: 0; font-family: var(--font-sans); line-height: 1; }
  .btn-sm:hover { background: var(--color-background-secondary); }
  .btn-sm.minus { background: var(--color-background-danger); border-color: var(--color-border-danger); color: var(--color-text-danger); }
  .btn-sm.minus:hover { opacity: 0.8; }
  .btn-sm:disabled { opacity: 0.3; cursor: not-allowed; pointer-events: none; }

  /* Detail panel */
  .detail-panel { border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 1.25rem; background: var(--color-background-primary); position: sticky; top: 1.5rem; align-self: start; max-height: 82vh; overflow-y: auto; }
  .detail-empty { font-size: 13px; color: var(--color-text-tertiary); font-style: italic; text-align: center; padding: 2rem 0; }
  .detail-name { font-size: 16px; font-weight: 500; margin-bottom: 6px; }
  .detail-meta { display: flex; gap: 6px; margin-bottom: 0.875rem; flex-wrap: wrap; }
  .detail-desc { font-size: 13px; color: var(--color-text-secondary); line-height: 1.65; }
  .detail-stat-row { display: flex; justify-content: space-between; margin-top: 0.5rem; font-size: 13px; }
  .detail-stat-lbl { color: var(--color-text-secondary); }
  .detail-stat-val { font-weight: 500; }
  .detail-divider { border: none; border-top: 0.5px solid var(--color-border-tertiary); margin: 0.875rem 0; }
  .detail-actions { display: flex; gap: 8px; margin-top: 0.75rem; align-items: center; }
  .detail-count { font-size: 14px; font-weight: 500; min-width: 60px; text-align: center; color: var(--color-text-secondary); }
  .buy-btn { flex: 1; padding: 8px; border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-md); background: var(--color-background-primary); font-size: 13px; font-weight: 500; cursor: pointer; font-family: var(--font-sans); color: var(--color-text-primary); }
  .buy-btn:hover { background: var(--color-background-secondary); }
  .buy-btn.remove { background: var(--color-background-danger); border-color: var(--color-border-danger); color: var(--color-text-danger); }
  .buy-btn:disabled { opacity: 0.35; cursor: not-allowed; }
  .detail-lock-note { font-size: 12px; font-style: italic; margin-top: 0.625rem; padding: 6px 10px; border-radius: var(--border-radius-md); }
  .detail-lock-note.race { background: var(--color-background-warning); color: var(--color-text-warning); }
  .detail-lock-note.level { background: var(--color-background-danger); color: var(--color-text-danger); }
  .detail-lock-note.prereq { background: var(--color-background-info); color: var(--color-text-info); }
  .detail-lock-note.maxed { background: var(--color-background-tertiary); color: var(--color-text-secondary); }

  /* Confirm modal */
  .modal-backdrop { position: fixed; inset: 0; background: rgba(0,0,0,0.45); display: flex; align-items: center; justify-content: center; z-index: 1000; }
  .modal { background: var(--color-background-primary); border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-lg); padding: 1.5rem; max-width: 400px; width: 90%; }
  .modal-title { font-size: 15px; font-weight: 500; margin-bottom: 0.75rem; }
  .modal-body { font-size: 13px; color: var(--color-text-secondary); line-height: 1.6; margin-bottom: 1rem; }
  .modal-affected { font-size: 12px; color: var(--color-text-danger); margin: 0.5rem 0 1rem; padding: 8px 10px; background: var(--color-background-danger); border-radius: var(--border-radius-md); }
  .modal-btns { display: flex; gap: 8px; }
  .modal-btn { flex: 1; padding: 8px 12px; border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-md); font-size: 13px; font-weight: 500; cursor: pointer; font-family: var(--font-sans); background: var(--color-background-primary); color: var(--color-text-primary); }
  .modal-btn:hover { background: var(--color-background-secondary); }
  .modal-btn.confirm { background: var(--color-background-danger); border-color: var(--color-border-danger); color: var(--color-text-danger); }
  .modal-btn.confirm:hover { opacity: 0.85; }

  /* Magic panel */
  .magic-panel { border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-lg); background: var(--color-background-primary); margin-bottom: 0.75rem; overflow: hidden; }
  .magic-panel-header { padding: 9px 14px; background: var(--color-background-secondary); font-size: 12px; font-weight: 500; letter-spacing: 0.5px; color: var(--color-text-secondary); cursor: pointer; display: flex; justify-content: space-between; align-items: center; user-select: none; }
  .magic-panel-header:hover { background: var(--color-background-tertiary); }
  .magic-header-sub { font-weight: 400; opacity: 0.7; margin-left: 6px; }
  .magic-chev { font-size: 10px; }
  .magic-panel-body { padding: 1rem 1.25rem 1.25rem; }
  .magic-section-label { font-size: 11px; font-weight: 500; letter-spacing: 1px; text-transform: uppercase; color: var(--color-text-tertiary); margin-bottom: 8px; }
  .magic-spheres-row { display: flex; gap: 10px; flex-wrap: wrap; }
  .magic-sphere-card { flex: 1; min-width: 140px; border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-md); padding: 10px 12px; background: var(--color-background-primary); }
  .magic-sphere-card.owned { border-color: var(--color-border-info); background: var(--color-background-info); }
  .magic-sphere-card.locked { opacity: 0.4; }
  .magic-sphere-title { font-size: 12px; font-weight: 500; margin-bottom: 6px; }
  .magic-sphere-card.owned .magic-sphere-title { color: var(--color-text-info); }
  .magic-sphere-actions { display: flex; gap: 6px; align-items: center; }
  .magic-sphere-select { flex: 1; font-size: 12px; padding: 3px 6px; border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-md); background: var(--color-background-primary); color: var(--color-text-primary); font-family: var(--font-sans); }
  .magic-sphere-btn { font-size: 12px; padding: 3px 10px; border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-md); background: var(--color-background-primary); color: var(--color-text-primary); cursor: pointer; font-family: var(--font-sans); white-space: nowrap; }
  .magic-sphere-btn:hover { background: var(--color-background-secondary); }
  .magic-sphere-btn.remove { background: var(--color-background-danger); border-color: var(--color-border-danger); color: var(--color-text-danger); }
  .magic-sphere-btn:disabled { opacity: 0.35; cursor: not-allowed; }
  .magic-levels-row { display: flex; gap: 8px; }
  .magic-level-card { flex: 1; border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 10px 8px; background: var(--color-background-primary); display: flex; flex-direction: column; align-items: center; gap: 6px; min-width: 0; }
  .magic-level-card.forced { border-color: var(--color-border-warning); background: var(--color-background-warning); }
  .magic-level-card.locked { opacity: 0.35; }
  .magic-level-card.complete { border-color: var(--color-border-success); background: var(--color-background-success); }
  .magic-level-title { font-size: 11px; font-weight: 500; color: var(--color-text-secondary); white-space: nowrap; }
  .magic-level-card.forced .magic-level-title { color: var(--color-text-warning); }
  .magic-level-card.complete .magic-level-title { color: var(--color-text-success); }
  .magic-level-cost { font-size: 10px; color: var(--color-text-tertiary); }
  .magic-slots-dots { display: flex; gap: 3px; flex-wrap: wrap; justify-content: center; }
  .magic-dot { width: 10px; height: 10px; border-radius: 50%; border: 1px solid var(--color-border-secondary); background: var(--color-background-secondary); }
  .magic-dot.filled { background: var(--color-text-info); border-color: var(--color-border-info); }
  .magic-dot.filled-warning { background: var(--color-text-warning); border-color: var(--color-border-warning); }
  .magic-dot.filled-success { background: var(--color-text-success); border-color: var(--color-border-success); }
  .magic-level-btns { display: flex; gap: 4px; align-items: center; }
  .magic-level-count { font-size: 11px; color: var(--color-text-secondary); min-width: 24px; text-align: center; }

  @media (max-width: 640px) {
    .summary-top { grid-template-columns: 1fr; }
    .summary-left { border-right: none; border-bottom: 0.5px solid var(--color-border-tertiary); }
    .skills-layout { grid-template-columns: 1fr; }
    .detail-panel { position: static; }
    .magic-levels-row { flex-wrap: wrap; }
    .magic-level-card { min-width: 60px; }
  }
@media print {
  body > * { display: none !important; }
  #print-area { display: block !important; }
}
#print-area { display: none; }
</style>
</head>
<body>
<div class="app">

<!-- Bug report button -->
<div style="position:fixed;top:12px;right:12px;z-index:1000">
  <button onclick="openBugReport()" style="padding:5px 12px;border:0.5px solid #5a3a1a;border-radius:var(--border-radius-md);background:#2a1800;color:#c08040;font-family:var(--font-sans);font-size:11px;font-weight:500;cursor:pointer;opacity:0.75;transition:opacity 0.2s" onmouseenter="this.style.opacity='1'" onmouseleave="this.style.opacity='0.75'">🐛 Report Bug</button>
</div>

<!-- Summary panel -->
<div class="summary-panel">
  <div class="summary-top">
    <div class="summary-left">
      <div class="panel-label">Character</div>
      <div class="fields-grid">
        <div class="field-item full">
          <label class="field-lbl">Name <span style="font-style:italic;opacity:0.6">(optional)</span></label>
          <input type="text" id="inp-name" placeholder="Enter a name…" oninput="s.name=this.value;render()">
        </div>
        <div class="field-item">
          <label class="field-lbl">Race</label>
          <select id="sel-race" onchange="onRaceChange(this.value)" onclick="if(s.race)showRaceDetail(s.race)">
            <option value="">— select —</option>
            <optgroup label="── Common ──" disabled></optgroup>
            <optgroup label="Bestial"><option>Savar'Aving</option></optgroup>
            <optgroup label="Construct"><option>Gargylen</option></optgroup>
            <optgroup label="Dwarven"><option>Mountain Dwarf</option></optgroup>
            <optgroup label="Elven"><option>Dark Elf</option><option>High Elf</option><option>Wild Elf</option></optgroup>
            <optgroup label="Fae"><option>Wood Fae</option></optgroup>
            <optgroup label="Goblinoid"><option>Orc</option></optgroup>
            <optgroup label="Humanoid"><option>Ajaunti</option><option>Einher</option><option>Hobling</option><option>Human</option></optgroup>
            <optgroup label="── Uncommon (75 frags) ──" disabled></optgroup>
            <optgroup label="Uncommon"><option>Am'Rath</option><option>Faun</option><option>Minotaur</option><option>Kobold</option><option>Ogre</option><option>Squamata</option></optgroup>
            <optgroup label="── Rare (150 frags) ──" disabled></optgroup>
            <optgroup label="Rare"><option>Avian</option><option>Blackmane</option><option>Draconian</option><option>Fire Elf</option><option>Goblin</option><option>Risen</option><option>Wolven</option><option>Yokai</option></optgroup>
            <optgroup label="── Obscure (250 frags) ──" disabled></optgroup>
            <optgroup label="Obscure"><option>Carnal Fae</option><option>Faceless</option><option>Gnome</option><option>Ice Elf</option><option>Sidhe</option><option>Vulcan Dwarf</option></optgroup>
          </select>
        </div>
        <div class="field-item">
          <label class="field-lbl">Culture <span style="font-style:italic;opacity:0.6">(optional)</span></label>
          <select id="sel-culture" onchange="onCultureChange(this.value)">
            <option value="">— select —</option>
          </select>
        </div>
        <div class="field-item">
          <label class="field-lbl">Occupation</label>
          <select id="sel-occ" onchange="s.occupation=this.value;repriceCostdSkills();revalidateAll();render()">
            <option value="">— select —</option>
            <option>Mercenary</option><option>Ranger</option><option>Templar</option>
            <option>Nightblade</option><option>Assassin</option><option>Wytchhunter</option>
            <option>Mage</option><option>Druid</option><option>Bard</option>
          </select>
        </div>
        <div class="field-item">
          <label class="field-lbl">Vocation</label>
          <select id="sel-voc" onchange="onVocationChange(this.value)">
            <option value="">— select —</option>
          </select>
        </div>
        <div class="field-item">
          <label class="field-lbl">Blankets applied</label>
          <input type="number" id="inp-blankets" min="0" value="0" oninput="s.blankets=Math.max(0,parseInt(this.value)||0);revalidateAll();render()">
        </div>
      </div>
    </div>
    <div class="summary-right">
      <div class="panel-label">Skills acquired</div>
      <div class="skills-right-list" id="skills-list"><span class="empty-note">No skills yet</span></div>
      <div style="padding-top:10px">
        <button onclick="openCharacterSummary()" style="width:100%;padding:7px 16px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-primary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:12px;font-weight:500;cursor:pointer">📄 Character Summary</button>
      </div>
      <div style="padding-top:6px">
        <button onclick="openSpellBuilder()" style="width:100%;padding:7px 16px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-primary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:12px;font-weight:500;cursor:pointer">✦ Spell List Builder</button>
      </div>
      <div style="padding-top:6px">
        <button onclick="resetCharacter()" style="width:100%;padding:7px 16px;border:0.5px solid var(--color-border-danger, #5a2020);border-radius:var(--border-radius-md);background:transparent;color:var(--color-text-danger, #c05050);font-family:var(--font-sans);font-size:12px;font-weight:500;cursor:pointer">↺ Reset Character</button>
      </div>
    </div>
  </div>
  <div class="stats-bar">
    <div class="stat-cell"><span class="stat-lbl">Level</span><span class="stat-val" id="st-level">1</span></div>
    <div class="stat-cell"><span class="stat-lbl">Body</span><span class="stat-val" id="st-body">—</span></div>
    <div class="stat-cell"><span class="stat-lbl">Strength</span><span class="stat-val" id="st-str">0</span></div>
    <div class="stat-cell"><span class="stat-lbl">Blankets</span><span class="stat-val" id="st-blankets">0</span></div>
    <div class="stat-cell"><span class="stat-lbl">CP total</span><span class="stat-val" id="st-cptotal">150</span></div>
    <div class="stat-cell"><span class="stat-lbl">CP spent</span><span class="stat-val" id="st-cpspent">0</span></div>
    <div class="stat-cell" style="flex:2;min-width:160px">
      <span class="stat-lbl">CP remaining</span>
      <span class="stat-val" id="st-cprem">150</span>
      <span class="stat-sub" id="st-cpwarn"></span>
    </div>
    <div class="stat-cell"><span class="stat-lbl">Frags</span><span class="stat-val" id="st-frags">0</span></div>
  </div>
</div>

<!-- Skills section -->
<div class="skills-page">
  <div class="page-title">Skills</div>
  <div class="detail-panel" id="detail-panel" style="margin-bottom:0.75rem"><div class="detail-empty">Hover a skill to see details</div></div>
  <div class="skills-layout">
    <div class="skill-categories" id="skill-cats"></div>
  </div>
</div>

<!-- Magic panel — always visible, outside skill categories -->
<div class="magic-panel" id="magic-panel" style="margin-top:0.75rem">
  <div class="magic-panel-header" onclick="toggleMagic()">
    <span>Magic <span class="magic-header-sub" id="magic-header-sub"></span></span>
    <span class="magic-chev" id="magic-chev">▼</span>
  </div>
  <div class="magic-panel-body" id="magic-panel-body">
    <div class="magic-section-label">Spheres of magic</div>
    <div class="magic-spheres-row" id="magic-spheres-row"></div>
    <div class="magic-section-label" style="margin-top:1rem">Spell levels 1–5</div>
    <div class="magic-levels-row" id="magic-levels-row-a"></div>
    <div class="magic-section-label" style="margin-top:0.75rem">Spell levels 6–9 &amp; ritual</div>
    <div class="magic-levels-row" id="magic-levels-row-b"></div>

    <!-- Buy to level -->
    <div style="margin-top:1rem;padding-top:1rem;border-top:0.5px solid var(--color-border-tertiary);display:flex;align-items:center;gap:10px;flex-wrap:wrap">
      <span style="font-size:12px;font-weight:500;color:var(--color-text-secondary);white-space:nowrap">Buy to level:</span>
      <select id="buy-to-level-sel" style="width:auto;min-width:120px;font-size:13px;padding:4px 8px">
        <option value="">— select level —</option>
        <option value="1">Level 1</option>
        <option value="2">Level 2</option>
        <option value="3">Level 3</option>
        <option value="4">Level 4</option>
        <option value="5">Level 5</option>
        <option value="6">Level 6</option>
        <option value="7">Level 7</option>
        <option value="8">Level 8</option>
        <option value="9">Level 9</option>
      </select>
      <button style="font-size:12px;padding:5px 14px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-primary);color:var(--color-text-primary);cursor:pointer;font-family:var(--font-sans)" onclick="buyToLevel(document.getElementById('buy-to-level-sel').value)">Purchase</button>
      <button style="font-size:12px;padding:5px 14px;border:0.5px solid var(--color-border-danger);border-radius:var(--border-radius-md);background:var(--color-background-danger);color:var(--color-text-danger);cursor:pointer;font-family:var(--font-sans)" onclick="resetSpellSlots()">Reset Spells</button>
      <span style="font-size:11px;color:var(--color-text-tertiary);font-style:italic">Automatically purchases all prerequisite slots in the correct pyramid order</span>
    </div>
  </div>
</div>

</div>

<!-- Confirm modal -->
<div class="modal-backdrop" id="modal" style="display:none">
  <div class="modal">
    <div class="modal-title" id="modal-title"></div>
    <div class="modal-body" id="modal-body"></div>
    <div class="modal-affected" id="modal-affected" style="display:none"></div>
    <div class="modal-btns">
      <button class="modal-btn" onclick="closeModal()">Cancel</button>
      <button class="modal-btn confirm" id="modal-confirm">Remove</button>
    </div>
  </div>
</div>

<!-- Spell List Builder Modal -->
<div id="spell-builder-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.85);z-index:2800;align-items:flex-start;justify-content:center;padding:1.5rem;overflow-y:auto">
  <div style="background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);width:100%;max-width:900px;margin:0 auto;overflow:hidden">

    <!-- Header -->
    <div style="display:flex;align-items:center;justify-content:space-between;padding:1rem 1.25rem;border-bottom:0.5px solid var(--color-border-secondary);background:var(--color-background-secondary)">
      <div>
        <div style="font-size:15px;font-weight:600;color:var(--color-text-primary)">✦ Spell List Builder</div>
        <div style="font-size:11px;color:var(--color-text-tertiary);margin-top:2px">Assign spells to your memorised slots</div>
      </div>
      <div style="display:flex;gap:8px;align-items:center">
        <button onclick="sbToggleIncants()" id="sb-incant-btn" style="padding:5px 12px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-tertiary);color:var(--color-text-secondary);font-family:var(--font-sans);font-size:11px;cursor:pointer">📜 Show Incantations</button>
        <button onclick="sbPrintSummary()" style="padding:5px 12px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-tertiary);color:var(--color-text-secondary);font-family:var(--font-sans);font-size:11px;cursor:pointer">🖨 Print Spell List</button>
        <button onclick="closeSpellBuilder()" style="background:none;border:none;font-size:20px;cursor:pointer;color:var(--color-text-tertiary);padding:2px 6px;line-height:1">✕</button>
      </div>
    </div>

    <!-- Spheres row (read-only from character) -->
    <div id="sb-spheres-bar" style="padding:10px 1.25rem;border-bottom:0.5px solid var(--color-border-tertiary);background:var(--color-background-secondary);display:flex;gap:12px;flex-wrap:wrap;align-items:center">
      <span style="font-size:11px;color:var(--color-text-tertiary);text-transform:uppercase;letter-spacing:0.5px">Active Spheres:</span>
      <span id="sb-spheres-display" style="font-size:12px;color:var(--color-text-secondary);font-style:italic">None selected</span>
    </div>

    <!-- Body: two-column layout -->
    <div style="padding:1rem 1.25rem;display:flex;gap:1rem;align-items:flex-start">

      <!-- Table column -->
      <div style="flex:1;min-width:0">
      <div id="sb-no-sphere" style="display:none;text-align:center;padding:2rem;color:var(--color-text-tertiary);font-size:13px;font-style:italic">
        No spheres of magic selected on your character. Purchase a Sphere of Magic in the Magic section first.
      </div>

      <!-- Summary -->
      <div id="sb-summary" style="display:none;margin-bottom:1rem">
        <div style="font-size:11px;font-weight:600;color:var(--color-text-secondary);text-transform:uppercase;letter-spacing:0.5px;margin-bottom:8px">Spell Summary</div>
        <div id="sb-summary-grid" style="display:grid;grid-template-columns:repeat(auto-fill,minmax(240px,1fr));gap:8px"></div>
      </div>

      <!-- Table -->
      <div id="sb-table-wrap" style="border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);overflow:hidden">
        <table id="sb-table" style="width:100%;border-collapse:collapse">
          <thead>
            <tr style="background:var(--color-background-secondary)">
              <th style="padding:8px 12px;font-size:11px;font-weight:600;color:var(--color-text-secondary);text-transform:uppercase;letter-spacing:0.5px;text-align:center;width:70px">Level</th>
              <th style="padding:8px 12px;font-size:11px;font-weight:600;color:var(--color-text-secondary);text-transform:uppercase;letter-spacing:0.5px;text-align:center;width:55px">Slot</th>
              <th style="padding:8px 12px;font-size:11px;font-weight:600;color:var(--color-text-secondary);text-transform:uppercase;letter-spacing:0.5px;text-align:left">Spell</th>
              <th id="sb-incant-th" style="padding:8px 12px;font-size:11px;font-weight:600;color:var(--color-text-secondary);text-transform:uppercase;letter-spacing:0.5px;text-align:left;display:none">Incantation</th>
            </tr>
          </thead>
          <tbody id="sb-body"></tbody>
        </table>
      </div>
      </div><!-- end table column -->

      <!-- Description panel -->
      <div id="sb-desc-panel" style="width:260px;flex-shrink:0;position:sticky;top:0;background:var(--color-background-secondary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);padding:12px;font-size:12px;line-height:1.6;min-height:200px">
        <div style="font-size:11px;font-weight:600;color:var(--color-text-tertiary);text-transform:uppercase;letter-spacing:0.5px;margin-bottom:8px">Spell Details</div>
        <div id="sb-desc-content" style="color:var(--color-text-tertiary);font-style:italic;font-size:12px">Select a spell from the table to see its description and incantation.</div>
      </div>

    </div><!-- end body -->
  </div>
</div>

<!-- Bug Report Popup -->
<div id="bug-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.75);z-index:4500;align-items:center;justify-content:center;padding:1rem">
  <div style="background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);padding:1.5rem;max-width:560px;width:100%;max-height:90vh;overflow-y:auto">
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:0.5rem">
      <div style="font-size:15px;font-weight:600">🐛 Report a Bug</div>
      <button onclick="closeBugReport()" style="background:none;border:none;font-size:20px;cursor:pointer;color:var(--color-text-secondary);padding:2px 6px;line-height:1">✕</button>
    </div>
    <div style="font-size:12px;color:var(--color-text-secondary);margin-bottom:1.25rem;line-height:1.5">
      Describe the issue below. Your current character state will be captured automatically and included in the report.
    </div>

    <div style="margin-bottom:1rem">
      <label style="font-size:12px;font-weight:500;display:block;margin-bottom:5px">Bug description <span style="color:var(--color-text-danger)">*</span></label>
      <textarea id="bug-description" rows="5" placeholder="What happened? What did you expect to happen? Steps to reproduce..."
        style="width:100%;padding:8px 10px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;resize:vertical;box-sizing:border-box;line-height:1.5"></textarea>
    </div>

    <div id="bug-state-preview" style="background:var(--color-background-secondary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-md);padding:10px;margin-bottom:1.25rem;font-size:11px;color:var(--color-text-secondary);line-height:1.6;max-height:160px;overflow-y:auto;white-space:pre-wrap;font-family:monospace"></div>

    <div id="bug-status" style="font-size:12px;min-height:18px;margin-bottom:0.75rem"></div>

    <div style="display:flex;gap:8px;justify-content:flex-end">
      <button onclick="closeBugReport()" style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;cursor:pointer">Cancel</button>
      <button id="bug-submit-btn" onclick="submitBugReport()"
        style="padding:8px 18px;border:0.5px solid #5a3a1a;border-radius:var(--border-radius-md);background:#2a1800;color:#c08040;font-family:var(--font-sans);font-size:13px;font-weight:500;cursor:pointer">Submit Report</button>
    </div>
  </div>
</div>

<!-- Disclaimer Overlay -->
<div id="disclaimer-overlay" style="position:fixed;inset:0;background:rgba(0,0,0,0.85);z-index:5000;display:flex;align-items:center;justify-content:center">
  <div style="background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);padding:2rem;max-width:460px;width:90%;text-align:center">
    <div style="font-size:22px;margin-bottom:0.75rem">⚠️</div>
    <div style="font-size:16px;font-weight:600;margin-bottom:1rem;color:var(--color-text-primary)">Unofficial Character Builder</div>
    <div style="font-size:13px;color:var(--color-text-secondary);line-height:1.7;margin-bottom:1.5rem">
      This is an unofficial character builder. There may be bugs. The actual rulebook supersedes anything in this builder if there are any discrepancies.
    </div>
    <button onclick="document.getElementById('disclaimer-overlay').style.display='none';window._disclaimerSeen=true"
      style="padding:10px 32px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:14px;font-weight:500;cursor:pointer">
      Proceed
    </button>
  </div>
</div>

<!-- Weapon Choice Popup -->
<div id="weapon-choice-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.7);z-index:2700;align-items:center;justify-content:center;padding:1rem">
  <div style="background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);padding:1.5rem;max-width:420px;width:100%">
    <div style="font-size:15px;font-weight:600;margin-bottom:0.4rem" id="weapon-choice-title"></div>
    <div style="font-size:12px;color:var(--color-text-secondary);margin-bottom:1rem;line-height:1.5" id="weapon-choice-subtitle"></div>
    <div style="margin-bottom:1.25rem">
      <label style="font-size:12px;font-weight:500;display:block;margin-bottom:6px">Select weapon type</label>
      <select id="weapon-choice-sel" onchange="weaponChoiceUpdateBtn()"
        style="width:100%;padding:8px 12px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px">
        <option value="">— select weapon —</option>
      </select>
    </div>
    <div style="display:flex;gap:8px;justify-content:flex-end">
      <button onclick="closeWeaponChoicePopup()" style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;cursor:pointer">Cancel</button>
      <button id="weapon-choice-confirm" onclick="confirmWeaponChoice()" disabled
        style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-tertiary);font-family:var(--font-sans);font-size:13px;font-weight:500;cursor:not-allowed">Purchase</button>
    </div>
  </div>
</div>

<!-- Weapon Choice Popup -->
<div id="weapon-choice-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.7);z-index:2700;align-items:center;justify-content:center;padding:1rem">
  <div style="background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);padding:1.5rem;max-width:420px;width:100%">
    <div id="weapon-choice-title" style="font-size:15px;font-weight:600;margin-bottom:0.4rem"></div>
    <div id="weapon-choice-subtitle" style="font-size:12px;color:var(--color-text-secondary);margin-bottom:1.25rem;line-height:1.6"></div>
    <div style="margin-bottom:1.25rem">
      <label style="font-size:12px;font-weight:500;display:block;margin-bottom:6px" id="weapon-choice-label">Select weapon</label>
      <select id="weapon-choice-sel"
        style="width:100%;padding:8px 12px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px">
        <option value="">— select —</option>
      </select>
    </div>
    <div style="display:flex;gap:8px;justify-content:flex-end">
      <button onclick="closeWeaponChoicePopup()" style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;cursor:pointer">Cancel</button>
      <button id="weapon-choice-confirm" onclick="confirmWeaponChoice()" disabled
        style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-tertiary);font-family:var(--font-sans);font-size:13px;font-weight:500;cursor:not-allowed">Purchase</button>
    </div>
  </div>
</div>

<!-- Spell Summary Overlay (print target only) -->
<div id="spell-summary-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.7);z-index:2100;overflow-y:auto;padding:2rem 1rem">
  <div id="spell-summary-content" style="max-width:800px;margin:0 auto;background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);padding:2rem;position:relative">
    <div id="spell-summary-body"></div>
  </div>
</div>

<!-- Elemental Attunement Popup -->
<div id="elemental-attunement-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.7);z-index:2700;align-items:center;justify-content:center;padding:1rem">
  <div style="background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);padding:1.5rem;max-width:400px;width:100%">
    <div style="font-size:15px;font-weight:600;margin-bottom:0.4rem">Elemental Attunement</div>
    <div style="font-size:12px;color:var(--color-text-secondary);margin-bottom:1.25rem;line-height:1.6">
      Choose an additional elemental type. Once chosen, this selection is permanent.
    </div>
    <div style="margin-bottom:1.25rem">
      <label style="font-size:12px;font-weight:500;display:block;margin-bottom:6px">Element</label>
      <select id="elemental-attunement-sel" style="width:100%;padding:8px 12px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px">
        <option value="">— choose element —</option>
      </select>
    </div>
    <div style="display:flex;gap:8px;justify-content:flex-end">
      <button onclick="closeElementalAttunementPopup()" style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;cursor:pointer">Cancel</button>
      <button id="elemental-attunement-confirm" onclick="confirmElementalAttunement()" style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-primary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;font-weight:500;cursor:pointer">Purchase</button>
    </div>
  </div>
</div>

<!-- Paragon Popup -->
<div id="paragon-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.7);z-index:2600;align-items:center;justify-content:center;padding:1rem">
  <div style="background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);padding:1.5rem;max-width:440px;width:100%">
    <div style="font-size:15px;font-weight:600;margin-bottom:0.4rem">Paragon</div>
    <div style="font-size:12px;color:var(--color-text-secondary);margin-bottom:1.25rem;line-height:1.6">
      As a Paragon you may add one Light or Dark spell (max 7th Circle) to your repertoire, memorized in place of a regular spell slot. Choose your sphere alignment and the spell level below.
    </div>

    <div style="margin-bottom:1rem">
      <label style="font-size:12px;font-weight:500;display:block;margin-bottom:6px">Sphere alignment</label>
      <div style="display:flex;gap:8px">
        <button id="paragon-light-btn" onclick="paragonSetSphere('Light')"
          style="flex:1;padding:8px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;cursor:pointer">☀ Light</button>
        <button id="paragon-dark-btn" onclick="paragonSetSphere('Dark')"
          style="flex:1;padding:8px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;cursor:pointer">🌑 Dark</button>
      </div>
    </div>

    <div style="margin-bottom:1.25rem">
      <label style="font-size:12px;font-weight:500;display:block;margin-bottom:6px">Spell level <span style="color:var(--color-text-tertiary);font-weight:400">(max 7th Circle)</span></label>
      <select id="paragon-level-sel" onchange="paragonUpdateCost()"
        style="width:100%;padding:8px 12px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px">
        <option value="">— select level —</option>
      </select>
    </div>

    <div id="paragon-cost-display" style="font-size:13px;color:var(--color-text-secondary);margin-bottom:1.25rem;min-height:20px"></div>

    <div style="display:flex;gap:8px;justify-content:flex-end">
      <button onclick="closeParagonPopup()" style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;cursor:pointer">Cancel</button>
      <button id="paragon-confirm-btn" onclick="confirmParagon()" disabled
        style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-tertiary);font-family:var(--font-sans);font-size:13px;font-weight:500;cursor:not-allowed">Purchase</button>
    </div>
  </div>
</div>

<!-- Vocation Prereq Popup -->
<div id="voc-prereq-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.7);z-index:2500;align-items:center;justify-content:center;padding:1rem">
  <div style="background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);padding:1.5rem;max-width:560px;width:100%;max-height:85vh;overflow-y:auto;position:relative">
    <div id="voc-prereq-body"></div>
    <div style="display:flex;justify-content:flex-end;margin-top:1rem;padding-top:0.75rem;border-top:0.5px solid var(--color-border-tertiary)">
      <button onclick="closeVocPrereqPopup()" style="padding:8px 24px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;font-weight:500;cursor:pointer">Done</button>
    </div>
  </div>
</div>

<div id="char-summary-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,0.7);z-index:2000;overflow-y:auto;padding:2rem 1rem">
  <div id="char-summary-content" style="max-width:800px;margin:0 auto;background:var(--color-background-primary);border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-lg);padding:2rem;position:relative">
    <button onclick="closeCharacterSummary()" style="position:absolute;top:1rem;right:1rem;background:none;border:none;font-size:20px;cursor:pointer;color:var(--color-text-secondary);line-height:1">✕</button>
    <div id="char-summary-body"></div>
    <div style="margin-top:2rem;padding-top:1rem;border-top:0.5px solid var(--color-border-tertiary);display:flex;gap:8px;justify-content:flex-end">
      <button onclick="printCharacterSummary()" style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;cursor:pointer">🖨 Print</button>
      <button onclick="closeCharacterSummary()" style="padding:8px 18px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-primary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:13px;cursor:pointer">Close</button>
    </div>
  </div>
</div>

<script>
const RACIAL_CP = 50, DEFAULT_MAX = 10;

const TABLE = [
  {level:1,threshold:150,cpPer:65,warrior:6,rogue:4,scholar:3},
  {level:2,threshold:250,cpPer:43,warrior:8,rogue:5,scholar:4},
  {level:3,threshold:350,cpPer:34,warrior:10,rogue:6,scholar:4},
  {level:4,threshold:450,cpPer:28,warrior:12,rogue:7,scholar:5},
  {level:5,threshold:550,cpPer:24,warrior:14,rogue:8,scholar:6},
  {level:6,threshold:650,cpPer:22,warrior:16,rogue:9,scholar:6},
  {level:7,threshold:750,cpPer:19,warrior:18,rogue:10,scholar:7},
  {level:8,threshold:850,cpPer:17,warrior:20,rogue:11,scholar:8},
  {level:9,threshold:950,cpPer:16,warrior:22,rogue:12,scholar:8},
  {level:10,threshold:1050,cpPer:15,warrior:24,rogue:13,scholar:9},
  {level:11,threshold:1150,cpPer:14,warrior:26,rogue:14,scholar:10},
  {level:12,threshold:1250,cpPer:13,warrior:28,rogue:15,scholar:10},
  {level:13,threshold:1350,cpPer:12,warrior:30,rogue:16,scholar:11},
  {level:14,threshold:1450,cpPer:12,warrior:32,rogue:17,scholar:12},
  {level:15,threshold:1550,cpPer:11,warrior:34,rogue:18,scholar:12},
  {level:16,threshold:1650,cpPer:11,warrior:36,rogue:19,scholar:13},
  {level:17,threshold:1750,cpPer:10,warrior:38,rogue:20,scholar:14},
  {level:18,threshold:1850,cpPer:10,warrior:40,rogue:21,scholar:14},
  {level:19,threshold:1950,cpPer:10,warrior:42,rogue:22,scholar:15},
  {level:20,threshold:2050,cpPer:10,warrior:44,rogue:23,scholar:16},
];

const OCC_CLASS = {
  Mercenary:'warrior',Ranger:'warrior',Templar:'warrior',
  Nightblade:'rogue',Assassin:'rogue',Wytchhunter:'rogue',
  Mage:'scholar',Druid:'scholar',Bard:'scholar'
};

const RACES = {
  "Savar'Aving":{cpBonus:0,fragCost:0,lore:"The Savar'Aving are a matriarchal race of cat-people who resemble humanoid hunting cats. Their society is ruled by women and views male Savar'Aving as second-class citizens. It is rare to find a dominant male Savar'Aving who is free and even more rare for him to survive for long. The Savar'Aving are a strong, proud race with deep ties to nature. They have recently suffered a catastrophic plague of necromantic origin that killed many of their people and then turned them into Undead. The few Savar'Aving that survive today struggle to put to rest their Undead sisters and attempt to rebuild their once great society. The Savar'Aving were originally known simply as the Savar, but those who survived the plague began to call themselves Savar'Aving to remind themselves that, no matter what fate throws at them, they will triumph. Life Span: 40-60 years. Language: Hindi. Racial Characteristics: Their distinguishing characteristics are make-up appropriate for the type of cat being played, and possibly the use of a prosthetic feline nose if make-up is sub-par or your subspecies is similar looking to another race. Completely black cats may not be played.",auto:[
    {name:"Natural Claws",kind:"advantage",desc:"Savar'Aving are all born with retractable claws. These claws can be retracted or extended on a 3 count. While the claws are extended, the Savar'Aving may not use any other weapons or shields. Savar'Aving receive a free proficiency in <Medium Weapons Group Proficiency: Claws> and may use one claw weapon in their good hand and nothing in their off hand. They may buy specializations with them as Medium Weapon Specialization: Claws. Should a Savar'Aving purchase the skill \"Ambidexterity\", they may use a second claw weapon in their off-hand. Savar'Aving claws act like normal medium weapons, with the exception that they cannot be destroyed or disarmed. Claws otherwise act like regular weapons for the purposes of augmentation; they may be made Master Crafted, Legendary, have alchemy applied to them, and so on. Augmentations must be done per claw. If the augmentation would normally be destroyed, destroying it simply returns the claws to their natural state. If the Savar'Aving resurrects, their claws will lose any augmentations applied to them."},
    {name:"Plagued",kind:"disadvantage",desc:"While the worst of the plague seems to have passed, its effects on the Savar'Aving people still linger. As a result, all living Savar'Aving take x4 damage from Infliction. As with all racial vulnerabilities, Infliction damage will bypass any thresholds a Savar'Aving might have. Furthermore, should a Savar'Aving enter their Death Count via Infliction, they will immediately rise as a mindless lesser Undead. Once a Savar'Aving enters this form, their Death Count is immediately over and they cannot be brought back through any means, magical or otherwise. The Savar'Aving's Body points will be restored. This Undeath does not grant the Savar'Aving any of the special abilities of Undead, but they will have a Magic threshold and immunity to effects that target the mind or living body, such as charms, poisons and saps. However, they will still suffer all the negative effects such as Control Undead and x4 damage from the Healing Sphere. While in this form, the Savar'Aving may not use their spells or abilities and may only swing base weapon damage. They are berserked and will attack anyone or anything around them for up to 10 minutes or until destroyed, at which point they will become a pile of ash."},
  ],purchased:[{name:"Cat-Like Reflexes",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Savar'Aving",prereqs:[],desc:"A Savar'Aving with this ability can use their claws to swat away a single spell. By striking a spell packet with one of their claws, the Savar'Aving can call \"Innate Cat-Like Reflexes!\" and deflect the spell. This call can be made after the packet is blocked, as long as it is called within 3 seconds. If the packet then hits the Savar'Aving or anyone else, the spell will affect that person. This ability is usable once per day per purchase. As always, claw swings must be done safely according to the rules of weapon combat."}]},
  "Gargylen":{cpBonus:0,fragCost:0,lore:"The Gargylen are a sentient race of half-construct, half-living gargoyles. Originally slaves, they have since broken free from the oppressive yoke of their mage creators. This construct race has proven that they have free will and are sentient. They have also developed a method of reproduction. Very little is known about them, and they have no recognized territory or homeland. A Gargylen's skin is stone grey and often hardened, making them less susceptible to conventional weapons. All Gargylen are horned and although some have wings, they are all flightless. They are an enigma, and questions surround their purpose or moral standings. Most seem to possess an instinctual need to protect the innocent, although this is certainly not the case with all Gargylen. Gargylen came into existence in the in-game year 2240 (1998), so Gargylen characters can be no older than that. Gargylen babies mature into adults in six months. Lifespan: Immortal. Language: Common (English). Racial Characteristics: Grey skin with large horns protruding from the forehead. Note: wings are optional, but will not allow flight.",auto:[
    {name:"Alternative Healing",kind:"advantage",desc:"A Gargylen may be healed as if their body was made of armour. Every 1 minute of Blacksmithing will heal the Gargylen 10 Body. See the Blacksmithing skill for more detail. Should the Gargylen enter their \"Bleed\" count, any use of the Blacksmith skill to heal/Refit will pause the \"Bleed\" count much like the First Aid skill does. If the Blacksmith is interrupted, or stops Refitting the Gargylen, the attempt will fail and the Gargylen will continue their \"Bleed\" count from where they last left off. Any successful Refit while in the \"Bleed\" count will heal the Gargylen to 1 Body."},
    {name:"Healing Limitation",kind:"disadvantage",desc:"Although a Gargylen possesses the same living organs as most other races, they are still part construct. As a result, the normal methods of healing and first aid will not function. A Gargylen may only heal damaged Body points with the Blacksmithing skill. Gargylen cannot have Body points restored by magic, Alchemy, or the First Aid/Physician skills, although First Aid may still be used to halt a Gargylen's Bleed Count and raise them to 0 Body. Mending used on Gargylen will take the same amount of time as standard blacksmithing would to heal them for the same amount (up to 10 Body per minute). A Life Spell will still function as normal."},
  ],purchased:[
    {name:"Stone Skin",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Gargylen",prereqs:[],desc:"A Gargylen who has purchased this skill has learned a finer degree of control over their crafted body. When the skill is used, the Gargylen's skin becomes as hard as stone, making them less susceptible to all weapons. The Gargylen must declare \"Innate Stone Skin\" and proceed to complete a 30 second count. Once this count is completed, for the duration of 1 hour a Gargylen gains temporary Body points based on the Gargylen's level. At 1st level the Body bonus is 20 Body points, at 5th level it is 30 and at 10th level it is 40. These Body points act as normal Body points with the exception that they are damaged and removed first from the Gargylen's Body point Total and cannot be healed or refit. While Stone Skin is active, the Gargylen suffers x2 damage from all Battle Magic spells and magic abilities that replicate a Battle Magic spell which damage into Body, such as Ego Rend, Necrotic Blast, etc. This x2 damage will extend past the bonus Body points allotted by Stone Skin and will carry over onto the Gargylen's permanent Body points. After all of the Stone Skin Body points are removed, the x2 vulnerability will end (although any damage from the final strike that rolls over into the Gargylen's normal Body will still include the vulnerability). Stone Skin may be ended by the Gargylen with an uninterruptible 30 second count. A Gargylen's Stone Skin will not affect, in any way, their Armour Points or any other magical or non-magical protections. This skill is usable once per day, per purchase."},
    {name:"Body Point Bonus (Gargylen)",maxPurchases:2,bodyBonus:5,strBonus:0,raceReq:"Gargylen",prereqs:[],desc:"This skill represents extra constitutional training the Gargylen has gone through, beyond what is standard for their race and grants +5 Body. This skill can only be purchased twice throughout the character's entire existence."},
  ]},
  "Mountain Dwarf":{cpBonus:0,fragCost:0,lore:"Mountain Dwarves are famed miners and smiths, though they may specialize in any number of trades. All dwarves sport a full beard and, although they are generally shorter than humans, they are on average stockier and hairier. Life Span: 250-300 years. Language: German. Racial Characteristics: All Mountain Dwarves have a full beard at least 6 inches in length, adorned with gems and/or jewellery, regardless of whether they are male or female. If a Dwarf's beard is ever cut, it will grow back within a few minutes.",auto:[
    {name:"Resist Toxin",kind:"advantage",desc:"Allows the user to \"Racial Resist Toxin\" any toxin, alchemy, or disease, be it Magical or non-Magical in nature, once per day. The user may choose which toxin to resist and when. As a racial benefit, it may be used to \"Resist\" Chemistry."},
    {name:"Restriction: Gas Globes & Magic Items",kind:"disadvantage",desc:"Dwarves have a hard time using magic items and alchemical gas globes, partially due to their clumsy and thick fingers and also because of their distaste for both. In dwarven culture, magic items with activation words are considered \"cheating\" and frowned upon. Gas globes are rarely used among dwarves due to their resistance to toxin. All dwarves must activate magical items twice in order to get a single use out of them. This does not use up two charges; instead they must state the incant twice in succession instead of once. This disadvantage does not apply to magic items which are \"always on\" or otherwise do not have activation requirements. Also, gas globes must be prepared for double the count it normally takes before they can be thrown."},
  ],purchased:[{name:"Body Point Bonus (Mountain Dwarf)",maxPurchases:3,bodyBonus:5,strBonus:0,raceReq:"Mountain Dwarf",prereqs:[],desc:"This skill represents extra constitutional training the Mountain Dwarf has gone though, beyond what is standard for their race and grants +5 Body. This skill can only be purchased three times."}]},
  "Dark Elf":{cpBonus:0,fragCost:0,lore:"Dark Elves are an underground dwelling race that is sensitive to sunlight. Because of this, Dark Elves shun the surface world during daylight hours and often live underground. The Dark Elves are mistrusted by the other races, mainly because of their dark reputation for deception and murder, as well as their natural aptitude with Alchemy. Life Span: 700-1000 years. Language: Latin. Racial Characteristics: Short pointed ears with black tips. Grey makeup covering the eyes that extends to the temples. Black veins around the outer edges of the eyes and extending from around the mouth, outwards along the cheeks and downwards towards the neck. Optional: Veins down the neck, black lipstick.",auto:[
    {name:"Natural Chemists",kind:"advantage",desc:"Dark Elves have a natural affinity for alchemy and are trained from an early age to use it offensively against rivals. All Dark Elves are capable of throwing alchemical gas globes and do not need to purchase any skills to do so."},
    {name:"Diurnal Vulnerability",kind:"disadvantage",desc:"Between the hours of 6 AM and 6 PM and while outside of darkness, Dark Elves may not be healed by any means other than by First Aid, Physician, and Life effects. If a Dark Elf enters an enclosed structure that includes a minimum of three walls plus ceiling for more than 10 minutes, they will regain their susceptibility to all forms of healing. Between the hours of 6 PM and 6 AM, Diurnal Vulnerability does not apply no matter the amount of light present."},
  ],purchased:[{name:"Spite Blood",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Dark Elf",prereqs:[],desc:"Generations of living underground and eating the local flora has caused Dark Elven blood to gain a slight toxicity. Drawing a small amount of blood and enhancing it with their talents as natural alchemists allows Dark Elves to produce a single dose of lethal toxin in the form of an alchemical gas globe. It takes 1 minute to draw enough blood to create a globe and does 1 Body point of damage to the Dark Elf. The globe can only be used by the Dark Elf who created it. When thrown, the Spite Blood globe will do 10 Acid damage. A Dark Elf who has purchased Spite Blood multiple times may stack together up to three doses to create a single gas globe of increasing damage. These doses must be stacked at the time of creation and cannot be combined once manufactured. A single dose will do 10 damage, two doses mixed together will do 25 damage and finally 3 doses combined will do 50 damage. Spite Blood gas globes are considered blood for the purposes of Wytchcraft, vampires, etc. When thrown, the call is \"Innate X Acid\" and can be resisted with standard anti-toxin defenses / resistances. Each purchase of this ability allows the creation of 1 dose per day. This alchemy will last for 5 days. This skill is usable once per day per purchase."}]},
  "High Elf":{cpBonus:0,fragCost:0,lore:"High Elves are a long-lived race that make their home primarily in cities. All High Elves are graceful, artistic and magically inclined. Although wise, they are perceived by other races as arrogant and rude. Life Span: 700-1000 years. Language: French. Racial Characteristics: Short pointed ears.",auto:[
    {name:"Magical Aptitude",kind:"advantage",desc:"This skill gives the High Elf one free Battle Magic spell-slot on character creation. This free spell-slot can be used to store any spell they can cast, up to their highest-level spell-slot. This free spell-slot in no way contributes to their pyramid or the prerequisites needed to raise it. Aside from that limitation, this free spell slot functions in every other way like a normal purchased slot. Example: A High Elf Mage with 1 purchased 4th level spell-slot may use Magical Aptitude to gain an additional 4th level or lower spell, determined at their reset."},
    {name:"Death's Doors",kind:"disadvantage",desc:"High Elves have always held a deep spiritual attunement to the forests and the land. Recent events have weakened this attunement, and in doing so have weakened the High Elves connection to the Spirit world. Should a High Elf enter their Death Count they will have 2 minutes less to receive a Life Spell than the time allotted to other races."},
  ],purchased:[{name:"Resist Psionics",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"High Elf",prereqs:[],desc:"Allows the user to \"Racial Resist Psionics\" any effect from the Psionics Sphere of Magic as well as all mind altering attacks. Mind altering attacks are considered effects which change your emotional state or control your mind in any way. Examples of mind altering effects are a Hobling's Taunt ability, a Bard's Songs of Aversion and Love, Confusion, Sleep, Enrage, Feeblemind, Forget, and Hallucinate, plus Ritual mind altering spells and monster effects which are mind altering. This may be used once per day per purchase."}]},
  "Wild Elf":{cpBonus:0,fragCost:0,lore:"Wild Elves do their best to co-exist with nature, believing that the beasts and land are here for far more than simple exploitation. They consider few things worse than taking more than you need from the world. Examples of this would be mining expeditions, industrial forestry or commercial fishing. While they are intelligent enough to understand the ways of civilization and industrial progress, they choose to live a life outside of it. Wild Elves have no formal cities or homeland and tend to live in nomadic tribes. Life Span: 700-1000 years. Language: Italian. Racial Characteristics: Short pointed ears. Tribal tattoos on the face.",auto:[
    {name:"Chosen Enemy",kind:"advantage",desc:"Upon character creation, the Wild Elf must choose one Chosen Enemy racial group against which they are additionally effective. The reasons for this vary from Wild Elf to Wild Elf. Some Wild Elves despise a race that at some point has done great harm to them, their family or the natural balance of the forest. Others have learned to hunt their Chosen Enemy to support their tribe, with no particular emotional investment. A player can choose as their Chosen Enemy racial group one of the following: Angels/Demons, Animals, Bestial, Brood, Constructs, Draconic, Dwarves, Elementals, Elves, Fae, Goblinoids, Humanoids, Plants, Spirits, Undead (excluding vampires), Vermin. The Chosen Enemy ability will grant the Wild Elf a +1 damage bonus on any melee or ranged weapon while fighting against their Chosen Enemy. This bonus will increase +1 for every 3 levels the Wild Elf gains. +1 at first level, +2 at fourth level, +3 at 7th level and so on. This damage bonus will not carry over to any other racial group, but does apply to any race within the racial group. For example, a Wild Elf with Chosen Enemy: Elves does bonus damage against Dark Elves, High Elves, Wild Elves, etc. If the Wild Elf isn't certain whether a creature fits into their Chosen Enemy category, they may state, \"Chosen Enemy <Type>?\" and the creature will respond with yes or no. Some creatures are able to hide what kind of creature they are. In those cases, Chosen Enemy does not work. Chosen Enemy cannot be changed after character creation."},
    {name:"Armour Restriction (Wild Elf)",kind:"disadvantage",desc:"Viewed as abhorrence to nature, a Wild Elf will never equip Armour made primarily of steel, iron, or any other metal. This disadvantage does not apply to metal buckles, fasteners or studs used to hold or reinforce the Armour. This penalty does not apply to metal weapons, items and objects not used as Armour, but proper role-play should still be observed."},
  ],purchased:[
    {name:"Nature's Cache",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Wild Elf",prereqs:[],desc:"Once a day per purchase, a Wild Elf is able to construct a small temporary shelter for themselves and up to 4 allies chosen at the time of creation. This 10 foot by 10 foot area provides multiple benefits and lasts 1 hour or less. It can only be constructed outdoors, but functions on any terrain. To use it the Wild Elf should affix their Nature's Cache tag to a location, which then becomes the center of the cache and state \"Innate Nature's Cache\". Hidden Scent: Those inside the cache are undetectable by hostile animals and insects. Forage: The Wild Elf can spend 10 minutes searching for healing herbs, which will provide 10 Healing points total, divided up as desired, to all within the shelter. These herbs will expire with the shelter if unused. The Pack: For the hour after the cache ends, all members of the camp will gain +1 damage with weapons against any opponent with which they all have simultaneous line of sight. This damage bonus does not stack with other uses of The Pack. Natural Intuition: While in the cache, the Wild Elf may query the surrounding lands, detecting its current state of being and any areas of impurity or corruption. This is a difficult task and is not always successful. The Wild Elf should attempt to find a Shaper prior or during the use of Nature's Cache. If no Shaper is available, the lands are unclear with their answer."},
    {name:"Body Point Bonus (Wild Elf)",maxPurchases:1,bodyBonus:5,strBonus:0,raceReq:"Wild Elf",prereqs:[],desc:"This skill represents extra constitutional training the Wild Elf has gone though, beyond what is standard for their race and grants +5 Body. This skill can only be purchased once throughout the character's entire existence."},
  ]},
  "Wood Fae":{cpBonus:0,fragCost:0,lore:"Distant cousins to the Faerie Folk, Wood Fae are rumoured to have been born of magic within the forests of the world. This may account for many of the Wood Fae having an affinity to natural creatures. Quite contrary to their faerie folk cousins, the Wood Fae have an extreme dislike for all forms of charms and will go to nearly any length to oppose mind-altering spells or effects. They are not only averse to practicing Charming Magics themselves but are even able to remove Charming effects from others. They are for the most part very carefree and friendly. They generally live a polyamorous lifestyle, though they rarely keep one mate for more than 10 years. Life Span: 1000-1200 years. Language: Gaelic. Racial Characteristics: Long pointed ears, and small horns that grow out of their foreheads.",auto:[
    {name:"Lust for Life",kind:"advantage",desc:"A Wood Fae's natural attunement to the forest and all things living has given them a lust for life that other races lack. Should a Wood Fae drop into their Bleed Count they are given a full two minutes before entering their Death Count rather than the standard one minute."},
    {name:"Iron Aversion",kind:"disadvantage",desc:"Wood Fae will take x2 damage from any source using the suffix \"Iron\" in its damage call. Carrying iron items is permitted, but doing so will cause great discomfort and should be roleplayed accordingly. This disadvantage applies to damage taken to both Armour and Body. As with all racial vulnerabilities, iron damage will bypass any thresholds a Wood Fae might have."},
  ],purchased:[{name:"Charm Break",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Wood Fae",prereqs:[],desc:"This ability has two functions. Firstly, it can allow the user to \"Racial Resist Charm\" all charm-based attacks. Charm-based attacks are considered effects which instill friendship or loyalty. Specific examples of charms are a Bard's Songs of Love, Charm, and Dominate plus Ritual charm spells and monster effects which are charm-based. Resisting in this manner uses up the ability. The second function is the ability to break an active charm effect on another person. This can only be accomplished through 10 seconds of talking to the Charmed character then declaring \"Innate Charm Break\" while touching them. Doing this uses up the skill for the day and creates a visible effect like any racial resistance does when it is used. Charm Break is usable once per day per purchase."}]},
  "Orc":{cpBonus:0,fragCost:0,lore:"Orcs, or \"Green-Skins\" as they are commonly called, are a fierce and combative goblinoid race. Orcs normally organize themselves into tribes and clans that consist of ogres, kobolds and other goblinoid races. Orcs appreciate strength and skill in combat above all things. They are less intelligent than a human is, but generally stronger and more disciplined. Life Span: 30-40 years. Language: Russian. Physical Characteristics: Green skin (varying tones).",auto:[
    {name:"Immune to Fear",kind:"advantage",desc:"Whether brave or stupid, Orcs cannot suffer the effects of fear. The immunity is always active. Orcs should call 'No Effect' when fear effects are used on them."},
    {name:"Charmable",kind:"disadvantage",desc:"The same mental toughness that grants Orcs immunity to fear also causes them to be susceptible to Charm effects. The Charm spell and Charm alchemy, as well as any Charm monster abilities will completely control the Orc. This means that instead of only being susceptible to friendly suggestions, the Orc will blindly follow any commands, including suicidal orders. These commands may include anything from killing a loved one to suicide. The commands can include forcing the victim to tell the truth as they know it (which may or may not be the OOG truth known by the player). A note to victims of this effect: You are never expected to do anything that makes you uncomfortable OOG. This includes but is not limited to being forced to do unsafe acts, actions of an inappropriate sexual nature or anything else that makes you uncomfortable for any reason, OOG. Although the potency of the effect is increased, its duration is not and the Orc will have full memory of all events when the charm wears off or is remove by standard means. Note that this only applies to effects that copy the Charm spell specifically, not all charm-like effects such as Taunt, Song of Love, Dominate, etc."},
  ],purchased:[{name:"Orcish Constitution",maxPurchases:1,bodyBonus:5,strBonus:1,raceReq:"Orc",prereqs:[],desc:"Purchasing this racial grants an orc the combination of Strength Point Bonus and Body Point Bonus. Furthermore, when an Orc has 50% or less of their total natural Body points (rounded down) they gain +1 damage to all melee weapon swings. This skill may only be purchased once."}]},
  "Ajaunti":{cpBonus:0,fragCost:0,lore:"An extravagant, passionate and amicable people, the Ajaunti (\"Aja\" for short) are a nomadic and colourful race. Where and when the Aja culture came to be is a mystery. Full of life, love and celebration, the Aja place high value in songs, dancing, and storytelling. Life never stops moving, so the Aja never stop moving either. Wanderers by choice and welcoming of strangers, Aja \"clans\" slowly criss-cross the continent in large caravans, following the weather and the winds of fate. The Ajaunti are always willing to share their wine, campfires and wisdom with any willing to join them. Life Span: 60-80 years. Language: Romanian. Racial Characteristics: As an Ajaunti, it is required for the PC to talk with a thick middle European accent and dress with a flamboyant & extravagant fashion sense.",auto:[
    {name:"Eyes of the Mother",kind:"advantage",desc:"When the Blood Curse which prevented all Ajaunti from casting magic was removed, it was replaced with a boon by an unknown benefactor. Perhaps it was a benevolent God who felt pity on the Ajaunti for what was done to them, or perhaps it was the Ancestors of the Aja themselves. Whatever the source, Ajaunti cannot be surprised with violence, as if a greater power is always watching over them. All Aja are immune to the Surprise prefix. The defensive call for this ability is \"Racial Foresight!\". It may be used at will."},
    {name:"Lost in Memories",kind:"disadvantage",desc:"When an Ajaunti dies, they have the normal 1 in 10 chance of remembering their death. If they fail to remember, Aja lose 24 hours of memories, not the standard 1 hour. In addition, if an Aja forgets their death there is a 50% chance that they will bring something back with them. When this occurs, the Aja will know it has happened upon resurrecting but will not know any further details. This can take 3 forms, chosen by a Shaper: 1) A cursed item returns on their body. These items are always negative and can only be removed by effects which remove Greater Curses. The item's history and specifics of the curse will be decided by the Shaper. 2) A restless spirit materialises within 1 day's travel of where the Aja resurrected. This ghost will attempt to find the Aja and will seek their aid in putting their spirit to rest. 3) A hostile spirit from the Deadlands arrives. It instinctively knows where the Aja can be found and will locate the Aja within 24 hours, seeking to destroy them."},
  ],purchased:[{name:"Ancestor's Wisdom",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Ajaunti",prereqs:[],desc:"When heroism is required, the Ajaunti gift for inspiration can rake the coals of greatness in others. To initiate Ancestor's Wisdom, the Ajaunti must tell a story of how one of their ancestors overcame adversity or performed an act of heroism to inspire those who listen. The story must last at least one minute but may go longer if desired. After the minute has passed, the Ajaunti may then choose one or more targets from the audience to receive a boon from the ancestors. This is done by touching the forehead of the listener and declaring \"Innate Ancestor's Wisdom (Type)\". The nature of the story told will determine what wisdom the Ajaunti is trying to pass along to their audience and all recipients must be granted the same type of boon. If a second Ajaunti is present during the story, they may add to the story to increase the potency of the boon. The Ajaunti assisting in the story must either speak for one additional minute or must play music during the tale. The assistant does not need to expend their own use of Ancestor's Wisdom to participate. If over 10 Aja members of the same clan (including the Aja using Ancestor's Wisdom plus their assistant) are present for the ceremony, it will become even more powerful. These additional clan members may participate or may simply observe. Ancestor's Wisdom may be used once a day per purchase, but each type of ceremony may only be performed once a month. Ceremony of Courage: Performing this ceremony will extend the Bleed and/or Death Counts of up to 3 targets for the next hour. If a single Aja performs the ceremony it will add a minute to the target(s) Bleed Counts. If assisted, it adds a minute to both Bleed and Death Counts. If 10 or more clan members are involved, it will double the duration of both counts. Ceremony of Celebration: This ceremony will create a permanent item for each target of the ceremony. These items will gain no effect beyond being permanent and they cannot have been magically enchanted to begin with. If they are kept by the recipient for 1 year they will turn into catalysts of a type and emotion desired by the owner. Ceremony of Hex Breaking: This ceremony will allow an Ajaunti to remove any one curse that is afflicting a target. It will permanently remove any Lesser Curse. If an assistant is used, the Ceremony of Hex Breaking may temporarily remove Greater Curses for 1 hour. If 10 or more clan members are present, then the ceremony may effect up to 3 targets simultaneously and has a chance to permanently remove Greater Curses with shaper approval. Ceremony of Mourning: This ceremony grants the ability to communicate with the ghost of a departed (final death) spirit for 10 minutes, so long as the final death occurred within the past year. The spirit must be willing to participate and a Shaper or marshal is required to perform this ceremony. Spirits spoken to in this manner cannot recall anything about their death and they cannot speak, but they can hear and respond with body language. If an assistant is used, the ghost can speak. If more than 10 members of the clan are present, the spirit remains for an hour."}]},
  "Einher":{cpBonus:0,fragCost:0,lore:"A semi-nomadic Northern people, the Einher are very superstitious by nature. Though the Einher enjoy being shockingly vulgar, they are very serious about any conduct that may disrespect them or their kin. As such, they tend to avoid disrespecting others, unless they are looking for a fight. For an Einher it is important to know the difference between a friendly jab at someone and the sort of thing that blood will be shed for. The Einher have an irrational fear of fog, whether magical or natural. They will suffer from the effects of paranoia and/or hallucination if confronted by fog. The thicker it is, the worse the effects. This fear is strictly roleplayed. The Einher detest Ice Elves. Throughout their history, the Ice Elves have attempted to force the worship of Pandora upon them, causing much bad blood between the two civilizations. Life Span: 60-80 years. Language: Swedish. Racial Characteristics: Einher must wear two or more of the following: furs, kilts, and braided hair.",auto:[
    {name:"Resist Cold",kind:"advantage",desc:"Resist Cold allows the user to \"Racial Resist Cold\" one cold-based effect. As a Racial Ability, it may be used to \"Resist\" Ritual Magic. This skill is automatically given on character creation, cannot be purchased for multiple uses, and is only usable once per day."},
    {name:"Hell's Embrace",kind:"disadvantage",desc:"The Einher live for battle. It is their belief that if they die their final death in combat, their souls travel to a great hall where they will fight and drink for eternity. It is every Northman's fear that they will die alone outside of combat. Einher who die outside of combat have a 50% chance of taking two deaths on their character card for the one they take in game. An Einher who has died outside of combat will first flip a coin to determine if the death taken is counted as one or two, then the deaths are applied to their character card, and finally, if required, an additional flip(s) to see if they succumb to final death."},
  ],purchased:[
    {name:"Berserker Rage",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Einher",prereqs:[],desc:"A Northman can incite in himself a powerful Berserker Rage. The character must cry out \"Innate BERSERK!\" for a ten-count, i.e., \"Berserk 1, berserk 2, berserk 3...\" while working themselves into a frothing frenzy. For the duration of one combat, the character gains +1 Strength, +5 Body, and is immune to Fear effects. From the point at which the fight ends, it takes 5 minutes for the effects of Berserk to wear off. The character cannot end the rage sooner and must continue to fight so long as opponents are visible. Multiple uses of this skill may be expended to stack its effects, although this will not increase the duration. This skill is usable once per day, per purchase."},
    {name:"Body Point Bonus (Einher)",maxPurchases:1,bodyBonus:5,strBonus:0,raceReq:"Einher",prereqs:[],desc:"This skill represents extra constitutional training the Einher has gone though, beyond what is standard for their race and grants +5 Body. This skill can only be purchased once throughout the character's entire existence."},
    {name:"Strength Point Bonus (Einher)",maxPurchases:1,bodyBonus:0,strBonus:1,raceReq:"Einher",prereqs:[],desc:"This skills represents raw physical power, increasing the character's Strength rating by +1. This skill can only purchased once throughout the character's entire existence."},
  ]},
  "Hobling":{cpBonus:0,fragCost:0,lore:"A typically small, peaceful people with furry feet and hands, bushy eyebrows, and fuzzy sideburns, Hoblings, in general, are a peace and comfort-loving race. Most are horrified by violence and are easily scared off by the slightest danger. However, there are still a great many that find themselves in awe of the world and travel it attempting to learn about (and experience) everything. They are fun-loving and mischievous, enjoying anything that is exciting despite whatever possible danger there may be. These are the Hoblings most often encountered by the other races, since they travel the world over. These Hoblings are often considered an annoyance by other races, but the Hoblings still greatly enjoy the company of any people and love to tell and listen to stories of adventures. All these Hoblings really wish to do is have fun and enjoy life to its fullest. Life Span: 170-200 years. Language: Japanese. Racial Characteristics: Large fuzzy sideburns and eyebrows. Furry hands and feet are optional but encouraged.",auto:[
    {name:"Taunt",kind:"advantage",desc:"This skill allows the Hobling to Taunt a target, inciting them into combat. The target will immediately attack the taunting Hobling, ignoring all other targets until the Hobling is on the ground unmoving, out of line-of-sight, or physically unobtainable. The target is still free-willed and able to fight with strategy and cunning but they must attack immediately, and must target the taunting Hobling. After the Hobling is down or has left line-of-sight, the target may then choose to stop combat if they wish. In order for this racial to be effective, the Hobling must actually taunt the target with 2 insults, declare \"Innate Taunt\" then hit with a successful packet strike. This skill is automatically given on character creation, cannot be purchased for multiple uses and is only usable once per day. Hobling Taunt is considered a Psionic attack but is a racial and cannot be resisted by anything short of another racial ability. Some example taunts are: \"Go soak your head in a bucket. Then some fool might mistake it for a helm and therefore mistake you for a knight\" and \"You have something on your face. Oh wait! That is your face!\""},
    {name:"Small Size",kind:"disadvantage",desc:"Hoblings can only purchase proficiency and specializations from the Simple weapon and Exotic weapon groups. No exotic weapon may be used that is greater than 16 inches but other weapons (such as staves in the Simple Group) are not affected."},
  ],purchased:[{name:"Racial Dodge",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Hobling",prereqs:[],desc:"Allows the subject to dodge any attack, calling \"Racial Dodge\", so long as it is not a trap of any kind, or some other unreasonable damage-causing incident, such as falling off a tower. This skill is usable once per day per purchase. It is not possible to dodge a Surprise Attack, Power Word, Area of Effect or Massive damage. You must be conscious to dodge."}]},
  "Human":{cpBonus:50,fragCost:0,lore:"Humans are the most populous of the sentient, civilized races. They range widely in appearance, culture and diversity. Life Span: 60-80 years. Language: Common (English).",auto:[
    {name:"Character Point Bonus",kind:"advantage",desc:"Humans begin with 50 extra CP upon character creation. This bonus CP does not count towards a character's level."},
  ],purchased:[{name:"Body Point Bonus (Human)",maxPurchases:1,bodyBonus:5,strBonus:0,raceReq:"Human",prereqs:[],desc:"This skill represents extra constitutional training the Human has gone though, beyond what is standard for their race and grants +5 Body. This skill can only be purchased once throughout the character's entire existence."}]},
};

// Frag race costs by tier
const FRAG_RACE_COSTS = { Uncommon:75, Rare:150, Obscure:250 };

const FRAG_RACES = {
  // Uncommon
  "Am'Rath":{tier:"Uncommon",fragCost:75,cpBonus:0,lore:"The Am'Rath tribes are a version of humanity in its rawest and most primitive form. They are resilient, vicious and unforgiving opponents. A semi-organized and war-like people, they have divided themselves into tribes with differing priorities and leadership. Some tribes are deeply spiritual and shamanistic, some are focused on expansion and conquest, others are little more than rampaging Am'Raths. Life Span: 40-60 years. Language: Primordial Common (English). Racial Characteristics: Bone fetishes and/or beads worn throughout hair and facial hair, colourful tribal tattoos.",auto:[
    {name:"Simple Weapon Damage Bonus",kind:"advantage",desc:"Am'Raths gain +1 damage to all weapons in the simple weapon group."},
    {name:"Simple Weapon Restriction",kind:"disadvantage",desc:"To an Am'Rath, all melee weapons outside the Simple Weapon group are considered \"exotic\" for purposes such as proficiencies, slays and specializations. Ranged weapons are not included in this disadvantage."},
  ],purchased:[
    {name:"Clobber",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Am'Rath",prereqs:[],desc:"This physical attack can be used with any melee strike and will cause 25 points of damage, the damage type based on the weapon used. If the attack misses, the skill is used. It may be augmented with magic and alchemy. It is used by calling out \"Innate Clobber!\" before the attack. Clobber may be used once per day per purchase."},
  ]},
  "Faun":{tier:"Uncommon",fragCost:75,cpBonus:0,lore:"Fauns are a benevolent and care-free race, often mistaken for Fae. In fact, they were once forest spirits, given mortal, Bestial form. Most Fauns are friendly and compassionate, yet shy and reserved. Fauns have a natural affinity for forests and will feel drawn toward them as a habitat. Life Span: 1000-1200 years. Language: Punjabi. Racial Characteristics: Black on the underside of the nose, philtrum and upper lip. Ram horns, antlers or wooden branches. White dots on cheekbones. Faun ears (low hanging or \"floppy\" large ears).",auto:[
    {name:"Companion",kind:"advantage",desc:"A Faun may declare another living creature a \"companion\" each day. This companion is decided at reset and cannot be changed until the next reset. If their companion enters their Death Count a Faun may place both hands on their body and pause the Death Count. After 60 seconds of concentration, their companion will be affected by an \"Innate Magic Life\" effect from the Nature sphere. This ability may be used once per day."},
    {name:"Restriction to Nature Healing",kind:"disadvantage",desc:"When it comes to magical healing, Fauns cannot be healed by any magic outside of the Nature sphere. This includes all Body Point healing and healing effects other than Mending. Natural and alchemical versions of these effects will work. Additionally, consuming a Goodberry will heal a Faun for 2 Body when they are in their Bleed Count, instead of the regular 1 Body. Life spells from outside the Nature sphere will work on Fauns but not as effectively — the Faun will receive the normal benefits of a Life spell, except that they will only be healed to 1 Body, not full Body. Life effects from Nature sources will operate as normal."},
  ],purchased:[
    {name:"Forest Revival",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Faun",prereqs:[],desc:"Fauns may, once per day per purchase, fully heal their Body by placing both hands on any living tree within a forest and concentrating for 60 seconds. During this time they may not use any other skills and are considered to be \"concentrating\" as per spell-casting. Body Points are gained immediately at the end of the 60 second count."},
  ]},
  "Minotaur":{tier:"Uncommon",fragCost:75,cpBonus:0,strBonusPerFiveLevels:1,lore:"Minotaurs were a once proud and noble race, residing deep within the Fae Realm. Cursed by the Elder Fae, they were transformed into monstrous brutes with the body of a human and the head of a bull, and driven underground for many centuries. Most Minotaurs are extremely superstitious due to torturous games played on them by the Fae. Life Span: 50-60 years. Language: Welsh. Racial Characteristics: Brown makeup and large bull horns. White or light tan makeup around the mouth and the bottom of the nose in a muzzle shape covering at least 25% of the face. Black line extending from the nose to the top of the lips, and black lips.",auto:[
    {name:"Enhanced Strength",kind:"advantage",desc:"Minotaurs are incredibly strong. They will gain +1 Strength every five levels, starting at level 1, giving them +2 Strength at level 6, +3 Strength at level 11, and so on."},
    {name:"Fae Susceptibility",kind:"disadvantage",desc:"Centuries of mind manipulation by the Fae have altered Minotaurs' reactions to mind magic. If a Fae hits a Minotaur with a magical mind effect of any kind, the Minotaur will become enraged for one minute. During this time, they may not attack the source of the magic. Once the minute is complete, the Minotaur will no longer be enraged and the mind-altering effect will affect them as normal. The mind alteration's duration begins at this point. Fae able to induce this effect include True Fae, Redcaps and even the thin blooded relatives such as Carnal Fae and Wood Fae but not other Minotaurs."},
  ],purchased:[
    {name:"Fae Ward",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Minotaur",prereqs:[],desc:"A Minotaur with this ability may craft a special magical Fae Ward, capable of preventing entry by any Fae creature, including those with only trace amounts of Fae blood in their veins. The Fae Ward must be carved on an object containing at least a small amount of iron and must be at least 1 square foot in size. The carving takes 10 minutes of roleplaying. Once erected, no Fae creature may cross within 10 feet of the Ward. The Ward lasts for 5 days unless moved, defaced or destroyed. This ability is usable once per day per purchase."},
  ]},
  "Kobold":{tier:"Uncommon",fragCost:75,cpBonus:0,lore:"Kobolds are often stupid but crafty creatures. They appear as dog-like Goblinoid creatures with red skin, large incisors and black fingernails. Kobolds have become a universal pest in every corner of the world. They have a natural affinity for blowing themselves up with explosives and are well known for their love of shiny things. Life Span: 170-200 years. Language: Pig Latin. Racial Characteristics: Red makeup on exposed skin, high-pitched annoying voice, black underside of nose around nostrils, horizontal black lines across bridge of nose.",auto:[
    {name:"Innate Sap",kind:"advantage",desc:"A Kobold receives one free Sap skill every other level, starting at first level. These Innate Saps are identical to the purchased skill. This racial does not hamper the Kobold's ability to purchase the Sap skill. The call for this is \"Innate Sap\"."},
    {name:"Frailty",kind:"disadvantage",strBonus:-2,desc:"Kobolds are frail and weak creatures. A Kobold has a -2 strength penalty. This means they swing for one less damage, to a minimum of one."},
  ],purchased:[
    {name:"KABOOM!",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Kobold",prereqs:[],desc:"Kobolds are natural Trappers. A Kobold may use this natural affinity to make an extraordinary, unique trap, even without the Trapper skill. This is similar to an Explosive Trap. For every 1 RM used to create the trap, it will do 2 points of damage to everyone within 5 feet of the trap when triggered. If the Kobold has 4 levels of Trapper, this amount is raised to 3 points damage per 1 RM. Kobolds will receive one KABOOM! trap tag per day per purchase."},
  ]},
  "Ogre":{tier:"Uncommon",fragCost:75,cpBonus:0,bodyBonusPerLevel:2,lore:"Typically massive, lumbering brutes, Ogres can best be described as monstrous. With superior strength and constitution, Ogres are the muscle and brute force in every Greenskin army. While not the brightest of thinkers, they are cunning, and what they can't out-think they will out-smash. Life Span: 10-12 years. Language: Polish. Racial Characteristics: Yellow skin and prosthetic tusks, red or white war paint covering at least 25% of the face.",auto:[
    {name:"Ogre Constitution",kind:"advantage",bodyBonus:5,strBonus:2,desc:"Because of their incredible size and strength, Ogres begin with +2 Strength, and +5 Body. Furthermore, Ogres gain an additional +2 Body per level."},
    {name:"Untempered Rage",kind:"disadvantage",desc:"If an Ogre takes more than 15 points of damage directly to their Body from any single effect from any source, they immediately fly into a mindless rage. They will immediately attack everyone nearby, friends and foes alike. This onslaught may only be stopped by dropping the Ogre into its Death count. After 10 minutes have passed since the attack, the effect will wear off."},
  ],purchased:[
    {name:"Ogre Smash",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Ogre",prereqs:[],desc:"By summoning all of their great strength into a single melee attack, an Ogre can target an opponent's weapon or shield, causing grievous amounts of damage to it. Weapons and shields struck by this attack are affected by a \"Shatter\" effect, destroying them unless they are immune or have resistance. To activate, the Ogre must let out a blood curdling war cry followed by the call \"Innate Physical Smash!\" This ability will only stay active for 10 seconds and is considered used even if the attack misses. Usable once per day per purchase."},
  ]},
  "Squamata":{tier:"Uncommon",fragCost:75,cpBonus:0,lore:"\"Squamata\" is a general term to describe a number of green-skinned lizard-like races: the Boggrel (frog people), the Gremmel (lizard people), and the Shak'tar (snake people). Although quite distinctive in regards to culture, personality and even physical appearance, these races all share the same advantages and disadvantages. Life Span: 40-50 years. Language: Samoan. Racial Characteristics: Makeup must look like a type of colourful lizard (Gremmel), frog/toad (Boggrel), or snake (Shak'tar) in a minimum of two colours.",auto:[
    {name:"Seal Pores",kind:"advantage",desc:"Squamata's pores are sealed to prevent toxic substances from entering the bloodstream, making them immune to packet-delivered alchemical attacks, stating \"No Effect\". This defense will not function against ingested or contact alchemy. Chemistry Gas Globes may also be resisted in this manner."},
    {name:"Soft Underbelly",kind:"disadvantage",desc:"All Squamata take x2 damage from all physical weapon damage with \"Body\" in the call. As with all racial vulnerabilities, physical Body weapon damage will bypass any thresholds a Squamata might have."},
  ],purchased:[
    {name:"Venomous Spit",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Squamata",prereqs:[],desc:"This ability allows the Squamata to spit an alchemical Venom attack at a target. For 10 minutes, the victim will be in constant pain and cannot cast spells unless they have the Combat Wizardry skill. After 10 minutes, the Venom will have worked its way through the target's system and they will take \"Alchemical 25 Body Poison\". This effect does not stack and can be cured by any means that removes a poison. The Squamata must prepare their Venom on a 3-count and has 1 minute to spit it at their target. Usable once per day per purchase."},
  ]},
  // Rare
  "Avian":{tier:"Rare",fragCost:150,cpBonus:0,lore:"Avians are a race of mountain-dwelling bird people. They are tinkerers and inventors, one of the few races to circumvent magic with simple and basic steam-based machinery. Avians are linked to the Shadow Plane through generations of its use by their ancestors and their spirits have become tainted with its presence. Life Span: 70-90 years. Language: Hebrew. Racial Characteristics: Feathered eyebrows and hair and yellow nails.",auto:[
    {name:"Spirit Anchor",kind:"advantage",desc:"Spirit Anchor allows an Avian to anchor their spirit to a specific location and be able to \"shadow step\" to it on a 10 second count, stating \"Innate Spirit Anchor 1, Innate Spirit Anchor 2…\", once per day. This magical transportation is done via travel through the Plane of Shadow. The anchor itself is an in-game item that must be represented by an active glow-stick or LED attached to a \"mechanical\" steam-machinery based item approved by a Shaper. If the Spirit Anchor is destroyed, a new one can be created after an hour's work. If an Avian attempts to transport themselves to a destroyed anchor, they will die."},
    {name:"Shadow Mark",kind:"disadvantage",desc:"Avian spirits are irrevocably tied to the Shadow Plane. If an Avian enters its Death Count, they gain a Shadow Mark within 1 hour. This Mark will last until the next skill reset. If an Avian dies, they will resurrect with a permanent Mark. Each Mark adds +5 seconds to the Avian's Anchor count, +1 damage from all magic sources and -1 Strength. These negatives only affect the Avian between 6 PM and 6 AM."},
  ],purchased:[
    {name:"Create Goggles",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Avian",prereqs:[],desc:"This ability allows the Avian to create a mechanical set of Goggles which only they can use. By spending 10 minutes gathering pieces of scrap the Avian can state \"Innate Create Goggles\" and make them magical. Once created, an Avian has 10 seconds to infuse these Goggles with any 1st to 3rd Circle spell effect. Purchasing this ability a second time will grant all spells up to 6th circle and a 3rd purchase will grant up to 9th circle. The Goggles function as a 1/day magical item and last 5 days before the magic fades."},
  ]},
  "Blackmane":{tier:"Rare",fragCost:150,cpBonus:0,lore:"Blackmanes were once exceptionally powerful spirits of the Deadlands, cursed to possess the unwilling bodies of the living over and over for eternity. They are bound to Arthos as wandering spirits who claim by force the flesh of mortals whose spirit has been separated from their body. Language: Common (English). Racial Characteristics: The racial requirements of the possessed race. Additionally, they can manifest dripping orange veins around the eyes at will.",auto:[
    {name:"Deadlands Possession",kind:"advantage",desc:"Blackmanes must possess a body to exist in this world. The player can choose any race within the Core rulebook other than human and will gain the racial appearance requirements and the automatic racial that comes with that race. When a Blackmane dies, the body it was possessing dies as well, leaving behind a finalled corpse. The spirit is forced into the spiritless body of a new NPC who is actively manifested in the Deadlands. This process repeats until the Blackmane fails their final death flip."},
    {name:"Favoured Vulnerability",kind:"disadvantage",desc:"All harmful spells from the favoured spheres (Light/Dark/Draconic) do x4 damage and have a x2 duration (if applicable). Blackmanes cannot be the target of any beneficial favoured magic or gain the Favoured or Paragon skills."},
  ],purchased:[
    {name:"Spirit Fusing",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Blackmane",prereqs:[],desc:"Blackmanes can fuse their spirits to material objects, spending 1 minute to create spirit links naturally with any item they are touching which is not Favoured (Dark, Light or Draconic) in nature. Blackmanes may have 1 active Spirit Fusing per purchase. Additionally, Blackmanes may \"steal\" an existing spirit link that belongs to another person so long as that person is within their Death count, requiring a 1-minute count while touching the spirit linked item."},
  ]},
  "Draconian":{tier:"Rare",fragCost:150,cpBonus:0,lore:"Draconians are rumoured to have descended from a bloodline infused with Draconic magic. Morally and philosophically, Draconians are usually matched closely with the Dragon whose colour they share. Almost all Draconians find Divine Magic and the Gods morally reprehensible. Draconians appear as humanoid dragons of various colours. Life Span: Immortal. Language: Old English. Racial Characteristics: At least two large horns protruding from the forehead and scales done in sequins, makeup or prosthetic covering 40% of the face and all other exposed skin.",auto:[
    {name:"Natural Threshold",kind:"advantage",desc:"Draconians have a thick layer of scales which become harder than steel as they age. They gain a natural (normal) threshold of one for every three levels, starting at level 1, giving them a 2 Normal threshold at level 4, 3 Normal threshold at level 7, and so on."},
    {name:"Weak Spirit",kind:"disadvantage",desc:"Due to the nature of their existence, Draconian spirits are considered weaker than normal. They get one \"free\" death before they must begin flipping, instead of the normal two."},
  ],purchased:[
    {name:"Reflect Divine",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Draconian",prereqs:[],desc:"Once a day per purchase, a Draconian may use a natural ability to reflect Divine Magic back on its originator, calling \"Racial Reflect Divine\". The Draconian has the option of not reflecting the spell if they so choose. Because this is a racial ability, it affects both Battle Magic and ritual spells as well as anything with \"Light\" or \"Dark\" in the call. It can be stacked with magical protections such as Shield Magic. Usable once per day per purchase."},
  ]},
  "Fire Elf":{tier:"Rare",fragCost:150,cpBonus:0,lore:"This hardy, desert-native branch of elvendom goes by the name Cindus'Thalan, or Fire Elf. Fire Elves are regarded by many other races as inhospitable, hard-headed, and merciless. Having a population much more numerous than their few fertile lands can provide, most Fire Elves wander in small tribes following the rains. Life Span: 700-1000 years. Language: Arabic. Racial Characteristics: Red eye shadow and eye sockets with optional orange and yellow highlights, elf ears (with red tips), loose-fitting and light-weight desert clothing.",auto:[
    {name:"Resist Fire",kind:"advantage",desc:"Fire Elves are extremely resilient to heat. Once a day they may call \"Racial Resist Fire\" to any magic or elemental attack involving fire or heat, and take no damage from it."},
    {name:"Armour Restriction (Fire Elf)",kind:"disadvantage",desc:"Fire Elves are limited to 10AP worth of physical armour at level 1. That amount rises by +5AP per level. The fire elf may physically wear more armour but will receive no benefit beyond those numbers."},
  ],purchased:[
    {name:"Endurance",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Fire Elf",prereqs:[],desc:"When struck by an effect that would drop a Fire Elf into their Bleed Count via a number based attack (melee, magic, acid, etc.) the Fire Elf may call \"Racial Endurance!\" and remain at 2 Body points, regardless of how much damage they have taken. Endurance cannot be used against numeric attacks that drop a character into their Death Count, such as Elemental attacks. Usable once per day per purchase."},
  ]},
  "Goblin":{tier:"Rare",fragCost:150,cpBonus:0,lore:"Filthy, disgusting and mischievous, Goblins are generally regarded by all civilized races to be a plague upon the lands. Traditionally the frontline fodder of the \"Greenskin\" forces, Goblins excel in trapping, torture and treachery. They love the taste of kobold flesh. Life Span: 40-60 years. Language: Ukrainian. Racial Characteristics: Green skin, long pointed green ears, and thin black veins on the neck and around the mouth.",auto:[
    {name:"Parasites (Advantage)",kind:"advantage",desc:"The racial parasites that live in all Goblins come with a surprising advantage. Goblins can vomit these parasites onto creatures to keep them from bleeding out. If a Goblin spends 10 seconds vomiting on a target in their Bleed Count, they will be stabilised and go to 0 Body. This ability may be used at will but the Goblin must consume some type of organic matter larger than an apple in between uses. This ability cannot be used on other Goblins."},
    {name:"Parasites (Disadvantage)",kind:"disadvantage",desc:"Goblins, constantly living in filth and muck, have become host to racial parasites that feed off their spirit and vitality. These microscopic parasites are incurable even through resurrection and will always consume one half of all healing that is administered to the Goblin (rounded down) to a minimum of 1."},
  ],purchased:[
    {name:"Amorphic Mucus",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Goblin",prereqs:[],desc:"All Goblins are equipped with a gland that produces mucus which, when coughed up, has the ability to replicate certain types of alchemy. To use this skill the Goblin must excrete and cough up the Amorphic venom on a 10 second count. After being excreted, the Amorphic Mucus must be put in contact with any alchemical gas globe for 1 minute. If successful, the mucus will harden and take on the exact same properties of the alchemy it was exposed to but will expire in 1 hour. Only one Amorphic Mucus may be prepared at any given time. Usable once per day per purchase."},
  ]},
  "Risen":{tier:"Rare",fragCost:150,cpBonus:0,lore:"A hybrid race, the Risen are capable of both stepping into the world of the living and that of Undeath. Risen start life at Undeath, likely as one of the thousands created by long dead necromancers or forced to rise out of ancient cursed graveyards. Hand picked by other Risen and forcefully put through a secretive process only known as the Harrowing, the mindless Undead is transformed into a new form. Language: Common (English). Racial Characteristics: While in living form a Risen is a sad reflection of their original race. In Undead form a Risen is recognized as a fast moving rotting corpse.",auto:[
    {name:"Dual Race",kind:"advantage",desc:"A Risen's automatic advantage is dependent on which form they are in. Undead Form: 0 Silver Threshold levels 1-5 (6PM-6AM only), 0 Magic Threshold levels 6+ (6PM-6AM only), heals from Infliction, +2 Strength Bonus, considered a sentient Greater Zombie. Living Form: Heals from Healing, senses as Life, no advantages of the original living race."},
    {name:"Dual Race (Disadvantage)",kind:"disadvantage",desc:"Undead Form: Senses as both Undead and Necromancy, x4 Magic Body damage from Healing spells, Daytime Vulnerability (1 Arcane damage per second if uncovered and outdoors 6AM-6PM), susceptible to spells targeting Undead, requires 2 Life effects to take out of Death Count. Living Form: All as if living, senses as original pre-Undead race."},
  ],purchased:[
    {name:"Spirit Skinning",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Risen",prereqs:[],desc:"Any creature that has a spirit, is capable of resurrection, and is in their Bleed Count or unable to interrupt a killing blow, may be Spirit Skinned. The Risen must state \"Innate Spirit Skinning\" and then perform a Killing Blow. If successful, the target is instantly placed into their Death Count and part of their spirit is transferred into the Risen. The Risen must immediately transform to their living form. A Risen may use Spirit Skinning at will. However, the maximum number of Spirit Recalls on their spirit is equal to the number of times they have purchased the Spirit Skinning ability."},
  ]},
  "Wolven":{tier:"Rare",fragCost:150,cpBonus:0,lore:"The Wolven race has only been known to exist for a few hundred years, rumoured to have been brought into existence by ancient druids to defend their sacred henges and groves. Wolven look towards the eldest in their communities to solve disputes, consider respect to be the highest of virtues, and are natural hunters. Life Span: 40-60 years. Language: Greek. Racial Characteristics: Appropriate make-up for the type of canine being played, large pointed ears and a tail.",auto:[
    {name:"Natural Hide",kind:"advantage",desc:"Wolven are born with a natural thick hide. A Wolven will gain 2 AP (Armour Points) per level, starting with 2 AP at level 1. This armour works in every respect to normal armour save that it cannot be refit. For a Wolven to repair their Natural Hide, they must heal it as though it were Body. Normal armour may be worn on top of Natural Hide."},
    {name:"Vulnerability to Fire",kind:"disadvantage",desc:"Wolven have a natural fear of and vulnerability to fire. A Wolven will take x2 damage from all sources of fire, including Magical and Elemental. Should a Wolven take fire damage to Body, they will suffer a Cower effect from the source of that damage. The Wolven must attempt to flee the source of their fear and cower behind any large physical object for 10 seconds before they regain their nerve. As with all racial vulnerabilities, fire damage will bypass any thresholds a Wolven might have."},
  ],purchased:[
    {name:"Sense Undead",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Wolven",prereqs:[],desc:"Allows the player to sense Undead. To sense the Undead, the Wolven must roleplay that they are sniffing (\"scenting\") the air for 10 seconds uninterrupted, then state \"Innate Sense Undead\" in a normal speaking voice. Any Undead who hear the \"Sense Undead\" will respond \"Here\" in a normal speaking voice. This ability does not grant the detector any information on the type of Undead and will not allow Wolven to sense vampires. Usable at will."},
    {name:"Strength Bonus (Wolven)",maxPurchases:1,bodyBonus:0,strBonus:1,raceReq:"Wolven",prereqs:[],desc:"This skill represents raw physical power, increasing the character's Strength rating by +1. This skill can only be purchased once throughout the character's entire existence."},
  ]},
  "Yokai":{tier:"Rare",fragCost:150,cpBonus:0,lore:"Once a pack of fox Wolven known as the Charmolipi, the Yokai are a cursed race doomed by a selfless sacrifice to exist within the shattered state between demonic and mortal. Buried inside of each of them is a demon that hungers for blood, subdued only by their nomadic lifestyle and sheer force of inner will. Life Span: 80-100 years. Language: Greek and Japanese. Racial Characteristics: White makeup base on face with red and black around eyes and red lips. White with red or black canine ears. Red whisker lines on face. Nose black at the bottom with a thin black line on the philtrum. At least one burned demonic symbol on face.",auto:[
    {name:"Foxfire",kind:"advantage",desc:"The Yokai have been infused with demonic energy and can focus it into short bursts of destructive power through their physical attacks. After stating \"Innate Foxfire\" the Yokai will gain a Magic Fire aura for 10 minutes. This enchants the Yokai's spirit to deal +0 Magic Fire using any melee weapon the Yokai is proficient with for the duration. This ability is usable once per day."},
    {name:"The Stranger Within",kind:"disadvantage",desc:"Yokai are simultaneously mortal and demonic. As such, Yokai will sense as demonic in response to \"Sense Demonic\" calls. They will also count as a Greater Demon for the purposes of skills such as Angelic/Demonic Arts and Exorcism. Finally, Yokai take x2 damage from Psionic spell damage, bypassing any thresholds they may have."},
  ],purchased:[
    {name:"Enemy of my Enemy",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Yokai",prereqs:[],desc:"Once per day per purchase a Yokai may strike a Lesser Demon with a packet attack and call \"Innate Arcane Control Lesser Demon\". For the next hour the target will do anything asked of it, including sacrificing itself. This ability has no effect against Greater Demons. While a Yokai has a Lesser Demon under their control they will be viewed by all other demons as a demon themselves."},
  ]},
  // Obscure
  "Carnal Fae":{tier:"Obscure",fragCost:250,cpBonus:0,lore:"With grey skin and yellow veins, Carnal Fae tend to stand out in a crowd. They are a practical race, with a tendency towards self-preservation and a grim sense of humour. Although once mostly Fae-blooded, the millennia of exile has diluted their connection to the Dark Fae. Life Span: 5000-6000 years. Language: Gaelic. Racial Characteristics: Long pointed ears, grey skin and yellow veins which spider web over their body.",auto:[
    {name:"Destroy Light",kind:"advantage",desc:"This racial ability will allow the Carnal Fae to extinguish any magical or non-magical light source. The call for this ability is \"Innate Destroy Light\". If targeting a stationary light source not held by someone, a packet must be thrown and land within 5 feet of the light source to extinguish it. If held by a creature with a spirit, only the creature must be hit. This skill may be used once per day."},
    {name:"Vulnerability to Iron",kind:"disadvantage",desc:"A Carnal Fae cannot touch cold iron without experiencing extreme discomfort. If damage is called and a Carnal Fae is struck with an iron weapon, the Carnal Fae will take iron damage x4. As with all racial vulnerabilities, iron damage will bypass any thresholds a Carnal Fae might have."},
  ],purchased:[
    {name:"Greater Resist Magic",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Carnal Fae",prereqs:[],desc:"This racial ability will allow the Carnal Fae to resist any single incoming magical attack. This absorbs the attack, causing no ill effects to the Carnal Fae. This racial ability will stop any magical attack regardless of power, including ritual, Draconic and Arcane Magic, excluding ritual backlashes and flaws. The defensive call for this ability is \"Racial Greater Resist Magic\". This skill may be used once per day per purchase."},
  ]},
  "Faceless":{tier:"Obscure",fragCost:250,cpBonus:0,lore:"The Faceless are a dark and morbid race, ex-slaves of a demon master long thought to be dead. Appearing as mostly human, Faceless wear elaborate masks to cover a scarred or blank face underneath. All Faceless have amnesia, as their freedom came at a price — no memories of what came before it. Life Span: Immortal. Language: Common (English). Racial Characteristics: Venetian (carnival) style masks at all times covering at least the top 3/4ths of the face. The face under the mask is either featureless and pure white or a gruesome mess of scars.",auto:[
    {name:"Permanent Non-Detection",kind:"advantage",desc:"The Faceless cannot be detected by any means, natural or magical. They do not need to answer to calls of \"Sense Life\" or similar. Their presence is even hidden from that of ultra-powerful beings such as Gods and Dragons."},
    {name:"Demonic Spirit",kind:"disadvantage",desc:"The Faceless have been tainted by demonic powers. As such, Faceless take x4 damage from sources of Psionic damage and this is considered a racial vulnerability. As with all racial vulnerabilities, Psionic damage will bypass any thresholds a Faceless might have. Also, Banish and Exorcism spells will not return a Faceless to their home plane but they will drop the Faceless into their Death Count akin to a Death effect."},
  ],purchased:[
    {name:"Unmasked",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Faceless",prereqs:[],desc:"A Faceless may choose to remove their mask, releasing substantial anti-magical powers as a result, calling \"Innate Unmask <Sphere>\". Doing so gives the Faceless immunity to one sphere of magic of their choosing other than Psionics for 10 minutes after the mask is removed. While their mask is not being worn, a Faceless will lose their \"Non-Detection\" racial and instead will detect as everything. Not wearing their mask is draining for a Faceless, and it may only be done once per day per purchase."},
  ]},
  "Gnome":{tier:"Obscure",fragCost:250,cpBonus:0,lore:"Passionately curious and natural inventors, Gnomes are the less robust, more scholarly cousins of the Dwarves. Their cultural distaste for magic has driven them to pursue physical arts and sciences with an obsessive devotion. Gnomes have a distrust for all Fae. Gnomish society is a meritocracy valued based on contributions to inventive progress. Life Span: 400-500 years. Language: Finnish. Racial Characteristics: Freckles and colourful hair, plus a squeaky voice and gnomish style clothing (tinker/mechanic).",auto:[
    {name:"Scavenger",kind:"advantage",desc:"Gnomes have a natural talent for finding useful scrap, repurposing junk into amazing gadgets. At each Logistics, Gnomes may collect 5 universal RM."},
    {name:"Psychosomatic Static",kind:"disadvantage",desc:"Gnomes hate magic and magical items in particular. If a Gnome comes into contact with a magic item they will begin to itch violently, as if they were allergic to it, and must scratch themselves frantically. While the itching continues the Gnome is unable to speak, cast or use any skills, but can move at normal speed. This prevents a Gnome from activating magic items that have per day/hour/etc. abilities. Gnomish hatred of magic is a racial disadvantage and is therefore impossible to overcome."},
  ],purchased:[
    {name:"Gnomish Device",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Gnome",prereqs:[],desc:"Through skilled tinkering a Gnome can create fantastical gadgets which mimic magic items without being magical. For each purchase of Gnomish Device, a Gnome is able to build and maintain one additional Device. The Gnome may choose from 3 lists of 10 Devices during Logistics: Offensive, Defensive and Utility. Each Gnomish Device has one per day power and one negative effect. After the initial use, a Gnome may feed 5 RM to the Device to use it again, up to 5 times per day. Gnomish Devices do not expire but may be abandoned and replaced during Logistics."},
  ]},
  "Ice Elf":{tier:"Obscure",fragCost:250,cpBonus:0,lore:"Perhaps the most isolated, xenophobic and secretive of all Elven races, the Ice Elves call the tundras of the frozen north their homeland. All Ice Elves are tied to the dark goddess Pandora on a spiritual level. Acceptance of pain as a method to grow stronger is a core feature in almost every Ice Elf's upbringing. Life Span: 700-1000 years. Language: Portuguese. Racial Characteristics: Pointed ears with blue tips. Pale, blue-tinged skin with dark blue markings and ice-like designs around the eyes and upper face.",auto:[
    {name:"Scion of Suffering",kind:"advantage",desc:"Ice Elves are conditioned to carry on when physical pain would leave any other race unable to do more than cry for help. When at 0 or 1 Body, Ice Elves remain conscious and able to perform all actions they normally could at 2 Body, without falling unconscious. Use of this ability does not require the skill Self Mutilate."},
    {name:"Pandora's Touch",kind:"disadvantage",desc:"Ice Elves are marked from birth by the dark magics of Pandora. If \"Sense Dark\" calls are used, they must respond. Ice Elves have a permanent aura on their spirit of \"Active Dark Magic\" at all times. Like Angels they are vulnerable to Psionic magic, and take x2 from Psionic damage. Exorcism effects do not affect them."},
  ],purchased:[
    {name:"Memories in Flesh",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Ice Elf",prereqs:[],desc:"Once a day an Ice Elf may recall a lesson by carving into their skin with a blade a phrase, an image, a symbol, etc., that reminds them of their lesson. Doing so takes 5 minutes of focused concentration and will return the use of any tagged (daily, hourly, etc.) character ability or skill that has been used since last reset. This ability may only be used when the Ice Elf is at full Body and will not return any skill or ability more than once per day. Using this racial ability will lower the Ice Elf to 1 Body at the end of the 5 minutes. Usable once per day per purchase."},
  ]},
  "Sidhe":{tier:"Obscure",fragCost:250,cpBonus:0,lore:"Sidhe are a race of \"pure\" fae, unlike the diluted blood of Wood Fae and Carnal Fae. Mischievous and meddling by nature, even the best intentions of a Sidhe rarely come without strings attached. Sidhe are potent spell casters tied to the sun and moon. \"Day Sidhe\" are usually optimistic, where \"Night Sidhe\" tend to be more distrustful. Life Span: 5000-6000 years. Language: Gaelic. Racial Characteristics: Long pointed ears and large horns. Contour the hairline and cheekbones in white/gold/orange/yellow for Day Sidhe or black/blue/grey/purple for Night Sidhe.",auto:[
    {name:"Formless Casting",kind:"advantage",desc:"This racial allows a Sidhe to cast Battle Magic spells without requiring a free casting hand or the need to speak. In-game the Sidhe will remain motionless and silent during casting while still correctly stating the spell's incant out of game. This racial ability functions at will for Day Sidhe between 6 AM-6 PM and for Night Sidhe between 6 PM-6 AM. To activate, a Sidhe must state \"Formless Casting\" prior to any incants."},
    {name:"Fleeting Death Count",kind:"disadvantage",desc:"Sidhe spirits on the mortal realm are weak. Sidhe have a 10 second Death Count which cannot be extended or paused in any way. During these 10 seconds the Sidhe can stand on their feet as a spirit and cast any one spell from memory. They cannot speak during this time (minus their one incant) and both feet must remain planted after they have stood up. They are completely invulnerable for this period. Only a magical Life effect will revive them. The 10 second window only exists for the Sidhe if they are in their matching time cycle."},
  ],purchased:[
    {name:"Magic Echo",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Sidhe",prereqs:[],desc:"Sidhe have the ability to \"Echo\" a spell that they have cast against a target. If their target successfully defends against a spell, the Sidhe can cause it to strike a second time in an attempt to bypass defenses. By using this racial, a Sidhe can force their opponent to defend a second time or take the effect. When the target is hit by a spell and calls an appropriate defense, the Sidhe may then call \"Innate Echo!\", causing the target to be instantly hit by the spell again. This skill cannot be used to Echo magic items. Usable once per day per purchase."},
  ]},
  "Vulcan Dwarf":{tier:"Obscure",fragCost:250,cpBonus:0,lore:"A hardy and quick-tempered race, the fire-infused Vulcan Dwarves make their home within mountains, particularly volcanoes. When the Black Dragon Styphon awoke, their subterranean kingdom was sieged by Undead and the majority of their population was enslaved. Some Vulcan Dwarves have managed to escape their volcanic home and have begun to explore the surface world. Life Span: 400-500 years. Language: Danish. Racial Characteristics: Red beards shorter than 6 inches in length, black eye sockets with black veins that spiral out from their sockets.",auto:[
    {name:"Volcanic Skin",kind:"advantage",desc:"Vulcan Dwarves have an extremely thick skin due to their acclimatization within an active volcano. The possession of this thick skin gives a Vulcan Dwarf the ability to resist any single Body damage attack, once per day, by calling \"Racial Resist\". Resisting an attack this way will also allow the Vulcan Dwarf to resist any effects that would have affected the Vulcan Dwarf if the attack was successful."},
    {name:"Crippling Vulnerability to Cold",kind:"disadvantage",desc:"Vulcan Dwarves take x4 damage from Ice. Furthermore, if a Vulcan Dwarf is dropped into their Bleed Count via an Ice attack they will explode into chunks of frozen body parts and enter their Death Count, removing the Bleed Count entirely. Only a Life spell or some other form of miracle will bring them back to life at that point. As with all racial vulnerabilities, Ice damage will bypass any thresholds a Vulcan Dwarf might have."},
  ],purchased:[
    {name:"Endure Fire",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,raceReq:"Vulcan Dwarf",prereqs:[],desc:"Vulcan dwarves have the ability to endure massive amounts of heat. Once per day per purchase a Vulcan Dwarf is able to endure elemental and magical fire for 10 minutes. During those 10 minutes they will subtract 25 damage from all sources of fire and heat to a minimum of 0. Each time this ability is purchased an additional -25 is added and an additional use is gained. This ability is activated by stating \"Racial Endure Fire\"."},
  ]},
};

// Occupation order for cost lookup: M R T N A W M D B
const OCC_ORDER = ['Mercenary','Ranger','Templar','Nightblade','Assassin','Wytchhunter','Mage','Druid','Bard'];

// Favoured Vocation cost tables — index matches SKILLS costs array order [M,R,T,N,A,W,Mg,Dr,Ba]
// Champion: Paladin, Dread Knight — uses Champion column for all skills
// Demagogue: Lightweaver, Darkweaver, Dragon Knight — uses Demagogue column
const FAVOURED_CHAMPION_COSTS = {
  // Production
  'Alchemy':90, 'Artifice':85, 'Blacksmith':75, 'Chemistry':100, 'Create Scroll':50, 'Tradesman':40, 'Trapper':85,
  // Scholar
  'Anatomy':40, 'Demonic/Angelic Arts':40, 'Elemental Attunement':25, 'First Aid':60, 'Mysticism':50,
  'Necromantic Arts':40, 'Physician':45, 'Read & Write':50, 'Read Magic':30, 'Read Magic: Advanced':50,
  'Read Magic: Ritual':50, 'Advanced Ritual Casting':275,
  // Warrior
  'Ambidexterity':40, 'Florentine':50, 'Flurry of Blows':45, 'Heavy Armour':10, 'Self Mutilate':15,
  'Shield':50, 'Slay/Parry':120, 'Slay/Parry: Master':140, 'Slay/Parry: Subsequent':120, 'Slay/Parry: Master Subsequent':140,
  'Specialization +1: Weapon Group':160, 'Specialization +1: Weapon Specific':100,
  'Weapon Group Proficiency: Medium':40, 'Weapon Group Proficiency: Large':70,
  'Weapon Specific Proficiency: Exotic':110, 'Weapon Refocus':70,
  // Rogue
  'Critical +2: Specific':140, 'Critical +2: Group':180, 'Dodge':170, 'Dodge: Additional':170,
  'Execute':170, 'Execute: Master':190, 'Execute: Subsequent':170, 'Execute: Master Subsequent':190,
  'Garrotte':140, 'Sap':55, 'Vital Blow':85,
};

const FAVOURED_DEMAGOGUE_COSTS = {
  // Production
  'Alchemy':70, 'Artifice':120, 'Blacksmith':110, 'Chemistry':80, 'Create Scroll':40, 'Tradesman':40, 'Trapper':85,
  // Scholar
  'Anatomy':40, 'Demonic/Angelic Arts':45, 'Elemental Attunement':25, 'First Aid':60, 'Mysticism':50,
  'Necromantic Arts':45, 'Physician':45, 'Read & Write':40, 'Read Magic':15, 'Read Magic: Advanced':25,
  'Read Magic: Ritual':40, 'Advanced Ritual Casting':200,
  // Warrior
  'Ambidexterity':75, 'Florentine':110, 'Flurry of Blows':100, 'Heavy Armour':65, 'Self Mutilate':15,
  'Shield':100, 'Slay/Parry':200, 'Slay/Parry: Master':220, 'Slay/Parry: Subsequent':200, 'Slay/Parry: Master Subsequent':220,
  'Specialization +1: Weapon Group':200, 'Specialization +1: Weapon Specific':180,
  'Weapon Group Proficiency: Medium':80, 'Weapon Group Proficiency: Large':130,
  'Weapon Specific Proficiency: Exotic':150, 'Weapon Refocus':40,
  // Rogue
  'Critical +2: Specific':180, 'Critical +2: Group':200, 'Dodge':200, 'Dodge: Additional':200,
  'Execute':200, 'Execute: Master':220, 'Execute: Subsequent':200, 'Execute: Master Subsequent':220,
  'Garrotte':150, 'Sap':60, 'Vital Blow':100,
};

// Spheres that cost an additional 100 frags when selected with Favoured Vocations
const FAVOURED_FRAG_SPHERES = ['Sigil','Wytchcraft','Necromancy','Dredgecraft'];

// Exclusive spheres — only accessible to specific Favoured Vocations
const EXCLUSIVE_SPHERES = {
  'Light':    ['Paladin','Lightweaver'],
  'Dark':     ['Dread Knight','Darkweaver'],
  'Draconic': ['Dragon Knight'],
};

const FAVOURED_VOCATIONS = {
  "Paladin": {
    fragCost: 250, cpCost: 50, group: 'Champion',
    exclusiveSphere: 'Light',
    prereqs: "Any occupation.",
    lore: "Where Lightweavers are the voice of the Gods, Paladins are the hand of their God in the mortal realm. To do this, they use their personal brand of holy tools. Each class ability for Paladins involves an item of power. These items may be anything the player desires, so long as it is of the type specified. The exact item should suit the God served. Upon purchasing each class ability, the item must be collected in game by the Paladin, have a value of 10 gold or more, and be Blessed by their God. The Paladin must perform a 10 minute Rite on the item, whereupon it becomes spirit-linked and indestructible. Items of power are considered created with the Light sphere and radiate Light magic. An item of power can be given to a Lightweaver of the same God, allowing the Lightweaver to use its powers for 1 hour.",
    abilities: [
      {name:"Defender",       cp:30,  tier:3,  bodyBonus:3, desc:"This ability allows the Paladin to channel the power of their God into a melee weapon or non-simple ranged weapon, known as their Defender. This will grant the effects of an item of power. Each purchase of this ability grants the Paladin +3 Body permanently. Each time this ability is purchased the Paladin may change weapons if desired. Any enchantments on the previous weapon not gained via Paladin class abilities will be lost if the weapon is switched. This class ability does not grant the weapon skill needed to use the weapon."},
      {name:"Holy Ring",      cp:60,  tier:6,  desc:"This ring grants the Paladin a magic aura for any weapon they swing with the hand the ring is on. It will also allow the Paladin to touch cast or Spellstrike a Light Bolt once per day. The call for this is \"Activate Light Bolt 20 Light\" if it is touch cast or \"Activate Spellstrike Light Bolt 20 Light\" if it is Spellstruck. This damage will be halved if the target has any active Bless spell on their person. These powers only work via the hand wearing the ring. They will work for two-handed weapons and missile weapons. Each additional purchase of this ability allows the Paladin to create a new ring with the same properties."},
      {name:"Holy Symbol",    cp:90,  tier:9,  desc:"This Holy Symbol must be the symbol of the Paladin's God. If the Paladin has purchased the Light sphere, it must be their spell focus. It cannot be the same item as their Defender. The Holy Symbol must be held or displayed to use either of its abilities.\n\nThis Symbol will grant the Paladin the ability to Power Word Directed Arcane Rebuke Undead and Demons. To use this power the Paladin must state in a loud voice \"Innate Power Word Directed Arcane Rebuke <Undead/Demon>\". The target is physically pushed away from the Paladin until it is at least 10 feet away. The target may not get closer than 10 feet away from the Paladin while the Paladin maintains concentration and holds their Holy Symbol towards the target at eye level with both hands. This ability can be used at will but it takes 1 minute of prayer to recharge for further use.\n\nThe Holy Symbol also grants the Paladin the ability to call forth a massive pillar of elemental destruction via packet attack. Upon purchase of the skill, the Paladin must select the elemental type. This selection is permanent. The call for this is \"Activate Light Holy Pillar – 20 Massive Elemental <type>\". Holy Pillar is usable once per day per purchase. Subsequent purchases may select different elemental types."},
      {name:"Headpiece",      cp:120, tier:12, desc:"To activate this ability, the Paladin must state \"Activate Headpiece\". This ability augments the other class abilities as follows for 10 minutes: (1) The Defender may swing for Elemental damage of a type of the Paladin's choosing. The Defender also grants the Paladin one Parry, but if this is used the Elemental damage ends as well. (2) The Holy Rings grant +5 damage (total, not per ring) to any weapon held in a hand wearing one. (3) The Holy Symbol's Arcane Rebuke now becomes a Destroy effect for Lesser Undead and Demons. To use this power, the Paladin must state \"In the name of <God> I destroy you, Undead/Demon! Innate Power Word Directed Arcane Destroy Undead/Demon\".\n\nThe Headpiece must be worn for the 10 minutes this ability is active. This ability is usable once per day per purchase and does not stack."},
    ]
  },
  "Dread Knight": {
    fragCost: 250, cpCost: 50, group: 'Champion',
    exclusiveSphere: 'Dark',
    prereqs: "Any occupation.",
    lore: "Where Darkweavers are the voice of the Gods, Dread Knights are the hand of their God in the mortal realm. To do this, they use their personal brand of unholy tools. Each class ability for Dread Knights involves an item of power. These items may be anything the player desires, so long as it is of the type specified. The exact item should suit the God served. Upon purchasing each class ability, the item must be collected in game by the Dread Knight, have a value of 10 gold or more, and be Blessed by their God. The Dread Knight must perform a 10 minute Rite on the item, whereupon it becomes spirit-linked and indestructible. Items of power are considered created with the Dark sphere and radiate Dark magic. An item of power can be given to a Darkweaver of the same God, allowing the Darkweaver to use its powers for 1 hour.",
    abilities: [
      {name:"Harbinger's Blade", cp:30,  tier:3,  bodyBonus:3, desc:"This ability allows the Dread Knight to channel the power of their God into a melee weapon or non-simple ranged weapon, known as their Harbinger's Blade. This will grant the effects of an item of power. Each purchase of this ability grants the Dread Knight +3 Body permanently. Each time this ability is purchased the Dread Knight may change weapons if desired. Any enchantments on the previous weapon not gained via Dread Knight class abilities will be lost if the weapon is switched. This class ability does not grant the weapon skill needed to use the weapon."},
      {name:"Unholy Ring",       cp:60,  tier:6,  desc:"This ring grants the Dread Knight a magic aura for any weapon they swing with the hand the ring is on. It will also allow the Dread Knight to touch cast or Spellstrike a Dark Bolt once per day. The call for this is \"Activate Dark Bolt 20 Dark\" if it is touch cast or \"Activate Spellstrike Dark Bolt 20 Dark\" if it is Spellstruck. This damage will be halved if the target has any active Bless spell on their person. These powers only work via the hand wearing the ring. They will work for two-handed weapons and missile weapons. Each additional purchase of this ability allows the Dread Knight to create a new ring with the same properties."},
      {name:"Unholy Symbol",     cp:90,  tier:9,  desc:"This Unholy Symbol must be the symbol of the Dread Knight's God. If the Dread Knight has purchased the Dark sphere, it must be their spell focus. It cannot be the same item as their Harbinger's Blade. The Unholy Symbol must be held or displayed to use either of its abilities.\n\nThis Symbol will grant the Dread Knight +2 Strength for one hour if they perform a Killing Blow on a creature capable of resurrection, at will. The creature must either final or resurrect for this effect to occur. The call for this is \"Innate Spirit Drain\" following the Killing Blow. The Strength bonus cannot be stacked with itself by killing multiple creatures but if it is lost it can be replaced at will.\n\nThe Unholy Symbol also grants the Dread Knight a packet delivered attack, once per day per purchase. The call for this ability is \"Activate Magic Dark Maelstrom\". Maelstrom constricts the target in black tentacles, rendering them unable to speak or move. After 10 seconds the target is hit with a Death effect. If anyone else touches the target during the 10 seconds, they will be hit with the same effect. If the target receives any numeric healing during the 10 seconds, this will remove the Maelstrom effect from them. Each purchase of this ability grants the Dread Knight another use of Maelstrom."},
      {name:"Headpiece",         cp:120, tier:12, desc:"To activate this ability, the Dread Knight must state \"Activate Headpiece\". This ability augments the other class abilities as follows for 10 minutes: (1) The Harbinger's Blade may swing for Elemental damage of a type of the Dread Knight's choosing. The Harbinger's Blade also grants the Dread Knight one Parry, but if this is used the Elemental damage ends as well. (2) The Unholy Rings grant +5 damage (total, not per ring) to any weapon held in a hand wearing one. (3) The Unholy Symbol's Spirit Drain can now stack, granting the Dread Knight +1 Strength for each creature killed after the first to a maximum of +6.\n\nThe Headpiece must be worn for the 10 minutes this ability is active. This ability is usable once per day per purchase and does not stack."},
    ]
  },
  "Lightweaver": {
    fragCost: 250, cpCost: 50, group: 'Demagogue',
    exclusiveSphere: 'Light',
    prereqs: "Any occupation.",
    lore: "Lightweavers are the voice of the Gods of Light. They create Holy Altars devoted to their God, serve as spiritual leaders, and access divine power through sacred bonds and vessels. Each Holy Altar requires a physical representation in game decorated to match the God to which it is devoted. The Altar is empowered for 5 days at a time and has 100 Body and a 10 Normal threshold once empowered.",
    abilities: [
      {name:"Holy Altar",    cp:30,  tier:3,  desc:"This ability creates a Holy Altar devoted to the creator's God. To create a Holy Altar, the Lightweaver performs a 10 minute rite devoted to their God and then states \"Innate Create Holy Altar\". This will empower the Altar with their God's power for 5 days. If a Holy Altar is moved more than 20 feet from its original location, it will lose its empowerment. Only one Holy Altar can be active at any time. Once empowered, Holy Shrines have 100 Body and a 10 Normal threshold.\n\nHoly Altars allow its creator to transfer active Blesses from their own spirit to other people or items within 20 feet by stating \"Innate Transfer\" and touching the target.\n\nAdditionally, Holy Altars create 3 vials of holy water each day per purchase. Once removed from the Altar, they last for 1 hour. The vials may: (1) function as a light source (repped by a green, yellow or red glow stick or LED light); (2) be thrown at an Undead or demon to inflict 10 Alchemical Acid (packet delivered); or (3) be consumed to grant the consumer a Bless of the Lightweaver's God lasting 5 days."},
      {name:"Sacred Bond",   cp:60,  tier:6,  desc:"Sacred Bond links the Lightweaver to their Holy Altar from a distance. Each of the two abilities may be used once per day per purchase: (1) The Lightweaver may grant 15 Mending to any target. The call is \"Innate Arcane 15 Mend\". It may be touch cast or packet delivered. (2) The Lightweaver may activate magical items with \"per day\" or \"ever\" charges left on the Altar as if they were in possession of it, via a 10 minute RP Rite. This works within 1 km of the Altar. Sacred Bond cannot be used with items which have Dark or Draconic magic. Only one Sacred Bond may be active per purchase."},
      {name:"Sacred Vessel", cp:90,  tier:9,  desc:"This ability allows the Lightweaver to perform a 1 minute Rite to create a Sacred Vessel for their Holy Altar. These Vessels can store Battle Magic spells (up to level 7) while they remain on the Altar. Spells may be from any core rulebook sphere or the Light sphere. Spells cast by the Lightweaver will not be lost from memory, but spells cast by others will. After absorbing a spell, the Vessel requires 1 hour to attune. The Sacred Vessel itself may only be used by the Lightweaver. Stored spells are used by stating \"Activate Vessel: <Spell Name>\". Each Sacred Vessel can store a single spell castable infinite times by the Lightweaver within 20 feet of the Altar. After the first use, each subsequent use must consume a blessed catalyst. A Sacred Vessel will last for 5 days. One Sacred Vessel may exist per purchase of this ability."},
      {name:"Church",        cp:120, tier:12, desc:"At the 12th level, the Lightweaver may construct a truly Holy Church devoted to their God, pray for 10 minutes and then state \"Innate Create Church\" to activate it. The Church is a 20 foot square centered around the Holy Altar and must be properly phys-repped with excellent props.\n\nThe Holy Altar is now indestructible but its duration remains the same. The Church may be destroyed by physically removing or destroying the majority of the holy items, trappings, and vestments. Once per event, a Lightweaver casting a ritual within their Church may re-pull a stone when determining the success of the ritual. The Lightweaver may decide whether the area inside Church is considered day or night at all times via a 10 minute Rite involving candles.\n\nIf a person within the Church has a Light Bless of any God and they are struck by a Dark or Draconic spell, the Bless will act as a Shield Magic and be expended. If the Lightweaver is struck by a Dark or Draconic spell and they have a Bless, it will function like a Reflect Magic and be expended. Sacred Vessels from other Lightweavers may be created on the Holy Altar and will only function for the owner of the Church."},
    ]
  },
  "Darkweaver": {
    fragCost: 250, cpCost: 50, group: 'Demagogue',
    exclusiveSphere: 'Dark',
    prereqs: "Any occupation.",
    lore: "Darkweavers are the voice of the Gods of Darkness. They create Unholy Altars devoted to their God, serve as spiritual leaders, and access unholy power through sacred bonds and vessels. Each Unholy Altar requires a physical representation in game decorated to match the God to which it is devoted. The Altar is empowered for 5 days at a time and has 100 Body and a 10 Normal threshold once empowered.",
    abilities: [
      {name:"Unholy Altar",  cp:30,  tier:3,  desc:"This ability creates an Unholy Altar devoted to the creator's God. To create an Unholy Altar, the Darkweaver performs a 10 minute rite devoted to their God and then states \"Innate Create Unholy Altar\". This will empower the Altar with their God's power for 5 days. If an Unholy Altar is moved more than 20 feet from its original location, it will lose its empowerment. Only one Unholy Altar can be active at any time. Once empowered, Unholy Shrines have 100 Body and a 10 Normal threshold.\n\nUnholy Altars allow its creator to transfer active Blesses from their own spirit to other people or items within 20 feet by stating \"Innate Transfer\" and touching the target.\n\nAdditionally, Unholy Altars create 3 vials of unholy blood each day per purchase. Once removed from the Altar, they last for 1 hour. The vials may: (1) function as a light source (repped by a green, yellow or red glow stick or LED light); (2) be thrown at a target to cause 10 seconds of Alchemical Blindness (packet delivered); or (3) be consumed to grant the consumer a Bless of the Darkweaver's God lasting 5 days."},
      {name:"Sacred Bond",   cp:60,  tier:6,  desc:"Sacred Bond links the Darkweaver to their Unholy Altar from a distance. Each of the two abilities may be used once per day per purchase: (1) The Darkweaver may grant 15 Mending to any target. The call is \"Innate Arcane 15 Mend\". It may be touch cast or packet delivered. (2) The Darkweaver may activate magical items with \"per day\" or \"ever\" charges left on the Altar as if they were in possession of it, via a 10 minute RP Rite. This works within 1 km of the Altar. Sacred Bond cannot be used with items which have Light or Draconic magic. Only one Sacred Bond may be active per purchase."},
      {name:"Sacred Vessel", cp:90,  tier:9,  desc:"This ability allows the Darkweaver to perform a 1 minute Rite to create a Sacred Vessel for their Unholy Altar. These Vessels can store Battle Magic spells (up to level 7) while they remain on the Altar. Spells may be from any core rulebook sphere or the Dark sphere. Spells cast by the Darkweaver will not be lost from memory, but spells cast by others will. After absorbing a spell, the Vessel requires 1 hour to attune. The Sacred Vessel itself may only be used by the Darkweaver. Stored spells are used by stating \"Activate Vessel: <Spell Name>\". Each Sacred Vessel can store a single spell castable infinite times by the Darkweaver within 20 feet of the Altar. After the first use, each subsequent use must consume a blessed catalyst. A Sacred Vessel will last for 5 days. One Sacred Vessel may exist per purchase of this ability."},
      {name:"Church",        cp:120, tier:12, desc:"At the 12th level, the Darkweaver may construct a truly Unholy Church devoted to their God, pray for 10 minutes and then state \"Innate Create Church\" to activate it. The Church is a 20 foot square centered around the Unholy Altar and must be properly phys-repped with excellent props.\n\nThe Unholy Altar is now indestructible but its duration remains the same. The Church may be destroyed by physically removing or destroying the majority of the unholy items, trappings, and vestments. Once per event, a Darkweaver casting a ritual within their Church may re-pull a stone when determining the success of the ritual. The Darkweaver may decide whether the area inside Church is considered day or night at all times via a 10 minute Rite involving candles.\n\nIf a person within the Church has a Dark Bless of any God and they are struck by a Light or Draconic spell, the Bless will act as a Shield Magic and be expended. If the Darkweaver is struck by a Light or Draconic spell and they have a Bless, it will function like a Reflect Magic and be expended. Sacred Vessels from other Darkweavers may be created on the Unholy Altar and will only function for the owner of the Church."},
    ]
  },
  "Dragon Knight": {
    fragCost: 250, cpCost: 50, group: 'Demagogue',
    exclusiveSphere: 'Draconic',
    prereqs: "Any occupation.",
    lore: "Dragon Knights are devoted servants of the great Dragons of Maud'madir. They create Draconic Shrines devoted to their patron Dragon and access draconic power through covenants and troves. Each Draconic Shrine requires a physical representation in game decorated to match the Dragon to which it is devoted. The Shrine is empowered for 5 days at a time and has 100 Body and a 10 Normal threshold once empowered.",
    abilities: [
      {name:"Draconic Shrine",    cp:30,  tier:3,  desc:"This ability creates a Draconic Shrine devoted to the creator's Dragon. To create a Draconic Shrine, the Dragon Knight performs a 10 minute rite devoted to their Dragon and then states \"Innate Create Draconic Shrine\". This will empower the Shrine with their Dragon's power for 5 days. If a Draconic Shrine is moved more than 20 feet from its original location, it will lose its empowerment. Only one Draconic Shrine can be active at any time. Once empowered, Draconic Shrines have 100 Body and a 10 Normal threshold.\n\nDraconic Shrines allow its creator to transfer active Dragon Marks from their own spirit to other people or items within 20 feet by stating \"Innate Transfer\" and touching the target.\n\nAdditionally, Draconic Shrines create 3 vials of ink the colour of the Dragon Knight's Dragon each day per purchase. Once removed from the Shrine, they last for 1 hour. The vials may: (1) function as a light source; (2) be applied to the target's skin to grant a +2 threshold of whatever type the target already has for 1 hour (if no threshold, they receive a 2 Normal threshold); or (3) be consumed to grant the consumer a Dragon Mark of the Dragon Knight's Dragon lasting 5 days."},
      {name:"Draconic Covenant", cp:60,  tier:6,  desc:"Draconic Covenant links the Dragon Knight to their Draconic Shrine from a distance. Each of the two abilities may be used once per day per purchase: (1) A Dragon Knight can corrupt and use Divine magic items brought to their Shrine via a 10 minute Rite stating \"Innate Divine Corruption!\". The item is destroyed and its abilities — now corrupted — are absorbed by the Dragon Knight. All times-per-day charges become times-ever; all continuous powers become 1 hour. The absorbed powers last 5 days. (2) A banner with the symbol or colour of the Dragon Knight's patron Dragon may be activated for one hour. Anyone with a Dragon Mark of the same Dragon will receive a magic aura on their weapon swings while within line of sight of the banner, up to 100 feet."},
      {name:"Draconic Trove",    cp:90,  tier:9,  desc:"This ability allows the Dragon Knight to perform a 1 minute Rite to create a Draconic Trove for their Draconic Shrine. These Troves can store Battle Magic spells (up to level 7) while they remain on the Altar. Spells may be from any core rulebook sphere or the Draconic sphere. Each Draconic Trove can store three spells at once, cast within 1 minute of each other. Once stored, anyone with a Dragon Mark of the Trove's creator's Dragon, or any Dragon Knight, may access the stored spells. A Draconic Trove will last for 5 days. One Draconic Trove may exist per purchase of this ability."},
      {name:"Temple",            cp:120, tier:12, desc:"At the 12th level, the Dragon Knight may construct a truly magnificent Temple devoted to their Dragon, meditate for 10 minutes and then state \"Innate Create Temple\" to activate it. The Temple is a 20 foot square centered around the Draconic Shrine and must be properly phys-repped with excellent props.\n\nThe Draconic Shrine is now indestructible but its duration remains the same. The Temple may be destroyed by physically removing or destroying the majority of the items, trappings, and vestments. Once per event, a Dragon Knight casting a ritual within their Temple may re-pull a stone when determining the success of the ritual. The Dragon Knight may decide whether the area inside Temple is considered day or night at all times via a 10 minute Rite involving candles.\n\nIf a person within the Temple has a Dragon Mark of any Dragon and they are struck by a Dark or Light spell, the Dragon Mark will act as a Shield Magic and be expended. If the Dragon Knight is struck by a Dark or Light spell and they have a Dragon Mark, it will function like a Reflect Magic and be expended. Draconic Troves from other Dragon Knights may be created on the Draconic Shrine and will only function for the owner of the Temple."},
    ]
  },
};

function isFavouredVocation(vocName){ return !!FAVOURED_VOCATIONS[vocName]; }
function getFavouredVocationData(){ return s.vocation ? FAVOURED_VOCATIONS[s.vocation] : null; }
function getFavouredCostTable(){
  const fv = getFavouredVocationData();
  if(!fv) return null;
  return fv.group === 'Champion' ? FAVOURED_CHAMPION_COSTS : FAVOURED_DEMAGOGUE_COSTS;
}



const CULTURES = {
  "Taliss Pride": {
    races: ["Savar'Aving"],
    lore: "The Taliss Pride are a pride of guerilla warriors from Felnir tasked during the necromantic plague to combat not just the undead but the sources of necromancy, especially Malagant and his minions, functioning similar to traditional wytch hunters. Originally hunting exclusively within Felnir's forests, they have now spread beyond it. The Taliss Pride seek out churches of Malagant or other powerful necromancers with an intent to destroy any source of undeath without hesitation or mercy. Sometimes they are forced to operate outside the law and they will not hesitate to do so.",
    indoctrination: "If invited to petition, a Savar'Aving is given a special brew to drink once a month for a year which slowly infuses their claws with magic, allowing them to better combat the undead. This is a long process and the magical effect will not be strong enough to make a discernible difference until the final, most potent brew is offered. During the year, the initiate is expected to fight and destroy undead using a variety of tactics. The bigger the kill, the more dangerous the mission, the more Taliss will be impressed. The Taliss also value stealth, ambushes and similar tactics. If accepted, a Savar'Aving's claws will become permanently magical against undead and the brew is no longer required.",
    racialCharacteristicAddition: "A noticeable snow-white streak of fur, at least 6 inches long, either on the face or starting on the face and moving into the hairline. If the fur pattern naturally included streaks, the Taliss streak should replace one of them.",
    purchased: [
      {name:"Redeemer's Claws",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"A Taliss Pride member's Claws always swing for +0 Magic damage against Undead (identified via Necromantic Arts or witnessed taking damage from Healing). If they already swing for Magic damage, they swing for +1 additional damage. This ability is always on but does not stack.\n\nOnce per day per purchase, if a Taliss Savar takes Infliction damage from an Undead (identified as above), they may call \"Innate Redeemer's Claws\" to seal the Infliction in their Claws for a time. For one minute they do not take the damage or any effect from the attack. If the Undead who delivered the attack is reduced to 0 Body before the end of the minute, the delayed Infliction is harmlessly released without touching the Taliss's spirit. If not, the Taliss takes the full effect after the minute ends. Only one Infliction attack may be delayed at a time."},
    ]
  },
  "Granite Sentries": {
    races: ["Gargylen"],
    lore: "After the Duesworn Fellowship joined the Amaranthian Legion and began building permanent fortifications, Gargylen smiths were tasked with ensuring their guards were as fortified as possible to defend their new homeland. They created the highest quality armor they could to improve protection, but wondered: could the armor be used to augment the Gargylen themselves? Although the process was difficult and dangerous, the Gargylen smiths developed a method of grafting increasingly stronger pieces of armor onto their test subjects with the help of Mountain Dwarven smiths and the knowledge of lesser Gargylen physiology carried by the Forgeborn. Coupled with intense training, these new augmentations allowed the bearers to maintain a permanent form of their previously temporary Stone Skin abilities. Those with the most powerful augments and grueling training regimens even began to shrug off certain types of attacks altogether. Unfortunately, this newly fortified form left the Granite Sentries permanently vulnerable to magics that dealt damage directly to the Body.",
    indoctrination: "While any Gargylen can become a Granite Sentry, they must first gain the approval of a Forgeborn smith trained in the augmentation process. Assuming the Forgeborn agrees, the Gargylen must prove their fortitude by withstanding each of the excruciating and lengthy augmentation sessions, while awake with their Stone Skin active. The process takes a year to complete. Every two months, the grandmaster smith will graft new pieces of armor into the Gargylen's layers of Stone Skin. The armor used as material components must be provided by the Gargylen subject. No more than one step can be completed every two months as the changes must be given time to heal, and the Gargylen must train to effectively utilize their new augmentations.\n\nThe first step requires a set of leather armor tags worth at least 50 Armour Points. The second step requires a set of chainmail armor tags worth at least 75 Armour Points. The third step requires a set of plate armor tags worth at least 100 Armour Points. The fourth step requires a Master Crafted metal shield. The fifth and final step requires Legendary armour tags worth at least 25 Armour Points (excluding the +1/zone bonus granted by Legendary status) that have an active Blueprint applied. All five sets of armour are required even if the Gargylen never advances their Granite Skin to the full extent.",
    racialCharacteristicAddition: "Any exposed skin must have granite-like flecks of black and white.",
    purchased: [
      {name:"Granite Skin",maxPurchases:5,bodyBonus:5,strBonus:0,prereqs:[],desc:"The Gargylen gains +5 permanent Body points but suffers double damage from all spells that damage the Body. The amount of permanent Body points gained can be increased with additional purchases. With two purchases, the total permanent Body points gained increases to +10; three purchases increases the total permanent Body points gained to +15 and grants a +5 Normal threshold; four purchases increases the total permanent Body points gained to +20; and finally, five purchases increases the total permanent Body points gained to +25 and grants a +0 Silver threshold."},
    ]
  },
  "Clan Icebreaker": {
    races: ["Mountain Dwarf"],
    lore: "A small clan from the frigid ice floes south of the Walking Sea, these hearty Dwarves sometimes travel south in search of adventure. While they originally stayed in the area due to the rich marble veins found in the islands, they've grown fond of the challenges and isolation. To help them survive in their inhospitable climate they commonly chew the leaf of the Rockbud plant which permanently damages their vitality but enables them to withstand the extreme cold. They dwell underground in sheltered cave systems near the shoreline and come up to fish and hunt. They have a reputation for disliking long conversations and being extremely close-knit.",
    indoctrination: "Elders of Clan Icebreaker prefer isolation, so finding one to mentor under can be difficult, though not impossible. Once an Elder is found, they may be convinced to teach their ways by means of up to a year's service. The applicant will be tasked to bring them the hearts of three Rimesnapper lobsters. Rimesnapper lobsters feed on Rockbud plants, which are a type of seaweed that grows on the shores of the colder regions of the Elemental plane of Ice. A secret Icebreaker recipe brews Rimesnapper hearts into a tea which transforms a Mountain Dwarf's famous vitality into a means of summoning frost over their weaponry. The applicant Dwarf will be given a special fishing lure by the Elder and told to find a pond. When the lure enters the water, the water will begin to freeze. After 30 minutes the water will be frozen over completely and open a rift to the plane of Ice near a Rimesnapper fish, which will be drawn through the rift, into the material plane. The Dwarf (and friends) must fight the horse-sized, aggressive lobster, which uses Elemental Ice and its massive claws to defend itself. Once three hearts are collected in this manner, they may be returned to the Elder and brewed into tea.",
    racialCharacteristicAddition: "Light blue around the eyes and white streaks in the beard.",
    purchased: [
      {name:"Ice Blade",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"By stating \"Innate Ice Blade\", a Clan Icebreaker Dwarf can summon elemental ice to cover their weapon. This mimics the effect of Greater Elemental Blade, adding +5 damage in addition to the weapon's normal damage and changing the damage type to \"Magic Ice\" against one specific target. This effect will remain on the target's spirit until they change targets, go more than one minute without attacking, or they or their target are no longer conscious. This ability can stack with the spell \"Elemental Blade\". This ability is useable once per day per purchase."},
    ]
  },
  "House Mortuus": {
    races: ["Dark Elf"],
    lore: "Darkness rules within Antioch, both literally and figuratively. But even in a city famous for wickedness being a way of life, there is one noble house whose presence can intimidate even clerics of Raze – House Mortuus. Less a true noble house and more of mage's guild which studies necromancy and undeath exclusively, they have nonetheless been given noble status within the Dark Elven capital. Initiation to the House is open to any Dark Elf who desires it, no matter who they might serve in body or spirit, so long as they are driven to furthering the study of necromancy. On rare occasions, even non-magi are welcomed into the fold.",
    indoctrination: "Although House Mortuus is based out of Antioch, its members do not need to live there. House Mortuus is in constant need of agents in the field, performing experiments, collecting magic items and watching over initiates who seek to join the House. If a Dark Elf shows promise they may be invited to join. During the year, the petitioner will be expected to collect knowledge and lore specific to necromancy, donate necromantic magic items, catalysts, ritual scrolls and similar, as well as show promise as a necromancer themselves or assist those who are. This is a cutthroat process, and it would not be frowned upon for one petitioner to outright murder a competitor. Once finally accepted into the House an elaborate necromantic ritual is cast on the petitioner by members of House Mortuus, which permanently changes their biology and makes them naturally capable of controlling necromantic energies.",
    racialCharacteristicAddition: "Purple veins instead of black.",
    purchased: [
      {name:"Death Clad",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"Masters of undeath, members of House Mortuus can clothe themselves in necromantic energies that would mutilate anyone else. When a House Mortuus Dark Elf takes Infliction damage, they can state \"Innate Death Clad\", taking no damage and instead gaining Magical armour equal to twice the Infliction they would have taken. Eg: If the Dark Elf is hit by a spell that deals 10 Infliction, they would instead gain +20 Magical armour. This armour cannot be refit and is removed before physical armour. It can stack with other sources of Magical armour but not itself. While the Dark Elf has any amount of Magical armour from this ability, Lesser Undead will ignore them so long as the Dark Elf takes no hostile action against them. They should state \"Innate Undead Affinity\" when passing Undead to indicate this. The Magical armour lasts for 1 hour or until destroyed. This ability is usable once per day per purchase."},
    ]
  },
  "Domaine Magique": {
    races: ["High Elf"],
    lore: "Prior to the destruction of Suvant, the elvish kingdom contained a small but well-respected mage's guild. After Suvant's fall, some of the mages who were outside of the city during its fall chose to rebuild within Day'ten but many others have chosen to travel the world, teaching what they know to other High Elves and to continue their own pursuit of magical knowledge. Given the High Elves' natural affinity for magic, only they may learn the Ritual Affinity of the Domaine Magique.",
    indoctrination: "Joining the Domaine Magique is a straightforward process and one which should be familiar to most magi. First, one must petition a current member and offer to become their apprentice. Members of the Domaine Magique will not simply train anyone who requests it. An applicant must prove that they possess not only great potential as a student but will also be a valuable asset to their mentor as they pursue their own studies. The prospective student will be expected to assist their mentor when needed and, once a month for one year, they must also demonstrate their skill in ritual magic at a level of difficulty which pushes their ability to its maximum. Sometimes this test will be to the benefit of their mentor in their own field of study and quite often it will be a dangerous endeavour. After a year of apprenticeship, if the mentor deems the student worthy, a ritual will be cast upon them, twisting their natural defence against psionics into a similar defence for ritual magic.",
    racialCharacteristicAddition: "Milky white fingernails and lips.",
    purchased: [
      {name:"Ritual Affinity",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"Once per day per purchase, the user can perform one of three abilities: Resist the effects of a ritual flaw against themselves (but not backlash); Gain an extra ritual spell slot that can be used solely to act as a secondary caster in a ritual; Decrease the effective level of a ritual which they are casting (primary or secondary) by 1, as long as at least one other High Elf is participating and the ritual is level 9 or above (this cannot stack).\n\nThe user may take advantage of the second ability even if they do not have any ritual slots of their own but must be able to read rituals and cast a sphere of magic."},
    ]
  },
  "Kraken": {
    races: ["Wild Elf"],
    lore: "Though they call themselves the Storto di Coa in their native tongue, these isolationist, sea-bound wild elves are more commonly known as the Kraken tribe to outsiders. Living upon a fleet of ancient, living wooden ships grown with powerful nature magic, they primarily serve as guardians and caretakers of sacred aquatic spaces. As prideful and prejudiced against land-dwellers as they are, occasionally an outsider proves themselves worthy of joining them in their venerable duty.",
    indoctrination: "Joining the Kraken tribe is difficult. They do not look kindly upon most outsiders and their trust must be earned through service. A prospective Kraken must forswear all loyalty to their old tribe, and they must serve as an agent of the Kraken tribe for many months prior to joining. Though the Kraken see the land as spiritually barren at best, they recognize that ignoring both it and the peoples that live upon it would be foolish. Thus, these agents serve as extensions of their will. At the direction of a proper Kraken they gather intelligence, eliminate threats, conduct trade, and so on. Once their sponsor believes they have proven themselves, the prospective Wild Elf is invited to join the tribe. They are fed a draught of enchanted saltwater drawn from Coa's Cove. This powerful drink forever changes their physiology, altering their ears to grant them a superb sense of balance as their limbs flow like water.",
    racialCharacteristicAddition: "\"Webbed\", serrated ears.",
    purchased: [
      {name:"Freedom of Movement",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"This ability grants the user Freedom of Movement for 1 minute, stating \"Racial Freedom of Movement\". This makes the user immune to any binding effect that would physically constrict them, any effect that would stun them, and any effect that would slow their movement in any manner that is not a Mind Altering effect or being knocked unconscious. This includes effects, such as Stun, Swampwalk, Snare, Bind, Web, Black Plague, Tread Water, etc., but not effects like Sap or Repel. The Kraken would call \"No Effect\" to any such effect. This ability is usable once per day per purchase."},
    ]
  },
  "House of Séasúir": {
    races: ["Wood Fae"],
    lore: "The House of Séasúir (Seasons) have become disenchanted with their chaotic, free-living kin. They have instead devoted themselves to the True Fae seasonal Courts, hoping to trade in their carefree upbringing for one of order, structure and servitude. The House of Séasúir is an organisation that serves the noble houses of the True Fae in whatever capacity is needed. The first step is to join the House of Séasúir, and to swear loyalty to the True Fae Courts in an elaborate ceremony involving Fae magic.",
    indoctrination: "To join House of Séasúir a Wood Fae must find and petition a True Fae noble house to sponsor them, through gifts or service. Gifts must be considered valuable to the True Fae they are attempting to impress, either due to craftsmanship or worth. The nature of the personal service greatly depends on the True Fae being petitioned and should not be taken lightly. Acts betraying one's friends and family or involving dangerous situations are not uncommon – the Fae do not trust lightly and test their would-be allies accordingly. This application period typically lasts for one year and in the end the Wood Fae may simply be thanked and never hear from the True Fae again… but if they've truly impressed a True Fae, the benefits may last a lifetime.",
    racialCharacteristicAddition: "Colourful swirling \"Fae style\" marks on the face and neck, typically matching the personality of the True Fae who sponsored them.",
    purchased: [
      {name:"Blessing of the Queen",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"To use this ability the Wood Fae must mark two locations as being \"Fae Touched\". This can be done by adding flowers, tying colourful ribbons or similar methods personal to their Fae sponsor. This ceremony must be roleplayed for 5 minutes at each location and the Wood Fae must not leave the areas during this time. The ceremony for the second location must occur within 1 hour of the first ceremony. Once completed, once per day per purchase, they may enter one of the two locations, touch the center and be transported to the other location on a 5 count. The time it takes to be transported to the other location is the time it takes the player to walk to that location. This ability will allow for passage through Nature-based barriers, such as Henges, but not other magical barriers such as Vaults. The two locations cannot be farther than 3 miles apart. The Wood Fae may take one \"passenger\" along with them so long as they are willing and an additional usage of Blessing of the Queen is expended. If the physical items marking the location are destroyed, the location will no longer work. Only one pair of locations may be created per day and to change either location, both must be redone."},
    ]
  },
  "Ebon Khan": {
    races: ["Orc"],
    lore: "The specifics of the arcane rites that created the newborn Ebon Khan Orcs of Amarinthia are kept closely guarded by the Den Mothers and their Hivefather Scissa Manyeyes. These fearsome Orcs took on the traits of Brood, to better combat their encroachment upon Orcish territory. After the Ebon Khan lost their localised hive mind upon the death of the Brood Matriarch dragon Ta-Ba-Ret, they gained a new appreciation for the individuality of the sisters and brothers that helped them during the Amarinthian War. As such, the Hivefather revealed an unprecedented secret: a rite to imbue Orcs with Brood essence even after they have come of age. While still macabre to some and lacking the true abilities of an Ebon Khan, the Hivefather's gift has been offered to many Orcs seeking a taste of their strange power.",
    indoctrination: "Once an Orc finds the Ebon Khan and asks to join, they will be questioned at length about their motivations. If accepted, they must hunt down as many Brood as possible. Each Brood must be captured alive and its chitin must be surgically removed, then brought back to their Ebon Khan mentor, who will typically grant an audience once per month. The hunt should start with a regular Brood and increase in danger to more powerful ones, finishing with a Tanker Brood. After each successful hunt, the Orc will be given an acid-soaked piece of Brood flesh to consume and they will be trained a little more. If their training is deemed successful at the end of the year, a ceremony will be performed by three Ebon Khan members involving Brood Oil, which can only be obtained from Brood Queens. The oil will be mixed into a chitin cocoon made from the pieces the Ebon Khan has obtained throughout the year, to simulate how true Ebon Khan are made at birth. The Orc steps inside the acid- and oiled-soaked cocoon, burning and changing them.",
    racialCharacteristicAddition: "Blood coloured mandible-shaped scars around lower mouth and chin, or scars around the face resembling eyes.",
    purchased: [
      {name:"Brood Constitution",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"While the Orc is above half their normal Body points (rounded down), they will Minimize Acid damage they receive. While they are at or below half their normal Body points, they can use their blood to coat their own weapon in an acidic solution on a 5 count, stating, \"Acid Coating 1, Acid Coating 2, etc.\" After doing this, the next swing they make within the next 5 minutes will do +0 Acid damage. This can be done once per minute and does not stack with itself. If they are interrupted while coating their weapon, they must wait a minute before trying again. Only the Ebon Khan Orc themself can benefit from this.\n\nEbon Khan may communicate telepathically with other Ebon Khan or creatures with the Hivemind ability at will, as long as they are within arm's length. This is represented by quietly speaking to the target OOG, who can respond in the same manner."},
    ]
  },
  "Clan Vinatore": {
    races: ["Ajaunti"],
    lore: "Clan Vinatore are a reclusive clan, travelling in pursuit of spirits needing to be put to rest or hiring themselves out to rich nobles with haunted property. Members of this clan consider doing this a mercy as they believe these spirits are trapped in this realm, unable to go to the afterlife. This does not mean that the Clan Vinatore underestimates the danger of these spirits – they come prepared. The Vinatore have dedicated themselves to aiding their ancestors and combating Haldora's influence in the Deadlands.",
    indoctrination: "Joining this clan involves performing a monthly séance, led by the Ajaunti's NPC mentor, for a year in which the Ajaunti physically travels into the Deadlands to briefly speak to an ancestor and help them in some way. The more ancestors helped, the more likely an Ajaunti will be accepted into Clan Vinatore. If their training has been completed and deemed a success, a final séance will be performed. In it, they will be visited by their ancestors, who will mark new member's cheek with the names of the ancestors they helped, as a reminder of those who have laid the foundation for the Ajaunti before them, and the eventual destination for all Ajaunti that are alive today.",
    racialCharacteristicAddition: "Flowing black script written on the cheek under the cheekbones that describes some ancestors and their names.",
    purchased: [
      {name:"Spirit Hook",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"The Ajaunti may throw a packet and declare \"Innate Arcane Spirit Hook\". If it strikes a target that is an Ethereal Undead, they will be affected by an Arcane Web effect that immobilizes them from the neck down. Creatures trapped this way are unable to do anything except talking, reading, and skills that require no movement. Trapped creatures may also activate Magical items if the items are touching them, though few items would be beneficial, for the victim cannot use their hands to direct the activated item by throwing packets. Creatures with a Strength bonus of +6 may rip free from the web, taking three seconds and doing 6 Body in the process regardless of threshold. Otherwise, they may be cut out which takes 6 minutes of time to completely remove the sticky strands. Webbed creatures cannot be moved. This effect lasts as long as the Ajaunti has line of sight of the Undead.\n\nIf used on a ghost whose spirit is trapped in the Deadlands, this ability will function as a binding circle and force it to remain in place. This does not give the Ajaunti control over the creature but it does prevents its escape. Once a creature is successfully struck with the packet, a 5-foot diameter circle of salt and ash will appear centered around the ghost. The Ajaunti can keep the ghost in the circle indefinitely until it is put to rest or the circle is destroyed. The ghost can converse through the circle, assuming anyone has the ability to understand it. Should the circle be crossed or breached by anything or anyone, the effect will end immediately and the ghost trapped inside will be freed. The Ajaunti may choose to drop the circle at any time. The circle perimeter must be represented by a rope or a similarly identifying prop.\n\nThis ability has no impact on people who are possessed by ghosts. This ability is usable once per day per purchase."},
    ]
  },
  "True Berserker": {
    races: ["Einher"],
    lore: "Many Einher can conjure up an inner controlled rage which makes them truly fearsome in battle, but some Einher go further. These Einher embrace tradition and spirituality and make that strength a lifestyle of its own. Most holy to a True Berserker is their Mantle: a realistic wolf or bear headpiece which has internal hooks and spikes that dig into the Einher's flesh when worn. The Mantle represents the Berserker offering themselves to the wolf or bear spirit, inviting them to possess their body for the battle. While the Mantle is not strictly necessary to use their Berserker Poison, it is considered incredibly important. A lost or destroyed Mantle can be replaced with minimal effort so long as the Berserker has access to another full bear or wolf skin.",
    indoctrination: "To become a True Berserker, an Einher must first meet and convince an existing True Berserker to tutor them. If accepted, this mentorship begins with the Einher making a short pilgrimage to an isolated location in the wilderness. There they will remain for a week, meditating and consuming hallucinogenic mushrooms. The purpose of this spiritual journey is to form a bond with either the wolf or bear, which will become the base of their Mantle. If successful they will return to their mentor where they will be given ten tasks over the course of a year. These tasks will be tests of strength, endurance and hardship. The final test will involve hunting a bear or wolf, the more fearsome the better, with no armour and only simple weapons. Not every test need be successful – sometimes the greatest lessons are taught in failure – but the Einher must show resolve and succeed at the final test, as the Berserker's Mantle will be made from that final kill.",
    racialCharacteristicAddition: "Pictish-style war paint covering any exposed flesh.",
    purchased: [
      {name:"Berserker Poison",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"The Einher may brew an \"Ingested Alchemical Berserker Poison\" that lasts until reset. This brew takes 10 minutes to make and is made from bodily fluids, local fungi and water from a source that is spiritually significant to the character. Unlike regular ingested alchemy, the brew cannot be mixed with any other food or drink. This brew can be ingested or poured over the Berserker's Mantle, where the liquid will drip into the hooks that are lodged in the True Berserker's skin. When a True Berserker drinks this brew, they will go in a Berserk state in which they are immune to fear effects and gain 1 AP for any unarmoured armour location. This armour cannot be repaired. They will also gain +1 Strength. The Strength and AP increase by 1 when the character purchases the skill four, seven and ten times. While in their Berserk state, the Einher must try to kill anyone who they consider an opponent, and anyone who gets in their way, friend or foe. If there are no opponents remaining, they will perform a Killing Blow on any unconscious opponents to ensure that they are dead. At the end of a fight, it takes 5 minutes for the effects of Berserk to wear off. The character cannot end the rage sooner and must continue to fight so long as opponents are visible, even if they are cleansed of the Berserker Poison itself. Afterwards, no skills or abilities may be used for the same length of time that they were Berserking, to a minimum of 10 minutes. If anyone but a True Berserker drinks this brew, they will take an Alchemical Enrage effect for 60 seconds, causing them to attack the first person they see. They will not gain any of the other effects. This ability is useable once per day per purchase. This ability does not stack."},
    ]
  },
  "Five Sons Bakery": {
    races: ["Hobling"],
    lore: "It is a poorly kept secret that this famous Berphauntian bakery is a front for a business that supplies poisons and alchemy to the world's assassins. Their products are frequently used to deliver vials, but as they are also genuinely fabulous bakers, they also create such wonders as a poisoned bread which cannot be detected by normal means, known as \"the Humble Loaf\". Five Sons will only hire Hoblings due to their racial ability to develop an immunity to this undetectable poison and they must be initiated via consuming a toxin which grants it. Unfortunately, this immunity permanently alters the Hobling's nervous system, impairing their natural ability to move quickly.",
    indoctrination: "To become a \"baker\" at Five Sons, the Hobling must gain their attention by showing their skill as an alchemist or chemist. This will lead to being offered a franchise of the bakery. The process takes a year, mostly because the hopeful baker must consume a vial of toxin once a month and build up their immunity to the poison of the Humble Loaf. This is very much a business arrangement; the prospective baker must create orders sent to them by Five Son's (and may earn a profit by doing so) and are encouraged to set up their own shop.",
    racialCharacteristicAddition: "Consuming the toxin when joining the bakery causes a permanent purple discolouration around the mouth and lips.",
    purchased: [
      {name:"Adapted Insides",maxPurchases:DEFAULT_MAX,bodyBonus:0,strBonus:0,prereqs:[],desc:"The same numbing of the Hobling's nerves that causes their natural quickness to slow also causes a resilience to dangerous substances. A Hobling with Adapted Insides is highly resistant to all forms of alchemy, including ingested or beneficial alchemies, excluding acid and chemistry. The first time they are hit with alchemy in a day, they resist the effect and their resistance disappears for 1 second. The second time, their resistance disappears for 10 seconds. The third time removes it for 1 minute. The fourth time removes it for 10 minutes. Each subsequent time removes it for 1 hour. The refractory period resets during the daily skill reset. Once per day per purchase they may fully resist a single acid or chemistry effect, which does not trigger a refractory period."},
    ]
  },
};

// Get CP cost for a skill given current occupation (or Favoured Vocation cost table)
function getSkillCost(sk){
  if(sk._racial) return RACIAL_CP;
  if(!sk.costs) return sk.cp || 0; // fixed CP (frag-only skills, occ abilities, etc.)
  // Favoured Vocation overrides all skill costs with its own table
  const favTable = getFavouredCostTable();
  if(favTable && favTable[sk.name] !== undefined) return favTable[sk.name];
  const idx = OCC_ORDER.indexOf(s.occupation);
  if(idx === -1) return sk.costs[0];
  return sk.costs[idx];
}

// Helper to build a skill object with per-occupation costs
// costs array order: M R T N A W M D B
function skill(name, costs, prereqs, opts){
  return {
    name,
    costs, // [M,R,T,N,A,W,Mg,Dr,Ba]
    frag: opts&&opts.frag ? opts.frag : 0,
    maxPurchases: opts&&opts.max ? opts.max : DEFAULT_MAX,
    bodyBonus: opts&&opts.body ? opts.body : 0,
    strBonus: opts&&opts.str ? opts.str : 0,
    occupational: opts&&opts.occ ? true : false,
    prereqPerPurchase: opts&&opts.prereqPerPurchase ? true : false,
    _weaponChoice: opts&&opts._weaponChoice ? opts._weaponChoice : null,
    prereqs: prereqs || [],
    desc: opts&&opts.desc ? opts.desc : 'Description coming soon.',
  };
}

// Helper for frag-only skills — fixed frag cost and CP cost, no per-occupation pricing
function fragSkill(name, frag, cp, prereqs, opts){
  return {
    name,
    costs: null, // no per-occupation pricing — cost is fixed
    cp: cp,
    frag: frag,
    maxPurchases: opts&&opts.max ? opts.max : DEFAULT_MAX,
    bodyBonus: opts&&opts.body ? opts.body : 0,
    strBonus: opts&&opts.str ? opts.str : 0,
    prereqPerPurchase: opts&&opts.prereqPerPurchase ? true : false,
    prereqs: prereqs || [],
    desc: opts&&opts.desc ? opts.desc : 'Description coming soon.',
    _fragOnly: true,
  };
}

const SCHOOLS_OF_MAGIC = [
  'Healing','Elemental','Psionics','Nature','Protections',
  'Dark','Light','Draconic','Sigil','Necromancy','Wytchcraft','Dredgecraft'
];

const SPELL_LEVEL_COSTS = [
  [30,30,10,20,40,10,10,10,10],   // L1
  [40,30,10,20,60,10,10,10,10],   // L2
  [80,60,20,40,80,20,20,20,20],   // L3
  [100,60,30,40,100,30,20,20,30], // L4
  [100,90,40,60,100,30,30,30,30], // L5
  [120,90,50,60,120,40,30,30,40], // L6
  [120,120,60,80,120,50,40,40,60],// L7
  [150,120,70,80,150,50,40,40,70],// L8
  [150,150,80,100,150,60,50,50,80]// L9
];

const RITUAL_BASE_COSTS = [40,30,30,20,40,20,10,10,30];

// ---- Pyramid helpers ----
function getSlotsByLevel(){
  const counts = Array(11).fill(0); // indices 0-10, use 1-9
  s.owned.filter(o=>o._spellSlot && o._spellSlotLevel>=1 && o._spellSlotLevel<=9)
         .forEach(o=>{ counts[o._spellSlotLevel]++; });
  return counts;
}

function getSpellSlotCount(level){ 
  if(level === undefined) return s.owned.filter(o=>o._spellSlot).length;
  return s.owned.filter(o=>o._spellSlot && o._spellSlotLevel === level).length;
}
function getRitualSlotCount(){ return s.owned.filter(o=>o._ritualSlot).length; }

function getSpellLevelCost(level){
  const idx = OCC_ORDER.indexOf(s.occupation);
  const costs = SPELL_LEVEL_COSTS[level-1];
  return costs ? (idx>=0 ? costs[idx] : costs[0]) : 0;
}

function getRitualSlotNextCost(){
  const rank = getRitualSlotCount()+1;
  const idx = OCC_ORDER.indexOf(s.occupation);
  const base = idx>=0 ? RITUAL_BASE_COSTS[idx] : RITUAL_BASE_COSTS[0];
  return base*rank;
}

function addSpellSlot(level){
  if(!s.occupation) return;
  const {canAdd} = getManualSpellState();
  if(!canAdd.includes(level)) return;
  const cp = getSpellLevelCost(level);
  s.owned.push({name:`Spell Slot: ${ordinal(level)} Circle`, _spellSlot:true, _spellSlotLevel:level, _cat:'Magic', cp, frag:0, bodyBonus:0, strBonus:0, costs:null});
  render();
}

// Manual purchase state — only skill prereq gates, zero pyramid rules
function getManualSpellState(){
  const slots = getSlotsByLevel();
  const hasSphere = getPurchaseCount('Sphere of Magic: 1st') > 0;
  const hasReadMagicAdv = getPurchaseCount('Read Magic: Advanced') > 0;
  const canAdd = [];
  const canRemove = [];
  for(let lvl=1; lvl<=9; lvl++){
    const have = slots[lvl];
    // Determine if this level is unlocked by prereqs
    const prereqMet = lvl <= 4 ? hasSphere : (hasSphere && hasReadMagicAdv);
    if(prereqMet){
      if(have < 5) canAdd.push(lvl);
      if(have > 0) canRemove.push(lvl);
    }
  }
  return {canAdd, canRemove, slots};
}

// Pyramid rules — used only by buyToLevel
function getPyramidState(){
  const slots = getSlotsByLevel();
  const hasSphere = getPurchaseCount('Sphere of Magic: 1st') > 0;
  const hasReadMagicAdv = getPurchaseCount('Read Magic: Advanced') > 0;
  if(!hasSphere) return {canBuy:[], forced:null, slots};

  const canBuy = [];
  let forced = null;

  for(let lvl=1; lvl<=9; lvl++){
    const have = slots[lvl];
    if(have >= 5) continue;
    if(lvl === 1){ canBuy.push(1); continue; }
    // Level 5 requires Read Magic: Advanced for any slot
    if(lvl === 5 && !hasReadMagicAdv) continue;
    if(slots[lvl-1] < have + 1) continue;
    let chainValid = true;
    for(let l=2; l<lvl; l++){
      if(slots[l] > slots[l-1]){ chainValid=false; break; }
    }
    if(!chainValid) continue;
    canBuy.push(lvl);
  }

  for(let lvl=2; lvl<=8; lvl++){
    if(slots[lvl] >= slots[lvl+1] + 2 && slots[lvl+1] < 5){
      forced = lvl + 1;
      break;
    }
  }

  if(forced !== null){
    return {canBuy: canBuy.filter(l=>l===1||l>=forced), forced, slots};
  }
  return {canBuy, forced:null, slots};
}

function removeSpellSlot(level){
  const {canRemove} = getManualSpellState();
  if(!canRemove.includes(level)) return;
  for(let i=s.owned.length-1; i>=0; i--){
    if(s.owned[i]._spellSlot && s.owned[i]._spellSlotLevel===level){
      s.owned.splice(i,1);
      break;
    }
  }
  render();
}



// Prereq skill chain needed before spell slots
const MAGIC_PREREQ_CHAIN = [
  {name:'Read & Write',    costs:[70,60,45,55,70,45,40,50,40], prereqs:[]},
  {name:'Read Magic',      costs:[45,35,20,25,40,25,15,15,25], prereqs:[{name:'Read & Write',minCount:1}]},
  {name:'Read Magic: Advanced', costs:[50,45,30,35,50,35,25,25,35], prereqs:[{name:'Read Magic',minCount:1}]},
];
// Sphere 1 prereq chain (Read Magic required, handled separately via buySphere)

function buyPrereqSkillsForMagic(){
  // Purchase Read & Write, Read Magic, Read Magic: Advanced if not owned
  for(const sk of MAGIC_PREREQ_CHAIN){
    if(getPurchaseCount(sk.name) === 0){
      const idx = OCC_ORDER.indexOf(s.occupation);
      const cp = idx>=0 ? sk.costs[idx] : sk.costs[0];
      s.owned.push({...skill(sk.name, sk.costs, sk.prereqs, {}), _cat:'Scholar', cp});
    }
  }
}

function buyPrereqSkillsForLevel5(){
  // Also need Read Magic: Advanced for level 5 slot 2+
  if(getPurchaseCount('Read Magic: Advanced') === 0){
    const sk = MAGIC_PREREQ_CHAIN[2];
    const idx = OCC_ORDER.indexOf(s.occupation);
    const cp = idx>=0 ? sk.costs[idx] : sk.costs[0];
    s.owned.push({...skill(sk.name, sk.costs, sk.prereqs, {}), _cat:'Scholar', cp});
  }
}

// Buy to level: auto-purchase prereq skills + sphere + all slots up to full pyramid at targetLevel
function buyToLevel(targetLevel){
  if(!targetLevel || !s.occupation) return;
  const tl = parseInt(targetLevel);
  if(isNaN(tl) || tl<1 || tl>9) return;

  // Full 1-45 purchase sequence: each entry is [level, slot]
  const SEQUENCE = [
    [1,1],[1,2],[2,1],[1,3],[2,2],[3,1],[1,4],[2,3],[3,2],[4,1],
    [1,5],[2,4],[3,3],[4,2],[5,1],[2,5],[3,4],[4,3],[5,2],[6,1],
    [3,5],[4,4],[5,3],[6,2],[7,1],[4,5],[5,4],[6,3],[7,2],[8,1],
    [5,5],[6,4],[7,3],[8,2],[9,1],[6,5],[7,4],[8,3],[9,2],[7,5],
    [8,4],[9,3],[8,5],[9,4],[9,5]
  ];

  // Find the index of the first slot at targetLevel
  const stopIdx = SEQUENCE.findIndex(([lvl])=>lvl===tl);
  if(stopIdx === -1) return;

  // Step 1: clear all existing spell slots
  s.owned = s.owned.filter(o=>!o._spellSlot);

  // Step 2: purchase prereq skills if missing
  buyPrereqSkillsForMagic();

  // Step 3: purchase Sphere 1 if missing
  if(getPurchaseCount('Sphere of Magic: 1st') === 0 && getPurchaseCount('Read Magic') > 0){
    buySphere(1, true);
  }

  // Step 4: if target level >= 5, need Read Magic: Advanced
  if(tl >= 5) buyPrereqSkillsForLevel5();

  // Step 5: purchase slots 0..stopIdx inclusive in sequence order
  for(let i=0; i<=stopIdx; i++){
    const [lvl] = SEQUENCE[i];
    const cp = getSpellLevelCost(lvl);
    s.owned.push({
      name: `Spell Slot: ${ordinal(lvl)} Circle`,
      _spellSlot: true,
      _spellSlotLevel: lvl,
      _cat: 'Magic',
      cp, frag:0, bodyBonus:0, strBonus:0, costs:null
    });
  }

  render();
}


// ---- Magic panel render ----
let magicOpen = false;
function resetSpellSlots(){
  s.owned = s.owned.filter(o=>!o._spellSlot && !o._ritualSlot);
  render();
}

function toggleMagic(){ magicOpen=!magicOpen; renderMagicPanel(); }

function renderMagicPanel(){
  const body = document.getElementById('magic-panel-body');
  const chev = document.getElementById('magic-chev');
  const sub = document.getElementById('magic-header-sub');

  const totalSlots = getSpellSlotCount();
  const sphere1 = getPurchaseCount('Sphere of Magic: 1st');
  const sphere2 = getPurchaseCount('Sphere of Magic: 2nd');
  const sphere3 = getPurchaseCount('Sphere of Magic: 3rd');
  const sphereCount = sphere1+sphere2+sphere3;

  sub.textContent = sphereCount ? `(${sphereCount} sphere${sphereCount>1?'s':''}, ${totalSlots} slot${totalSlots!==1?'s':''})` : '';
  chev.textContent = magicOpen?'▲':'▼';
  body.style.display = magicOpen?'block':'none';

  if(!magicOpen) return;

  renderMagicSpheres();
  renderMagicLevels();
}

function renderMagicSpheres(){
  const row = document.getElementById('magic-spheres-row');
  const sphere1 = getPurchaseCount('Sphere of Magic: 1st');
  const sphere2 = getPurchaseCount('Sphere of Magic: 2nd');
  const sphere3 = getPurchaseCount('Sphere of Magic: 3rd');
  const hasSphere1 = sphere1>0, hasSphere2 = sphere2>0, hasSphere3 = sphere3>0;

  const readMagic = getPurchaseCount('Read Magic')>0;

  const sphereDefs = [
    {num:1, label:'Sphere 1', owned:hasSphere1, prereq:readMagic,  missingPrereq:'Read Magic',          costs:[100,100,75,75,100,75,25,50,50]},
    {num:2, label:'Sphere 2', owned:hasSphere2, prereq:hasSphere1, missingPrereq:'Sphere of Magic: 1st', costs:[200,200,175,175,200,175,150,175,175]},
    {num:3, label:'Sphere 3', owned:hasSphere3, prereq:hasSphere2, missingPrereq:'Sphere of Magic: 2nd', costs:[300,300,275,275,300,275,200,225,225]},
  ];

  row.innerHTML = sphereDefs.map(sp=>{
    const idx = OCC_ORDER.indexOf(s.occupation);
    const cost = idx>=0 ? sp.costs[idx] : sp.costs[0];
    const schoolKey = `s_school_${sp.num}`;
    const selectedSchool = s[schoolKey]||'';
    const usedSchools = [s.s_school_1||'', s.s_school_2||'', s.s_school_3||''].filter(Boolean);

    return `<div class="magic-sphere-card${sp.owned?' owned':''}${!sp.prereq&&!sp.owned?' locked':''}">
      <div class="magic-sphere-title">${sp.label}${sp.owned&&selectedSchool?' — '+selectedSchool:''}</div>
      ${sp.owned
        ? `<div class="magic-sphere-actions">
            <select class="magic-sphere-select" onchange="setSphereSchool(${sp.num},this.value)">
              <option value="">— choose school —</option>
              ${SCHOOLS_OF_MAGIC.map(sc=>{
                const isExclusive = Object.keys(EXCLUSIVE_SPHERES).includes(sc);
                const isAllowed = isSphereSchoolAllowed(sc);
                const isUsed = usedSchools.includes(sc) && sc!==selectedSchool;
                const disabled = isUsed || (isExclusive && !isAllowed);
                return `<option value="${sc}"${sc===selectedSchool?' selected':''}${disabled?' disabled':''}>${sc}</option>`;
              }).join('')}
            </select>
            <button class="magic-sphere-btn remove" onclick="removeSphere(${sp.num})">Remove</button>
           </div>
           ${selectedSchool && FAVOURED_FRAG_SPHERES.includes(selectedSchool) ? `<div style="font-size:10px;color:var(--color-text-warning);margin-top:3px">+100 frags (${selectedSchool})</div>` : ''}
           ${selectedSchool === 'Elemental' ? `<div style="margin-top:8px;padding-top:8px;border-top:0.5px solid var(--color-border-tertiary)">
             <div style="font-size:11px;color:var(--color-text-secondary);margin-bottom:5px">Primary Attunement <span style="color:var(--color-text-danger)">*</span></div>
             ${s.elementalAttunements.length===0
               ? `<select class="magic-sphere-select" onchange="setElementalAttunement(this.value)" style="font-size:11px">
                   <option value="">— choose element —</option>
                   ${['Fire','Stone','Lightning','Ice'].map(el=>`<option value="${el}">${el}</option>`).join('')}
                 </select>`
               : `<div style="display:flex;flex-wrap:wrap;gap:4px">${s.elementalAttunements.map(el=>`<span style="font-size:11px;padding:1px 8px;border-radius:100px;background:var(--color-background-tertiary);color:var(--color-text-primary)">${el}</span>`).join('')}</div>`
             }
           </div>` : ''}`
        : `<div class="magic-sphere-actions">
            ${!sp.prereq
              ? `<span style="font-size:11px;color:var(--color-text-warning);font-style:italic">Needs: ${sp.missingPrereq}</span>`
              : `<span style="font-size:11px;color:var(--color-text-tertiary)">${s.occupation?cost+' cp':'— cp'}</span>`
            }
            <button class="magic-sphere-btn" onclick="buySphere(${sp.num})" ${!sp.prereq||!s.occupation?'disabled':''}>Purchase</button>
           </div>`
      }
    </div>`;
  }).join('');
}

function setElementalAttunement(element){
  if(!element) return;
  if(!s.elementalAttunements.includes(element)){
    s.elementalAttunements.push(element);
  }
  render();
}

function getElementalAttunements(){
  return s.elementalAttunements || [];
}


function setSphereSchool(num, school){
  const prev = s['s_school_'+num]||'';
  s['s_school_'+num]=school;
  // If switching away from Elemental, remove attunements and Elemental Attunement skill purchases
  if(prev==='Elemental' && school!=='Elemental'){
    s.elementalAttunements = [];
    s.owned = s.owned.filter(o=>!o._elementalAttunement);
  }
  render();
}

function buySphere(num, silent=false){
  if(!s.occupation) return;
  const costs = [[100,100,75,75,100,75,25,50,50],[200,200,175,175,200,175,150,175,175],[300,300,275,275,300,275,200,225,225]];
  const prereqs = [['Read Magic'],['Sphere of Magic: 1st'],['Sphere of Magic: 2nd']];
  const names = ['Sphere of Magic: 1st','Sphere of Magic: 2nd','Sphere of Magic: 3rd'];
  const pre = prereqs[num-1];
  for(const p of pre){ if(getPurchaseCount(p)===0) return; }
  if(getPurchaseCount(names[num-1])>0) return;
  // Favoured cost table override
  const favTable = getFavouredCostTable();
  let cp;
  if(favTable){
    if(getFavouredVocationData()&&getFavouredVocationData().group==='Demagogue'){
      cp = [50,175,225][num-1];
    } else {
      cp = [50,200,300][num-1];
    }
  } else {
    const idx = OCC_ORDER.indexOf(s.occupation);
    cp = idx>=0 ? costs[num-1][idx] : costs[num-1][0];
  }
  s.owned.push({name:names[num-1], _spherePurchase:true, _cat:'Magic', cp, frag:0, bodyBonus:0, strBonus:0, costs:null, prereqs:[], maxPurchases:1});
  if(!silent) render();
}

// Check if a sphere school is selectable given current vocation
function isSphereSchoolAllowed(school){
  // Check exclusive spheres — only available to specific Favoured Vocations
  for(const [sphere, allowed] of Object.entries(EXCLUSIVE_SPHERES)){
    if(school === sphere){
      return s.vocation && allowed.includes(s.vocation);
    }
  }
  return true;
}

// Extra frag cost for selecting certain schools (Sigil, Wytchcraft, Necromancy, Dredgecraft)
function getFavouredSphereFragSurcharge(){
  // 100 frag surcharge per Sigil/Wytchcraft/Necromancy/Dredgecraft sphere owned
  let surcharge = 0;
  ['s_school_1','s_school_2','s_school_3'].forEach((key, i)=>{
    // Only count if the sphere is actually purchased
    const sphereNames = ['Sphere of Magic: 1st','Sphere of Magic: 2nd','Sphere of Magic: 3rd'];
    if(s[key] && FAVOURED_FRAG_SPHERES.includes(s[key]) && getPurchaseCount(sphereNames[i]) > 0){
      surcharge += 100;
    }
  });
  return surcharge;
}



function removeSphere(num){
  const names = ['Sphere of Magic: 1st','Sphere of Magic: 2nd','Sphere of Magic: 3rd'];
  const name = names[num-1];
  // Check dependents
  const deps = [];
  if(num===1){
    // Removing sphere 1 removes all spell slots, ritual slots, sphere 2&3
    if(getSpellSlotCount()>0) deps.push(`All ${getSpellSlotCount()} spell slot(s)`);
    if(getRitualSlotCount()>0) deps.push(`All ${getRitualSlotCount()} ritual slot(s)`);
    if(getPurchaseCount('Sphere of Magic: 2nd')>0) deps.push('Sphere of Magic: 2nd');
    if(getPurchaseCount('Sphere of Magic: 3rd')>0) deps.push('Sphere of Magic: 3rd');
  } else if(num===2){
    if(getPurchaseCount('Sphere of Magic: 3rd')>0) deps.push('Sphere of Magic: 3rd');
  }
  if(deps.length){
    showModal(`Remove ${name}?`, 'This will also remove:', deps, ()=>{
      doRemoveSphere(num);
    });
  } else {
    doRemoveSphere(num);
  }
}

function doRemoveSphere(num){
  const names = ['Sphere of Magic: 1st','Sphere of Magic: 2nd','Sphere of Magic: 3rd'];
  if(num<=1){
    s.owned = s.owned.filter(o=>!o._spellSlot);
    s.owned = s.owned.filter(o=>!o._ritualSlot);
    // Clear elemental attunements if Elemental was a selected school
    if(s['s_school_1']==='Elemental'||s['s_school_2']==='Elemental'||s['s_school_3']==='Elemental'){
      s.owned = s.owned.filter(o=>!o._elementalAttunement);
      s.elementalAttunements = [];
    }
    s['s_school_1']='';
  }
  if(num<=2){
    // Remove sphere 3 purchase when sphere 2 is removed
    s.owned = s.owned.filter(o=>!(o.name==='Sphere of Magic: 3rd' && o._spherePurchase));
    // Clear elemental attunements if Elemental was school 2 or 3
    if(s['s_school_2']==='Elemental'||s['s_school_3']==='Elemental'){
      s.owned = s.owned.filter(o=>!o._elementalAttunement);
      s.elementalAttunements = [];
    }
    s['s_school_2']='';
  }
  if(num<=3){
    // Clear elemental attunements if Elemental was school 3
    if(s['s_school_3']==='Elemental'){
      s.owned = s.owned.filter(o=>!o._elementalAttunement);
      s.elementalAttunements = [];
    }
    s['s_school_3']='';
  }
  s.owned = s.owned.filter(o=>!(o.name===names[num-1] && o._spherePurchase));
  render();
}

function renderMagicLevels(){
  const {canBuy, forced, slots} = getPyramidState();
  const hasSphere = getPurchaseCount('Sphere of Magic: 1st')>0;

  // Row A: levels 1-5
  const rowA = document.getElementById('magic-levels-row-a');
  rowA.innerHTML = [1,2,3,4,5].map(lvl=>buildLevelCard(lvl,slots,canBuy,forced,hasSphere)).join('');

  // Row B: levels 6-9 + ritual
  const rowB = document.getElementById('magic-levels-row-b');
  const ritualCount = getRitualSlotCount();
  const hasRitualPrereq = getPurchaseCount('Read Magic: Ritual')>0 && getSlotsByLevel()[9]>=1;
  const ritualLocked = !hasRitualPrereq;
  const ritualDone = ritualCount>=10;
  const nextRitualCost = getRitualSlotNextCost();

  const hasReadMagicRitual = getPurchaseCount('Read Magic: Ritual') > 0;
  const hasNinthCircle = getSlotsByLevel()[9] >= 1;
  const ritualLockNote = !hasReadMagicRitual
    ? `<div style="font-size:9px;color:var(--color-text-warning);text-align:center">Needs Read Magic: Ritual</div>`
    : !hasNinthCircle
      ? `<div style="font-size:9px;color:var(--color-text-warning);text-align:center">Needs 1× 9th Circle</div>`
      : '';

  const ritualCard = `<div class="magic-level-card${ritualLocked?' locked':''}${ritualDone?' complete':''}">
    <div class="magic-level-title">Ritual</div>
    <div class="magic-slots-dots">${Array(10).fill(0).map((_,i)=>`<div class="magic-dot${i<ritualCount?' filled-success':''}"></div>`).join('')}</div>
    <div class="magic-level-cost">${hasRitualPrereq&&s.occupation ? nextRitualCost+'cp' : '—'}</div>
    <div class="magic-level-btns">
      <span class="magic-level-count">${ritualCount}/10</span>
      <button class="btn-sm" onclick="addRitualSlot()" ${ritualDone||ritualLocked||!s.occupation?'disabled':''}>+</button>
    </div>
    ${ritualLockNote}
  </div>`;

  rowB.innerHTML = [6,7,8,9].map(lvl=>buildLevelCard(lvl,slots,canBuy,forced,hasSphere)).join('')+ritualCard;
}

function buildLevelCard(lvl, slots, canBuy, forced, hasSphere){
  const count = slots[lvl]||0;
  const isComplete = count>=5;
  const cost = getSpellLevelCost(lvl);

  // Prereq check only — no pyramid gating for manual purchases
  const hasReadMagicAdv = getPurchaseCount('Read Magic: Advanced') > 0;
  const prereqMet = lvl <= 4 ? hasSphere : (hasSphere && hasReadMagicAdv);
  const isLocked = !prereqMet;
  const addDisabled = isLocked || isComplete || !s.occupation;
  const removeDisabled = count === 0 || isLocked;

  // For visual indicators on the buyToLevel pyramid state
  const isForced = forced===lvl;
  const dotClass = isForced ? 'filled-warning' : isComplete ? 'filled-success' : 'filled';
  const subtitle = isForced ? ' ⬆' : '';

  let lockNote = '';
  if(!hasSphere) lockNote = `<div style="font-size:9px;color:var(--color-text-tertiary);text-align:center">Needs Sphere 1</div>`;
  else if(lvl >= 5 && !hasReadMagicAdv) lockNote = `<div style="font-size:9px;color:var(--color-text-warning);text-align:center">Needs Read Magic: Adv.</div>`;

  return `<div class="magic-level-card${isForced?' forced':''}${isLocked?' locked':''}${isComplete?' complete':''}">
    <div class="magic-level-title">${ordinal(lvl)} Circle${subtitle}</div>
    <div class="magic-slots-dots">${Array(5).fill(0).map((_,i)=>`<div class="magic-dot${i<count?' '+dotClass:''}"></div>`).join('')}</div>
    <div class="magic-level-cost">${prereqMet&&s.occupation ? cost+'cp' : '—'}</div>
    <div class="magic-level-btns">
      <span class="magic-level-count">${count}/5</span>
      <button class="btn-sm" onclick="addSpellSlot(${lvl})" ${addDisabled?'disabled':''}>+</button>
    </div>
    ${lockNote}
  </div>`;
}

function addRitualSlot(){
  if(!s.occupation) return;
  if(getRitualSlotCount()>=10) return;
  if(getPurchaseCount('Read Magic: Ritual')===0) return;
  if(getSlotsByLevel()[9]<1) return;
  const rank=getRitualSlotCount()+1;
  const cp=getRitualSlotNextCost();
  s.owned.push({name:`Ritual Slot (rank ${rank})`,_ritualSlot:true,_ritualSlotRank:rank,_cat:'Magic',cp,frag:0,bodyBonus:0,strBonus:0,costs:null});
  render();
}

function removeRitualSlot(){
  const owned=s.owned.filter(o=>o._ritualSlot);
  if(!owned.length) return;
  const advOwned=getPurchaseCount('Advanced Ritual Casting')>0;
  const wouldHaveZero=owned.length===1;
  if(advOwned&&wouldHaveZero){
    showModal('Remove last ritual slot?','Advanced Ritual Casting requires at least 1 ritual slot. Removing this will also remove Advanced Ritual Casting.',['Advanced Ritual Casting'],()=>{
      s.owned=s.owned.filter(o=>!o._ritualSlot||o._ritualSlotRank!==owned[owned.length-1]._ritualSlotRank);
      s.owned=s.owned.filter(o=>!(o.name==='Advanced Ritual Casting'&&!o._auto));
      render();
    });
    return;
  }
  const last=owned[owned.length-1];
  const idx=s.owned.lastIndexOf(last);
  if(idx>=0) s.owned.splice(idx,1);
  render();
}


// Occupational abilities — keyed by occupation name, 4 tiers each
// Costs: 3rd=30, 6th=60, 9th=90, 12th=120
// Prerequisites enforced via level gates and tier chain
const OCC_ABILITIES = {
  "Mercenary": [
    {name:"Hamstring", cp:30, tier:3, desc:"An Occupational Ability for Mercenaries, this skill allows the Mercenary to injure the target's leg and hamper their movement. To activate this skill the Mercenary must successfully strike the target's leg with a weapon and call out \"Innate 3 Body Hamstring.\" If the hit is successful, the target will take 3 Body damage and temporarily loses mobility in the injured leg, slowing their movement to 1 step every 3 seconds. This skill may be stacked if purchased more than once, allowing the damage to increase for each time it is used. For example, if Hamstring is purchased 3 times all three may be used simultaneously to create a \"Innate 9 Body Hamstring\" attack. Lastly, specific damage types may be called such as \"silver\" or \"magic\" based on the weapon used to hamstring. This makes walking slow and running impossible. This effect will last until the target receives at least 3 Body points worth of healing. This skill is usable once per day, per purchase."},
    {name:"Head-Butt",  cp:60, tier:6, desc:"An Occupational Ability for Mercenaries, a Head-Butt attack will stun the target for 5 seconds. While stunned, a victim is unable to take any action, including blocking, moving and the use of skills, minus the ability to call \"interrupt\" against Killing Blows and any counts against them. Automatic defenses such as Shield Magic will still operate, but ones requiring conscious thought such as Advanced Shield Magic will not. It may be used at will but only once per target, per day. To use the attack, place your palms on victim's shoulders, facing the victim from the front, and state \"Innate Physical Head-Butt\". If the attacker naturally swings for a type of damage other than Normal, this damage type is placed in front of the normal call. There is no numerical value for this attack, so when determining if the attack is stopped by a defender's threshold, only the damage threshold type is taken into account. For example, an \"Innate Silver Physical Head-Butt\" will breach a defender's +2 Silver threshold, but not a Magic one. A helmet on the defender will negate the attack, regardless of the damage type. A secondary effect of this ability allows the mercenary to escape a Garrotte. A Mercenary can use a Head-Butt attack while being Garrotted but the attack will be negated if the Garrotter is wearing a helmet. To escape a Garrotte the Mercenary does not need to be facing their attacker, but must place their hands on their attacker's hands and state \"Physical Head-Butt\". Performing a Head-Butt will do 1 Body damage to the attacker, which cannot be avoided in any way. Self Mutilate is not needed to use this ability."},
    {name:"Dismember",  cp:90, tier:9, desc:"An Occupational Ability for Mercenaries, this skill will sever the arms or legs of a target. By calling out \"Innate 5 Body Dismember!\" before striking an arm or leg, the Mercenary is able to deliver 5 points of Body damage and sever the limb from their victim. This skill may be stacked if purchased more than once, allowing the damage to increase for each time it is used. For example, if Dismember is purchased 3 times all three may be used simultaneously to create a \"Innate 15 Body Dismember\" attack. Also, specific damage types may be called such as \"silver\" or \"magic\" based on the weapon used to Dismember. The skill is consumed regardless of whether the attack is successful or not. It will work on arms and legs only. The skill may be used once per day per purchase."},
    {name:"Razor's Edge",cp:120,tier:12,desc:"An Occupational Ability for Mercenaries, this skill allows the Mercenary to sharpen, hone, or reinforce any weapon to add a +1 to its base damage for 1 year. The ability may be used once per day per purchase and takes 10 minutes of in-game time to complete. If the process is interrupted during that time, that day's use of Razor's Edge is used up and considered to be wasted. Once complete, the skill tag must be attached to the weapon, beside the weapon tag. Otherwise, a new tag, with the new base damage, must be signed off / authorized by a Shaper. If a Razor's Edged weapon is enchanted, the Razor's Edge will expire when the enchantment does. This skill may only be used on non-Magical weapons and each weapon may only have one Razor's Edge on it at a time."},
  ],
  "Ranger": [
    {name:"Detoxify",      cp:30,  tier:3,  desc:"An Occupational Ability for Rangers, this skill allows the Ranger to remove toxins and Alchemical substances from the target's bloodstream. It takes 10 uninterrupted seconds for the Ranger to remove the toxin from the target. If, at any time, the Ranger stops, or takes damage to Body, the Detoxify fails and the skill is considered used. It will work on any toxin or Alchemical substance which can be cured by a standard Antidote, regardless of how long the toxin has been in the target's system. The call for this ability is \"Innate Detoxify\". This skill is usable once per day, per purchase."},
    {name:"Trailblazing",  cp:60,  tier:6,  desc:"An Occupational Ability for Rangers, this skill allows the Ranger to call \"Innate Trailblazing\" to release themselves from any magical or alchemical binding effect that requires a strength bonus to escape from without taking any Body damage. This skill does not function against any man-made devices like bear traps or manacles. This skill is usable once per day, per purchase."},
    {name:"Nature's Grasp",cp:90,  tier:9,  desc:"An Occupational Ability for Rangers, this skill allows the Ranger to infuse any weapon with the binding power of Nature. It takes 10 seconds to infuse one weapon and during that time, the Ranger must concentrate by rubbing the weapon with leaves, dirt or other symbols of nature. If the Ranger is interrupted, or takes damage to Body, the ability fails and is used up for the day. If successfully created, the weapon's damage suffix is changed to \"Magic Body\" and, when used, will entangle the target in a Web effect. When a target is successfully hit, roots will rise up from the ground, immobilising them from the neck down. It takes a 6 minute count to cut free from the entanglement, or the target may rip it out if they have at least +6 Strength and the skill Self Mutilate, suffering 6 Body damage in the process. If the target is not cut or ripped free, the web will remain until Line of Sight to the Ranger is broken. The call for this attack would be \"Innate <damage> Magic Body Web\". This infusion will last 5 days or until first used. This skill is usable once per day, per purchase."},
    {name:"Call of the Hunt",cp:120,tier:12,desc:"An Occupational Ability for Rangers, this skill will summon into being a powerful Hunt-Master to hunt a target that has offended nature. Not to be used lightly, this skill will summon forth the Hunt-Master and their hounds. This skill can only be used by the Ranger between the hours of 6am and 6pm. The ability requires a 10-minute ritual and requires the Ranger's full attention. Should the Ranger use any other skill or ability, take damage to Body, or become distracted for more than 60 seconds, the ability will fail and be consumed for the event. During these 10 minutes, the Ranger must commune with nature, stating their reasons for calling the Hunt, and end by sacrificing a living creature (animal will suffice) to the Hunt-Master. The sacrifice should be performed in a way appropriate to the culture of a Ranger and which respects the gift given by the sacrifice. The more elaborate this ritual is, the stronger the Huntsman will be. This ceremony should take place in front of a marshal. At the end of the ritual, the marshal will ask the Ranger whether they would like an NPC Hunt-Master and hounds, or if they, and up to 3 of their friends, would like to act as the Hunt-Master and their hounds. If the Ranger requests an NPC Hunt-Master, and NPC camp has the NPCs to spare, the Hunt-Master and their hounds will appear between the hours of 6pm and 6am that night.\n\nIf the Ranger requests to act as the Hunt-Master themself, or NPC camp does not have NPCs to spare, the Ranger will become imbued with the power of a Hunt-Master and up to three other PCs will be imbued with the power of the Hunt-Master's hounds. Anyone who wishes to be part of this must have been involved in the ceremony. The Ranger and their friends will be given claws, horns, and anything else they require for the role. The Ranger will keep their own skills, abilities, etc., but will also be given additional Hunt-Master abilities. The PC hounds will have only the hound abilities. While in this form, the Ranger and their hounds must hunt down their target. If they stop hunting or do something else, the effect ends. A marshal may end the hunt early if they feel the Ranger is not actually hunting their target. While in this form, the Ranger can sense the general direction of their target (ie: north, west, etc.) until they get within 1 mile of the target. Within 1 mile of the target, the Ranger can \"Sense\" their target at will by stating, \"Sense [Target]\". If a PC dies as the Hunt-Master, they take a death and resurrect like normal. If a PC dies as a hound, they resurrect but their death is not recorded.\n\nThe Hunt-Master is not a mindless creature chained to the will of the Ranger. It is an aspect of nature and can act with intelligence, cunning and fury. Should the Ranger use this ability frivolously or without warrant, they may find themselves the hunted. The movement of the Hunt-Master and their hounds is limited to the natural and rural environment. They cannot cross constructed bridges, city streets made of anything but dirt, or enter buildings or other dwellings which are not naturally occurring. The Hunt-Master will not hunt mindless creatures or those without a Spirit. This ability can only be used by the Ranger once per event."},
  ],
  "Templar": [
    {name:"Burn Slot",      cp:30,  tier:3,  desc:"An Occupational Ability for Templars, this skill allows the Templar to \"burn\" any unused Battle Magic or Ritual Magic level spell-slots to add damage, at the value of +2 Magic/slot, to their next weapon strike. The Templar may choose how many of their unused slots to burn at the time of the swing. Any spells stored in those slots are lost. E.g. A Templar who normally swings for \"2 Normal\" with their sword chooses to burn 3 slots, the call would be \"Innate 8 Magic\" for that one swing. The level of the slot does not matter for this purpose. If the swing misses or is blocked, the damage is not used up, so the defending player should declare \"Hit\" if the strike hit successfully. The Templar must call \"Active Burn Slot\" for every subsequent swing. The Burn Slot remains active for a maximum of 1 minute, or until used. Either way, the skill is used up and the slots are burnt. This skill is considered used if it hits a shield being wielded or if the target uses a defense to stop it after being hit, but the target will take no damage. This skill is usable once per day, per purchase."},
    {name:"Scroll Harvest", cp:60,  tier:6,  desc:"An Occupational Ability for Templars, this skill will allow the Templar to activate a Battle Magic scroll without it being consumed. To activate this skill, the Templar must hold the target scroll, verbally state \"Innate Scroll Harvest <scroll name>\" then verbally incant the spell on the scroll. The scroll will activate normally but will not be consumed by the casting. This class ability will work on scrolls level 1 to 7. For scroll levels 8 to 9, two uses of Scroll Harvest must be used. Normal rules for activating a Battle Magic scroll apply. This ability does not grant the Templar the Read Magic Ability, which must be purchased separately. This skill is usable once per day, per purchase."},
    {name:"Weapon Break",   cp:90,  tier:9,  desc:"An Occupational Ability for the Templar, this skill will allow the Templar to shatter an opponent's weapon, spraying the target with the shattered pieces. The Templar may break an opponent's weapon using their own weapon, like a physical effect, so long as the weapon is hit. This ability will also work on shields. If the shatter is successful, the target will also be dealt 15 damage of whatever type their weapon was dealing when it was struck. This damage type includes Normal, Magic, silver, etc., but does not include Body damage or Alchemical effects. Shields deal Normal damage. The call is \"Innate Weapon Break!\" This skill is usable once per day per purchase."},
    {name:"Weapon Conduit", cp:120, tier:12, desc:"An Occupational Ability for Templars, this skill will allow the Templar to absorb, store and redirect Battle Magic spells and magical effects which exactly copy a Battle Magic spell which they have successfully been hit with, through their melee weapon. The Templar may use any source for this Battle Magic including: spells they cast on themselves, offensive spells cast at them, scrolls, or even Battle Magic producing Magic items.\n\nTo effectively use Weapon Conduit the Templar must first absorb a Battle Magic spell they are the target of. By stating \"Innate Weapon Conduit!\" at the time of absorption, the Templar's own body will absorb the spell and then act as a conduit, sending it though their own weapon, on to another target. Once a spell is stored in the weapon, the Templar may unleash it at their will in the form of a Spellstrike. To activate the spell inside the weapon the Templar must call out \"Spellstrike <spell>\" The Templar has 1 minute to unleash their absorbed spell before the stored power of the spell explodes from their body. If the Templar fails to unleash their stored spell within that time, they suffer 15 points of magic damage. Stored spells do not stack on the Templar. Spellstrikes may be only used in conjunction with melee weapons. This ability can be used once per day per purchase."},
  ],
  "Nightblade": [
    {name:"Feint",        cp:30,  tier:3,  desc:"An Occupational Ability for Nightblades, this skill allows the Nightblade to quickly evade any packet-delivered alchemical attack they are successfully struck with. To use this ability, the Nightblade must state \"Innate Feint,\" in order to avoid the attack. This skill also has the additional benefit of acting as the pre-requisite for the rogue skill Dodge, without requiring the Nightblade to purchase the skill Critical. Each purchase of Feint fulfills the pre-requisite for a single purchase of Dodge. This ability may be used once per day per purchase."},
    {name:"Duplicate Key",cp:60,  tier:6,  desc:"An Occupational Ability for Nightblades, this ability will create a duplicate of any key, Magical or otherwise. This ability will work on any mundane key, wizard lock key, ward keys etc. This ability requires the original key or a pre-existing duplicate to be touched by the Nightblade and a declaration of \"Innate Duplicate Key\" must be said aloud. The duplicate will last for 1 year or until used once. This ability may be used once per day, per purchase."},
    {name:"Dim",          cp:90,  tier:9,  desc:"An Occupational Ability for Nightblades, this skill allows the Nightblade to become invisible and non-corporeal so long as they do not move, attack, or make any sound. To use the skill the Nightblade must be in darkness. A character is in darkness when words on a page held at arm's length cannot be read. Dimming requires a three-count, \"Innate Dim 1, Dim 2…\", both entering and exiting the Dim. Should a light source destroy the shadow the Nightblade will automatically be forced out of Dim (still requiring an exiting 3 count). While dimmed, a Nightblade must put on a white, out-of-game headband, or place their hand/weapon on their head. This ability does not hide the Nightblade from Sense abilities. This skill may be used once per day, per purchase."},
    {name:"Passwall",     cp:120, tier:12, desc:"An Occupational Ability for Nightblades, this ability allows the Nightblade to ethereally attune a small section of a normally solid surface, allowing them to pass back and forth through it, stating \"Innate Passwall\". It will allow the Nightblade to enter and exit through the surface, but only once per direction. This attunement will work on any object that is less than 3 feet in thickness, such as stone walls and doors (including magical and ritual barriers). Only the Nightblade, mundane untagged clothing, Spirit linked items, and items made from the Duplicate Key skill, may enter. All other items must be left behind. If or when the Nightblade exits through the attuned surface, they may bring any items with them. The attuned surface will last 5 minutes. The ability requires 1 minute of uninterrupted concentration before using. If Body damage is taken during the 1 minute of preparation, the skill is used up and wasted. It may be used once per day per purchase."},
  ],
  "Assassin": [
    {name:"Shiv",         cp:30,  tier:3,  desc:"An Occupational Ability for Assassins, this skill allows the Assassin to turn any single simple- or medium-sized weapon or stiletto swing into Body damage equal to the weapon's base damage. If a stiletto is used, the damage is x2. Preparing the Shiv attack requires a 3-count - \"Innate Shiv 1, Innate Shiv 2, Innate Shiv 3\". This skill can be combined with any other skill or ability as if it were a normal weapon swing. This effect is used up regardless of whether the attack hits or misses. The Assassin has 1 minute to use the Shiv before it expires. This skill is usable only by the Assassin who prepares it and is usable once per day per purchase."},
    {name:"Silent Strike", cp:60,  tier:6,  desc:"An Occupational Ability for Assassins, this skill allows the Assassin to add a silencing effect to one of their Normal attacks. For this effect to activate successfully, the attack must damage the target into Body. If the attack does not damage the target into Body, this skill will fail. This silencing effect lasts until the target receives at least 1 Body point of healing. To activate this skill the Assassin must declare \"Innate Silent Strike\". Once activated the Assassin has one hour to engage their prey, adding the suffix \"Silence\" once to their next weapon swing. This skill may be used in conjunction with an Execute to create a Silent Kill. To use the ability in this manner the assassin must declare \"Silent Kill\". A silent kill functions exactly the same as an execute save that the target is silenced and cannot scream. The Silent Strike skill may be used once per day, per purchase."},
    {name:"Spirit Sever",  cp:90,  tier:9,  desc:"An Occupational Ability for Assassins, this skill allows the Assassin to cut the astral strands that bind a Spirit to its body. This skill must be used on a target in their Death Count and takes 30 seconds to complete. During this time, the Assassin must stay with the target, actively cutting the invisible strands that tie the target's Spirit to their body. If successful, the target Spirit must forgo the remaining time in their Death Count and immediately attempt to Resurrect. While the Assassin is using this skill, it is suggested that the target continue their normal Death Count, outlined by their race, in the event the Assassin fails. The 30 second Spirit Sever count must be said by the Assassin, loud enough for the target to hear. If at any point the Assassin stops counting, is interrupted, uses any other skill or if the target was so far along in their Death Count they Resurrect before the Assassin finishes, this skill will fail. This skill will also fail if used on a conscious target or a target in their Bleed Count. This skill can be used once per day per purchase."},
    {name:"Penetration",   cp:120, tier:12, desc:"An Occupational Ability for Assassins, this skill allows the Assassin to bypass armour and Magical protections for a single physical attack. When used, the Assassin may add the \"Innate Surprise Penetrating\" prefix to their damage call for one melee or ranged attack that strikes their opponent from behind. A penetrating attack ignores all non-ritual level protections, non-racial abilities, and any armour the target may be wearing. Protections which are ignored are not used up by this attack. If the Assassin misses their target with their swing or the attack is physically blocked by another weapon or shield, this ability is used up for the day. It is usable once per day per purchase. Penetration may be used in conjunction with any Rogue skill, even if said skill explicitly states that it may be not used in conjunction with other skills."},
  ],
  "Wytchhunter": [
    {name:"Wytch Mark / Opposed Sphere", cp:30,  tier:3,  desc:"An Occupational Ability for Wytch Hunters, this skill serves two purposes:\n\nFirst, it allows for the creation of a glowing magical symbol that will store any Battle Magic spell cast into it by the Wytch Hunter within 60 seconds of its creation. This spell must be cast by the Wytch Hunter or through a magic item used by them. The symbol must be represented by a green light and must remain stationary and unhidden. The tag for the Wytch Mark must be attached on or next to the green light, as well as the spell tag if one is used. The Wytch Hunter must choose one of their opposed spheres and write that on the Wytch Mark tag, stating \"Innate Wytch Mark <Sphere>\". Once prepared, the Wytch Mark will activate the next time a person with active magic (a spell with a duration in progress) from the chosen sphere or a person holding an item with active magic from the chosen sphere comes within 10 feet of it. If this occurs, the target will be automatically struck by the stored spell as if they had been successfully hit by a spell packet. For the purposes of defenses, the attack is presumed to have a call of \"Magic <spell>\". If no spell is cast into the Wytch Mark, it will do 1 Magic damage instead. Once the Wytch Mark is activated, it will vanish. A Wytch Mark can be destroyed and is considered to have 1 Body Point. Wytch Marks last 5 days or until activated. This ability may be used once per day per purchase.\n\nSecondly, purchasing this ability allows the Wytch Hunter to choose one hated sphere. Until this class ability is purchased for the first time, a Wytch Hunter has no opposing sphere of magic. This class ability may be purchased multiple times, each time allowing the Wytch Hunter to choose a new sphere of magic if they desire, otherwise multiple purchases will simply unlock more uses of the Wytch Mark per day."},
    {name:"Twist of the Tongue",         cp:60,  tier:6,  desc:"An Occupational Ability for Wytch Hunter, this skill will allow the Wytch Hunter to inflict a terrible attack on any target, twisting and spiraling their tongue, should they cast from any of the Wytch Hunter's opposed spheres. This packet delivered attack, if successfully landed, will sit, impervious to all methods of removal, on a target's spirit for the next hour like a magical trap. If at any time during that duration the target casts a spell from the Wytch Hunters hated spheres, from memory, scroll, or magic item, their tongue will twist and spiral once the spell is cast. A target with a twisted tongue may grunt and squeal but cannot cast, engage in coherent speech or use any skills, items or abilities that require speech for duration of one hour. This infliction may not be healed or cured, even if the target dies and is given a life spell. Only successful resurrection or duration expiry will restore the targets tongue. The call for this ability is \"Innate Arcane Twist of the Tongue <Spheres>\", e.g. \"Innate Arcane Twist of the Tongue Necromancy Psionics\". The Wytch Hunter need not list each of their opposed spheres, if they do not wish each sphere to be impacted. This ability is usable once per day per purchase."},
    {name:"Karmic Ricochet",             cp:90,  tier:9,  desc:"An Occupational Ability for Wytch Hunters, this ability will allow the Wytch Hunter to absorb any Battle Magic spell and return it back to the caster. This ability can absorb a spell from the Wytch Hunter's Opposed Spheres of Magic that successfully strikes them, or any other target within 10 feet of the Wytch Hunter, by verbally declaring \"Innate Arcane Ricochet\". If the spell is one which allows the caster to throw more than one packet, the Wytch Hunter must absorb the first packet for the Ricochet to be effective. The Wytch Hunter then has 3 seconds to ricochet that spell back to the original caster or into the ground via spell packet or touch-cast. If they fail to do this or do not ricochet it within the 3 seconds, the Wytch Hunter will take the full effect of the spell themselves. When returning the spell, the Wytch Hunter must declare \"Innate Ricochet Magic <spell name>!\" before throwing the packet. This returning spell will have no effect on any other target other than the original caster or the Wytch Hunter. The spell being returned is an exact duplicate of the one that was captured by the Wytch Hunter. This ability is usable once per day, per purchase."},
    {name:"Counter Magic",               cp:120, tier:12, desc:"An Occupational Ability for Wytch Hunters, this Arcane packet-delivered or touch attack will negate or destroy any Battle Magic and most Ritual spells of the Wytch Hunters Hated spheres. This ability may also counter any spell that hits the Wytch Hunter, so long as it is within their Hated spheres. Counter Magic will act the same as an Advanced Shield Magic spell in this regard and the defensive call is \"Innate Arcane Counter Magic\".\n\nWhen used offensively, Counter Magic will destroy any one spell within the Hated Spheres of Magic that is active on the target and has a duration other than instant. The call for this attack is \"Innate Arcane Counter Magic: <specific spell OR sphere>\". If a sphere is part of the call, the target chooses one active spell within that sphere to be removed. If a spell named in the call is active on the target, it is destroyed. If the specific spell called is not active on the target, the Counter Magic fails without activating defenses. This ability is usable once per day, per purchase.\n\nCounter Magic may be used against a target without a spirit, such as a cabin. Once again, either a specific spell may be targeted or a sphere. If an OOG note has been left describing an active spell effect (such as a Ward) and it is destroyed by the Wytch Hunter, they may leave their Counter Magic tag attached to the note to indicate that it no longer exists."},
  ],
  "Mage": [
    {name:"Identify Magic Item",    cp:30,  tier:3,  desc:"An Occupational Ability for Mages, this skill allows the Mage to identify a magic item by consuming a Catalyst of any type. The Mage must touch a Catalyst of any type, as well as the item they are attempting to identify, and state \"Innate Identify\". The Catalyst will be consumed in a brilliant flash of blue light. The effect(s), flaw(s), activation word, expiry, and any other traits on the magic item tag will be revealed to the Mage. This skill is usable once per day, per purchase."},
    {name:"Mana Harvest",           cp:60,  tier:6,  desc:"An Occupational Ability for Mages, this skill allows the Mage to harvest spent Battle Magic spells by consuming Catalysts. For this ability to be successful the Mage must touch the appropriate number of Catalysts, choose which used Battle Magic spell they are going to recall, and declare \"Innate Mana Harvest <spell>\". The Catalyst(s) will be consumed in a brilliant flash of blue light and the Mage's ability to cast that chosen spell will be recalled. To harvest a Circle 1-3 spell, the mage must consume one Catalyst of any type. To harvest a Circle 4-6 spell, the mage must consume two Catalysts of any type. To harvest a Circle 7-9 the mage must consume three Catalysts of any type. A Discord Catalyst will count as if it were two Catalysts. This ability will only recall a Battle Magic spell into memory that has already been used and will not allow the Mage to rememorize a new one in its place. This skill is usable at will but may only be used once per spell slot."},
    {name:"Create Familiar",        cp:90,  tier:9,  desc:"An Occupational Ability for Mages, this skill allows the Mage to create, and bring to life, a magical Familiar. This Familiar is a part of the Mage, created from their raw magic. Only one such creature can exist at a time for the Mage, and the creature is considered to have animal intelligence. The Mage may choose the Familiar's form at creation, but it must in some way represent one of the Spheres of Magic that the Mage can cast. Once decided, a Familiar's form cannot be changed. Its size is limited to no greater than a large housecat. The Familiar is spirit linked to its creator, and cannot leave the Mage's person. It has no skills or abilities of its own, possesses no Spirit and cannot die, unless the Mage dies and resurrects. At any point, the Mage can choose to kill the Familiar, just by willing it. Doing so causes the Familiar to dissipate. While in existence, the Familiar will hold one Battle Magic spell that the caster can currently cast. This spell is chosen when the Familiar is first created and can be changed or reset when the Mage chooses to re-memorize their spells for that day. At any point, the Mage can cast that spell as if they had the extra spell-slot in their pyramid. Once done, the Familiar is now \"empty\" and cannot store another spell until the Mage resets for the day. The Familiar will also help in the casting of Rituals. The Familiar can act as a secondary caster in a Ritual the Mage casts as the primary caster, once per day. To create a Familiar, the Mage must spend one hour performing a rite to create an entity from raw magic. Once the hour has passed, the Mage must declare \"Innate Create <Sphere> Familiar\" for the ritual to be complete. The Familiar must be visually represented by the Mage. A doll or stuffed toy will suffice, as long as it in some way resembles the Sphere of Magic chosen. This skill may be used once per day, per purchase."},
    {name:"Power Nexus",            cp:120, tier:12, desc:"An Occupational Ability for Mages, this skill allows the Mage to create a circle of power used in the casting of Ritual Magic for any Sphere that the Mage knows. Casting a ritual using a Power Nexus will add 1 White stone to the ritual bag. A Power Nexus will also allow the Mage to \"Sense Catalyst\" at will, so long as the mage is inside the circle. Those within range of the detection must announce how many (and what type of) Catalysts they carry on their person, even if they are outside of the circle. This circle is not equipped with a barrier or any other abilities unless the Mage alters it with ritual magic. A final ability of a Power Nexus is to have the Nexus transform into a circle of protection for 10 minutes. This transformation will change the Nexus into a Circle of Protection against one of these specific groups that must be declared at the time of transformation via \"Innate Power Nexus: Circle of Protection from <name>!\": Any racial group in the rulebook (such as \"Elves\"), Lesser Angels, Lesser Demons, Lesser Undead, Animals, Brood, Constructs, Elementals, Plants, Magical Beasts, Spirits or Vermin. Only one type of protection can be active at a time and it cannot be changed once active. When a circle is modified in this manner, it will last for 10 minutes then the entire circle will vanish permanently. While active the protective circle will prevent its target \"type\" from crossing the circle or performing hostile actions through it, but it will not act as a barrier to any other creature.\n\nThe Mage must visually represent this circle of power with a rope or some other method that clearly outlines its borders. A circle of power created with Power Nexus is 10 feet in diameter; however, multiple uses of this ability by the same Mage at creation will increase the diameter of this circle by 10 feet and add 1 White stone to each ritual cast using the Nexus per use. This circle of power will last for 5 days and cannot be destroyed save via Ritual Magic. The Mage can choose to destroy this circle at any time they wish. For this skill to be successful, the Mage must visually represent their Circle and declare \"Innate Magic Power Nexus!\" This skill can be used once per day per purchase."},
  ],
  "Druid": [
    {name:"Create Grove",  cp:30,  tier:3,  desc:"An Occupational Ability for Druids, this skill awakens a 10-foot diameter circle of natural wilderness with druidic energy. A Grove grants the following powers: it allows the creator to see and identify any True Fae creature that steps within its boundary and the Grove creates an empathetic bond with its creator. This allows the Druid to sense the emotions of the Grove and vice versa. A Grove's emotion can change based on perceived threats to the grove or unnatural corruption of the lands surrounding it. These indicators will always be vague and cannot tell a druid specifics about the reasons for the emotional state, only that they exist. A Grove does not provide a barrier or any other protection to those inside, and cannot be augmented in any way, other than upgrading it to a Henge for which it is a prerequisite. It takes a 1-hour role-play ritual to create the Grove. Groves must have their boundary visibly defined by a rope or other marker but these markers can be natural, such as vegetation. Groves can only be made outdoors. They may contain structures such as tents, but only if the structure is small enough to fit completely inside the Grove. A Druid may have 1 Grove active at a time, per guild. The grove can be moved by releasing the druidic energy back to nature and performing the 1-hour role-play ritual again elsewhere. If a druid who has created a Grove dies a final death, the Grove fades away."},
    {name:"Forest Meld",   cp:60,  tier:6,  desc:"An Occupational Ability for Druids, this skill allows the Druid to become one with the forest, hiding their presence. To successfully activate this skill the Druid must use a tree with a thickness such that they are unable to completely wrap the fingers of both their hands around its trunk. A 3 count declaration must be said aloud \"Innate Forest Meld 1, Forest Meld 2 ...\" At this point, the Druid will merge into the tree and must place their hand/weapon on their head, or don a white headband, to show they are out of game. The Druid may stay hidden inside the tree until they will the skill to end, breaks concentration, or the tree takes 1 Body point of damage. At that point, the Druid will be ejected from the tree, again with a 3 count. While melded, a Druid is able to hear sounds as normal. A Druid who has created a Henge may choose to merge with it, if it is large enough, and forgo the expulsion due to Body damage. In this case the Druid will not be ejected unless the Henge dies, at which point so will the Druid. This skill may be used once per day, per purchase."},
    {name:"Totem",         cp:90,  tier:9,  desc:"An Occupational Ability for Druids, this skill allows the Druid to shape-shift into their Totem Animal. The Totem Animal must be chosen upon purchase and cannot be changed after purchase. Subsequent purchases allow the Druid to select an additional Totem Animal. Totem may be used once per day per purchase.\n\nWhen used, this skill will transform a Druid into their chosen animal form. The animal cannot be smaller than a fox or larger than a brown bear. The animal may not be one that is capable of flight and must be natural/normal (not supernatural). It takes one minute to activate, and requires the Druid's full concentration. If they become distracted, use any other skill, or take damage to Body during the transformation, the ability fails and is considered used for that day. All carried items and clothing will magically merge into the Totem form. These items cannot be retrieved until the Totem ends. This ability will fail if the Druid attempts to shape-shift while carrying an item with a Spirit or something that is larger than half their size.\n\nThe Totem change lasts for 1 hour and may be terminated at will (taking 1 minute to change back). If detected for magic, a Totem will glow and thus can be distinguished from a regular animal. Being in Totem form is considered a race change, so the Druid will detect as the Totem animal and not their original race, and will have neither the advantages nor disadvantages of their original race. While in their Totem form, the Druid should think and behave as the animal does.\n\nTotem Animal stats (calculated from level 1): 1 Normal threshold (+1 every 3 levels), 2 damage via Claw (+1 every 3 levels), 20 Body (+5 every 3 levels), 1 \"25 Slay\" every 5 levels. While in Totem form the Druid will take x2 damage from all silver weapons. Once shifted back, the Druid will be fully healed (unless in Death count) and any Alchemical toxins or non-Magical diseases will be removed."},
    {name:"Henge",         cp:120, tier:12, desc:"An Occupational Ability for Druids, this ability upgrades any Grove the Druid has created into something much more powerful. Once created a Grove will gain a \"Heart\" - a living organism at the center of the new Henge, which powers it and acts as its lifeforce. This Heart must be represented by living vegetation at the center of the Henge and must be marked with a tag. A Henge's size and boundaries will mirror that of the Grove it was created from.\n\nA Henge has the abilities of a Grove, with the following additions: The Henge Heart has 100 Body points and a magic threshold. The Henge offers an always active, frictionless, spherical barrier. Those invested in the Henge may pass freely through the barrier and may \"Recognize\" others through the barrier on a 3-count. This barrier will prevent the passage of everything, with the exception of air, light, sound and gaze attacks, unless the ability specifically states otherwise. Attacks cannot be made from the inside of the Henge to the outside, even by investees. The Henge can have as many people invested in it as the druid desires (done through a 1 hour role-play only ritual). Being invested in a Henge persists through death. The Henge can resurrect spirits as per a Resurrection Circle and will do so automatically in 10 minutes. The Henge allows anyone invested to \"reject\" anything that has a Spirit and is not invested, forcing them outside the boundary. The Henge allows anyone invested to see any Spirit in the Henge, including Ghosts and those that walk in the Fae Realm. The Henge will act as a Nature ritual circle and as a secondary caster for those rituals. The Henge allows anyone invested to transport to the Fae realm once per day.\n\nWhen a Henge Heart is killed, if the creator is within 5 miles of it, the creator will be hit with a repeating Arcane Death once per hour until they resurrect. A druid may have 1 active Henge per guild. If the druid who created the Henge dies a final death, all investees become divested and the Henge fades away."},
  ],
  "Bard": [
    {name:"Song of Aversion",   cp:30,  tier:3,  desc:"Duration: Concentration. This Occupational Ability allows for a Bard in danger to cloud the minds of their foes, confusing their foes to their exact presence and hiding them for a few precious moments. This skill does not grant the Bard true invisibility but it will obfuscate their person, causing all around them to avoid and ignore the Bard for a short period. To activate this skill, the Bard must state \"Innate Song of Aversion!\" Once activated the Bard's feet must remain stationary and for the next 15 seconds they must repeatedly state \"Active Song of Aversion\". While the skill is active all those around the Bard that can hear their voice and know the general location of the Bard within ten feet, but the Bard will appear blurred and displaced. They will unconsciously miss if they try to blindly attack or swing wildly in the area the Bard is hiding. This does not grant the Bard immunity to damage from Area of Effect spells or effects or the effects of Power or Command Words. This skill is intended to give the Bard a few moments to put away their valuable instruments to avoid harm and/or hopefully allow their friends to regroup and save them from the attack. This ability is usable once per day per purchase."},
    {name:"Song of Love",       cp:60,  tier:6,  desc:"Duration: 4 Hours. An Occupational Ability for Bards, this song will allow the bard to magically charm up to two individuals of their choosing, so long as both hear the bard's performance from start to finish and are serenaded by the bard at least once. In order for a serenade to be successful, the song must have a duration of at least 5 seconds, and the targets of the serenade must make eye contact with or be touched by the singer. Once the performance is complete, the bard must either state \"Innate Arcane Charm: Target's Name\" or convey to the target that they have been affected. Each target will then take the effect of an Arcane Command Word Charm Spell. The player may determine, out of game, whether this causes infatuation or a very strong friendship. This Command Word is not detectable when used, nor is spoken or cast by the Bard. Instead, it is a representation of the overall effect the Bard's song has on its targets. Both the Charm and the potential infatuation will not cause the target to do things outside of their nature but they will act as if the bard is their new best friend and possibly lover. They will believe almost anything the Bard says to be true, they will protect the Bard with their lives if asked. A charmed target will not kill themselves or assassinate other loved ones unless somehow tricked or deceived. This effect will last for 4 hours after which the charm effect will wear off. This ability is usable once per day per purchase."},
    {name:"Song of Intermission",cp:90, tier:9,  desc:"Duration: Concentration up to 30 minutes. An Occupational Ability for Bards, this song will allow the Bard to use their performance to suspend or extend any spell or effect that is currently being counted or in duration. In order for this effect to work the target of the duration or count must hear the Bard's song and willingly accept its effects to allow the duration or count to be extended. The Song of Intermission is so powerful that it can even delay death, pausing a willing victim's death or Bleed Count, until help can be found. This function will work even if the dead or dying target cannot hear. To activate this song, the Bard must state \"Innate Song of Intermission\" then begin their performance piece. Song of Intermission will not affect any spell or effect that fails. This skill may only be used on one target at a time, though the target of the ability may be changed on a 3 count. This skill will last at most 1 minute per the Bard's level. This skill is usable once per day per purchase."},
    {name:"Song of Heroism",    cp:120, tier:12, desc:"Duration: Concentration. This Occupational Ability allows the Bard to perform a masterpiece of heroic inspiration, leading allies to victory and bringing life back to the injured. In order for those listening to become heroic, they must consider the Bard an ally (that is to say, do not wish them harm), and have heard the song for at least 30 seconds. Once the requirements have been made all those that can hear the Bard will become inspired, gaining +2 Strength, an aura on their Spirit allowing them to swing any weapon for magic damage, and finally they become immune to the effects of Fear. To further this, all those who are under the effects of this song and are within 10 feet of the Bard, will regenerate 1 Body every minute so long as they are conscious or semi-conscious. This song has no effect on those in their Bleed or Death Counts. To activate this song, the bard must state \"Innate Song of Heroism!\" and if possible, shouts it often to inform those around them that the song is still active. If the Bard's concentration is broken, the bard must then shout \"Heroism Over!\" The Song of Heroism will not stack with other bard songs. This skill is usable once per day per purchase."},
  ],
};

// Build occupational ability skills for the current occupation
function getOccAbilitySkills(){
  // If vocation selected, use vocation abilities instead
  const vocSkills = getVocationSkills();
  if(vocSkills !== null) return vocSkills;

  if(!s.occupation) return [];
  const abilities = OCC_ABILITIES[s.occupation];
  if(!abilities) return [];

  return abilities.map(ab=>{
    const prereqs = [];
    if(ab.tier > 3){
      const prevTierAb = abilities.find(a=>a.tier===ab.tier-3);
      if(prevTierAb) prereqs.push({name:prevTierAb.name, minCount:1});
    }
    return {
      name: ab.name,
      costs: null,
      cp: ab.cp,
      frag: 0,
      maxPurchases: ab.maxPurchases || DEFAULT_MAX,
      bodyBonus: ab.bodyBonus || 0,
      strBonus: ab.strBonus || 0,
      occupational: true,
      _occAbilityTier: ab.tier,
      _vocationAbility: true,
      prereqs,
      desc: ab.desc,
    };
  });
}

// VOCATIONS — optional, cost 150 frags, replace occupational abilities
// occupations: which occupations can take this vocation (any occupation if empty)
const VOCATIONS = {
  "Archer": {
    fragCost: 150,
    occupations: [], // available to all
    prereqs: "Weapon Group Proficiency: Medium or Large and Weapon Specialization (Specific or Group).",
    lore: "The Archer vocation is a ranged specialist, augmenting their ability to use bows, crossbows and thrown weapons. A straightforward set of abilities, the Archer seeks to increase the damage their ranged weapon does and attempts to keep the distance between themselves and their target.",
    abilities: [
      {name:"Arrow Dodge",     cp:30,  tier:3,  desc:"Once per day per purchase the Archer may use a \"dodge\" defense against a single arrow, bolt, or thrown weapon that hits them, negating the attack as per the dodge skill. It will not function against surprise attacks. The call for this ability is \"Innate Arrow Dodge!\""},
      {name:"Stand and Deliver",cp:60, tier:6,  desc:"Stand and Deliver allows the Archer to steady which and fire a more damaging ranged attack. The Archer must plant both feet (crossbow users may also choose to kneel or brace their crossbow on a table or stable object) and state \"Innate Stand and Deliver\". The Archer may add +2 to their damage with their ranged attacks for as long as they maintain the position. Moving from that position or taking damage of any kind will cancel this effect and they must wait at least a minute before they can use it again. Using any type of Dodge skill or spell protections will not break this effect. This ability may be purchased multiple times. Each purchase increased the damage modifier by an additional +2. (+2 for one purchase, +4 for two purchases, etc.)."},
      {name:"Maim",            cp:90,  tier:9,  desc:"At 9th level, an Archer can fire a projectile that when struck will cripple the target's defenses temporarily. For 60 seconds after being hit with a Maim attack, the victim will receive x2 damage from all physical sources and be affected by a \"Swampwalk\" effect, forcing them to pause for 3 seconds between each step of movement. The archer must call out \"Innate <damage> Maim!\" and the attack must hit Body to function. If the Maim attack misses, the skill is lost. This ability is useable once per day per purchase."},
      {name:"Death Arrow",     cp:120, tier:12, desc:"Death Arrow allows an Archer to concentrate and focus on a shot with the hopes of killing their target in a single strike. After 10 seconds of concentration the Archer will be ready to fire. If the 10 seconds are interrupted the archer must begin the 10 seconds again, but the skill will not be wasted. Only releasing the missile will activate the skill. After the preparation time the Archer may fire with a call of \"Innate <damage> Death!\", with the damage amount being their normal damage call. The damage must strike Body points to take effect. If it does, the target will immediately drop into their Death Count as if struck by a death effect. If the attack misses, the Archer may fire a second Death Arrow within 10 seconds. Regardless of whether that attack hits or misses, the ability will be used up. It is usable once per day per purchase."},
    ]
  },
  "Artisan": {
    fragCost: 150,
    occupations: [],
    prereqs: "Level 10 Tradesman or Level 5 Tradesman and 5 levels of production skills (total).",
    lore: "Artisans seek to be masters of their trades and crafts, and of merchandising in general. Most Artisans have focused on earning wealth and fame through trade and manufacturing rather than adventuring. Skilled marketers and vendors, streetwise and charming, Artisans prove that there's more ways to earn fame and fortune than spell and sword.",
    abilities: [
      {name:"Treasure Hunter", cp:30,  tier:3,  desc:"Artisans have a nose for gold. Treasure Hunter allows them to sense gold and silver at will by touching the target and performing a 3 count – \"Innate Sense Coin 1, Sense Coin 2, Sense Coin 3.\" If the target has gold or silver coins in their possession they must respond with \"Here!\" in a normal speaking voice. The sense and response calls are considered out of game. Doing this does not let the Artisan know the exact pinpoint location of the gold, only that it is on the person. In game, this is the Artisan hearing the familiar jingle of coins and watching the target's body language as they move. This has no effect on coins not on a person but will work on corpses and immobile targets. Eg: It cannot be used to detect gold inside chests.\n\nTreasure Hunter also helps Artisans loot bodies. Once per day per purchase, the Artisan may touch a target that is unconscious, dying or dead, and which they have already used Sense Coin on within the 3 seconds, and ask out of game one of the following questions: \"Innate Treasure Hunter – do you have any coins / magic items / gems / catalysts on you?\" Doing this will instantaneously loot the target of all tags of that type (coin, magic item, gem or catalyst). The target must hand over all the tags of that type on their person, regardless of whether the target has any ranks of Looting."},
      {name:"Bribe",           cp:60,  tier:6,  desc:"In times of dire need, an Artisan may slip out of dangerous situations by offering up a charm-infused bribe. If the Artisan offers a target an item worth at least 1 gold piece or 10 RM in base creation value which they have created themselves, they may be able to save their skin. While holding out the item the Artisan must declare \"Innate Magic Bribe!\" and strike the target with a spell packet. If target defends against the Bribe, for every 3 gold or 50 RM in base creation value of the item, the Artisan may use an \"Innate Echo!\" effect in a second attempt. If the initial Bribe is resisted but the Echo is successful, the original Bribe attempt will be temporarily forgotten – its memory suppressed by the glamour of the item being offered a second time. If the Bribe succeeds, the target will not be aware that they are being charmed until the effect wears off.\n\nWhen a Bribe is successful, the Artisan has 3 seconds to place the item on the ground or in the target's hands, as decided by the target. The target will then take the item. For the next minute, the target cannot take hostile action against the Artisan unless the Artisan initiates any hostile actions toward the target. Actions are determined to be hostile or not by the target of the Bribe. The target will not necessarily trust the Artisan; they will simply avoid initiating hostilities. Bribe has no effect against mindless and Undead creatures and it can be resisted the same way as a magical charm. Items made with conventional production skills may be used for this skill. This skill can be used once per day per purchase."},
      {name:"Magnum Opus",     cp:90,  tier:9,  desc:"For each purchase of Magnum Opus an Artisan may choose to augment either their Production or Tradesman skills. At Logistics, they can craft a single item through their Production skills using any type of RM. Alternatively, the Artisan can focus on their Tradesman skills and increase the value of one item created by 3 gold. No matter which of the abilities is used, a catalyst will be generated. This catalyst must be a physical tool that was used somehow in the item's creation. Both its type and emotion radiated may be decided by the Artisan. An Artisan may choose to stack uses of this ability to create a single, even more expensive item. For example, they could use 3 uses of this ability to increase the value of the item by 9 gold. This skill may be used once per event (at Logistics) per purchase."},
      {name:"Vault",           cp:120, tier:12, desc:"When an Artisan reaches this level of skill they may call in favours to build the ultimate strong-room free of charge – the Vault, a 10'x10'x10' square room with a ritual-level magical barrier. The Vault must be phys-repped by a tent or building, or the inside of a tent or building. The Vault has one door and one key, which is spirit linked to the Artisan. The Vault may have windows, but even they will be magically protected. This magical barrier is special and cannot be breached or dispelled by any means, including such powers as Passwall, Counter Magic or ritual Destroy Magic, other than Shaper approved abilities. Only those with a spirit-linked key may enter the Vault. For each additional purchase of Vault an Artisan may increase the Vault's size by 10'x10'x10', may add an additional spirit-linked key to one additional person and may add another door if desired. All lock(s) and key(s) will be tagged and have matching numbers assigned to them. If anyone with a spirit-linked key suffers a final death the key will spirit link to the first person who touches it, but the magic will permanently dissipate after 5 days. If the Artisan dies a final death, the Vault loses its magic and becomes a normal building.\n\nThe Artisan may only have one Vault at a time. If desired, the Artisan can deactivate their Vault and create another somewhere else. If a Vault is deactivated, the Artisan may not make another for 5 days – favours take time to cash in. It takes 10 minutes to create a new Vault. A Vault cannot be constructed around a person or creature. When the new Vault is created, the Artisan will receive a number of new keys equal to their purchases of this ability. The old keys will become normal keys which do not unlock anything."},
    ]
  },
  "Battle Mage": {
    fragCost: 150,
    occupations: [],
    prereqs: "Sphere of Magic: 2nd or Spell Slot: 4th Circle.",
    lore: "The Battle Mage Vocation allows a spell caster to improve their Battle Magic spells and create temporary magic items. This Vocation is popular with those who prefer to focus on battle spells and less on ritual magic, or those who simply want to increase the potency of their magic. Hybrid classes such as templars and wytch hunters might also find the skills in this vocation useful.",
    abilities: [
      {name:"Amulet",          cp:30,  tier:3,  desc:"This class ability allows the Battle Mage to enchant any item smaller than an apple to store 1 Battle Magic spell, 3rd level or lower. The spell must be cast into the item and remains there for 5 days. Although the spell must be cast, it is immediately returned to the Battle Mage's memory and is not expended from the spell slot. One Amulet may be created per purchase of this ability. Once created, the Amulet may be used by anyone by stating \"Activate: <Spell Name>\". Although the Amulet detects as magic and is affected by dispel magic, it can be destroyed by normal means. Only one Amulet can be active per purchase of this ability, when the spell within a Amulet is cast, that Amulet's state returns to that of the normal object originally used. This skill may be used once per day per purchase."},
      {name:"Maximize",        cp:60,  tier:6,  desc:"In order to use this class ability, the Battle Mage must state \"Innate Maximize:\" before a spell incant for a spell that involves damaging or healing with numerical amounts and a duration of instant. If the spell is successfully cast, those healing or damaging numbers are x2. The Battle Mage must state the total number at the end of the incant. This is extremely taxing to the Battle Mage and after the spell is cast they are stunned for 5 seconds and cannot use any skills whatsoever. While stunned, the Battle Mage is unable to take any action, including blocking, moving and the use of skills, minus the ability to call \"interrupt\" against killing blows. They may also interrupt any counts against them. Automatic defenses such as Shield Magic will still operate, but ones requiring conscious thought such as Advanced Shield Magic will not.\n\nMaximize may be used once per day per purchase and if the spell is miscanted the maximize ability will be wasted."},
      {name:"Twin Spell",      cp:90,  tier:9,  desc:"When casting a Battle Magic spell and using Twin Spell, the Battle Mage is able to throw two packets simultaneously, either two packets in one hand or a packet in each hand. Both packets are considered the same spell and either packet will do what the spell would normally do. No more than 1 second can pass between throwing both packets. For defensive purposes they are considered two separate spells. In order to activate this class ability, the Battle Mage must state \"Innate Twin Spell:\" before the incant. Although considered two spells, only one spell is removed from the mage's memory and spell slot. If the spell is miscanted, the Twin Spell ability will be wasted.\n\nThe magical energy required to duplicate a spell is taxing on the mind, the Battle Mage will thus be stunned for the next 5 seconds after using this ability. The effects of this stun are identical to those of Maximize. Twin Spell can be used once per day per purchase."},
      {name:"Wizard Staff",    cp:120, tier:12, desc:"Starting at 12th level, the Battle Mage is able to create a powerful staff for their own use. This process takes 10 minutes of concentration and requires a staff to imbue with this power. Any type of staff may be used. During that creation, the Battle Mage must choose to align their staff with any one spell sphere they have purchased. Once created the staff will function as a magic weapon in the hands of its creator and will swing for magic. Also, the sphere they have chosen to align with their staff no longer requires the use of incants to cast. Those incants are replaced with \"Magic <Spell>\", eg: \"Magic Swarm\". The staff must be in the hands of the Battle Mage for all abilities to function, it will act like a simple staff in the hands of anyone else. If a Battle Mage wishes to align their Wizard Staff to a different sphere the same staff may be used but the 10 minutes of concentration must be completed again. For purposes of destruction, the staff is considered whatever type of staff was used to create it and can be broken like one. A Wizard Staff will last 5 days before the magic fades, returning it to its previous state. A Wizard Staff may be created once per day per purchase, but only one may exist at any time."},
    ]
  },
  "Blood Reaver": {
    fragCost: 150,
    occupations: [],
    prereqs: "Self Mutilate, Anatomy and First Aid.",
    lore: "As their name implies, Blood Reavers collect blood from magic users and use it as the source of their power. The most proficient Blood Reavers can draw forth magic spells and abilities and can make their enemies more vulnerable to their attacks. Blood Reavers come in many forms, from the scholarly mage studying the fringes of magical theory to the shamanistic orc who rips magic from the minds of their enemies. Woe be to those who cross the path of the Wytch who studies this art.",
    abilities: [
      {name:"Blood Harvest",   cp:30,  tier:3,  desc:"By touching a target and stating, \"Innate Magic Blood Harvest\", a Blood Reaver can instantly magically transfer 1 litre of blood from the target to an empty vessel which is waiting in their off hand. The Blood Reaver's hand will briefly glow red and cause 1 Magic Body damage to the target. If the damage is negated, Blood Harvest will fail. Blood collected in this manner will last for 3 months, not the standard 1 month duration. This ability can be resisted via Resist Magic, Shield Magic and other forms of defence against magical spell-like touch-casts. If used against targets without blood or used without an appropriate empty vessel, it will have no effect and the ability will be used up. If successfully used, the tag for Blood Harvest should be signed by the target OOG when next possible, and the tag must be affixed to the vessel used to hold the blood until it is used or expires. This ability is useable once per day per purchase."},
      {name:"Master of Vitae", cp:60,  tier:6,  desc:"The Blood Reaver can now utilise the power they've been studying. By stating \"Innate Master of Vitae\" while holding 1 litre of blood from a specific target in their off hand, the Blood Reaver will have 10 minutes to physically touch that same living target and state \"Arcane Blood Infusion\". Doing so will consume the blood, heal the Blood Reaver to full Body and will reset the duration of any active Battle Magic spells on the Blood Reaver as if they had just been cast. A Blood Reaver cannot use their own blood for this ability and must use the blood of a target which is capable of resurrection. This ability is useable once per day per purchase."},
      {name:"Blood Boil",      cp:90,  tier:9,  desc:"By possessing at least one litre of a target's blood, the Blood Reaver may cause that target to become vulnerable to the Blood Reaver's attacks. To activate this ability the Blood Reaver must hold their target's blood in one hand (within a container) while pointing at the target and stating, \"Arcane Power Word Directed: Blood Boil\". Unless the target resists the ability, all physical attacks made by the Blood Reaver for the next 10 minutes will have their damage doubled against the target. This damage should be calculated by the target, as the Blood Reaver might be unaware of duration or resistances. In addition, any Battle Magic spells successfully cast by the Blood Reaver against the target will gain the \"Penetrating\" prefix. Activating this ability will consume the blood, even if the target successfully resists. This ability is useable once per day per purchase."},
      {name:"Tap the Vein",    cp:120, tier:12, desc:"Tap the Vein allows the Blood Reaver to steal a memorised spell or magical ability from the mind of a target that has a functioning metabolism which uses blood. To do so, the Blood Reaver must touch a target within their Bleed count and state, \"Arcane Tap the Vein – what is the highest level spell you have memorized?\" If the target does not resist and has a spell memorised, they must inform the Blood Reaver OOG what their highest level spell is and provide the spell tag for it. If the target has multiple spells at the highest level they may decide which to offer. The offered spell is then lost from the memory of the target and the Blood Reaver has 1 hour to cast the spell by stating \"Magic <spell name>\". This ability will function with all Battle Magic spells, including all spells from spheres from the Soul Frag book.\n\nIf the target of Tap the Vein has no spells memorised, the Blood Reaver may ask them OOG if they have any hourly or daily natural magical abilities. If so, the target will inform the Blood Reaver of up to 3 magical abilities they possess and the Blood Reaver may select one to steal. The target will lose a use of this ability and the Blood Reaver will have 1 hour to use the ability by stating \"Magic <ability name>\".\n\nA Blood Reaver may choose to use Tap the Vein to learn the target's highest level spell or hourly/daily natural abilities without stealing them.\n\nIf the target has no spells memorised or magical abilities, Tap the Vein will fail but will not be used up. Tap the Vein does not function against occupational abilities. This ability is useable once per day per purchase."},
    ]
  },
  "Brew Master": {
    fragCost: 150,
    occupations: [],
    prereqs: "Level 5 Create Alcohol or Level 5 Alchemy.",
    lore: "The Brew Master Vocation empowers its user through intoxication and the power of alcoholic drinks. The Brew Master's abilities either require its user to be drunk, or they cause intoxication through their use. Not uncommon among the Dwarves, Orcs and Einher, it's still possible to find a Brew Master in almost any tavern across Maud'madir.",
    abilities: [
      {name:"Iron Gut",        cp:30,  tier:3,  desc:"Possessing Iron Gut gives the Brew Master x2 maximum Stamina. Also, while the Brew Master's Stamina is lower than maximum they gain +5 Body and all hand to hand damage is increased by +2 damage. Iron Gut may only be purchased once.", maxPurchases:1},
      {name:"Mixologist",      cp:60,  tier:6,  desc:"The Mixologist Class Ability allows its user to spend 1 minute concocting a special alcoholic drink. There are three different types of drink that can be created through Mixologist:\n1) A potent beverage that does 20 points of Stamina damage and has 3 servings.\n2) A soothing drink that does 10 points of Mending for any creature that can drink it, but also does 4 Stamina damage.\n3) A flaming bottle of alcohol which explodes on impact when thrown (packet delivered or boffer-safe bottle rep) and does 10 Elemental Fire damage. \"10 Elemental Fire!\" is the call when thrown.\nA Brew Master can create 1 drink total per day, per purchase. Each drink lasts 5 days before becoming inert. These drinks cannot be time-extended."},
      {name:"Firebreathing",   cp:90,  tier:9,  desc:"At 9th level, a Brew Master can ingest pure alcohol then spit it out and light it on fire. This is a packet delivered attack that does 25 points of Elemental Fire damage. Even though the alcohol is never swallowed it is still potent enough to cause 5 Stamina damage to the Brew Master each time Firebreathing is used. Firebreathing may only be used once per day per purchase and the call is \"Innate Firebreathing – 25 Elemental Fire!\""},
      {name:"Drunken Master",  cp:120, tier:12, desc:"When a Brewmaster with Drunken Master reaches 0 Stamina, instead of becoming a slurring mess of intoxication like everyone else, they may choose to enter the eye of the storm. At 0 Stamina they may activate Drunken Master, stating \"Innate Drunken Master\". A Brew Master may also choose to activate this ability by taking 40 Stamina damage in less than one minute, which will reduce them to 0 Stamina regardless of their true total stamina. If they activate this ability, for 10 minutes they gain a 2 Normal threshold, a +1 Strength, +5 damage with hand to hand, 2 Parries with hand to hand, an immunity to Charm effects, an immunity to further stamina damage and +25 Body points. When the 10 minutes expires the Brew Master returns to 1 Stamina. As normal, a Drunken Master cannot use other skills while they are at 0 Stamina. This ability may be used once per day per purchase."},
    ]
  },
  "Bounty Hunter": {
    fragCost: 150,
    occupations: [],
    prereqs: "Sap and Ambidexterity.",
    lore: "Bounty Hunters are specialists in the art of capture or killing of criminals and fugitives for bounties. Some Bounty Hunters will hunt to kill and others will track, then capture people to extract information or a reward. Most Bounty Hunters operate in a grey area between the laws. Their motivations vary – some do the work for coins and will take bounties from anyone, while others are politically motivated or work with the law to assist in the apprehension of criminals.",
    abilities: [
      {name:"Mercy",           cp:30,  tier:3,  desc:"This ability allows a Bounty Hunter to add the suffix \"Mercy\" to the end of a weapon swing call. Eg: \"4 Normal Mercy\". A \"Mercy\" suffix means that the attack will not drop the target below 0 Body regardless of how much numerical damage it does. This ability may be combined with other weapon skills. This ability may be used at will. Note that Mercy will not prevent damage from other sources."},
      {name:"Bola",            cp:60,  tier:6,  desc:"Bolas are a special thrown item designed to trip up a target's legs and force them to the ground. This ability is delivered via a spell packet, which represents multiple weighted balls attached together with rope. The call is \"Innate Bola – Physical Snare\". If successfully struck by the spell packet, the victim's right foot will be stuck to the ground as per the Snare spell. A target can only be affected by one Bola at a time. The Bounty Hunter must be holding a Bola phys-rep in their off hand at the time of the throw. This ability can be used at will so long as the player has 1 Bola tag for each Bola thrown. A Bola may be cut through with a two-minute count and may also be ripped free from by the victim if a +2 or greater strength is used, both of which will destroy the Bola. Ripping free will cause the victim to take 2 points of damage straight to Body regardless of threshold. It takes three seconds to rip free from the Bola. Bola tags can be reused if the Bola spell packet is recovered in game and has not been destroyed. A Bounty Hunter can recover the Bola if it misses the target, or if they remove the Bola from the victim on a 5 count. Bola tags cost 20 RM of blacksmithing material to create. Bounty Hunters can make a number of Bolas up to their number of purchases of this ability during Logistics. This does not require the Blacksmithing skill. Bolas expire 2 years after creation. Bolas are considered tools, not weapons, and cannot be enchanted, augmented, made of silver, etc. Bola phys-reps should be a string or small rope with a ball at each end and should never actually be thrown."},
      {name:"Smoke Bomb",      cp:90,  tier:9,  desc:"This area-of-effect blindness attack is activated by the Bounty Hunter throwing a spell packet at their feet and declaring \"Innate Alchemical Smoke Bomb!\" This will blind anyone within a 10-foot radius of the Bounty Hunter for 10 seconds, except for the Bounty Hunter. This is usable once per day per purchase."},
      {name:"Impale",          cp:120, tier:12, desc:"This ability causes a tagged throwing weapon to strike a vital point on the target, causing extreme pain which prevents the victim from using any tag skills until the victim performs a 10-second count to remove the weapon while not moving, or until 60 seconds have passed. The call for this is \"Innate 5 Body Impale\". Until the weapon is removed or the time expires, the victim can move no faster than 1 step per second. Removing the weapon manually causes an additional 1 Body of damage. Impale will only function against living targets and those that feel pain. It cannot be combined with other skills and the damage cannot be increased, though specific damage types such as \"Silver\" or \"Magic\" may be called based on the weapon used. This ability is usable once per day per purchase."},
    ]
  },
  "Conqueror": {
    fragCost: 150,
    occupations: [],
    prereqs: "Slay with a 2-handed weapon (other than simple weapons). All Conqueror abilities require the use of a two-handed melee weapon (other than simple weapons).",
    lore: "Conquerors are larger than life heroes who charge into battle and leave strategy to the bookworms. They fight the biggest monsters, earn the most glory and believe that every minute you spend talking you could be punching the bad guy in the mouth instead. They believe that shields are for cowards, hate monologues and think brute force is the only effective problem solver. They specialize in two-handed weapons and kicking ass.",
    abilities: [
      {name:"Grit",            cp:30,  tier:3,  desc:"This ability allows the user to resist one physical attack that would destroy, detach, disable or break one of their limbs, once per day per purchase."},
      {name:"Ego Armour",      cp:60,  tier:6,  desc:"While wearing 20 or fewer points of physical armour, a Conqueror may state \"Innate Ego Armour\" to double their physical armour points using this ability. This is not magical in nature. It simply makes the armour being worn twice as effective. Each purchase of this ability will raise the maximum armour that this ability can be used with by 5. Ego Armour cannot be repaired once damaged. If any armour is physically removed or put on, the effect will end. Otherwise, the additional points will remain until destroyed or until skill reset. This ability does not stack with itself. This ability is useable once per day per purchase."},
      {name:"Breakthrough",    cp:90,  tier:9,  desc:"This ability only works against targets with shields. The Conqueror must state \"Innate Physical Breakthrough\". They can then swing, once, for 40 points of damage to the shield itself. The swing must strike the shield itself. Regardless of whether the shield is destroyed by that damage, the target must drop it. If the shield is destroyed by the damage, the target will also be stunned for 5 seconds. This ability is useable once per day per purchase."},
      {name:"Rallying Cry",    cp:120, tier:12, desc:"After yelling \"Innate Rallying Cry. Blood and glory!\", the Conqueror will gain +5 damage with all Conqueror-appropriate weapons for the next minute. Anyone else who hears the shout who is also using Conqueror weapons or who is a Conqueror themselves will also gain +5 damage to their next swing with a Conqueror weapon, within the next minute. This will affect both friends and foes. This ability does not stack with itself. This ability is useable once per day per purchase."},
    ]
  },
  "Shaman": {
    fragCost: 150,
    occupations: [],
    prereqs: "Level 7 Mysticism or Spell Slot 5th Circle (Nature sphere).",
    lore: "Shamans are practitioners of mysterious arts which link themselves to the spirits of the animal kingdom, called 'Animists'. Almost every culture on Maud'madir has versions of Shamans within it – mystical seers, wise storytellers and potent allies. To the Wild Elves they are called 'Wildspeakers', communing with nature directly. Einher Shamans are distrusted but highly valued for their wisdom and divination. Goblin Shamans are powerful 'Warcallers' in battle, augmenting the strength of their Warband. Some Shamans are reclusive, interacting with only their own kin or when aid is directly requested. Other Shamans take the role of advisors or soothsayers.\n\nShamans tend not to take direct action. Instead, they aid those who join them by sharing their wisdom or empowering them through magical Fetishes. The Shaman's closest allies are called 'Braids', which Shamans name. Braids are almost always the same race as the Shaman, although rare exceptions may be made. No person can ever be a member of more than one Braid at a time. If a Braid member ever becomes a Shaman they will be removed from the Braid to forge their own path. Likewise, if a Braid or Shaman's Fetish is not Empowered for a year, their connection to the Braid will fade and they will be removed from it. If the Shaman finals, the Braid connection disappears.",
    abilities: [
      {name:"Rite of Weaving/Unweaving", cp:30,  tier:3,  desc:"This rite allows a Shaman to induct new members into their Braid, build them a Fetish, and Empower a Braid member's Fetish when its power fades. The first time a Shaman uses a Rite of Weaving they will do so for themselves, creating their own Fetish and becoming a true Shaman. Fetishes are sacred items that should be personal and important to the Braid member. Creating or Empowering a Fetish requires the Shaman to perform a ceremony at least 10 minutes long. The specifics of the ceremony will depend on the Shaman's culture, race and style.\n\nIf the Braid member is new, the Shaman will decide on an Animist animal for the new Braid member based on their personality and will present them with their Fetish. This Fetish must be made by the Shaman and should be smaller than a child's doll, but otherwise can be anything. The Braid's Animist may be any land-based animal and is considered to be either a Predator or a Prey Animist. The animal must be a natural, non-magical animal – bears are acceptable, basilisks are not. The Shaman states \"Innate Rite of Weaving\" and attaches the tag for their Rite of Weaving to the Fetish. Once the ceremony is complete, this new Fetish will grant Animal Kinship with that animal group for the Braid member at will. Animal Kinship will cause any animal of that group (eg: all 'cats' for a Lion Animist) to see the Braid member as friendly. It is used by stating \"Innate Magic Animal Kinship <animal>\". Animals in this group will not initiate hostilities against the Braid member but will respond to hostility normally. A Shaman may induct a new Braid member by creating a new Fetish for them once per day per purchase.\n\nThe Rite of Weaving may also be used to empower expired Fetishes at will by the Shaman. Being inducted into the Braid is considered a lifelong commitment, but the power of a Fetish will last for 5 days before needing to be empowered again. Should the Fetish be destroyed or leave their person, membership in the Braid continues, but the Rite of Weaving must be performed again to create a new Fetish. Empowering an existing Fetish does not use up a daily use of Rite of Weaving, but replacing a missing Fetish does. A Shaman may not empower another Shaman's Fetishes. A Shaman can have up to one Empowered Fetish per level of the Shaman, excluding themselves.\n\nA Shaman can sense their own Braid members with Empowered Fetishes. This can be accomplished by stating \"Sense Braid <Braid Name>!\". All Braid members with Empowered Fetishes must respond \"Here!\" out of game. This power may be used at will by the Shaman and once per day by Braid members.\n\nA Shaman can remove Braid members who have become disloyal – by force. To remove a Braid member, the Shaman must kill them and eat their heart to reclaim the Animist within it. The Shaman empowers each of the other Braid members with Empowered Fetishes who participate in this reclamation with +2 Strength for one hour once the body vanishes to resurrect or dies a final death. Either way they are removed from the Braid.\n\nFinally, Shaman are vulnerable to betrayal their own Braid members. A Shaman who is killed, directly or indirectly, by one of their Braid members who shares their race will have a 50% chance of taking two deaths upon resurrection. If the Braid member who committed the betrayal is of another race, this automatically raises to two deaths. This occurs even if the Shaman is unaware of the betrayal. The death must have been intentionally caused by the Braid member. The Braid member should report this to the Shaper team if the Shaman is unaware. The Shaman is vulnerable to this effect for up to one year after the betrayal."},
      {name:"Rite of War",     cp:60,  tier:6,  desc:"This ability allows the Shaman to strengthen and empower their Braid by banging on war drums, singing, or chanting. At the beginning of the Rite, the Shaman senses their Braid members with the Rite of Weaving. For each Braid member that the Shaman senses, the Shaman can resist any one physical strike or hostile Battle Magic spell. While the Rite of War is going on, all Braid members with Empowered Fetishes within earshot and line of sight will gain a power based on their Fetish, as described below. While the Rite of War is active, the Shaman can take no other action besides walking and performing the Rite. The Shaman cannot stop for more than 3 continuous seconds or the rite will end. To initiate a Rite of War the Shaman must state \"Innate: Rite of War!\" and then begin their performance. This rite is usable once per day per purchase and lasts for up to ten minutes.\n\nPredator: Predator Braid members with an Empowered Fetish participating in the Rite of War gain temporary hide armour worth 5 Armour Points. This armour increases by 5 AP for each Braid member, other than the Shaman and themselves, who participates in the Rite of War who has an Empowered Fetish. This armour functions like normal armour except that it cannot be refitted or repaired. To repair their natural hide, the Braid member must heal it as though it were Body points.\n\nPrey: When any Braid member with an Empowered Fetish falls into their Bleed or Death Count during the Rite of War, Braid members with Prey Animists may touch their fallen bodies and state \"Innate Spirit Walk 1, Innate Spirit Walk 2, Innate Spirit Walk 3\". This transfers the body in spirit form to the Shaman's location by calling on the target's Animist. Upon reaching the Shaman the body, including its possessions returns to the material world with the same Spirit Walk count. During this travel time, their Bleed or Death count will continue and their body cannot be Lifed because their spirit is not in it. If the spirit cannot find or reach the Shaman, they will return to their body. Their spirit will pass through non-magical barriers if any block their route to the Shaman, but must travel around magical barriers. This ability may be used at will by Prey Braids with Empowered Fetishes during the Rite of War."},
      {name:"Rite of Vision",  cp:90,  tier:9,  desc:"The Rite of Vision is a one minute ceremony that allows the Shaman to become a ghostly version of their Animist for a period of time. This ability may be used once per day. For each Braid present in the ceremony with an Empowered Fetish, the Rite of Vision becomes more powerful.\n\nTo begin, the Shaman must create a new Fetish of their mortal form, the size of a child's doll or larger. This Fetish will take the place of their body and has 1 Body point. All damage to this Fetish will cause the Shaman's physical body to fall into its Death Count when the Shaman returns to it. If there is no Marshal present when the Fetish is damaged, the killer must find a Marshal and inform them that they damaged the Fetish. The Marshal will then inform the Shaman. The Shaman's character sheet should be left with the Fetish along with the tag for the Rite of Vision.\n\nOnce their Fetish is prepared the Shaman will state \"Innate Rite of Vision!\". This will manifest a shimmering, transparent version of their Animist which they now possess. The Shaman's physical body and all items on them will be absorbed into their special Fetish. The Fetish cannot be moved by any means until the Shaman returns to it. The ghostly Animist is now controlled by the Shaman and all that it experiences will be experienced by the Shaman. The Animist has a silver threshold, 25 Body points, two claws which swing for 5 Normal each, and 25 hide Armour Points. This armour functions like normal armour except that it cannot be refitted or repaired. To repair their natural hide, the Shaman must heal it as though it were Body points. The Shaman may speak in this form.\n\nThe Shaman may touch cast one memorised spell through their claws for each Braid member that participated in the Rite of Vision. No other skills or abilities may be used and no items of any kind may be carried by the Animist. This possession will last for 10 minutes per Braid with an Empowered Fetish who participated in the Rite. When the duration expires or the Animist reaches 0 Body, the Shaman's spirit will return to their Fetish and their body will reform, along with anything it was wearing. If the Animist was destroyed by reaching 0 Body, when the Shaman's spirit returns to its body they will be at 2 Body. For the next hour, 2 Body will be their maximum Body. If a Shaman's special Fetish suffered damage during the Rite of Vision, upon returning to its body the Shaman enters their Death Count."},
      {name:"Rite of the Monolith", cp:120, tier:12, desc:"This powerful Rite will create a sacred area for the Shaman and their Braid, dominated by a large stone or monolith. The Shaman must perform a 1-hour roleplay rite to create the Monolith. This area will encompass a space 20 feet by 20 feet. The stone must be at least 5 feet but does not need to be real stone out of game. A Shaman may only have one active Monolith at a time. The Shaman can destroy their Monolith by doing 50 pts of damage to it. They may then create another somewhere else, after 5 days.\n\nThe area around the Monolith will function as a resurrection circle for the Shaman's Braid members who have Empowered Fetishes. Resurrections may be performed by the Shaman but will also happen automatically if they are not there. A Shaman may construct a special Spirit Mask for this purpose. This mask must be at least 1 foot long and 8 inches wide, made of wood or bone in game and have large adornments. It should not be able to be mistaken for an NPC mask. The Shaman's Animist animal should be represented in some manner on the mask. If the Shaman resurrects a Braid member while wearing this Spirit Mask and tells that Braid member a resurrection dream themed around them being their Animist, the resurrection will only take 5 minutes. The mask will only function for resurrections performed on Braid members within the Monolith area.\n\nOne per day per purchase, a magic, transparent barrier can be created around the Monolith area. It will last for 1 hour for every Empowered Fetish present within the area when activated. The entire barrier may be temporarily disabled at any time when active by the Shaman or any Braid members with Empowered Fetishes by stating \"Barrier up/down!\" at will. While the barrier is up, it behaves like a Circle of Protection. The magic of this barrier is considered ritual level.\n\nAny sentient creature capable of resurrection may be sacrificed upon the Monolith. If the creature suffers a Killing Blow and has their heart removed, any Braid members, including the Shaman, who eat a piece of it will gain +2 Strength for one hour once the body vanishes to resurrect or dies a final death. This power may be used once per Braid member or Shaman per day."},
    ]
  },
  "Stalwart": {
    fragCost: 150,
    occupations: [],
    prereqs: "Heavy Armour, Shield, and a Parry (Specific or Master).",
    lore: "The Stalwart vocation trains a character to master the use of a shield and in turn become a defensive force. Although one does not have to be a warrior to learn this vocation, its purpose is to defend the user – and others – from physical harm. This vocation is popular with guards, soldiers and those who have something of value they want to protect. Oaths and chivalry are not a requirement as the name might suggest, however being duty-bound is not uncommon to those who would risk their lives to protect others or ideals.",
    abilities: [
      {name:"Shield Parry",    cp:30,  tier:3,  desc:"This skill allows a Stalwart to call an \"Innate Shield Parry!\" defense to any physical attack that strikes their shield, once a day per purchase. All normal parry rules apply. This ability does not allow the Stalwart to parry with their weapon; the incoming strike must successfully strike their shield."},
      {name:"Conviction",      cp:60,  tier:6,  desc:"The Stalwart's Conviction ability allows them to grant themselves +10 temporary Body points once per day per purchase, stating \"Innate Conviction\". These Body points cannot be stacked with other temporary Body point bonuses (they will remove and over-ride the previous) except with other activations of this ability. These Body points cannot be healed and are taken off first when damage is struck to Body. These extra Body points will fade after exactly 24 hours have passed."},
      {name:"Fortress",        cp:90,  tier:9,  desc:"When Fortress is used, the Stalwart gains the ability to activate a defensive stance that grants the Stalwart a 5 Normal threshold and +40 armour points that remain as long as the Stalwart keeps one foot planted. The Stalwart also gains an immunity to fear effects during this time. While in Fortress, the Stalwart is immune to Strength-based pushing, magical or physical.\n\nThis ability can be activated once per day per purchase by planting a foot and stating \"Innate Fortress!\". When the defensive stance ends by the planted foot being raised or moved (it may swivel to change facing), the Stalwart needs a respite due to the sheer amount of physical and mental energy required. For 1 minute after Fortress ends, the Stalwart possesses -2 Strength and is unable to use any skills that have limited uses."},
      {name:"Imbue Shield",    cp:120, tier:12, desc:"Imbue Shield allows a Stalwart to spend 10 seconds of uninterrupted time imbuing a shield of any type with defensive power. This is done by concentrating on the shield for 10 seconds then stating \"Innate Imbue Shield!\". Once imbued, the shield allows any Battle Magic spell or Battle Magic level magical ability with the same name as a spell that strikes it to be \"resisted\" for 1 hour by simply stating \"Innate Resist!\" During this hour the Stalwart may also \"reflect\" one Battle Magic spell or Battle Magic level magical ability with the same name as a spell that strikes the shield back upon the caster by calling out \"Innate Reflect!\". If the shield is no longer equipped, the ability ends. The imbued shield may only be used by the Stalwart who activated it. Imbue Shield may be used once a day per purchase."},
    ]
  },
  "Swashbuckler": {
    fragCost: 150,
    occupations: [],
    prereqs: "Ambidexterity, plus either a Slay (Specific or Master) or a Dodge. To use any Swashbuckler ability, the Swashbuckler must have a 1-handed melee weapon in their main hand and must not hold any weapon in their off hand other than a dagger, throwing knife, or stiletto.",
    lore: "Swashbucklers are flamboyant and daring, larger than life adventurers who use their speed and wits rather than heavy armour and brute strength in combat. They come in many forms – pirates, duelists and brigands are all examples of Swashbucklers. Most Swashbucklers are romantics at heart, more concerned with winning fame and fortune than safety or consequence, though some Swashbucklers are far more dark and self serving in their motivations. You might encounter Swashbucklers on the high seas raising a cutlass over a canon, in gambling dens with aces up their sleeves or attempting to win your heart with a sword in hand and rose between their teeth. Most swashbucklers live very short lives but their legends may continue for centuries.",
    abilities: [
      {name:"Finesse",         cp:30,  tier:3,  desc:"Light on their feet and nimble, a Swashbuckler trains to maneuver around weapon strikes and absorb the inertia of blows. Each time this ability is purchased the Swashbuckler gains 5 Armour Points. These 5 AP are considered armour, but they cannot be repaired, refitted or augmented in any way. Finesse AP are removed before regular AP if the Swashbuckler takes damage. Finesse AP will regenerate as a Swashbuckler's energy returns. For every 60 second spent roleplaying limbering up, calming their breathing, tightening straps, etc., the Swashbuckler will regain up to 10 Finesse AP. During this time no other skills may be used. AP from Finesse will be temporarily lost if the Swashbuckler wears metal armour. If Finesse's AP are lost because of these restrictions it will take 10 seconds for them to return after the restrictions have been met. Finesse AP cannot be used if the Swashbuckler is unable to move."},
      {name:"En Garde!",       cp:60,  tier:6,  desc:"This ability improves a Swashbuckler's skill at fighting with a weapon in one hand against a single target. En Garde! Grants the Swashbuckler +1 damage with their main weapon for 10 minutes. This bonus damage is not granted to their off-hand weapon, if they use one. If the Swashbuckler has two weapons, they may select their 'main' weapon when the ability is activated. To activate this ability the Swashbuckler will point or motion toward one target and state: \"Innate En Garde!\" En Garde! only grants this damage bonus against the declared target. Each time this ability is purchased the Swashbuckler will gain an additional +1 damage and another 10 minute period in which they can use En Garde! per day. Eg: If purchased 3 times the Swashbuckler will gain +3 to main weapon damage for 10 minutes, three times a day. Only one En Garde! can be active at the same time."},
      {name:"Prise de Fer",    cp:90,  tier:9,  desc:"This physical attack will disarm an opponent's weapon and cause it to land in the Swashbuckler's hand. By striking the opponent's weapon with their own and calling \"Innate Prise de Fer!\" the Swashbuckler can force their opponent to give them the targeted weapon, if the Prise de Fer is successful. A Swashbuckler has a 3 second grace period to determine what to do with the captured weapon before any negative effects from the Swashbuckler weapon restrictions begin. Prise de Fer is considered a physical attack. It will not grant the skill to use the weapon captured. Prise de Fer will only function against 1-handed weapons unless two Prise de Fers are used at once. If the Swashbuckler does not have a free hand to catch the weapon it will fall on the ground at their feet. Prise de Fer is usable once per day per purchase."},
      {name:"Aegis",           cp:120, tier:12, desc:"By declaring \"Innate Aegis!\" the Swashbuckler may use the Parry defense multiple times within 10 seconds. For every level of the Swashbuckler, they may use one Parry. Parry enables the player to parry any weapon blow, as well as touch casted spells. To Parry an attack, the Swashbuckler simply calls \"Parry\", which negates the last hit taken. Parry cannot block Massive damage, Spellstrikes, or Surprise Attacks. While Aegis is active, no other skills may be used. Aegis may be used once per day per purchase."},
    ]
  },
  "Undead Hunter": {
    fragCost: 150,
    occupations: [],
    prereqs: "Necromantic Arts and either Weapon Specialization (Specific or Group) or Spell Slot: 5th Circle (Healing). All Undead Hunter abilities only work on Undead identified using Necromantic Arts or Undead witnessed taking damage from Healing.",
    lore: "Undead Hunters have undergone specialized training to hunt and destroy Undead creatures. This training is mostly appealing to those with physical combat training who want to refine their capabilities. An Undead Hunter's tools are potent. They have the means to heal themselves while damaging undead, force sunlight upon them and even destroy them outright.",
    abilities: [
      {name:"Hunter's Focus",    cp:30,  tier:3,  desc:"When the Undead Hunter wields any silver, Master Crafted or Legendary weapon they may call magic damage. This ability is usable at will."},
      {name:"Hunter's Attrition",cp:60,  tier:6,  desc:"Hunter's Attrition is a powerful magical ability that damages Undead while healing the Undead Hunter. By using a weapon appropriate for Hunter's Focus, an Undead Hunter may call \"Innate Spellstrike Hunter's Attrition: 25 Magic Healing\". When successfully delivered, this ability does 25 Magic Healing damage (100 Magic Body damage vs Undead) and also mends the Undead Hunter for 25 Body, in the appropriate type for them to heal from, regardless of race. This damage is considered healing magic for all purposes. In order for the healing function of this ability to function an Undead must have been successfully damaged. Hunter's Attrition can be used once per day per purchase."},
      {name:"Crystal of Light",  cp:90,  tier:9,  desc:"At 9th level an Undead Hunter can create and throw a magical crystal of sunlight, which when striking an Undead causes it to explode in natural sunlight. This sunlight will bathe the Undead for 1 minute and cause it to be affected as though it was between the hours of 6:00 AM and 6:00 PM. This will strip magical thresholds and supernatural strength from Undead and may have additional effects based on the Undead type. If the target is not Undead the crystal will have no effect and will not activate magical defenses. It may be used once per day per purchase and the call is \"Innate Arcane Crystal of Light\"."},
      {name:"Final Rest",        cp:120, tier:12, desc:"This ability allows an Undead Hunter to destroy an Undead creature immediately. By using a weapon appropriate for Hunter's Focus, an Undead Hunter may call \"Innate Spellstrike Arcane Destroy Greater Undead!\" against any Lesser or Greater Undead. While this will not destroy Ancient Undead, it will deal 50 Arcane damage and, for up to 1 minute, the Undead Hunter's next three swings deal +5 Healing against that particular Undead. This skill is usable once per day per purchase."},
    ]
  },
};

// Weapon types organized by proficiency group
const WEAPON_TYPES = {
  simple: ['Dagger/Knife','2-Handed Staff','Club','Thrown Weapon'],
  medium: ['Sword (1H)','Mace/Hammer (1H)','Spear (1H)','Axe (1H)','Bow','Claw'],
  large:  ['Great Sword (2H)','Polearm (2H)','Axe (2H)','Crossbow','Mace/Hammer (2H)'],
  exotic: ['Stiletto','Maul (2H)','Bastard Sword','Summoned Weapon'],
};

// Skills that require a specific weapon type to be chosen on purchase
const WEAPON_CHOICE_SKILLS = new Set([
  'Specialization +1: Weapon Specific',
  'Critical +2: Specific',
  'Slay/Parry',
  'Execute',
  'Execute: Subsequent',
]);

// Get all weapon types the character is currently proficient with
function getOwnedWeaponTypes(){
  const types = [...WEAPON_TYPES.simple]; // Simple always auto-granted
  if(getPurchaseCount('Weapon Group Proficiency: Medium')>0) types.push(...WEAPON_TYPES.medium);
  if(getPurchaseCount('Weapon Group Proficiency: Large')>0)  types.push(...WEAPON_TYPES.large);
  // Each Exotic Proficiency purchase grants one specific exotic weapon (tracked via _weaponType)
  const exoticOwned = s.owned
    .filter(o=>(o._baseSkillName||o.name)==='Weapon Specific Proficiency: Exotic' && o._weaponType)
    .map(o=>o._weaponType);
  exoticOwned.forEach(w=>{ if(!types.includes(w)) types.push(w); });
  // Fallback: if exotic purchased but no weapon type recorded, add all exotic
  const exoticCount = getPurchaseCount('Weapon Specific Proficiency: Exotic');
  if(exoticCount>0 && exoticOwned.length===0) types.push(...WEAPON_TYPES.exotic);
  return types;
}


// type: 'auto' = just buy it | 'choice' = player picks from options to fulfill criteria
const VOCATION_PREREQS = {
  'Archer': {
    auto: ['Weapon Group Proficiency: Medium', 'Specialization +1: Weapon Specific'],
    choice: []
  },
  'Artisan': {
    auto: [],
    choice: [
      {
        label: 'Level 10 Tradesman OR Level 5 Tradesman + 5 levels of production skills (total)',
        groups: [
          { label: 'Option A — Level 10 Tradesman (10 purchases)', skills: Array(10).fill('Tradesman') },
          {
            label: 'Option B — Level 5 Tradesman (5 purchases) + 5 levels of any production skills',
            skills: Array(5).fill('Tradesman'),
            flexible: { total: 5, pool: ['Alchemy','Blacksmith','Create Scroll','Trapper'] }
          },
        ]
      }
    ]
  },
  'Battle Mage': {
    auto: [],
    choice: [
      {
        label: 'Sphere of Magic: 2nd OR a 4th Circle Spell Slot',
        groups: [
          { label: 'Option A — Purchase Sphere of Magic: 2nd (requires Read Magic + Sphere 1 first)', skills: ['Read Magic'], spellLevel: null, buySphereTo: 2 },
          { label: 'Option B — Buy spell slots to 4th Circle', skills: ['Read Magic'], spellLevel: 4 },
        ]
      }
    ]
  },
  'Blood Reaver': {
    auto: ['Self Mutilate', 'Anatomy', 'First Aid'],
    choice: []
  },
  'Brew Master': {
    auto: [],
    choice: [
      {
        label: 'Level 5 Create Alcohol OR Level 5 Alchemy',
        groups: [
          { label: 'Option A — 5× Create Alcohol',
            skills: [],
            flexible: { total: 5, pool: ['Create Alcohol'] }
          },
          { label: 'Option B — 5× Alchemy',
            skills: [],
            flexible: { total: 5, pool: ['Alchemy'] }
          },
        ]
      }
    ]
  },
  'Bounty Hunter': {
    auto: ['Sap', 'Ambidexterity'],
    choice: []
  },
  'Conqueror': {
    auto: ['Weapon Group Proficiency: Large', 'Specialization +1: Weapon Group', 'Slay/Parry'],
    choice: []
  },
  'Shaman': {
    auto: [],
    choice: [
      {
        label: 'Level 7 Mysticism OR a 5th Circle Spell Slot (Nature sphere)',
        groups: [
          { label: 'Option A — 7× Mysticism',
            skills: [],
            flexible: { total: 7, pool: ['Mysticism'] }
          },
          { label: 'Option B — Buy spell slots to 5th Circle (Nature sphere)', skills: ['Read Magic'], spellLevel: 5 },
        ]
      }
    ]
  },
  'Stalwart': {
    auto: ['Heavy Armour', 'Shield'],
    choice: [
      {
        label: 'A Parry — Slay/Parry (Specific weapon) OR Slay/Parry: Master (Weapon Group)',
        groups: [
          { label: 'Option A — Slay/Parry (Specific weapon)', skills: ['Weapon Group Proficiency: Medium','Specialization +1: Weapon Specific','Slay/Parry'] },
          { label: 'Option B — Slay/Parry: Master (Weapon Group)', skills: ['Weapon Group Proficiency: Medium','Specialization +1: Weapon Group','Slay/Parry: Master'] },
        ]
      }
    ]
  },
  'Swashbuckler': {
    auto: ['Ambidexterity'],
    choice: [
      {
        label: 'A Slay (Specific or Master) OR a Dodge',
        groups: [
          { label: 'Option A — Slay/Parry (Specific weapon)', skills: ['Weapon Group Proficiency: Medium','Specialization +1: Weapon Specific','Slay/Parry'] },
          { label: 'Option B — Slay/Parry: Master (Weapon Group)', skills: ['Weapon Group Proficiency: Medium','Specialization +1: Weapon Group','Slay/Parry: Master'] },
          { label: 'Option C — Dodge (requires Critical +2: Specific)', skills: ['Weapon Group Proficiency: Medium','Critical +2: Specific','Dodge'] },
        ]
      }
    ]
  },
  'Undead Hunter': {
    auto: ['Necromantic Arts'],
    choice: [
      {
        label: 'Weapon Specialization (Specific or Group) OR a 5th Circle Spell Slot (Healing sphere)',
        groups: [
          { label: 'Option A — Specialization +1: Weapon Specific', skills: ['Weapon Group Proficiency: Medium','Specialization +1: Weapon Specific'] },
          { label: 'Option B — Specialization +1: Weapon Group', skills: ['Weapon Group Proficiency: Medium','Specialization +1: Weapon Group'] },
          { label: 'Option C — Buy spell slots to 5th Circle (Healing sphere)', skills: ['Read Magic'], spellLevel: 5 },
        ]
      }
    ]
  },
  'Paladin':      { auto: [], choice: [] },
  'Dread Knight': { auto: [], choice: [] },
  'Lightweaver':  { auto: [], choice: [] },
  'Darkweaver':   { auto: [], choice: [] },
  'Dragon Knight':{ auto: [], choice: [] },
};

function autoBuyVocationPrereqs(vocName){
  const vp = VOCATION_PREREQS[vocName];
  if(!vp) return;
  const allSk = SKILLS.flatMap(c=>c.skills);

  // Auto-buy the definite prereqs
  (vp.auto||[]).forEach(skillName=>{
    if(getPurchaseCount(skillName) > 0) return;
    const sk = allSk.find(s=>s.name===skillName);
    if(!sk) return;
    const cp = getSkillCost(sk);
    const cat = getSkillCat(skillName);
    s.owned.push({...sk, _cat:cat, _vocPrereq:true, cp});
  });

  // Show popup for choice prereqs
  if(vp.choice && vp.choice.length){
    showVocPrereqPopup(vocName, vp.choice, allSk);
  }
}

function getSkillCat(skillName){
  const WARRIOR_SKILLS = ['Ambidexterity','Florentine','Flurry of Blows','Heavy Armour','Self Mutilate','Shield',
    'Slay/Parry','Slay/Parry: Master','Slay/Parry: Subsequent','Slay/Parry: Master Subsequent',
    'Specialization +1: Weapon Group','Specialization +1: Weapon Specific',
    'Weapon Group Proficiency: Medium','Weapon Group Proficiency: Large',
    'Weapon Specific Proficiency: Exotic','Weapon Refocus'];
  const ROGUE_SKILLS = ['Critical +2: Specific','Critical +2: Group','Dodge','Dodge: Additional',
    'Execute','Execute: Master','Garrotte','Sap','Vital Blow'];
  const SCHOLAR_SKILLS = ['Anatomy','Mysticism','Demonic/Angelic Arts','Elemental Attunement',
    'First Aid','Necromantic Arts','Physician','Read & Write','Read Magic',
    'Read Magic: Advanced','Read Magic: Ritual','Advanced Ritual Casting'];
  if(WARRIOR_SKILLS.includes(skillName)) return 'Warrior';
  if(ROGUE_SKILLS.includes(skillName)) return 'Rogue';
  if(SCHOLAR_SKILLS.includes(skillName)) return 'Scholar';
  return 'Frag Skills';
}

function showVocPrereqPopup(vocName, choiceGroups, allSk){
  window._vocFlexState = window._vocFlexState || {};
  window._vocPrereqData = {vocName, choiceGroups, allSk};

  let html = `
    <div style="font-size:14px;font-weight:600;margin-bottom:0.5rem">Prerequisites for ${vocName}</div>
    <div style="font-size:12px;color:var(--color-text-secondary);margin-bottom:1rem;line-height:1.5">
      Some prerequisites require a choice. Select the option that best suits your character. Skills already owned won't be re-purchased.
    </div>`;

  choiceGroups.forEach((group, gi)=>{
    html += `<div style="background:var(--color-background-secondary);border-radius:8px;padding:12px;margin-bottom:12px">
      <div style="font-size:11px;font-weight:600;color:var(--color-text-warning);margin-bottom:10px;text-transform:uppercase;letter-spacing:0.5px">⚠ ${group.label}</div>`;

    group.groups.forEach((opt, oi)=>{
      const flexKey = `${vocName}_${gi}_${oi}`;

      if(opt.flexible){
        // Flexible distribution — fixed skills + freely distributed pool
        const {total, pool} = opt.flexible;
        if(!window._vocFlexState[flexKey]){
          window._vocFlexState[flexKey] = {};
          pool.forEach(sn=>{ window._vocFlexState[flexKey][sn]=0; });
        }
        const flexCounts = window._vocFlexState[flexKey];
        const totalAllocated = Object.values(flexCounts).reduce((a,b)=>a+b,0);

        // Fixed skills
        const fixedNeeded = {};
        (opt.skills||[]).forEach(sn=>{ fixedNeeded[sn]=(fixedNeeded[sn]||0)+1; });
        const fixedEntries = Object.entries(fixedNeeded);
        const fixedMet = fixedEntries.every(([sn,n])=>getPurchaseCount(sn)>=n);
        const metFlex = totalAllocated >= total;
        const allMet = fixedMet && metFlex;

        const fixedCp = fixedEntries.reduce((sum,[sn,n])=>{
          const sk=allSk.find(s=>s.name===sn);
          return sum+(sk?getSkillCost(sk)*Math.max(0,n-getPurchaseCount(sn)):0);
        },0);
        const flexCp = Object.entries(flexCounts).reduce((sum,[sn,n])=>{
          const sk=allSk.find(s=>s.name===sn);
          return sum+(sk?getSkillCost(sk)*Math.max(0,n-getPurchaseCount(sn)):0);
        },0);
        const totalCp = fixedCp + flexCp;

        html += `<div style="border:0.5px solid var(--color-border-secondary);border-radius:6px;padding:10px;margin-bottom:6px">
          <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px;flex-wrap:wrap;gap:6px">
            <div style="font-size:12px;font-weight:500">${opt.label}</div>
            <button onclick="buyVocPrereqOption(${gi},${oi},'${vocName}')" ${allMet?'disabled':''}
              style="padding:5px 14px;border:0.5px solid var(--color-border-secondary);border-radius:6px;background:${allMet?'var(--color-background-success)':'var(--color-background-primary)'};color:${allMet?'var(--color-text-success)':'var(--color-text-primary)'};font-size:11px;font-weight:500;cursor:${allMet?'default':'pointer'};white-space:nowrap;flex-shrink:0">
              ${allMet ? '✓ Fully met' : `Buy selected (${totalCp} CP)`}
            </button>
          </div>
          ${fixedEntries.length ? `
          <div style="margin-bottom:8px">
            <div style="font-size:10px;color:var(--color-text-tertiary);margin-bottom:4px;text-transform:uppercase;letter-spacing:0.4px">Fixed requirements</div>
            <div style="display:flex;flex-wrap:wrap;gap:4px">
              ${fixedEntries.map(([sn,n])=>{
                const owned=getPurchaseCount(sn)>=n;
                const sk=allSk.find(s=>s.name===sn);
                const cp=sk?getSkillCost(sk):0;
                return `<span style="font-size:11px;padding:2px 8px;border-radius:100px;background:${owned?'var(--color-background-success)':'var(--color-background-tertiary)'};color:${owned?'var(--color-text-success)':'var(--color-text-secondary)'}">
                  ${sn}${n>1?` ×${n}`:''}${!owned&&cp?` — ${cp*Math.max(0,n-getPurchaseCount(sn))}cp`:''}${owned?' ✓':''}
                </span>`;
              }).join('')}
            </div>
          </div>` : ''}
          <div>
            <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px">
              <div style="font-size:10px;color:var(--color-text-tertiary);text-transform:uppercase;letter-spacing:0.4px">Distribute ${total} levels — choose freely</div>
              <div style="font-size:11px;font-weight:600;color:${metFlex?'var(--color-text-success)':'var(--color-text-warning)'}">${totalAllocated}/${total}</div>
            </div>
            ${pool.map(sn=>{
              const cnt=flexCounts[sn]||0;
              const ownedCount=getPurchaseCount(sn);
              const sk=allSk.find(s=>s.name===sn);
              const cp=sk?getSkillCost(sk):0;
              return `<div style="display:flex;align-items:center;gap:8px;padding:5px 0;border-bottom:0.5px solid var(--color-border-tertiary)">
                <span style="flex:1;font-size:12px">${sn}</span>
                <span style="font-size:11px;color:var(--color-text-tertiary)">${cp}cp ea.</span>
                ${ownedCount>0?`<span style="font-size:10px;color:var(--color-text-success);white-space:nowrap">${ownedCount} owned</span>`:''}
                <button onclick="flexAdjust('${flexKey}','${sn}',-1,'${vocName}',${gi})" ${cnt<=0?'disabled':''}
                  style="width:26px;height:26px;border:0.5px solid var(--color-border-secondary);border-radius:4px;background:var(--color-background-secondary);color:var(--color-text-primary);cursor:pointer;font-size:15px;line-height:1;padding:0">−</button>
                <span style="min-width:22px;text-align:center;font-size:13px;font-weight:600">${cnt}</span>
                <button onclick="flexAdjust('${flexKey}','${sn}',1,'${vocName}',${gi})" ${totalAllocated>=total?'disabled':''}
                  style="width:26px;height:26px;border:0.5px solid var(--color-border-secondary);border-radius:4px;background:var(--color-background-secondary);color:var(--color-text-primary);cursor:pointer;font-size:15px;line-height:1;padding:0">+</button>
              </div>`;
            }).join('')}
          </div>
        </div>`;

      } else {
        // Standard fixed-list option
        const needed = {};
        opt.skills.forEach(sn=>{ needed[sn]=(needed[sn]||0)+1; });
        const skillEntries = Object.entries(needed);
        const skillsMet = skillEntries.every(([sn,n])=>getPurchaseCount(sn)>=n);

        // Check spell slot requirement if present
        const spellMet = !opt.spellLevel || getSpellSlotCount(opt.spellLevel) > 0;
        const sphereMet = !opt.buySphereTo || getPurchaseCount(`Sphere of Magic: ${opt.buySphereTo===1?'1st':opt.buySphereTo===2?'2nd':'3rd'}`) > 0;
        const allMet = skillsMet && spellMet && sphereMet;

        const missing = skillEntries.filter(([sn,n])=>getPurchaseCount(sn)<n);
        const totalCp = missing.reduce((sum,[sn,n])=>{
          const sk=allSk.find(s=>s.name===sn);
          return sum+(sk?getSkillCost(sk)*Math.max(0,n-getPurchaseCount(sn)):0);
        },0);

        const btnLabel = allMet ? '✓ Already met' :
                         opt.spellLevel ? `Buy + Fill to ${ordinal(opt.spellLevel)} Circle` :
                         opt.buySphereTo ? `Buy + Purchase Sphere${opt.buySphereTo>1?' chain':''}` :
                         !missing.length ? '✓ Already met' : `Buy (${totalCp} CP)`;

        html += `<div style="border:0.5px solid var(--color-border-secondary);border-radius:6px;padding:10px;margin-bottom:6px">
          <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px;flex-wrap:wrap;gap:6px">
            <div style="font-size:12px;font-weight:500">${opt.label}</div>
            <button onclick="buyVocPrereqOption(${gi},${oi},'${vocName}')" ${allMet?'disabled':''}
              style="padding:5px 14px;border:0.5px solid var(--color-border-secondary);border-radius:6px;background:${allMet?'var(--color-background-success)':'var(--color-background-primary)'};color:${allMet?'var(--color-text-success)':'var(--color-text-primary)'};font-size:11px;font-weight:500;cursor:${allMet?'default':'pointer'};white-space:nowrap;flex-shrink:0">
              ${btnLabel}
            </button>
          </div>
          <div style="display:flex;flex-wrap:wrap;gap:4px">
            ${skillEntries.map(([sn,n])=>{
              const isFullyOwned=getPurchaseCount(sn)>=n;
              const sk=allSk.find(s=>s.name===sn);
              const cp=sk?getSkillCost(sk):0;
              const label=n>1?`${sn} ×${n}`:sn;
              const costLabel=!isFullyOwned&&cp?` — ${cp*(n-getPurchaseCount(sn))}cp`:'';
              return `<span style="font-size:11px;padding:2px 8px;border-radius:100px;background:${isFullyOwned?'var(--color-background-success)':'var(--color-background-tertiary)'};color:${isFullyOwned?'var(--color-text-success)':'var(--color-text-secondary)'}">
                ${label}${costLabel}${isFullyOwned?' ✓':''}
              </span>`;
            }).join('')}
            ${opt.spellLevel ? `<span style="font-size:11px;padding:2px 8px;border-radius:100px;background:${spellMet?'var(--color-background-success)':'var(--color-background-tertiary)'};color:${spellMet?'var(--color-text-success)':'var(--color-text-secondary)'}">
              Spell slots to ${ordinal(opt.spellLevel)} Circle${spellMet?' ✓':''}
            </span>` : ''}
            ${opt.buySphereTo ? `<span style="font-size:11px;padding:2px 8px;border-radius:100px;background:${sphereMet?'var(--color-background-success)':'var(--color-background-tertiary)'};color:${sphereMet?'var(--color-text-success)':'var(--color-text-secondary)'}">
              Sphere of Magic: ${['1st','2nd','3rd'][opt.buySphereTo-1]}${sphereMet?' ✓':''}
            </span>` : ''}
          </div>
        </div>`;
      }
    });
    html += `</div>`;
  });

  document.getElementById('voc-prereq-body').innerHTML = html;
  document.getElementById('voc-prereq-overlay').style.display = 'flex';
}

function flexAdjust(flexKey, skillName, delta, vocName, gi){
  if(!window._vocFlexState || !window._vocFlexState[flexKey]) return;
  const counts = window._vocFlexState[flexKey];
  counts[skillName] = Math.max(0, (counts[skillName]||0) + delta);
  const {choiceGroups, allSk} = window._vocPrereqData;
  showVocPrereqPopup(vocName, choiceGroups, allSk);
}

function buyVocPrereqOption(groupIdx, optionIdx, vocName){
  const {choiceGroups, allSk} = window._vocPrereqData || {};
  if(!choiceGroups) return;
  const opt = choiceGroups[groupIdx].groups[optionIdx];
  const flexKey = `${vocName}_${groupIdx}_${optionIdx}`;

  if(opt.flexible){
    // Buy fixed skills first
    const fixedNeeded = {};
    (opt.skills||[]).forEach(sn=>{ fixedNeeded[sn]=(fixedNeeded[sn]||0)+1; });
    Object.entries(fixedNeeded).forEach(([sn,n])=>{
      const toBuy = Math.max(0, n - getPurchaseCount(sn));
      const sk = allSk.find(s=>s.name===sn);
      if(!sk) return;
      const cp = getSkillCost(sk);
      const cat = getSkillCat(sn);
      for(let i=0;i<toBuy;i++) s.owned.push({...sk,_cat:cat,_vocPrereq:true,cp});
    });
    // Buy flexible selections
    const flexCounts = (window._vocFlexState && window._vocFlexState[flexKey]) || {};
    Object.entries(flexCounts).forEach(([sn,n])=>{
      if(n<=0) return;
      const toBuy = Math.max(0, n - getPurchaseCount(sn));
      const sk = allSk.find(s=>s.name===sn);
      if(!sk) return;
      const cp = getSkillCost(sk);
      const cat = getSkillCat(sn);
      for(let i=0;i<toBuy;i++) s.owned.push({...sk,_cat:cat,_vocPrereq:true,cp});
    });
  } else {
    // Standard — buy all listed skills at required counts
    const needed = {};
    opt.skills.forEach(sn=>{ needed[sn]=(needed[sn]||0)+1; });
    Object.entries(needed).forEach(([sn,n])=>{
      const toBuy = Math.max(0, n - getPurchaseCount(sn));
      const sk = allSk.find(s=>s.name===sn);
      if(!sk) return;
      const cp = getSkillCost(sk);
      const cat = getSkillCat(sn);
      for(let i=0;i<toBuy;i++) s.owned.push({...sk,_cat:cat,_vocPrereq:true,cp});
    });
    // If this option requires spell slots, run buyToLevel after prereq skills are purchased
    if(opt.spellLevel){
      buyToLevel(opt.spellLevel);
    }
    // If this option requires purchasing spheres up to a specific number
    if(opt.buySphereTo){
      for(let i=1; i<=opt.buySphereTo; i++){
        buySphere(i, true);
      }
    }
  }

  const vp = VOCATION_PREREQS[vocName];
  showVocPrereqPopup(vocName, vp.choice, allSk);
  render();
}

// ---- Elemental Attunement popup ----
let _eaCat = null, _eaSi = null, _eaSk = null;

function openElementalAttunementPopup(cat, si, sk){
  // Check if already at max 3 attunements (first from sphere selection + up to 2 more from skill)
  const skillAttunements = s.owned.filter(o=>o._elementalAttunement).length;
  if(skillAttunements >= 3){ return; } // max 3 additional via skill (first is free with sphere)
  // Must have Elemental sphere selected
  const hasElemental = [s.s_school_1,s.s_school_2,s.s_school_3].includes('Elemental');
  if(!hasElemental){ return; }
  // Must have at least 1 primary attunement already
  if(s.elementalAttunements.length === 0){ return; }

  _eaCat = cat; _eaSi = si; _eaSk = sk;
  const ELEMENTS = ['Fire','Stone','Lightning','Ice'];
  const sel = document.getElementById('elemental-attunement-sel');
  sel.innerHTML = '<option value="">— choose element —</option>';
  ELEMENTS.filter(e => !s.elementalAttunements.includes(e)).forEach(e => {
    sel.innerHTML += `<option value="${e}">${e}</option>`;
  });
  document.getElementById('elemental-attunement-overlay').style.display = 'flex';
}

function confirmElementalAttunement(){
  const el = document.getElementById('elemental-attunement-sel').value;
  if(!el || !_eaSk) return;
  const cp = getSkillCost(_eaSk);
  s.owned.push({
    ..._eaSk,
    _cat: _eaCat,
    cp,
    _elementalAttunement: true,
    _chosenElement: el,
    name: `Elemental Attunement (${el})`,
    _baseSkillName: 'Elemental Attunement',
  });
  s.elementalAttunements.push(el);
  closeElementalAttunementPopup();
  render();
}

function closeElementalAttunementPopup(){
  document.getElementById('elemental-attunement-overlay').style.display = 'none';
  _eaCat = null; _eaSi = null; _eaSk = null;
}


let _wcCat = null, _wcSi = null, _wcSk = null;

function openWeaponChoicePopup(cat, si, sk){
  _wcCat = cat; _wcSi = si; _wcSk = sk;
  document.getElementById('weapon-choice-title').textContent = sk.name;

  const sel = document.getElementById('weapon-choice-sel');
  sel.innerHTML = '<option value="">— select —</option>';

  if(sk._weaponChoice === 'exotic'){
    // Exotic proficiency: choose one exotic weapon not yet owned
    document.getElementById('weapon-choice-subtitle').textContent =
      'Choose an exotic weapon to become proficient with.';
    const alreadyOwned = s.owned
      .filter(o=>(o._baseSkillName||o.name)==='Weapon Specific Proficiency: Exotic' && o._weaponType)
      .map(o=>o._weaponType);
    WEAPON_TYPES.exotic.forEach(w=>{
      const opt = document.createElement('option');
      opt.value = w; opt.textContent = w;
      if(alreadyOwned.includes(w)) opt.disabled = true;
      sel.appendChild(opt);
    });

  } else if(sk._weaponChoice === 'group'){
    // Group skills: offer only group names the character owns
    document.getElementById('weapon-choice-subtitle').textContent =
      'Choose the weapon group for this purchase. Only groups you are proficient with are shown.';
    const available = getAvailableWeaponGroups();
    available.forEach(g => {
      const opt = document.createElement('option');
      opt.value = g; opt.textContent = g;
      sel.appendChild(opt);
    });

  } else {
    // Specific skills: offer individual weapons from owned groups
    // Exotic weapons (Stiletto, Maul, Bastard Sword) are available to all specific skills
    // Summoned Weapon is ONLY available for Specialization +1: Weapon Specific
    const allowSummoned = sk.name === 'Specialization +1: Weapon Specific';
    document.getElementById('weapon-choice-subtitle').textContent =
      'Choose the specific weapon type for this purchase. Only weapons you are proficient with are shown.';
    const weaponTypes = getOwnedWeaponTypes();
    const groups = [
      {label:'Simple', weapons: WEAPON_TYPES.simple},
      {label:'Medium', weapons: WEAPON_TYPES.medium},
      {label:'Large',  weapons: WEAPON_TYPES.large},
      {label:'Exotic', weapons: WEAPON_TYPES.exotic.filter(w => w !== 'Summoned Weapon' || allowSummoned)},
    ];
    groups.forEach(({label, weapons}) => {
      const owned = weapons.filter(w => weaponTypes.includes(w));
      if(!owned.length) return;
      const grp = document.createElement('optgroup');
      grp.label = label;
      owned.forEach(w => {
        const opt = document.createElement('option');
        opt.value = w; opt.textContent = w;
        grp.appendChild(opt);
      });
      sel.appendChild(grp);
    });
  }

  weaponChoiceUpdateBtn();
  document.getElementById('weapon-choice-overlay').style.display = 'flex';
}

function weaponChoiceUpdateBtn(){
  const val = document.getElementById('weapon-choice-sel').value;
  const btn = document.getElementById('weapon-choice-confirm');
  if(val){
    btn.disabled = false;
    btn.style.cursor = 'pointer';
    btn.style.background = 'var(--color-background-primary)';
    btn.style.color = 'var(--color-text-primary)';
  } else {
    btn.disabled = true;
    btn.style.cursor = 'not-allowed';
    btn.style.background = 'var(--color-background-secondary)';
    btn.style.color = 'var(--color-text-tertiary)';
  }
}

function confirmWeaponChoice(){
  const weapon = document.getElementById('weapon-choice-sel').value;
  if(!weapon || !_wcSk) return;
  const cp = getSkillCost(_wcSk);
  s.owned.push({
    ..._wcSk,
    _cat: _wcCat,
    cp,
    _weaponType: weapon,
    _baseSkillName: _wcSk.name,
    name: `${_wcSk.name}: ${weapon}`,
  });
  closeWeaponChoicePopup();
  render();
}

function closeWeaponChoicePopup(){
  document.getElementById('weapon-choice-overlay').style.display = 'none';
  _wcCat = null; _wcSi = null; _wcSk = null;
}

// ---- Weapon data ----
const WEAPON_GROUPS = {
  Simple:  ['Dagger/Knife','2-Handed Staff','Club','Thrown Weapon'],
  Medium:  ['Sword (1H)','Mace/Hammer (1H)','Spear (1H)','Axe (1H)','Bow','Claw'],
  Large:   ['Great Sword (2H)','Polearm (2H)','Axe (2H)','Crossbow','Mace/Hammer (2H)'],
  Exotic:  ['Stiletto','Maul (2H)','Bastard Sword','Summoned Weapon'],
};

function getAvailableWeapons(){
  const weapons = [];
  WEAPON_GROUPS.Simple.forEach(w=>weapons.push({weapon:w,group:'Simple'}));
  if(getPurchaseCount('Weapon Group Proficiency: Medium')>0)
    WEAPON_GROUPS.Medium.forEach(w=>weapons.push({weapon:w,group:'Medium'}));
  if(getPurchaseCount('Weapon Group Proficiency: Large')>0)
    WEAPON_GROUPS.Large.forEach(w=>weapons.push({weapon:w,group:'Large'}));
  if(getPurchaseCount('Weapon Specific Proficiency: Exotic')>0)
    WEAPON_GROUPS.Exotic.forEach(w=>weapons.push({weapon:w,group:'Exotic'}));
  return weapons;
}

function getAvailableWeaponGroups(){
  const groups = ['Simple'];
  if(getPurchaseCount('Weapon Group Proficiency: Medium')>0) groups.push('Medium');
  if(getPurchaseCount('Weapon Group Proficiency: Large')>0) groups.push('Large');
  return groups;
}

let _paragonCat = null, _paragonSi = null, _paragonSphere = null;

function openParagonPopup(cat, si){
  // Hard block — check if Paragon already purchased or Favoured Vocation active
  if(s.owned.some(o=>o._paragon && !o._auto)) return;
  if(s.vocation && FAVOURED_VOCATIONS[s.vocation]) return;
  _paragonCat = cat; _paragonSi = si; _paragonSphere = null;
  const sel = document.getElementById('paragon-level-sel');
  sel.innerHTML = '<option value="">— select level —</option>';
  const slots = getSlotsByLevel();
  for(let lvl=1; lvl<=7; lvl++){
    if((slots[lvl]||0) > 0){
      const opt = document.createElement('option');
      opt.value = lvl;
      opt.textContent = `${ordinal(lvl)} Circle  (${lvl+10} CP)`;
      sel.appendChild(opt);
    }
  }
  // Reset state
  _paragonSphere = null;
  document.getElementById('paragon-light-btn').removeAttribute('data-active');
  document.getElementById('paragon-dark-btn').removeAttribute('data-active');
  ['paragon-light-btn','paragon-dark-btn'].forEach(id=>{
    const b = document.getElementById(id);
    b.style.background='var(--color-background-secondary)';
    b.style.color='var(--color-text-primary)';
    b.style.fontWeight='400';
  });
  document.getElementById('paragon-cost-display').textContent = '';
  const confirmBtn = document.getElementById('paragon-confirm-btn');
  confirmBtn.disabled = true;
  confirmBtn.style.cursor = 'not-allowed';
  confirmBtn.style.background = 'var(--color-background-secondary)';
  confirmBtn.style.color = 'var(--color-text-tertiary)';
  document.getElementById('paragon-overlay').style.display = 'flex';
}

function paragonSetSphere(sphere){
  _paragonSphere = sphere;
  ['paragon-light-btn','paragon-dark-btn'].forEach(id=>{
    const b = document.getElementById(id);
    b.style.background = 'var(--color-background-secondary)';
    b.style.color = 'var(--color-text-primary)';
    b.style.fontWeight = '400';
  });
  if(sphere === 'Light'){
    const b = document.getElementById('paragon-light-btn');
    b.style.background='#1a2a4a'; b.style.color='#85b7eb'; b.style.fontWeight='600';
  } else if(sphere === 'Dark'){
    const b = document.getElementById('paragon-dark-btn');
    b.style.background='#2a1a2a'; b.style.color='#c070c0'; b.style.fontWeight='600';
  }
  paragonUpdateCost();
}

function paragonUpdateCost(){
  const lvl = parseInt(document.getElementById('paragon-level-sel').value);
  const costEl = document.getElementById('paragon-cost-display');
  const confirmBtn = document.getElementById('paragon-confirm-btn');
  if(_paragonSphere && lvl >= 1 && lvl <= 7){
    const cp = lvl + 10;
    costEl.innerHTML = `<span style="color:var(--color-text-primary)"><strong>${_paragonSphere}</strong> sphere · ${ordinal(lvl)} Circle · <strong>${cp} CP</strong> · 100 frags</span>`;
    confirmBtn.disabled = false;
    confirmBtn.style.cursor = 'pointer';
    confirmBtn.style.background = 'var(--color-background-primary)';
    confirmBtn.style.color = 'var(--color-text-primary)';
  } else {
    costEl.textContent = !_paragonSphere ? 'Select a sphere alignment to continue.' : 'Select a spell level to continue.';
    confirmBtn.disabled = true;
    confirmBtn.style.cursor = 'not-allowed';
    confirmBtn.style.background = 'var(--color-background-secondary)';
    confirmBtn.style.color = 'var(--color-text-tertiary)';
  }
}

function confirmParagon(){
  const lvl = parseInt(document.getElementById('paragon-level-sel').value);
  if(!_paragonSphere || !lvl || lvl<1 || lvl>7) return;
  // Hard block — prevent duplicate purchase
  if(s.owned.some(o=>o._paragon && !o._auto)){ closeParagonPopup(); return; }
  const cp = lvl + 10;
  const cats = buildSkillCatList();
  const catObj = cats.find(c=>c.cat===_paragonCat);
  if(!catObj) return;
  const sk = catObj.skills[_paragonSi];
  s.owned.push({
    ...sk,
    _cat: _paragonCat,
    cp,
    frag: 100,
    _paragonSphere,
    _paragonLevel: lvl,
    name: `Paragon (${_paragonSphere}, ${ordinal(lvl)} Circle)`,
  });
  closeParagonPopup();
  render();
}

function closeParagonPopup(){
  document.getElementById('paragon-overlay').style.display = 'none';
  _paragonCat = null; _paragonSi = null; _paragonSphere = null;
}

function closeVocPrereqPopup(){
  document.getElementById('voc-prereq-overlay').style.display = 'none';
  render();
}

function getVocationSkills(){
  if(!s.vocation) return null;
  const voc = VOCATIONS[s.vocation] || FAVOURED_VOCATIONS[s.vocation];
  if(!voc) return null;

  return voc.abilities.map(ab=>{
    const prereqs = [];
    if(ab.tier > 3){
      const prevTierAb = voc.abilities.find(a=>a.tier===ab.tier-3);
      if(prevTierAb) prereqs.push({name:prevTierAb.name, minCount:1});
    }
    return {
      name: ab.name,
      costs: null,
      cp: ab.cp,
      frag: 0,
      maxPurchases: ab.maxPurchases || DEFAULT_MAX,
      bodyBonus: 0,
      strBonus: 0,
      occupational: true,
      _occAbilityTier: ab.tier,
      _vocationAbility: true,
      prereqs,
      desc: ab.desc,
    };
  });
}

function getVocationFragCost(){
  if(!s.vocation) return 0;
  const voc = VOCATIONS[s.vocation] || FAVOURED_VOCATIONS[s.vocation];
  return voc ? voc.fragCost : 0;
}


const SKILLS = [
  {cat:'General', skills:[]},

  {cat:'Production', skills:[
    skill('Alchemy',       [80,50,70,40,40,50,60,40,50], [], {desc:'Purchasing this skill opens up the world of Alchemy to your character. Each level of Alchemy purchased allows your character to create new Alchemical recipes from the in-game list of known alchemies. Alchemies with an asterisk beside them require special components to create, which must be found in-game. An Alchemist can also create mundane role play related effects with little effort. By spending 10 minutes gathering common and easily found herbs and ingredients, the Alchemist can create elixirs to cure many role-played ailments. These only cure mundane ill effects and cannot be used to mimic any spell effect or ability. It requires no skill to willingly drink an Alchemical concoction or to pour an elixir down an unconscious victim\'s throat. To use any non-ingested Alchemical creation, it must be shaken vigorously and prepared with a three count. You may only have one non-ingested Alchemical creation prepared at a time and you must prepare your own. Non-ingested Alchemy only remains prepared for 10 minutes, after which it must be prepared again before being used. Identify Alchemy: Each Alchemist has a basic knowledge of plants and herbs that allows them to identify known Alchemical concoctions after having examined the substance for one minute. Apply Ingested Alchemy (Level 2): For an ingested Alchemy to take effect the Alchemist must somehow attach the Alchemy tag onto or under the item holding the food/drink. Apply Contact Alchemy (Level 4): The Alchemist must spend one minute applying the contact elixir to the item. Contact alchemy may be applied to weapons or any other object. Reverse Engineer (Level 5): The Alchemist may reverse engineer Alchemy into its basic state, destroying the Alchemy but returning half its Raw Material value. Throw Gas Globe (Level 6): The declaration for all thrown Alchemy is "<type> Gas". Orange packets are used to represent Alchemical gas globes. Apply Contact on a 30 Count (Level 7): The Alchemist now only needs thirty seconds to apply contact alchemy to items. Prepare Alchemy on a 2 Count (Level 10): The Alchemist may now prepare alchemy on a 2 count.'}),
    skill('Artifice',      [75,75,80,90,100,90,120,110,95], [{name:'Blacksmith',minCount:10}], {desc:'The pinnacle of achievement for a Blacksmith is creating Blueprinted items. Blueprints are physical items that contain special instructions to allow a Legendary Blacksmith to craft powerful items. Given the right exotic material, Catalysts, time and the proper Blueprint, the Artificer can make armour and weapons that possess special and unique properties. Each Blueprint, and all the requirements, are different and must be found in-game. An Artificer may craft 1 Blueprinted item per event per level of Artificing. Only Artificers can read Blueprints. Artificers can read Blueprints even if they cannot read and write.'}),
    skill('Blacksmith',    [65,65,70,80,90,80,110,100,85], [], {desc:'This production skill allows the character to craft new weapons and armour as well as repairing damaged armour. Crafting new weapons and armour may only be done at logistics. Refitting (repairing) armour takes 60 seconds for every 10 points of armour to be refit and requires the Blacksmith and target to remain stationary. A Blacksmith can tell how much of a target\'s armour has been damaged by placing both hands on their torso and stating, "Blacksmithing 1, Blacksmithing 2, Blacksmithing 3, how much armour are you missing?" Repair While Moving (Level 3): The Blacksmith may now repair armour while moving. Reforge (Level 5): The Blacksmith may Reforge any shield, piece of armour or weapon, back into half of its value in Raw Material. +1 Strength (Levels 6 and 10): Hours and hours spent hammering metal have given the Blacksmith the kind of muscles every warrior desires. This Strength stacks with other Strength bonuses, including itself.'}),
    skill('Chemistry',     [90,60,80,50,50,60,70,50,60], [{name:'Alchemy',minCount:10}], {desc:'When an Alchemist has mastered everything Alchemy has to teach them, they can learn Chemistry. Chemistry Formulas create powerful alchemical concoctions. Given the right exotic material, Catalysts, time and the proper Formula, the Alchemist can make potions and elixirs that possess special and unique properties. Each Formula, and all the requirements, are different and must be found in-game. A Chemist may brew 1 Chemistry item per event per level of Chemistry. Chemistry is considered \'ritual level\'. Only Chemists can read Chemistry Formulas. Chemists can read Chemistry Formulas even if they cannot read and write.'}),
    skill('Create Scroll', [75,75,40,50,75,45,35,45,35], [{name:'Read Magic',minCount:1}], {desc:'This skill allows a character to create Battle Magic Scrolls. To make a Magical Scroll, the character must be able to cast that specific spell from memory. Glowing Ink (Level 2): This allows the scrollcrafter to create scrolls which can be cast in darkness. Scavenge Scroll (Level 4): The scribe may carefully salvage the scrollcrafting materials of an existing scroll to turn it into something new, returning half its Raw Material value. Create Tome (Level 6): The scrollcrafter has learned to create powerful Tomes of magic. This Tome may contain one of each Battle Magic scroll in a single sphere and is spirit linked to the first person who memorises from it. Scroll Mastery (Level 10): The scrollcrafter has now mastered all they need to create any scroll from the core rulebook, even if they cannot cast the sphere that scroll is from, although they will still need to be able to cast a spell of that level. Scrolls created with Scroll Mastery cost an additional 100% of the base Raw Material cost.'}),
    skill('Tradesman',     [40,40,40,40,40,40,40,40,35], [], {desc:'The Tradesman skill is a catch-all term for all other jobs or occupations. When purchasing this skill, a player must choose their trade. For each level of Tradesman the player has, they will receive either 3 silver worth of product or 5 units of Raw Material at Logistics. Players must choose which type of Raw Material (maximum of one) the skill can produce when it is purchased and have this approved by a Logistics Marshal. An appropriate Tradesman skill may aid in certain role-playing situations as determined by the Shaper running the encounter.'}),
    skill('Trapper',       [75,65,75,45,55,65,85,75,75], [], {desc:'This skill allows a character to create, set, and disarm traps. To arm or disarm a trap, the Trapper must have a level of Trapper equal to the level of trigger used. Traps and triggers can only be created at Logistics. An armed trap may be moved any distance, if it remains in contact with the mover and they move no faster than walking speed. Should the trap be thrown, dropped, or move faster than a walk, the trap goes off instantly. This skill also allows the character to create and pick in-game locks. A Trapper can pick a lock with a difficulty rating lower than or equal to their Trapper level, requiring a 1-minute count, once per day per purchase. A player with Trapper may also open locks by physically picking the phys-rep lock without consuming any daily uses. Salvage (Level 5): The Trapper may break down their locks and traps to repurpose the raw materials, returning half its value in Raw Material.'}),
  ]},
  {cat:'Scholar', skills:[
    skill('Anatomy',                [40,40,40,40,40,40,40,40,35], [], {max:1, desc:'This skill allows a user to check an individual\'s vital signs. Anatomy can be used on any living creature to glean information about their health and physical state. To use Anatomy, the player must place both hands on the torso of the target, call out "Anatomy 1, Anatomy 2, Anatomy 3", and then ask the player, out of game, one of the following questions: "Are you alive?", "Are you in your bleed count?", "Are you in your death count?", "Are you paralysed?", "Are you asleep?", "Are you unconscious?", "Is there alcohol in your system?", "Is there a toxin in your system?", "Is there a non-Magical disease in your system?" and "How much damage have you taken?" This skill is usable at will.'}),
    skill('Mysticism',              [50,50,50,50,50,50,50,50,50], [], {desc:'The art of the Mystic is one that has both amazed and frightened the unaware since the dawn of time. A Mystic excels in the contacting of lost spirits or ghosts to ask for, coerce, steal, or outright force their aid. Mysticism skills must be purchased in order of level and no level may be purchased more than once. A Mystic who finds themselves close to final death finds themselves with easier access to the Deadlands — if a Mystic has no free deaths left on their character card, they will be given two additional uses of any one skill of their choice that they have purchased. Level 1: Dead Sight — view lost souls and ghosts normally invisible to the mundane eye. Level 2: Augury — consult with Spirits via a medium of their choosing. Level 3: Eyes of the Soul — touch a corpse to attempt to lure the Spirit into retelling how it died (1 in 10 chance, costs 1 hour of blindness). Level 4: Foresight — implant subconscious foresight of upcoming danger into a target. Level 5: Manifest — rise as a visible spirit during Death Count. Level 6: Grim Counsel — speak directly to spirits and ghosts; combine with Augury to target a specific spirit. Level 7: Séance — gather Mystics to summon a specific spirit to answer 3 questions. Level 8: Unfetter — Manifest without the 10-foot restriction, remaining within line-of-sight. Level 9: Haunt — attempt to have a spirit choose a home as their connection to the mortal realm. Level 10: Betwixt and Between — immunity to Forget effects, 50% chance to remember deaths, doubles Death Count while Manifesting with a lantern.'}),
    skill('Demonic/Angelic Arts',   [75,75,60,75,75,60,55,60,50], [], {max:1, desc:'Demonic/Angelic Arts allow the user to identify and recognize the various holy and unholy creatures that exist on all the planes of the Heavens and Hells. This skill may only be used to answer the following questions: "Are you a Demonic/Angelic creature?", "What kind of Demon/Angel are you?", "Are you a greater or lesser Demon/Angel?", (Angelic only) "Which God do you serve, if any?", (Demonic only) "Are you currently under contract?" These questions are asked out of game, not to the Demon or Angel directly. Characters with Demonic/Angelic Arts take 2 less damage (to a minimum of 1) from attacks by their identified target no matter the type of attack. Only one target may be active at a time. To change targets, the user may ask one of the questions above, or simply state "Demonic/Angelic Arts 1, 2, 3" if the new target has already been identified.'}),
    skill('Elemental Attunement',   [25,25,25,25,25,25,25,25,25], [{name:'Sphere of Magic: 1st',minCount:1}], {max:3, desc:'This skill will allow an Elementalist to attune themselves to an additional Element. This additional attunement may be chosen when casting spells that require one. Example: A Fire Elementalist may purchase Elemental Attunement and choose Ice. The Elementalist can now choose between Ice or Fire when casting spells that require an Elemental type such as "<type> Strike." This skill can be purchased multiple times to grant access to additional Elements. The four elements are Fire, Ice, Stone and Lightning.'}),
    skill('First Aid',              [60,60,60,60,60,60,60,60,55], [{name:'Anatomy',minCount:1}], {max:1, desc:'Allows the user to bind wounds sufficiently to stop bleeding and heal some minor wounds. The process takes 1 minute to use and as long as it is being used, the target\'s Bleed Count is halted. If First Aid is interrupted, or if the wounded target moves or is moved in any way, the skill fails and the wounded target must continue their Bleed Count from where they left off. After a successful 1 minute of First Aid, the wounded target is healed to zero Body, bringing them to unconsciousness and halting their bleeding. First Aid also allows the character to bandage a target, healing one Body for each minute of bandaging up to the maximum allowed by their Physician level. A target in their Bleed Count cannot be bandaged. The player cannot bandage the same target more than once a day. It will not affect Undead in any way, with the exception that a player with Necromantic Arts may use this skill to heal Risen in Undead form.'}),
    skill('Necromantic Arts',       [75,75,60,75,75,60,55,60,55], [], {max:1, desc:'Necromantic Arts allows a user to recognize and identify whether or not standard identifiable signs of Undeath are present in an individual. It will not verify that something is alive, only whether or not it is Undead. This skill may only be used to answer the following questions: "Are you Undead?", "What kind of Undead are you?", "Are you lesser, greater or ancient Undead?", "How much damage have you taken (only to Undead)?" Characters with Necromantic Arts take 1 less damage (to a minimum of 1) from attacks by their identified target no matter the type of attack. Only one target may be active at a time. To change targets, the user may ask one of the questions above, or simply state "Necromantic Arts 1, 2, 3" if the new target has already been identified.'}),
    skill('Physician',              [45,45,45,45,45,45,45,45,40], [{name:'First Aid',minCount:1}], {desc:'After having mastered the art of Anatomy and First Aid, a character is ready to uncover the secrets of the living body. Every level of Physician will increase the amount of Body healed through First Aid bandaging by one, to a maximum of 11. Level 1 Barber: Perform First Aid on a moving target and extend their Bleed Count by 1 minute. Level 2 Pharmacist: Identify and cure non-Magical diseases (1 minute roleplay, once per 5 days per patient). Level 3 Physicker: Identify and purge toxins; target must be lying down unmoving for 1 minute. Level 4 Doctor: Perform minor surgeries (10 minutes, patient unconscious 30 minutes after); extend a dying target\'s Death Count by 5 minutes via CPR. Level 5 Surgeon: Perform major surgeries including re-attachment of lost limbs, removal of foreign life forms, and organ transplants. Level 6 Stasis Director: With a fellow physician, postpone death indefinitely by actively role playing keeping the patient\'s vitals in check. Level 7 Vital Warden: Perform a major surgery which restores all the target\'s hit points. Level 8 War Surgeon: Bandage at a rate of 2 Body per minute when working alone. Level 9 Specialist: Use intensive care single-handedly; perform anatomy checks while using any other physician skill. Level 10 Master Physician: Major and minor surgery time and patient unconsciousness period halved; a second surgery may be performed within five days.'}),
    skill('Read & Write',           [70,60,45,55,70,45,40,50,40], [], {max:1, desc:'This skill allows the character to read and write. Without this skill, you are illiterate. Without this skill a person can only know the letters to their own name and can count on their fingers. A character with this skill can read the names of Battle Magic spell scrolls, but nothing else.'}),
    skill('Read Magic',             [45,35,20,25,40,25,15,15,25], [{name:'Read & Write',minCount:1}], {max:1, desc:'This skill allows the user to cast Battle Magic spells from scrolls. They are limited to casting only Battle Magic from spell level 1 to level 4. To activate the scroll, the caster must have enough light to properly read the scroll. They must then read and speak the incantation of the spell. When used, a Battle Magic scroll is consumed and destroyed.'}),
    skill('Read Magic: Advanced',   [50,45,30,35,50,35,25,25,35], [{name:'Read Magic',minCount:1}], {max:1, desc:'This skill is the same as Read Magic, except that it allows the user to cast Battle Magic spells from spell level 5 to level 9.'}),
    skill('Read Magic: Ritual',     [90,80,50,60,90,60,40,40,50], [{name:'Read Magic: Advanced',minCount:1}], {max:1, desc:'This skill allows the user to read Ritual Magic scrolls.'}),
    skill('Advanced Ritual Casting',[300,300,275,275,300,275,200,225,225], [{name:'Read Magic: Ritual',minCount:1}], {max:1, desc:'This skill demonstrates an advanced understanding of ritual magics. The player may now cast rituals from the Advanced Spheres, Covenant and Enchantment, which do not have Battle Magic spells. A caster is limited to one ritual circle for every Sphere of magic they can cast, plus one. Any character with Advanced Ritual Casting may add two to this limit. Covenant is a specialised ritual-only sphere focused on assisting like-minded individuals, establishing guild-like groups called "Covenants" and creating a Sanctum for them to operate within. Enchantment is a ritual-only advanced sphere that primarily facilitates the creation of magical items, including rings, cloaks, weapons, wands, and extending the duration of rituals cast from other spheres.'}),
  ]},
  {cat:'Warrior', skills:[
    skill('Ambidexterity',                    [20,30,35,40,30,45,75,75,75],   [], {max:1, desc:'This skill allows a character to wield two one-handed weapons in combat. The player may wield a Medium or Simple Weapon they have proficiency with in their main hand and a Simple Weapon in their off hand.'}),
    skill('Florentine',                       [40,40,45,70,65,70,110,110,110],[{name:'Ambidexterity',minCount:1}], {max:1, desc:'This skill improves a character\'s training in the art of two weapon fighting. The player may now wield any one-handed weapon they have proficiency with in their main and off hand.'}),
    skill('Flurry of Blows',                  [40,50,55,75,65,75,125,100,125],[], {desc:'Through discipline and training, your character has learned the secret of tapping into raw emotion and harnessing it into strength defying attacks. This skill will allow the player to swing for +5 additional damage of the character\'s normal swinging type for the next 3 swings, hit or miss. The Flurry will stay active for 1 minute. If all 3 swings are not used by the end of the minute, they are lost. To activate this skill, the player must call "Flurry of Blows". This skill does not stack with other per-day use skills, abilities or spells, or itself. This skill is usable once per day per purchase.'}),
    skill('Heavy Armour',                     [15,20,20,40,45,45,65,60,65],   [], {max:1, desc:'This skill will allow the character to wear multiple layers of armour and increase their Armour Points far past the normal maximum. With this skill, the player may stack two types of armour on one location and add their AP values. A player is still limited to the AP that their out-of-game reps allow. Armour of the same type (eg: chain on chain) will not stack.'}),
    skill('Self Mutilate',                    [15,15,15,15,15,15,15,15,15],   [], {max:1, desc:'This skill represents the character\'s ability to overcome the instinct of self-preservation. A character may not willingly accept or cause themselves 1 Body or more worth of damage without this skill, and must actively fight any attempt to harm them, even if it is in their best interest. Without Self Mutilate, you may still enter a fight even without armour, but you must fight back or defend yourself and not simply allow yourself to be injured. This skill must also be purchased for a character to actively kill themselves or to consent to their own demise.'}),
    skill('Shield',                           [50,75,60,110,120,95,140,140,140],[], {max:1, desc:'This skill allows a character to properly use a shield or buckler. A shield will stop strikes from weapons only. Shields will also block Slays, using them up without harming the shield user, even if the shield is broken by the Slay. A buckler is a small shield strapped to the forearm that acts like a normal shield but can be used while holding something in the same hand. A buckler cannot be larger than 15 inches in diameter and cannot be disarmed while strapped to the forearm. Shields will not stop packet delivered or Spellstrike attacks. Without this skill, a player may use a shield if they hold it in both hands and do not use any other skills or abilities. A character with this skill may wield two shields at the same time, but only if both are held by their handles.'}),
    // Slay/Parry: primary (max 1), each purchase requires its own Specialization prereq
    skill('Slay/Parry',                       [100,120,130,170,150,170,250,200,250],[{name:'Specialization +1: Weapon Group|Specialization +1: Weapon Specific',minCount:1}], {max:1, prereqPerPurchase:true, _weaponChoice:'specific', desc:'This skill allows a character to use one Slay or Parry, per day, with a single weapon that the character is proficient in, chosen at purchase. Each additional purchase of Slay/Parry requires an additional purchase of the weapon specialisation. The player chooses whether to use this skill as a Slay or as a Parry each time they use it. A Slay is a powerful attack which does 50 points of damage — nothing besides Slay stacking may change this number. To use a Slay, the attacker must declare "You are not prepared!" and strike their opponent, then call "50 Slay!" A Parry enables the player to parry any weapon blow, as well as touch cast spells, by calling "Parry". Parry cannot block Massive damage, Spellstrikes, or Surprise Attacks.'}),
    skill('Slay/Parry: Master',               [120,140,150,190,170,190,270,220,270],[{name:'Specialization +1: Weapon Group',minCount:1}], {max:1, prereqPerPurchase:true, _weaponChoice:'group', desc:'This skill is the same as Slay/Parry, except that it is purchased for an entire Weapon Group rather than a specific weapon. The Slay or Parry may be used with any of the weapons within that Weapon Group.'}),
    // Subsequent: requires primary purchased once (not per purchase), then same prereqs as primary per purchase
    skill('Slay/Parry: Subsequent',           [100,120,130,170,150,170,250,200,250],[{name:'Slay/Parry',minCount:1,primaryGate:true},{name:'Specialization +1: Weapon Group|Specialization +1: Weapon Specific',minCount:1}], {max:9, prereqPerPurchase:true, _weaponChoice:'specific', desc:'Requires Slay/Parry to be purchased first. Each purchase requires an additional Weapon Specialization (Group or Specific). Functions identically to Slay/Parry for a single weapon the character is proficient in, chosen at purchase.'}),
    skill('Slay/Parry: Master Subsequent',    [120,140,150,190,170,190,270,220,270],[{name:'Slay/Parry: Master',minCount:1,primaryGate:true},{name:'Specialization +1: Weapon Group',minCount:1}], {max:9, prereqPerPurchase:true, _weaponChoice:'group', desc:'Requires Slay/Parry: Master to be purchased first. Each purchase requires an additional Weapon Group Specialization. Functions identically to Slay/Parry: Master for an entire Weapon Group.'}),
    skill('Specialization +1: Weapon Group',  [120,140,150,170,150,170,250,200,250],[{name:'Weapon Group Proficiency: Medium|Weapon Group Proficiency: Large|Weapon Specific Proficiency: Exotic',minCount:1}], {_weaponChoice:'group', desc:'This skill grants the player a +1 damage bonus with any weapon from a chosen Weapon Group that the character is proficient in, selected at purchase. This skill cannot be purchased for the Exotic weapon group.'}),
    skill('Specialization +1: Weapon Specific',[100,120,130,150,130,150,230,180,230],[{name:'Weapon Group Proficiency: Medium|Weapon Group Proficiency: Large|Weapon Specific Proficiency: Exotic',minCount:1}], {_weaponChoice:'specific', desc:'This skill grants the player a +1 damage bonus with a single weapon that the character is proficient in, chosen at purchase. If purchased for Summoned Weapons it will apply to all Summoned Weapons within an individual sphere.'}),
    skill('Weapon Group Proficiency: Medium',  [40,40,40,50,50,50,80,80,80],  [], {max:1, desc:'This skill allows the player to properly wield the following one-handed weapons: Bow, Sword, Mace, Spears, Battle Axe, and any other non-Exotic weapon with a base damage of 2. Bows do Body damage.'}),
    skill('Weapon Group Proficiency: Large',   [70,70,70,100,100,100,130,130,130],[], {max:1, desc:'This skill allows the player to properly wield the following two-handed weapons: Crossbow, Sword, Axe, Mace, Pole Arm, and any other non-Exotic weapon with a base damage of 4. Bonus damage from Strength will be applied to Large Weapon swings at a rate of +1 damage for every 1 point of Strength, rather than the standard +1 damage for every 2 points. Strength bonuses will not increase Crossbow damage. Crossbows do Body damage.'}),
    skill('Weapon Specific Proficiency: Exotic',[100,100,100,130,130,130,150,150,150],[], {max:4, _weaponChoice:'exotic', desc:'This skill allows the player to properly wield one of the following weapons: Stiletto (1 Body damage), two-handed Maul (5 damage), Bastard Sword (2 damage if wielded in one hand or 4 damage if wielded in both hands), or any other weapon that does Body damage or is summoned through magical means. Bonus damage from Strength will be applied to Maul swings at a rate of +1 damage for every 1 point of Strength, rather than the standard +1 damage for every 2 points. This skill can be purchased multiple times to allow a character to become proficient in multiple Exotic Weapons.'}),
    skill('Weapon Refocus',                    [40,40,40,40,40,40,40,40,40],  [], {desc:'This skill allows the player to revisit their local training ground and upgrade their Weapon Specific Specialization +1 or Critical +2 or Slay/Parry to a Group Specialization +1 or Critical +2 or Slay/Parry: Master. This skill may only be used as an upgrade, not to downgrade a Group skill to a Weapon Specific skill.'}),
  ]},
  {cat:'Rogue', skills:[
    skill('Critical +2: Specific',            [150,125,130,120,100,130,230,180,130],[{name:'Weapon Group Proficiency: Medium|Weapon Group Proficiency: Large|Weapon Specific Proficiency: Exotic',minCount:1}], {_weaponChoice:'specific', desc:'This skill allows the player to swing for +2 damage when striking a target from behind and +½ damage from the front, with a single weapon that the character is proficient in, chosen at purchase. The attack must hit the target on the back of their body (Upper Back, Mid Back, or Lower Back locations) to grant the +2 damage. The damage call is "<damage> Critical" when striking from behind. This skill is always active.'}),
    skill('Critical +2: Group',               [170,145,150,140,120,150,250,200,150],[{name:'Weapon Group Proficiency: Medium|Weapon Group Proficiency: Large|Weapon Specific Proficiency: Exotic',minCount:1}], {desc:'This skill is the same as Critical +2: Specific, except that it is purchased for an entire Weapon Group rather than a specific weapon. The Critical may be used with any of the weapons within that Weapon Group.'}),
    // Dodge: primary max 1, then Dodge: Additional for subsequent purchases (combined max 10)
    skill('Dodge',                            [170,140,150,100,120,130,250,200,80], [{name:'Critical +2: Specific|Critical +2: Group|Feint',minCount:1}], {max:1, desc:'This skill allows the player to dodge any attack except a Surprise Attack, Gaze Attack, Power Word, Area of Effect, Massive damage attack or other unreasonable damage-causing incident, such as falling off a cliff. Dodge is a Conscious defense. This skill is usable once per day per purchase.'}),
    skill('Dodge: Additional',                [170,140,150,100,120,130,250,200,80], [{name:'Dodge',minCount:1,primaryGate:true},{name:'Critical +2: Specific|Critical +2: Group|Feint',minCount:1}], {max:9, prereqPerPurchase:true, desc:'Requires Dodge to be purchased first. Each purchase requires an additional Critical +2 (Specific or Group) or Feint. Usable once per day per purchase.'}),
    // Execute: primary max 1, Subsequent requires primary once then same prereqs per purchase
    skill('Execute',                          [170,130,150,120,100,130,250,200,150],[{name:'Critical +2: Specific|Critical +2: Group',minCount:1}], {max:1, prereqPerPurchase:true, _weaponChoice:'specific', desc:'This skill will strike the victim\'s vital organs, mortally wounding them, with a single weapon that the character is proficient in, chosen at purchase. Each additional purchase of Execute requires an additional purchase of an appropriate Critical skill. An Execute must strike the target\'s torso and directly damage their Body points, rather than armour, to be successful. A successful Execute will instantly reduce a victim\'s Body points to -1 and drop them into their Bleed Count. The call for this skill is "Execute". If used from behind and strikes between the target\'s shoulder blades, the call will be "Surprise Execute". Execute may only be used in combination with the skills Shiv, Silent Strike, and Penetration. This skill is usable once per day per purchase.'}),
    skill('Execute: Master',                  [190,150,170,150,120,150,270,220,170],[{name:'Critical +2: Group',minCount:1}], {max:1, prereqPerPurchase:true, desc:'This skill is the same as Execute, except that it is purchased for an entire Weapon Group rather than a specific weapon. The Execute may be used with any of the weapons within that Weapon Group.'}),
    skill('Execute: Subsequent',              [170,130,150,120,100,130,250,200,150],[{name:'Execute',minCount:1,primaryGate:true},{name:'Critical +2: Specific|Critical +2: Group',minCount:1}], {max:9, prereqPerPurchase:true, _weaponChoice:'specific', desc:'Requires Execute to be purchased first. Each purchase requires an additional Critical +2 (Specific or Group). Usable once per day per purchase.'}),
    skill('Execute: Master Subsequent',       [190,150,170,150,120,150,270,220,170],[{name:'Execute: Master',minCount:1,primaryGate:true},{name:'Critical +2: Group',minCount:1}], {max:9, prereqPerPurchase:true, desc:'Requires Execute: Master to be purchased first. Each purchase requires an additional Critical +2: Group. Usable once per day per purchase.'}),
    skill('Garrotte',                         [100,85,120,85,60,65,150,150,95],  [], {max:1, desc:'This skill allows a player to kill a target by simulating the use of a Garrotte or razor wire around the target\'s neck. To use a Garrotte attack, the attacker must place both hands on the shoulders of the victim from behind and call "Surprise Garrotte". If the attack succeeds, the victim is silenced and drops anything they were holding. Garroting takes 20 seconds to take effect — the attacker must call "Garrotte 1, Garrotte 2, etc." After 20 seconds, the victim falls into their Death Count. The player must have a tagged Garrotte phys-rep held in one hand for the duration. If the victim is wearing a gorget (covering the front of the neck worth at least 2 AP), the Garrotte fails. A defending player may resist a Garrotte if the defender alone has at least +2 more Strength than the attacker. This skill is usable at will.'}),
    skill('Sap',                              [55,45,50,35,35,35,60,60,40],    [], {desc:'Sap is a Surprise Attack which allows a character to knock out a victim by touching them in the Upper Back armour location with a coreless, red hand to hand weapon. The attacker must be holding the tagged weapon they are Sapping with but does not physically strike the target. Upon a successful strike, the victim loses 1 Body point and is knocked unconscious for 10 minutes. The base damage for Sap is 1 — this damage may only be increased by Strength. The call for Sap is "<damage> <type> Sap". A Sapped character will awaken only once the Sap Body point damage is healed or 10 minutes have passed. No skills, spells, or abilities may be used in conjunction with Sap, except to change the damage type. This skill is usable once per day per purchase.'}),
    skill('Vital Blow',                       [85,65,75,50,55,65,120,100,75],  [], {desc:'This skill allows the player to deliver a devastating blow to a target\'s vital organs. A Vital Blow will damage the target for half their total Body, not their current Body, rounded up. This damage cannot be altered in any way. Two successful Vital Blows within 1 hour will immediately drop the target to 0 Body. A Vital Blow must strike the target\'s torso and directly damage their Body points, rather than armour, to be successful. If used from behind and strikes between the target\'s shoulder blades, the call will be "Surprise Vital Blow". Vital Blow will not affect creatures which are non-biological in nature. This skill is usable once per day per purchase.'}),
  ]},
  {cat:'Warrior Class Frag Skills', skills:[
    fragSkill('Battlefield Repair',  25,  30, [],                                                              {desc:'With this skill a Warrior can repair any recently destroyed or shattered shield so long as they have access to the wreckage. If given the destroyed remains and the shield was destroyed within the last hour, a Warrior can perform a Battlefield Repair on it. A repair takes 1 minute for every 10 threshold the shield had. If the repair is interrupted or an hour passes since its destruction and the shield is not fully repaired, the skill will fail and be used for the day. Lastly, this skill may be used to restore 1 "resist" on a Master Crafted shield. Master Crafted shields which do not have their resists repaired within the time limit will lose that resist forever. This skill is usable once per day per purchase.'}),
    fragSkill('Cripple',             30,  40, [],                                                              {desc:'This skill allows the warrior to attack a target\'s limb with a devastating crippling attack. If the attack is successful, Cripple does one Body to the target and cripples the struck limb for 5 seconds. If the limb is an arm, the target will be disarmed and unable to use that arm. A crippled leg denies the target the ability to move for the duration. Cripple must strike a limb to be successful. The damage call for this ability is "Cripple!" If the weapon\'s damage type is not normal, the damage type precedes "Cripple". There is no numerical value, so when determining if the attack is stopped by a threshold, only the damage threshold type is taken into account. Cripple cannot be stacked with any other ability and is usable once per day per purchase.'}),
    fragSkill('Decapitate',          75, 150, [{name:'Slay/Parry',minCount:1}],                               {prereqPerPurchase:true, desc:'This powerful ability attempts to separate the head from the body of a target and kill them in a single shot. Decapitate can only be used with a melee weapon the warrior is capable of Slaying with. The warrior must declare "You are not prepared!" then strike their opponent on the torso. The damage call is "10 Body Decapitate". If the target\'s Body is damaged they are immediately dropped into their Death Count. Creatures with no discernible heads are immune. Unlike a Slay, Decapitate does not remain active if the initial strike misses. The numerical damage cannot be changed, but the damage type may be altered. This skill is usable once per day per purchase and requires 1 Slay purchase for every purchase of Decapitate.'}),
    fragSkill('Dirt in the Eye',     30,  45, [],                                                              {desc:'This skill allows the warrior to temporarily blind a target by throwing dirt in their eyes. This is a packet-delivered attack and will not be successful if used with a weapon or if touch cast. The warrior must first touch a packet to the ground then successfully hit the target. The call for this ability is "Physical Dirt in the Eye!" Dirt in the Eye will blind the target for ten seconds. This skill cannot be stacked with any other ability or spell and is usable once per day per purchase.'}),
    fragSkill('Disembowel',          75, 100, [{name:'Specialization +1: Weapon Group|Specialization +1: Weapon Specific',minCount:1}], {desc:'This ability allows the warrior to create a grievous gash in the target\'s torso. The attack must strike the target\'s torso from the front. The call is "5 Body Disembowel" (or whatever damage type the weapon deals). If a target struck with this attack does not drop everything and use both hands to hold onto their lower stomach, they suffer a Death effect after 10 seconds. If the target does hold onto their guts, they have 1 minute before the Death effect. Healing the 5 Body damage before the time passes will stop the Death effect entirely. Disembowel does not affect creatures with alien physiology. The weapon used must be the same as the weapon with the prerequisite Specialization. This ability is useable once per day per purchase.'}),
    fragSkill('Trip',                20,  30, [],                                                              {desc:'A combat skill for warriors. To activate, the player must successfully strike the target\'s leg with a weapon and call "1 Body Trip!" If successful, the target must fall safely to the ground. The target may stand up again as soon as they have touched their torso to the ground. The damage type is based on the weapon used. Usable once per day per purchase.'}),
    fragSkill('Whirlwind of Blows',  40,  75, [{name:'Flurry of Blows',minCount:1}],                          {prereqPerPurchase:true, desc:'This skill enables a warrior to plant one foot, call "Whirlwind of Blows" and gain +5 damage to their swings. This effect continues indefinitely so long as one foot remains planted. The planted foot may swivel, but the skill ends if the planted foot is moved or raised. This skill may stack with other skills, abilities or spells unless otherwise stated. This skill is usable once per day per purchase and requires 1 Flurry of Blows purchase for every purchase of Whirlwind of Blows.'}),
  ]},
  {cat:'Rogue Class Frag Skills', skills:[
    fragSkill('Blindfighter',  15,  15, [], {desc:'Once per day per purchase, the character may resist a Blind effect.'}),
    fragSkill('Escape',        20,  50, [], {desc:'Once per day per purchase, the character may break free of any physical binding, as well as Leg Snare and Net traps. Examples of bindings are shackles, rope, manacles, etc. Doing so requires a 10 count which may be done in silence. Escape may not be used to free the rogue from locked areas, such as prison rooms or crow\'s cages.'}),
    fragSkill('Riposte',       75, 150, [], {desc:'The rogue with Riposte can use this ability against any attack that could be parried. After suffering an attack, a character with this ability may call "Riposte!" if they are holding a weapon. Doing so not only blocks the attack but also deals back to the original target the same damage and effects that were Riposted, which automatically hits. Ripostes can block missile damage, but the damage is not reflected back. The damage from a Riposte counter can be defended against with skills (Parry, Dodge, etc.) and spells (Magic Armour, etc.) but is considered to have been a successful strike. Riposte may be used once a day per purchase.'}),
    fragSkill('Sucker Punch',  30,  65, [], {desc:'This skill allows the rogue to sneak in a devastating attack to an unprepared opponent, stunning them for a short time. If the attack is successful, the target takes one Body, is blinded and is stunned for 5 seconds. While stunned, a victim is unable to take any action, including blocking, moving and the use of skills, minus the ability to call "interrupt" against Killing Blows and any counts against them. Automatic defenses such as Shield Magic will still operate, but ones requiring conscious thought such as Advanced Shield Magic will not. This skill may use the "Surprise" suffix if the attack is delivered from behind and between the target\'s shoulder blades. The rogue must strike the opponent on the torso with a red hand-to-hand or claw rep. The call is "Sucker Punch!" This skill cannot be stacked with any other skill and is usable once per day per purchase.'}),
    fragSkill('Thieves Cant',  20,  25, [], {max:1, desc:'This skill allows rogues access to a fundamental secret language understood by thieves universally. Thieves Cant is a fully coded language that is ever changing and evolving, so it can never be permanently broken by authorities. Upon purchase, the Rogue will receive an Out-of-Game decoder which will allow them to read and write messages in Thieves Cant. This code may not be given in written form to any other player. Rogues with this skill will always be updated with a new decoder packet by the Logistics Marshal should any change occur. You must possess the skill Thieves Cant to read Thieves Cant. Once purchased, this skill is always active.'}),
    fragSkill('Tumble',        30,  65, [], {desc:'Agility and dexterity are the tools of the rogue. By rolling with the punches, a rogue can tumble to take half damage (rounded down) from one single Area of Effect or Massive damage effect of their choice. The source of damage must contain a numerical damage amount. This skill has no effect on other negative effects such as paralyze, death, stun, etc. Tumble cannot stack with any other skill, including additional uses of Tumble, nor can any other method of damage reduction be applied prior to or after use. The defensive call is "Tumble!" This skill is usable once per day per purchase.'}),
  ]},
  {cat:'Scholar Class Frag Skills', skills:[
    fragSkill('Combat Wizardry', 50, 50, [{name:'Self Mutilate',minCount:1}], {max:1, desc:'When a mage purchases Combat Wizardry, their spell casting is no longer interrupted by Body damage. They may also speak while maintaining concentration. This skill is considered "always on".'}),
    fragSkill('Harvest',         50, 50, [],                                  {desc:'Once per day per purchase, when a mage casts a spell and it is blocked by a spell defense, they may call "Harvest!" and regain that spell in memory to cast again. This ability only functions if the spell is defended against with a magical protection like Shield Magic, or a Resist Magic natural ability or racial.'}),
    fragSkill('Mortician',       75, 25, [{name:'Anatomy',minCount:1}],       {desc:'This macabre ability allows the Mortician to examine a finalled corpse to determine what led to its demise. The skill will never identify a specific killer. It takes 10 seconds of examining the corpse to reveal the answer to each question: "Were you killed by magic, alchemy, or physical means?", "What was the sphere of magic/specific alchemy/weapon group that killed you?", "How long have you been a corpse?", "Has your body been moved?", "Were you taken by Surprise?" Morticians can also manipulate bodies to make future Morticians receive false information. Additionally, Morticians can look at a living or dead person\'s mole, birthmark or third nipple and determine whether it is a natural mark or one created supernaturally via Wytchcraft.'}),
    fragSkill('Refocus',         30, 30, [],                                  {desc:'Once per day per purchase with Refocus, when a mage casts a spell and misses their target with a spell packet, they may call "Refocus!" and regain that spell in memory to cast again.'}),
    fragSkill('Spell Parry',     35, 35, [],                                  {desc:'The Spell Parry skill allows a mage to counter a Battle Magic spell cast at them by using up a spell of the same sphere and level that they have memorized. If targeted and affected by a spell, the mage may expend a spell of the same sphere and level in memory and call "Spell Parry <spell name>!", nullifying the incoming spell but losing the spell in memory. If the mage whose spell was Spell Parried also possesses this skill, they may also call "Spell Parry!" to force their original spell through, expending another memorized spell. There is no limit to how often this ability may be used so long as the mage has spells in memory to counter. This ability only functions against magic spells cast from memory or via a magic item. It has no effect against natural abilities or monster racials.'}),
    fragSkill('Spell Switch',    50, 50, [],                                  {desc:'Once per day per purchase, the mage may exchange one spell they have memorized for another spell at a lower level. Spells may be switched with different spheres the caster knows, but they can never be equal or higher level. To use this ability the mage must declare: "Spell Switch: <spell being sacrificed> <new spell>". The new spell must be cast within 60 seconds of Spell Switch being used or both spells are lost.'}),
    fragSkill('Spell Versatility',0,  0, [],                                  {desc:'Spell Versatility is a Mage skill tied to an existing spell slot the character already owns. After purchasing Spell Versatility, the mage no longer has to memorize a specific spell for that slot and may cast spells "on the fly" from any of their spheres that can fill the slot. The Mage must still have the scrolls for any spells they wish to use with them at reset to study. Once a spell has been cast from the slot it is used until next reset. The frag cost is half the level of the slot being augmented + 5, and the CP cost is the same. This skill must be purchased per slot.'}),
  ]},
  {cat:'Frag Skills', skills:[
    fragSkill('Arcane Spirit',      10,  10, [], {desc:'Each purchase of this skill will allow a character to have 10 additional levels of rituals on their spirit, beyond the usual cap of 50 levels of rituals, total.'}),
    fragSkill('Battlefield Medic',  50,  75, [{name:'First Aid',minCount:1}], {max:1, desc:'This skill reduces the time it takes to stabilise a patient using First Aid. The Battlefield Medic takes only 40 seconds instead of 60 to bring a target from their Bleed Count to 0 Body. If the Battlefield Medic is assisted by someone with First Aid, the time comes down to 30 seconds. If two Battlefield Medics work to stabilise a patient together, it takes 20 seconds. This skill may only be purchased once.'}),
    fragSkill('Cold Dead Hands',    30,  20, [], {desc:'Characters with Cold Dead Hands will continue to hold onto whatever they were carrying if they become unconscious, asleep, or fall into their Bleed or Death counts. This does not render the character immune to disarming effects, including Garrotte. In order for items to be removed from the character\'s Cold Dead Hands, a standard loot count must be performed.'}),
    fragSkill('Create Alcohol',     10,  25, [], {desc:'With this skill, a character can create potent brews and drinks. For the first purchase, your character can create up to 3 Alcohol tags from a pool of 3 Stamina, divided up as the character wishes. Alcohol tags can only be created at Logistics but may have any name the brewer wishes. For each subsequent purchase, the character will have +3 Stamina added to their pool and create +1 Alcohol tag. Each Alcohol tag has 5 servings. A character with Create Alcohol can determine the Stamina damage value of an alcoholic beverage by examining it. Alcohol is considered a poison for the purpose of defending against or removing it.'}),
    fragSkill('Heavy Drinker',      10,  20, [], {max:1, desc:'This ability is purchasable by any character class and doubles their stamina total. This skill cannot be purchased more than once.'}),
    fragSkill('Intuition',          50,  50, [], {desc:'Whether from a sudden tingling feeling or the sensation of being watched, characters with Intuition are aware when they respond to Sense calls (or when they avoid a Sense call they would otherwise respond to due to Possuming or another effect). Characters will know the direction and rough location of what sensed them, but not exactly who or what did it. They will not know what the Sense call was looking for, only that it found them.'}),
    // Looting: Nightblade pays 10 CP, all others pay 15 CP
    {name:'Looting', frag:5, cp:15, costs:[15,15,15,10,15,15,15,15,15], maxPurchases:5, bodyBonus:0, strBonus:0, prereqPerPurchase:false, prereqs:[], _fragOnly:true,
     desc:'This skill trains the player in the art of both hiding and finding. This skill allows the target to subtract ten seconds from the standard 60-second loot count for every level of Looting they have purchased, to a minimum of ten seconds. This skill will also add ten seconds per level to any person trying to loot the player with the Looting skill. If a player with Looting is being looted, they need not inform the looter how long they will have to loot for OOG. Should the searching player search for the appropriate additional time, the target must give the searching player all items as per standard searching rules. This ability can be purchased a maximum of five times.'},
    {name:'Paragon', frag:100, cp:0, costs:null, maxPurchases:1, bodyBonus:0, strBonus:0, prereqPerPurchase:false, prereqs:[], _fragOnly:true, _paragon:true,
     desc:'Paragons are those who have proven to be faithful adherents of their God, without having devoted their lives to their service. Being a Paragon allows a character to add one Light or Dark spell, no higher than 7th circle depending on the God served, to their repertoire. Once the spell is chosen, the choice is permanent. The Paragon may then memorize that spell in the place of one of their regular spell slots. The Paragon must have a holy symbol to memorize and cast the spell. Requires Lead Shaper Approval. CP cost equals the level of the chosen spell slot + 10. Requires at least 1 spell slot. This skill may only be purchased once ever.'},
    fragSkill('Possum',             25,  30, [], {desc:'After lying still for 10 seconds, a character may activate Possum and become immune to Sense Life calls. This works for up to an hour or until the character moves or is moved. OOG movement to get comfortable, breathe, swat mosquitos, etc., will not end the effect. This ability is usable once per day per purchase.'}),
    fragSkill('Teacher',            50,  15, [], {desc:'Purchasing this skill allows a character to teach another character a Vocation or non-Renowned Frag Sphere that they currently have on their character sheet, once. If the Teacher wishes to teach further students, they must pay the frag cost, but not the CP cost, again for each thing taught. Teachers may only teach players from the Teacher\'s home guild. The amount of time and steps required to learn a Vocation or Sphere are determined by the Teacher.'}),
  ]},
];

// ---- State ----
let s = { name:'', race:'', culture:'', occupation:'', vocation:'', blankets:0, owned:[], openCats:{General:false, 'Frag Skills':false, Production:false, Scholar:false, 'Scholar Class Frag Skills':false, Warrior:false, 'Warrior Class Frag Skills':false, Rogue:false, 'Rogue Class Frag Skills':false, Racial:false}, hovered:null, s_school_1:'', s_school_2:'', s_school_3:'', elementalAttunements:[] };

// ---- Helpers ----
function getRaceData(){
  if(!s.race) return null;
  return RACES[s.race] || FRAG_RACES[s.race] || null;
}

function getCultureData(){
  if(!s.culture) return null;
  return CULTURES[s.culture] || null;
}

function getRaceFragCost(){
  if(!s.race) return 0;
  const fr = FRAG_RACES[s.race];
  return fr ? fr.fragCost : 0;
}

function getCultureFragCost(){
  return s.culture ? 100 : 0;
}

function getRacialAutoSkills(){
  const rd = getRaceData();
  if(!rd) return [];
  return (rd.auto||[]).map(a=>({...a, _auto:true, _racial:true, _cat:'Racial', cp:0, frag:0, bodyBonus:a.bodyBonus??0, strBonus:a.strBonus??0, costs:null, prereqs:[], maxPurchases:1}));
}

// Culture replaces racial purchased skills; auto skills remain from race
function getRacialPurchasedSkills(){
  const cd = getCultureData();
  if(cd) return (cd.purchased||[]).map(sk=>({...sk, _racial:true, _culture:true}));
  const rd = getRaceData();
  if(!rd) return [];
  return (rd.purchased||[]).map(sk=>({...sk, _racial:true}));
}

// ---- Culture change ----
function onVocationChange(val){
  // Remove previous vocation unlock skill, vocation/occ abilities, and auto-bought prereqs
  s.owned = s.owned.filter(o=>!o._vocationAbility && !o._occAbility && !o._favouredUnlock && !o._vocPrereq);
  s.vocation = val;
  if(val && FAVOURED_VOCATIONS[val]){
    s.owned.push({
      name:`Favoured: ${val}`,
      _favouredUnlock: true, _cat:'Frag Skills',
      cp: FAVOURED_VOCATIONS[val].cpCost,
      frag: 0, bodyBonus: 0, strBonus: 0,
      costs: null, prereqs: [], maxPurchases: 1,
      desc: `Unlocks the ${val} Favoured Vocation for ${FAVOURED_VOCATIONS[val].cpCost} CP. ${FAVOURED_VOCATIONS[val].prereqs}`,
    });
    showFavouredVocationDetail(val);
  } else if(val) {
    showVocationDetail(val);
  }
  // Auto-buy vocation skill prerequisites
  if(val) autoBuyVocationPrereqs(val);
  repriceCostdSkills();
  render();
}

function showFavouredVocationDetail(vocName){
  const voc = FAVOURED_VOCATIONS[vocName];
  if(!voc) return;
  const panel = document.getElementById('detail-panel');
  panel.innerHTML = `
    <div class="detail-name">${vocName}</div>
    <div class="detail-meta">
      <span class="tag" style="background:var(--color-background-warning);color:var(--color-text-warning)">Favoured Vocation</span>
      <span class="tag">${voc.group}</span>
      <span class="tag frag">${voc.fragCost} frags</span>
      <span class="tag">${voc.cpCost} CP unlock</span>
      ${voc.exclusiveSphere ? `<span class="tag race-req">${voc.exclusiveSphere} sphere</span>` : ''}
    </div>
    <div class="detail-desc" style="margin-top:8px;white-space:pre-line">${voc.lore}</div>
    <hr class="detail-divider">
    <div class="detail-stat-row"><span class="detail-stat-lbl">Prerequisites</span><span class="detail-stat-val">${voc.prereqs}</span></div>
    <div style="font-size:11px;color:var(--color-text-tertiary);font-style:italic;margin-top:8px">Replaces occupational abilities with: ${voc.abilities.map(a=>a.name).join(', ')}</div>
    <div style="font-size:11px;color:var(--color-text-tertiary);font-style:italic;margin-top:4px">Applies ${voc.group} skill cost table to all purchases.</div>
  `;
}

function showVocationDetail(vocName){
  const voc = VOCATIONS[vocName];
  if(!voc) return;
  const panel = document.getElementById('detail-panel');
  panel.innerHTML = `
    <div class="detail-name">${vocName}</div>
    <div class="detail-meta"><span class="tag">Vocation</span><span class="tag frag">150 frags</span></div>
    <div class="detail-desc" style="margin-top:8px;white-space:pre-line">${voc.lore}</div>
    <hr class="detail-divider">
    <div class="detail-stat-row"><span class="detail-stat-lbl">Prerequisites</span><span class="detail-stat-val">${voc.prereqs}</span></div>
    <div style="font-size:11px;color:var(--color-text-tertiary);font-style:italic;margin-top:8px">Replaces occupational abilities with: ${voc.abilities.map(a=>a.name).join(', ')}</div>
  `;
}

function populateVocationDropdown(){
  const sel = document.getElementById('sel-voc');
  const current = s.vocation;
  sel.innerHTML = '<option value="">— select —</option>';

  // Regular vocations
  const regGroup = document.createElement('optgroup');
  regGroup.label = 'Vocations (150 frags)';
  Object.keys(VOCATIONS).forEach(name=>{
    const opt = document.createElement('option');
    opt.value = name; opt.textContent = name;
    if(name === current) opt.selected = true;
    regGroup.appendChild(opt);
  });
  sel.appendChild(regGroup);

  // Favoured vocations grouped by Champion / Demagogue
  ['Champion','Demagogue'].forEach(group=>{
    const favGroup = document.createElement('optgroup');
    favGroup.label = `Favoured: ${group} (250 frags + 50 CP)`;
    Object.entries(FAVOURED_VOCATIONS).filter(([,v])=>v.group===group).forEach(([name])=>{
      const opt = document.createElement('option');
      opt.value = name; opt.textContent = name;
      if(name === current) opt.selected = true;
      favGroup.appendChild(opt);
    });
    sel.appendChild(favGroup);
  });
}


function onCultureChange(val){
  s.culture = val;
  s.owned = s.owned.filter(o=>!o._racial || o._auto);
  if(val) showCultureDetail(val);
  render();
}

function showCultureDetail(cultureName){
  const cd = CULTURES[cultureName];
  if(!cd) return;
  const panel = document.getElementById('detail-panel');
  panel.innerHTML = `
    <div class="detail-name">${cultureName}</div>
    <div class="detail-meta"><span class="tag">Culture</span> <span class="tag frag">100 frags</span> <span class="tag race-req">${cd.races.join(', ')}</span></div>
    <div class="detail-desc" style="margin-top:8px">${cd.lore}</div>
    <hr class="detail-divider">
    <div class="detail-stat-row"><span class="detail-stat-lbl">Racial Characteristic Addition</span><span class="detail-stat-val">${cd.racialCharacteristicAddition}</span></div>
    <div style="margin-top:10px"><span style="font-size:11px;font-weight:600;color:var(--color-text-secondary);text-transform:uppercase;letter-spacing:0.5px">Indoctrination Rite</span><div class="detail-desc" style="margin-top:6px;white-space:pre-line">${cd.indoctrination}</div></div>
    <div style="font-size:11px;color:var(--color-text-tertiary);font-style:italic;margin-top:8px">Replaces racial purchasable skill with: ${(cd.purchased||[]).map(p=>p.name).join(', ')}</div>
  `;
}

// ---- Race change ----
function onRaceChange(val){
  s.race = val;
  s.culture = '';
  s.owned = s.owned.filter(o=>!o._racial);
  // Rebuild culture dropdown
  const sel = document.getElementById('sel-culture');
  sel.innerHTML = '<option value="">— select —</option>';
  if(val){
    Object.entries(CULTURES).filter(([,cd])=>cd.races.includes(val)).forEach(([name])=>{
      const opt = document.createElement('option');
      opt.value = name; opt.textContent = name;
      sel.appendChild(opt);
    });
    showRaceDetail(val);
  } else {
    document.getElementById('detail-panel').innerHTML = '<div class="detail-empty">Hover a skill to see details</div>';
  }
  render();
}


function calcCP(blankets){
  const rd=getRaceData(); const bonus=rd?rd.cpBonus:0;
  if(blankets===0) return 150+bonus;
  let remaining=blankets, totalCP=150, rowIdx=0;
  while(remaining>0 && rowIdx<TABLE.length){
    const row=TABLE[rowIdx], nextRow=TABLE[rowIdx+1];
    if(!nextRow){ totalCP+=remaining*row.cpPer; remaining=0; }
    else{ const cpNeeded=nextRow.threshold-totalCP; const blanketsNeeded=Math.ceil(cpNeeded/row.cpPer); if(remaining>=blanketsNeeded){ totalCP+=blanketsNeeded*row.cpPer; remaining-=blanketsNeeded; rowIdx++; } else{ totalCP+=remaining*row.cpPer; remaining=0; } }
  }
  return Math.round(totalCP)+bonus;
}

function getLevelFromCP(cp){
  const rd=getRaceData(); const bonus=rd?rd.cpBonus:0; const adjCP=cp-bonus;
  const last=TABLE[TABLE.length-1];
  const prev=TABLE[TABLE.length-2];
  const CP_PER_LEVEL = last.threshold - prev.threshold; // 100
  const warriorInc = last.warrior - prev.warrior; // +2 per level
  const rogueInc   = last.rogue   - prev.rogue;   // +1 per level
  // Scholar: +1 every level EXCEPT levels divisible by 3 (skip at L3,6,9,12,15,18,21,24...)
  // scholarAtLevel(n) = 3 + count of levels 2..n where level%3 !== 0
  function scholarAtLevel(n){
    // levels 1..n where scholar increases: all except multiples of 3
    // increases = n-1 - floor((n-1)/3) ... but easier: sum from table then extrapolate
    // For n <= 20 use table; for n > 20 use formula
    const skips = Math.floor(n / 3); // levels 3,6,9... up to n
    // scholar starts at 3 at level 1, gains +1 per non-multiple-of-3 transition
    // transitions from L1 to Ln = n-1 total; skips = floor(n/3) of those
    return 3 + (n - 1) - Math.floor(n / 3);
  }
  if(adjCP>=last.threshold){
    const extraCP=adjCP-last.threshold;
    const extraLevels=Math.floor(extraCP/CP_PER_LEVEL);
    if(extraLevels===0) return last;
    const newLevel = last.level + extraLevels;
    return {
      level:   newLevel,
      threshold: last.threshold + extraLevels * CP_PER_LEVEL,
      cpPer:   last.cpPer,
      warrior: last.warrior + extraLevels * warriorInc,
      rogue:   last.rogue   + extraLevels * rogueInc,
      scholar: scholarAtLevel(newLevel),
    };
  }
  for(let i=TABLE.length-1;i>=0;i--){ if(adjCP>=TABLE[i].threshold) return TABLE[i]; }
  return TABLE[0];
}

function blanketsNeededToEarnCP(currentCPTotal, deficit){
  if(deficit<=0) return 0;
  const rd=getRaceData(); const bonus=rd?rd.cpBonus:0;
  const adjCP=currentCPTotal-bonus;
  const last=TABLE[TABLE.length-1];
  let rowIdx=0;
  for(let i=TABLE.length-1;i>=0;i--){ if(adjCP>=TABLE[i].threshold){ rowIdx=i; break; } }
  let blankets=0, cp=currentCPTotal, remaining=deficit;
  while(remaining>0){
    const row=rowIdx<TABLE.length?TABLE[rowIdx]:last;
    const nextRow=rowIdx+1<TABLE.length?TABLE[rowIdx+1]:null;
    const cpToNext=nextRow?(nextRow.threshold-(cp-bonus)):Infinity;
    const blanketsToNext=nextRow?Math.ceil(cpToNext/row.cpPer):Infinity;
    const blanketsForDeficit=Math.ceil(remaining/row.cpPer);
    if(!nextRow||blanketsForDeficit<=blanketsToNext){ blankets+=blanketsForDeficit; remaining=0; }
    else{ blankets+=blanketsToNext; remaining-=blanketsToNext*row.cpPer; cp+=blanketsToNext*row.cpPer; rowIdx++; }
  }
  return blankets;
}

function getBodyBonus(){
  const flatBonus = s.owned.filter(o=>o.bodyBonus).reduce((a,o)=>a+(o.bodyBonus||0),0);
  const rd = getRaceData();
  const level = getCurrentLevel();
  // Ogre: +2 Body per level
  const perLevelBonus = rd && rd.bodyBonusPerLevel ? rd.bodyBonusPerLevel * level : 0;
  return flatBonus + perLevelBonus;
}

function getStrBonus(){
  const flatBonus = s.owned.filter(o=>o.strBonus).reduce((a,o)=>a+(o.strBonus||0),0);
  const rd = getRaceData();
  const level = getCurrentLevel();
  // Minotaur: +1 Strength per 5 levels starting at level 1 (L1=1, L6=2, L11=3...)
  const perFiveLevelBonus = rd && rd.strBonusPerFiveLevels
    ? rd.strBonusPerFiveLevels * Math.ceil(level / 5)
    : 0;
  // Blacksmith: +1 Strength at level 6, another +1 at level 10
  const bsCount = getPurchaseCount('Blacksmith');
  const bsBonus = bsCount >= 10 ? 2 : bsCount >= 6 ? 1 : 0;
  return flatBonus + perFiveLevelBonus + bsBonus;
}
function getCurrentLevel(){ return getLevelFromCP(calcCP(s.blankets)).level; }
function getPurchaseCount(name){
  return s.owned.filter(o=>!o._auto && (o.name===name || o._baseSkillName===name)).length;
}

// Build all available skills list (for gate evaluation)
function buildSkillCatList(){
  const occClass = OCC_CLASS[s.occupation] || null;

  const FRAG_CAT_CLASS = {
    'Warrior Class Frag Skills': 'warrior',
    'Rogue Class Frag Skills':   'rogue',
    'Scholar Class Frag Skills': 'scholar',
  };

  const allCats = SKILLS.map(c=>({...c, skills:[...c.skills]}));
  const result = [];

  allCats.forEach(cat => {
    // Skip — all of these are inserted manually below
    if(FRAG_CAT_CLASS[cat.cat]) return;
    if(cat.cat === 'General') return;
    if(cat.cat === 'Frag Skills') return;

    result.push(cat);

    if(cat.cat === 'Warrior' && occClass === 'warrior'){
      const fc = allCats.find(c=>c.cat==='Warrior Class Frag Skills');
      if(fc) result.push(fc);
    }
    if(cat.cat === 'Rogue' && occClass === 'rogue'){
      const fc = allCats.find(c=>c.cat==='Rogue Class Frag Skills');
      if(fc) result.push(fc);
    }
    if(cat.cat === 'Scholar' && occClass === 'scholar'){
      const fc = allCats.find(c=>c.cat==='Scholar Class Frag Skills');
      if(fc) result.push(fc);
    }
  });

  // Racial goes first
  result.unshift({cat:'Racial', skills: getRacialPurchasedSkills()});
  if(s.openCats['Racial']===undefined) s.openCats['Racial']=false;

  // Frag Skills — always visible, sits between Racial and Occupational Abilities
  const genFrag = allCats.find(c=>c.cat==='Frag Skills');
  if(genFrag){
    result.splice(1, 0, genFrag);
    if(s.openCats['Frag Skills']===undefined) s.openCats['Frag Skills']=false;
  }

  // Occupational Abilities — after Racial and Frag Skills
  const occSkills = getOccAbilitySkills();
  if(occSkills.length){
    result.splice(2, 0, {cat:'Occupational Abilities', skills: occSkills});
    if(s.openCats['Occupational Abilities']===undefined) s.openCats['Occupational Abilities']=false;
  }

  // Remove old Frag Skills insert-at-index-2 block (now handled above)
  result.forEach(c=>{ if(s.openCats[c.cat]===undefined) s.openCats[c.cat]=false; });
  return result;
}

function ordinal(n){
  const suffixes=['th','st','nd','rd'];
  const v=n%100;
  return n+(suffixes[(v-20)%10]||suffixes[v]||suffixes[0]);
}

function allSkills(){ return buildSkillCatList().flatMap(c=>c.skills); }

// ---- Gate evaluation ----
// Returns null if purchasable, or a reason string if not
function getBlockReason(sk, ignoreMax){
  // Spell slot entry
  if(sk._spellSlotEntry){
    if(getPurchaseCount('Sphere of Magic: 1st') === 0) return 'prereq|Sphere of Magic: 1st|1';
    if(getSpellSlotCount() >= 45) return 'maxed';
    return null;
  }
  // Ritual slot entry
  if(sk._ritualSlotEntry){
    if(getPurchaseCount('Read Magic: Ritual') === 0) return 'prereq|Read Magic: Ritual|1';
    if(getSlotsByLevel()[9] < 1) return 'prereq|9th Circle slot|1';
    if(getRitualSlotCount() >= 10) return 'maxed';
    return null;
  }

  const count = getPurchaseCount(sk.name);
  const maxP = sk.maxPurchases || DEFAULT_MAX;
  const currentLevel = getCurrentLevel();

  // Elemental Attunement: max 3 purchases via skill (4 total inc. primary), needs Elemental sphere + primary attunement
  if(sk.name === 'Elemental Attunement'){
    const hasElemental = [s.s_school_1,s.s_school_2,s.s_school_3].includes('Elemental');
    if(!hasElemental) return 'prereq|Elemental Sphere|1';
    if(s.elementalAttunements.length === 0) return 'prereq|Primary Elemental Attunement|1';
    const skillPurchases = s.owned.filter(o=>o._elementalAttunement).length;
    if(skillPurchases >= 3) return 'maxed';
    if(s.elementalAttunements.length >= 4) return 'maxed'; // all 4 elements already attuned
  }
  if(sk._paragon){
    if(s.vocation && FAVOURED_VOCATIONS[s.vocation]) return 'paragon_favoured';
    if(s.owned.some(o=>o._paragon && !o._auto)) return 'maxed';
    if(getSpellSlotCount() === 0) return 'paragon_no_slots';
  }

  // Max purchases check (applies to all non-paragon, non-racial skills)
  if(!sk._paragon && !sk._racial && !ignoreMax && count >= maxP) return 'maxed';
  // Skip race check for racial category skills — they're already filtered to current race
  if(sk.raceReq && sk.raceReq !== s.race && !sk._racial) return 'race';

  // Racial skills: total racial purchases capped at ceil(currentLevel/2) (1 per odd level)
  if(sk._racial && !sk._auto){
    const maxAtLevel = Math.ceil(currentLevel / 2);
    const totalRacialOwned = s.owned.filter(o=>o._racial && !o._auto).length;
    if(!ignoreMax && totalRacialOwned >= maxAtLevel) return 'level';
  }

  // Occupational abilities: tier level gate (3rd, 6th, 9th, 12th)
  if(sk._occAbilityTier && currentLevel < sk._occAbilityTier){
    return `prereq|Level ${sk._occAbilityTier}|1`;
  }

  // Occupational skills: odd levels only
  if(sk.occupational && !sk._occAbilityTier && currentLevel % 2 === 0) return 'level';

  // Check prerequisites
  for(const pre of (sk.prereqs||[])){
    if(pre.name && pre.name.startsWith('Level ')){
      const reqLevel = parseInt(pre.name.split(' ')[1]);
      if(currentLevel < reqLevel) return `prereq|${pre.name}|1`;
    } else {
      const options = pre.name.split('|');
      const need = pre.minCount || 1;
      // primaryGate: flat one-time check — just needs 1 purchase regardless of how many times this skill is bought
      // prereqPerPurchase (non-primaryGate): need N copies of prereq for Nth purchase of this skill
      const required = (!pre.primaryGate && sk.prereqPerPurchase) ? need * (count + 1) : need;
      const have = options.reduce((sum, opt) => sum + getPurchaseCount(opt.trim()), 0);
      if(have < required){
        const label = options.join(' or ');
        return `prereq|${label}|${required}`;
      }
    }
  }
  return null;
}

// When occupation changes, re-price all owned costed skills at new occupation rate
function repriceCostdSkills(){
  s.owned.forEach(o=>{
    if(!o._auto && o.costs){
      o.cp = getSkillCost(o);
    }
  });
}

// When blankets/occupation/race changes, strip any purchased skills that no longer meet gates
function revalidateAll(){
  const currentLevel = getCurrentLevel();
  const toRemove = [];

  s.owned.filter(o=>!o._auto).forEach(o=>{
    // Occupational skills locked to odd levels
    if(o.occupational && !o._occAbilityTier && currentLevel % 2 === 0){
      toRemove.push(o.name || o._baseSkillName);
    }
    // Occupational ability tier gates (tier 1=3, 2=6, 3=9, 4=12)
    if(o._occAbilityTier && currentLevel < o._occAbilityTier){
      toRemove.push(o.name || o._baseSkillName);
    }
  });

  // Racial skill cap: total racial purchases capped at ceil(level/2)
  const racialMaxAtLevel = Math.ceil(currentLevel / 2);
  const racialOwned = s.owned.filter(o=>o._racial && !o._auto);
  if(racialOwned.length > racialMaxAtLevel){
    // Remove the most recently purchased racial skills (from end of owned array) to bring under cap
    const excess = racialOwned.length - racialMaxAtLevel;
    // Find the last N racial owned entries and mark them for removal
    const toRemoveRacial = racialOwned.slice(-excess).map(o=>o.name);
    toRemoveRacial.forEach(n=>toRemove.push(n));
  }

  if(toRemove.length){
    const names = [...new Set(toRemove)];
    const cascade = collectDependents(names);
    const allRemove = [...new Set([...names, ...cascade])];
    allRemove.forEach(name=>{
      // Also clean up attunements
      s.owned.filter(o=>(o.name===name||o._baseSkillName===name)&&!o._auto&&o._elementalAttunement)
        .forEach(o=>{ if(o._chosenElement) s.elementalAttunements=s.elementalAttunements.filter(e=>e!==o._chosenElement); });
      s.owned = s.owned.filter(o=>!((o.name===name||o._baseSkillName===name)&&!o._auto));
    });
  }
}

// Find all owned skills that have a prereq in 'removedNames'
function collectDependents(removedNames){
  const result = new Set();
  let changed = true;
  while(changed){
    changed = false;
    allSkills().forEach(sk=>{
      if(result.has(sk.name)) return;
      const skCount = getPurchaseCount(sk.name);
      if(skCount === 0) return;
      for(const pre of (sk.prereqs||[])){
        const options = (pre.name||'').split('|').map(o=>o.trim());
        const need = pre.minCount || 1;
        // prereqPerPurchase: Nth purchase needs N*need prereqs total
        const required = (!pre.primaryGate && sk.prereqPerPurchase) ? need * skCount : need;
        const isRemovedOption = options.some(opt => removedNames.includes(opt) || result.has(opt));
        if(isRemovedOption){
          const stillHave = options.reduce((sum,opt)=>{
            const cnt = getPurchaseCount(opt);
            const removing = (removedNames.includes(opt)||result.has(opt)) ? cnt : 0;
            return sum + cnt - removing;
          }, 0);
          if(stillHave < required){ result.add(sk.name); changed = true; }
        }
      }
    });
  }
  return [...result];
}

// ---- Stat calculations ----
function calcStats(){
  const cpTotal = calcCP(s.blankets);
  const row = getLevelFromCP(cpTotal);
  const cls = OCC_CLASS[s.occupation]||null;
  const baseBody = cls ? row[cls] : null;
  const body = baseBody != null ? baseBody + getBodyBonus() : null;
  const cpSpent = s.owned.filter(o=>!o._auto).reduce((a,sk)=>a+(sk.cp||0),0);
  const skillFrags = s.owned.filter(o=>!o._auto).reduce((a,sk)=>a+(sk.frag||0),0);
  const frags = getRaceFragCost() + getCultureFragCost() + getVocationFragCost() + getFavouredSphereFragSurcharge() + skillFrags;
  return {level:row.level, cpTotal, body, cpSpent, cpRem:cpTotal-cpSpent, frags, row};
}

function showRaceDetail(raceName){
  const rd = RACES[raceName] || FRAG_RACES[raceName];
  if(!rd) return;
  const panel = document.getElementById('detail-panel');
  const fragTier = FRAG_RACES[raceName] ? `<span class="tag frag">${FRAG_RACES[raceName].tier} — ${FRAG_RACES[raceName].fragCost} frags</span>` : `<span class="tag">Common</span>`;
  const cpBonus = rd.cpBonus ? `<div class="detail-stat-row"><span class="detail-stat-lbl">CP Bonus</span><span class="detail-stat-val">+${rd.cpBonus} cp</span></div>` : '';
  const autos = (rd.auto||[]);
  const advantages = autos.filter(a=>a.kind==='advantage');
  const disadvantages = autos.filter(a=>a.kind==='disadvantage');

  panel.innerHTML = `
    <div class="detail-name">${raceName}</div>
    <div class="detail-meta">${fragTier}</div>
    <div class="detail-desc" style="margin-top:8px">${rd.lore||'No lore available.'}</div>
    <hr class="detail-divider">
    ${cpBonus}
    ${advantages.length ? `<div class="detail-stat-row"><span class="detail-stat-lbl">Advantages</span><span class="detail-stat-val">${advantages.map(a=>a.name).join(', ')}</span></div>` : ''}
    ${disadvantages.length ? `<div class="detail-stat-row"><span class="detail-stat-lbl">Disadvantages</span><span class="detail-stat-val">${disadvantages.map(a=>a.name).join(', ')}</span></div>` : ''}
    ${(rd.purchased||[]).length ? `<div class="detail-stat-row"><span class="detail-stat-lbl">Purchasable</span><span class="detail-stat-val">${rd.purchased.map(p=>p.name).join(', ')}</span></div>` : ''}
    <div style="font-size:11px;color:var(--color-text-tertiary);font-style:italic;margin-top:8px">Select a skill in the Racial category to see full details.</div>
  `;
}

// ---- Auto-grants ----
function syncAutoGrants(){
  s.owned = s.owned.filter(o=>!o._auto);
  getRacialAutoSkills().forEach(ag=>s.owned.push(ag));
  // All characters get Simple Weapon Group Proficiency for free
  s.owned.push({
    name:'Weapon Group Proficiency: Simple',
    _auto:true, _cat:'Warrior',
    kind:'advantage',
    cp:0, frag:0, bodyBonus:0, strBonus:0,
    costs:null, prereqs:[], maxPurchases:1,
    desc:'All characters receive Simple Weapon Group Proficiency for free upon character creation. This skill allows the player to properly wield the following weapons: Dagger, Staff, Club, Thrown Weapon, Hand-to-Hand, and any other non-Exotic weapon with a base damage of 1.',
  });
  // Favoured Vocations auto-grant the Favoured skill at no CP or frag cost
  if(s.vocation && FAVOURED_VOCATIONS[s.vocation]){
    s.owned.push({
      name:'Favoured',
      _auto:true, _cat:'Frag Skills',
      kind:'advantage',
      cp:0, frag:0, bodyBonus:0, strBonus:0,
      costs:null, prereqs:[], maxPurchases:1,
      desc:'The Favoured are specially chosen by a God or Dragon from amongst the flock and elevated to the level of the truly revered. This skill grants access to unique Spheres of Magic and allows communion with their God or Dragon through prayer (minimum 10 minutes uninterrupted, between 6 PM and 12 AM). The Favoured may innately cast Bless or Dragon Mark once a day. Automatically granted by selecting a Favoured Vocation. Cannot be purchased separately.',
    });
  }
}

// ---- Main render ----
function render(){
  syncAutoGrants();
  populateVocationDropdown();
  const st = calcStats();

  document.getElementById('st-level').textContent = st.level;
  document.getElementById('st-body').textContent = st.body ?? '—';
  document.getElementById('st-str').textContent = getStrBonus();
  document.getElementById('st-blankets').textContent = s.blankets;
  document.getElementById('st-cptotal').textContent = st.cpTotal;
  document.getElementById('st-cpspent').textContent = st.cpSpent;

  const remEl = document.getElementById('st-cprem'), warnEl = document.getElementById('st-cpwarn');
  remEl.textContent = st.cpRem; warnEl.textContent = '';
  if(st.cpRem < 0){
    remEl.className = 'stat-val danger';
    const needed = blanketsNeededToEarnCP(st.cpTotal, Math.abs(st.cpRem));
    warnEl.textContent = needed+' more blanket'+(needed!==1?'s':'')+' needed';
  } else { remEl.className = 'stat-val'; }

  document.getElementById('st-frags').textContent = st.frags;

  renderSkillsPanel();
  renderSkillCats();
  renderMagicPanel();
  if(s.hovered) renderDetail();
}

// ---- Skills acquired panel ----
function renderSkillsPanel(){
  const sl = document.getElementById('skills-list');
  const allOwned = s.owned;
  if(!allOwned.length){ sl.innerHTML='<span class="empty-note">No skills yet</span>'; return; }

  // Clear and rebuild hover map
  Object.keys(_ownedHoverMap).forEach(k=>delete _ownedHoverMap[k]);
  let keyIdx = 0;
  const reg = (sk) => {
    const key = 'sk'+(keyIdx++);
    _ownedHoverMap[key] = sk;
    return key;
  };

  const tag = (cls, sk, label, badge='') => {
    const key = reg(sk);
    return `<div class="skill-tag ${cls}" style="cursor:pointer" onmouseenter="hoverOwnedSkill('${key}')">
      <span class="stag-name">${label}</span>${badge ? `<span class="stag-badge">${badge}</span>` : ''}
    </div>`;
  };

  const groups = {advantage:[], disadvantage:[], bycat:{}};
  allOwned.forEach(sk=>{
    if(sk._auto && sk._racial && sk.kind==='advantage') groups.advantage.push(sk);
    else if(sk._auto && sk._racial && sk.kind==='disadvantage') groups.disadvantage.push(sk);
    else{
      const c = sk._cat||'General';
      if(!groups.bycat[c]) groups.bycat[c]=[];
      groups.bycat[c].push(sk);
    }
  });

  let html = '';
  if(groups.advantage.length){
    html+='<div class="skills-group-label">Racial advantages</div>';
    html+=groups.advantage.map(sk=>tag('granted', sk, sk.name, 'auto')).join('');
  }
  if(groups.disadvantage.length){
    html+='<div class="skills-group-label">Racial disadvantages</div>';
    html+=groups.disadvantage.map(sk=>tag('disadvantage', sk, sk.name, 'auto')).join('');
  }

  Object.entries(groups.bycat).forEach(([cat,skills])=>{
    html+=`<div class="skills-group-label">${cat}</div>`;

    const spellSlots = skills.filter(o=>o._spellSlot);
    const regularSkills = skills.filter(o=>!o._spellSlot && !o._ritualSlot && !o._spherePurchase);
    const ritualSlots = skills.filter(o=>o._ritualSlot);
    const spheres = skills.filter(o=>o._spherePurchase);

    spheres.forEach(sp=>{ html+=tag('purchased', sp, sp.name); });

    if(spellSlots.length){
      const byLevel = {};
      spellSlots.forEach(o=>{ if(!byLevel[o._spellSlotLevel]) byLevel[o._spellSlotLevel]=[]; byLevel[o._spellSlotLevel].push(o); });
      Object.entries(byLevel).sort((a,b)=>a[0]-b[0]).forEach(([lvl,slots])=>{
        const summary = {...slots[0], name:`${ordinal(parseInt(lvl))} Circle`, desc:`${slots.length} purchased slot${slots.length>1?'s':''} at ${ordinal(parseInt(lvl))} Circle.`};
        html+=tag('purchased', summary, `${ordinal(parseInt(lvl))} Circle ×${slots.length}`);
      });
    }

    if(ritualSlots.length){
      const summary = {...ritualSlots[0], name:'Ritual Slots', desc:`${ritualSlots.length} ritual slot${ritualSlots.length>1?'s':''} purchased.`};
      html+=tag('purchased', summary, `Ritual Slots ×${ritualSlots.length}`);
    }

    const seen = {};
    regularSkills.forEach(sk=>{ if(!seen[sk.name]) seen[sk.name]={sk,count:0}; seen[sk.name].count++; });
    Object.values(seen).forEach(({sk,count})=>{
      html+=tag('purchased', sk, `${sk.name}${count>1?` ×${count}`:''}`);
    });
  });

  sl.innerHTML = html || '<span class="empty-note">No skills yet</span>';
}

// ---- Skill categories ----
function renderSkillCats(){
  const cats = buildSkillCatList();
  const currentLevel = getCurrentLevel();
  document.getElementById('skill-cats').innerHTML = cats.map((cat)=>{
    const open = s.openCats[cat.cat] === true;
    const isRacial = cat.cat === 'Racial';
    const visibleSkills = isRacial ? (s.race ? cat.skills : []) : cat.skills;

    return `<div class="skill-category-block">
      <div class="skill-cat-header" onclick="toggleCat('${cat.cat}')">
        <span>${cat.cat} <span style="font-weight:400;opacity:0.6">(${visibleSkills.length})</span></span>
        <span style="font-size:10px">${open?'▲':'▼'}</span>
      </div>
      ${open ? `<div class="skill-list">${
        visibleSkills.length===0 && isRacial
          ? `<div style="padding:10px 14px;font-size:13px;color:var(--color-text-tertiary);font-style:italic">Select a race to see racial skills</div>`
          : visibleSkills.map((sk,si)=>{
              const count = sk._paragon
                ? s.owned.filter(o=>o._paragon && !o._auto).length
                : getPurchaseCount(sk.name);
              const maxP = sk.maxPurchases || DEFAULT_MAX;
              const blockReason = getBlockReason(sk, false);
              // Hard lock: anything that isn't just "at max" or "racial level cap"
              const isRacialLevelCap = sk._racial && !sk._auto && blockReason === 'level';
              const isOccLevelGate = sk.occupational && blockReason === 'level';
              // isLocked = hard locked (hide +/- buttons entirely)
              // Soft states (show disabled +/-): maxed, racial level cap
              const isLocked = blockReason && blockReason !== 'maxed' && !isRacialLevelCap && !isOccLevelGate;
              // isMaxed = + button disabled
              const isMaxed = sk._paragon
                ? count >= 1
                : (blockReason === 'maxed' || isRacialLevelCap || isOccLevelGate);
              const isOwned = count > 0;

              // Build tag list
              let tags = isOwned ? `<span class="tag">purchased${count>1?` ×${count}`:''}</span>` : '';
              if(sk.frag) tags += `<span class="tag frag">${sk.frag} frag</span>`;
              if(sk.raceReq && sk.raceReq !== s.race) tags += `<span class="tag race-req">${sk.raceReq} only</span>`;
              if(blockReason && blockReason.startsWith('prereq|')){
                const [,prereqName,minCount] = blockReason.split('|');
                tags += `<span class="tag prereq-req">Needs: ${prereqName}${minCount>1?' ×'+minCount:''}</span>`;
              }
              if(isMaxed && blockReason === 'maxed') tags += `<span class="tag">max ${maxP}</span>`;
              else if(isOccLevelGate) tags += `<span class="tag lvl-req">Lvl ${currentLevel%2===0?currentLevel+1:currentLevel+2} required</span>`;

              // Special spell/ritual slot display
              const isSlotEntry = sk._spellSlotEntry || sk._ritualSlotEntry;
              const slotCount = sk._spellSlotEntry ? getSpellSlotCount() : (sk._ritualSlotEntry ? getRitualSlotCount() : 0);
              const slotMax = sk._spellSlotEntry ? 45 : 10;
              const slotDone = slotCount >= slotMax;
              const skCost = sk._spellSlotEntry ? getSpellSlotNextCost() : (sk._ritualSlotEntry ? getRitualSlotNextCost() : getSkillCost(sk));
              // Build human-readable lock reason for row
              let lockText = 'locked';
              if(blockReason){
                if(blockReason === 'race') lockText = `${sk.raceReq} only`;
                else if(blockReason === 'paragon_no_slots') lockText = 'Requires at least 1 spell slot';
                else if(blockReason === 'paragon_favoured') lockText = 'Incompatible with Favoured Vocation';
                else if(blockReason === 'level'){
                  const nextOddLvl = currentLevel % 2 === 0 ? currentLevel + 1 : currentLevel + 2;
                  lockText = sk._racial
                    ? `Max at this level — next slot at Lvl ${nextOddLvl}`
                    : sk.occupational
                    ? `Lvl ${nextOddLvl} required (odd levels only)`
                    : `Lvl ${nextOddLvl} required`;
                } else if(blockReason.startsWith('prereq|')){
                  const [,prereqName,minCount] = blockReason.split('|');
                  lockText = `Needs: ${prereqName}${parseInt(minCount)>1?' ×'+minCount:''}`;
                } else if(blockReason === 'maxed'){
                  lockText = `max ${maxP}`;
                }
              }

              const rowClass = [isOwned&&!isLocked?'owned':'', isLocked?'locked':''].filter(Boolean).join(' ');

              return `<div class="skill-row ${rowClass}" onmouseenter="hoverSkill('${cat.cat}',${si})" onclick="hoverSkill('${cat.cat}',${si})">
                <div class="skill-row-left">
                  <span class="skill-row-name">${sk.name}</span>
                  <div class="tags">${tags}</div>
                </div>
                <div class="skill-row-right">
                  <span class="cp-badge">${isSlotEntry ? (slotDone ? '—' : (s.occupation ? skCost+' cp' : '— cp')) : (s.occupation ? skCost+' cp' : '— cp')}</span>
                  ${!isLocked ? `
                    <button class="btn-sm minus" onclick="event.stopPropagation();tryRemoveOne('${cat.cat}',${si})" ${(isSlotEntry ? slotCount===0 : count===0)?'disabled':''}>−</button>
                    <span class="count-badge">${isSlotEntry ? slotCount+'/'+slotMax : sk._racial && !sk._auto ? s.owned.filter(o=>o._racial&&!o._auto).length+'/'+Math.ceil(currentLevel/2) : count+'/'+maxP}</span>
                    <button class="btn-sm" onclick="event.stopPropagation();addOne('${cat.cat}',${si})" ${(isSlotEntry ? slotDone : isMaxed)||(sk.costs&&!s.occupation)?'disabled':''}>+</button>
                  ` : `<span style="font-size:11px;color:var(--color-text-warning);font-style:italic;max-width:90px;text-align:right;line-height:1.3">${lockText}</span>`}
                </div>
              </div>`;
            }).join('')
      }</div>` : ''}
    </div>`;
  }).join('');
}

function toggleCat(n){ s.openCats[n]=s.openCats[n]===false?true:false; renderSkillCats(); }
function hoverSkill(cat,si){ s.hovered={cat,si}; renderDetail(); }

// Lookup map for owned skill hover — populated during renderSkillsPanel
const _ownedHoverMap = {};

function hoverOwnedSkill(key){
  const sk = _ownedHoverMap[key];
  if(!sk) return;
  const panel = document.getElementById('detail-panel');
  const cp = sk.cp != null ? sk.cp : 0;
  panel.innerHTML = `
    <div class="detail-name">${sk.name}</div>
    <div class="detail-meta">
      ${sk._auto ? '<span class="tag">auto-granted</span>' : '<span class="tag">purchased</span>'}
      ${sk.frag ? `<span class="tag frag">${sk.frag} frag</span>` : ''}
      ${sk.raceReq ? `<span class="tag race-req">${sk.raceReq} only</span>` : ''}
    </div>
    <div class="detail-desc">${sk.desc || 'No description available.'}</div>
    <hr class="detail-divider">
    ${!sk._auto && !sk._spellSlot && !sk._ritualSlot && !sk._spherePurchase ? `<div class="detail-stat-row"><span class="detail-stat-lbl">CP cost</span><span class="detail-stat-val">${cp} cp each</span></div>` : ''}
    ${sk.bodyBonus ? `<div class="detail-stat-row"><span class="detail-stat-lbl">Body bonus</span><span class="detail-stat-val">+${sk.bodyBonus}</span></div>` : ''}
    ${sk.strBonus ? `<div class="detail-stat-row"><span class="detail-stat-lbl">Strength bonus</span><span class="detail-stat-val">+${sk.strBonus}</span></div>` : ''}
  `;
}

// ---- Detail panel ----
function renderDetail(){
  const panel = document.getElementById('detail-panel');
  if(!s.hovered){ panel.innerHTML='<div class="detail-empty">Hover a skill to see details</div>'; return; }
  const cats = buildSkillCatList();
  const catObj = cats.find(c=>c.cat===s.hovered.cat);
  if(!catObj||!catObj.skills[s.hovered.si]){ panel.innerHTML='<div class="detail-empty">Hover a skill to see details</div>'; return; }

  const sk = catObj.skills[s.hovered.si];
  const count = getPurchaseCount(sk.name);
  const maxP = sk.maxPurchases || DEFAULT_MAX;
  const blockReason = getBlockReason(sk, false);
  const isLocked = blockReason && blockReason !== 'maxed';
  const isMaxed = count >= maxP;
  const currentLevel = getCurrentLevel();

  let lockNote = '';
  if(sk.raceReq && sk.raceReq !== s.race)
    lockNote = `<div class="detail-lock-note race">Requires ${sk.raceReq} race to purchase.</div>`;
  else if((sk.occupational || sk._racial) && currentLevel%2===0){
    const nextLvl = currentLevel%2===0?currentLevel+1:currentLevel+2;
    lockNote = `<div class="detail-lock-note level">${sk._racial?'Racial':'Occupational'} skill — available at level ${nextLvl} (odd levels only).</div>`;
  } else if(blockReason && blockReason.startsWith('prereq|')){
    const [,prereqName,minCount] = blockReason.split('|');
    lockNote = `<div class="detail-lock-note prereq">Missing prerequisite: <strong>${prereqName}</strong>${parseInt(minCount)>1?' (×'+minCount+' required)':''}.</div>`;
  } else if(isMaxed){
    lockNote = `<div class="detail-lock-note maxed">Maximum purchases reached (${maxP}).</div>`;
  }

  panel.innerHTML = `
    <div class="detail-name">${sk.name}</div>
    <div class="detail-meta">
      ${sk.frag?`<span class="tag frag">${sk.frag} frag</span>`:''}
      ${sk.raceReq?`<span class="tag race-req">${sk.raceReq} only</span>`:''}
      ${sk.occupational?`<span class="tag lvl-req">occupational</span>`:''}
    </div>
    <div class="detail-desc">${sk.desc}</div>
    <hr class="detail-divider">
    ${sk._spellSlotEntry || sk._ritualSlotEntry
      ? `<div class="detail-stat-row"><span class="detail-stat-lbl">Next cost</span><span class="detail-stat-val">${s.occupation ? (sk._spellSlotEntry ? getSpellSlotNextCost() : getRitualSlotNextCost())+' cp' : 'Select occupation'}</span></div>
         <div class="detail-stat-row"><span class="detail-stat-lbl">Purchased</span><span class="detail-stat-val">${sk._spellSlotEntry ? getSpellSlotCount()+' / 45' : getRitualSlotCount()+' / 10'}</span></div>`
      : `<div class="detail-stat-row"><span class="detail-stat-lbl">CP cost</span><span class="detail-stat-val">${sk.costs ? (s.occupation ? getSkillCost(sk)+' cp' : 'Select occupation') : (sk.cp||0)+' cp'} each</span></div>
         ${sk.costs && !s.occupation ? `<div style="font-size:11px;color:var(--color-text-tertiary);font-style:italic;margin-top:4px">Cost varies by occupation — select one to see your rate</div>` : ''}
         <div class="detail-stat-row"><span class="detail-stat-lbl">Purchases</span><span class="detail-stat-val">${count} / ${maxP}</span></div>`
    }
    ${sk.bodyBonus?`<div class="detail-stat-row"><span class="detail-stat-lbl">Body per purchase</span><span class="detail-stat-val">+${sk.bodyBonus}</span></div>`:''}
    ${sk.strBonus?`<div class="detail-stat-row"><span class="detail-stat-lbl">Strength per purchase</span><span class="detail-stat-val">+${sk.strBonus}</span></div>`:''}
    ${(sk.prereqs||[]).length?`<div class="detail-stat-row"><span class="detail-stat-lbl">Prerequisites</span><span class="detail-stat-val">${sk.prereqs.map(p=>p.name+(p.minCount>1?' ×'+p.minCount:'')).join(', ')}</span></div>`:''}
    ${lockNote}
    ${!isLocked ? `
      <div class="detail-actions">
        <button class="buy-btn remove" onclick="tryRemoveOne('${s.hovered.cat}',${s.hovered.si})" ${count===0?'disabled':''}>− Remove</button>
        <span class="detail-count">${count}/${maxP}</span>
        <button class="buy-btn" onclick="addOne('${s.hovered.cat}',${s.hovered.si})" ${isMaxed?'disabled':''}>+ Add</button>
      </div>` : ''}
  `;
}

// ---- Add / Remove logic ----
function addOne(cat, si){
  const cats = buildSkillCatList();
  const catObj = cats.find(c=>c.cat===cat); if(!catObj)return;
  const sk = catObj.skills[si];
  if(getBlockReason(sk, false)) return;
  if(sk.costs && !s.occupation) return;
  // Weapon choice skills require a popup to select weapon/group
  if(sk._weaponChoice){
    openWeaponChoicePopup(cat, si, sk);
    return;
  }
  // Elemental Attunement requires choosing an element
  if(sk.name === 'Elemental Attunement'){
    openElementalAttunementPopup(cat, si, sk);
    return;
  }
  // Paragon requires a special popup to choose sphere and spell level
  if(sk._paragon){
    openParagonPopup(cat, si);
    return;
  }
  const cp = getSkillCost(sk);
  s.owned.push({...sk, _cat:cat, cp});
  render();
}

function tryRemoveOne(cat, si){
  const cats = buildSkillCatList();
  const catObj = cats.find(c=>c.cat===cat); if(!catObj)return;
  const sk = catObj.skills[si];
  const count = getPurchaseCount(sk.name);
  if(count === 0) return;

  const dependents = [];
  allSkills().forEach(other=>{
    if(other.name === sk.name) return;
    const otherCount = getPurchaseCount(other.name);
    if(otherCount === 0) return;
    for(const pre of (other.prereqs||[])){
      const options = (pre.name||'').split('|').map(o=>o.trim());
      if(!options.includes(sk.name)) continue;
      const need = pre.minCount || 1;
      const totalHave = options.reduce((sum,opt)=>sum+getPurchaseCount(opt),0);
      // For prereqPerPurchase skills, the Nth purchase requires N * need prereqs
      // So check if removing one prereq drops below what's needed for otherCount purchases
      const required = (!pre.primaryGate && other.prereqPerPurchase) ? need * otherCount : need;
      if(totalHave - 1 < required) dependents.push(other.name);
    }
  });

  if(dependents.length){
    const cascade = collectDependents([sk.name]);
    const allAffected = [...new Set([...dependents, ...cascade])];
    showModal(
      `Remove "${sk.name}"?`,
      `Removing this purchase will break the prerequisites for the following skills, which will also be fully removed:`,
      allAffected,
      ()=>{ doRemoveOne(cat, si, sk.name, allAffected); }
    );
  } else {
    doRemoveOne(cat, si, sk.name, []);
  }
}

function doRemoveOne(cat, si, skillName, alsoRemove){
  // Remove one instance of skillName — match by name OR by _baseSkillName (for weapon-choice skills)
  const idx = s.owned.map((o,i)=>
    (o.name===skillName || o._baseSkillName===skillName) && !o._auto ? i : -1
  ).filter(i=>i>=0).pop();
  if(idx != null && idx >= 0){
    const removed = s.owned[idx];
    // If removing an elemental attunement skill, also remove that element from state
    if(removed._elementalAttunement && removed._chosenElement){
      s.elementalAttunements = s.elementalAttunements.filter(e => e !== removed._chosenElement);
    }
    s.owned.splice(idx, 1);
  }
  // Remove all instances of cascade skills, cleaning up attunements as we go
  alsoRemove.forEach(name=>{
    s.owned
      .filter(o => (o.name===name || o._baseSkillName===name) && !o._auto && o._elementalAttunement)
      .forEach(o => { if(o._chosenElement) s.elementalAttunements = s.elementalAttunements.filter(e=>e!==o._chosenElement); });
    s.owned = s.owned.filter(o => !((o.name===name || o._baseSkillName===name) && !o._auto));
  });
  render();
}

// ---- Modal ----
function showModal(title, body, affected, onConfirm){
  document.getElementById('modal-title').textContent = title;
  document.getElementById('modal-body').textContent = body;
  const affEl = document.getElementById('modal-affected');
  if(affected && affected.length){
    affEl.textContent = affected.join(', ');
    affEl.style.display = 'block';
  } else {
    affEl.style.display = 'none';
  }
  document.getElementById('modal-confirm').onclick = ()=>{ closeModal(); onConfirm(); };
  document.getElementById('modal').style.display = 'flex';
}

function closeModal(){
  document.getElementById('modal').style.display = 'none';
}

function openCharacterSummary(){
  document.getElementById('char-summary-body').innerHTML = buildSummaryHTML();
  document.getElementById('char-summary-overlay').style.display = 'block';
  document.getElementById('char-summary-overlay').scrollTop = 0;
}

function printCharacterSummary(){
  const html = document.getElementById('char-summary-body').innerHTML || buildSummaryHTML();
  document.getElementById('print-area').innerHTML = html;
  window.print();
}

function closeCharacterSummary(){
  document.getElementById('char-summary-overlay').style.display = 'none';
}

function buildSummaryHTML(){
  const st = calcStats();
  const currentLevel = getCurrentLevel();
  const strBonus = getStrBonus();

  // Helper
  const sec = (title, content) => `
    <div style="margin-bottom:1.5rem">
      <div style="font-size:11px;font-weight:600;color:var(--color-text-tertiary);text-transform:uppercase;letter-spacing:0.8px;margin-bottom:0.6rem;padding-bottom:4px;border-bottom:0.5px solid var(--color-border-tertiary)">${title}</div>
      ${content}
    </div>`;

  const row = (label, value, muted=false) => `
    <div style="display:flex;justify-content:space-between;align-items:baseline;padding:3px 0;font-size:13px">
      <span style="color:var(--color-text-secondary)">${label}</span>
      <span style="font-weight:500;color:${muted?'var(--color-text-tertiary)':'var(--color-text-primary)'};text-align:right;max-width:60%">${value}</span>
    </div>`;

  const pill = (text, color='var(--color-background-tertiary)', textColor='var(--color-text-secondary)') =>
    `<span style="display:inline-block;padding:2px 8px;border-radius:100px;background:${color};color:${textColor};font-size:11px;font-weight:500;margin:2px 2px 2px 0">${text}</span>`;

  // ---- Header ----
  const header = `
    <div style="margin-bottom:1.5rem;padding-bottom:1rem;border-bottom:1.5px solid var(--color-border-secondary)">
      <div style="font-size:24px;font-weight:600;margin-bottom:4px">${s.name || '<em style="color:var(--color-text-tertiary);font-style:italic;font-weight:400">Unnamed Character</em>'}</div>
      <div style="font-size:13px;color:var(--color-text-secondary);display:flex;flex-wrap:wrap;gap:6px;align-items:center">
        ${s.race ? pill(s.race) : ''}
        ${s.culture ? pill(s.culture, 'var(--color-background-info)', 'var(--color-text-info)') : ''}
        ${s.occupation ? pill(s.occupation) : ''}
        ${s.vocation ? pill(s.vocation, 'var(--color-background-warning)', 'var(--color-text-warning)') : ''}
      </div>
    </div>`;

  // ---- Core Stats ----
  const coreStats = sec('Core Statistics', `
    <div style="display:grid;grid-template-columns:1fr 1fr;gap:0 2rem">
      ${row('Level', currentLevel)}
      ${row('Body Points', st.body ?? '—')}
      ${row('Strength Bonus', strBonus > 0 ? `+${strBonus}` : `${strBonus}`)}
      ${row('Blankets', s.blankets)}
      ${row('CP Total', st.cpTotal)}
      ${row('CP Spent', st.cpSpent)}
      ${row('CP Remaining', st.cpTotal - st.cpSpent)}
      ${row('Frags', st.frags)}
    </div>`);

  // ---- Identity ----
  const identityLines = [
    s.race && row('Race', s.race),
    s.culture && row('Culture', s.culture),
    s.occupation && row('Occupation', s.occupation),
    s.vocation && row('Vocation', `${s.vocation}${isFavouredVocation(s.vocation) ? ' (Favoured)' : ''}`),
  ].filter(Boolean).join('');
  const identity = identityLines ? sec('Identity', identityLines) : '';

  // ---- Magic ----
  const sphere1 = getPurchaseCount('Sphere of Magic: 1st') > 0;
  const sphere2 = getPurchaseCount('Sphere of Magic: 2nd') > 0;
  const sphere3 = getPurchaseCount('Sphere of Magic: 3rd') > 0;
  let magicHTML = '';
  if(sphere1){
    const sphereLines = [];
    if(sphere1) sphereLines.push(row('Sphere 1', s.s_school_1 || '(school not selected)'));
    if(sphere2) sphereLines.push(row('Sphere 2', s.s_school_2 || '(school not selected)'));
    if(sphere3) sphereLines.push(row('Sphere 3', s.s_school_3 || '(school not selected)'));

    // Spell slots
    const slotsByLevel = getSlotsByLevel();
    const slotLines = Object.entries(slotsByLevel)
      .filter(([,count])=>count>0)
      .map(([lvl,count])=>row(`${ordinal(parseInt(lvl))} Circle`, `${count} slot${count>1?'s':''}`))
      .join('');

    const ritualCount = getRitualSlotCount();
    const ritualLine = ritualCount > 0 ? row('Ritual Slots', ritualCount) : '';

    magicHTML = sec('Magic', sphereLines.join('') + (slotLines||ritualLine ? `
      <div style="margin-top:8px;padding-top:8px;border-top:0.5px solid var(--color-border-tertiary)">
        <div style="font-size:11px;color:var(--color-text-tertiary);margin-bottom:4px">Spell Slots</div>
        ${slotLines}${ritualLine}
      </div>` : ''));
  }

  // ---- Racial ----
  const racialAutos = s.owned.filter(o=>o._auto && o._racial);
  const racialPurchased = s.owned.filter(o=>!o._auto && o._racial);
  let racialHTML = '';
  if(racialAutos.length || racialPurchased.length){
    const autoSection = racialAutos.length ? `
      <div style="margin-bottom:6px">
        <div style="font-size:11px;color:var(--color-text-tertiary);margin-bottom:3px">Automatic</div>
        <div>${racialAutos.map(sk=>pill(sk.name, 'var(--color-background-success)', 'var(--color-text-success)')).join('')}</div>
      </div>` : '';
    const purchasedSection = racialPurchased.length ? `
      <div>
        <div style="font-size:11px;color:var(--color-text-tertiary);margin-bottom:3px">${s.culture ? 'Culture' : 'Purchased'}</div>
        <div>${[...new Set(racialPurchased.map(sk=>sk.name))].map(name=>{
          const count = racialPurchased.filter(o=>o.name===name).length;
          return pill(count>1?`${name} ×${count}`:name);
        }).join('')}</div>
      </div>` : '';
    racialHTML = sec('Racial & Culture Abilities', autoSection + purchasedSection);
  }

  // ---- Occupational / Vocation Abilities ----
  const occOwned = s.owned.filter(o=>o._vocationAbility && !o._favouredUnlock);
  let occHTML = '';
  if(occOwned.length){
    const grouped = {};
    occOwned.forEach(o=>{ grouped[o.name]=(grouped[o.name]||0)+1; });
    const title = s.vocation ? `${s.vocation} Abilities` : 'Occupational Abilities';
    occHTML = sec(title, Object.entries(grouped).map(([name,count])=>
      `<div style="padding:4px 0;border-bottom:0.5px solid var(--color-border-tertiary);font-size:13px">
        <span style="font-weight:500">${name}</span>${count>1?`<span style="color:var(--color-text-tertiary);font-size:11px;margin-left:4px">×${count}</span>`:''}
      </div>`
    ).join(''));
  }

  // ---- Skills by category ----
  const skillCats = ['General','Production','Scholar','Warrior','Rogue'];
  let skillsHTML = '';
  skillCats.forEach(cat=>{
    const catOwned = s.owned.filter(o=>!o._auto && !o._racial && !o._vocationAbility && !o._favouredUnlock && !o._spellSlot && !o._ritualSlot && !o._spherePurchase && (o._cat===cat || (!o._cat && cat==='General')));
    if(!catOwned.length) return;
    const grouped = {};
    catOwned.forEach(o=>{ grouped[o.name]=(grouped[o.name]||0)+1; });
    skillsHTML += sec(cat + ' Skills', Object.entries(grouped).map(([name,count])=>
      `<div style="display:flex;justify-content:space-between;padding:3px 0;border-bottom:0.5px solid var(--color-border-tertiary);font-size:13px">
        <span>${name}</span>
        ${count>1?`<span style="color:var(--color-text-tertiary);font-size:11px">×${count}</span>`:''}
      </div>`
    ).join(''));
  });

  // Auto-granted non-racial skills (e.g. Simple Weapon Proficiency)
  const autoNonRacial = s.owned.filter(o=>o._auto && !o._racial);
  if(autoNonRacial.length){
    skillsHTML += sec('Automatic Skills', autoNonRacial.map(sk=>pill(sk.name, 'var(--color-background-success)', 'var(--color-text-success)')).join(''));
  }

  // ---- Notes ----
  const hasFavoured = s.vocation && isFavouredVocation(s.vocation);
  const favData = hasFavoured ? FAVOURED_VOCATIONS[s.vocation] : null;
  let notesHTML = '';
  if(hasFavoured && favData){
    const fragSpheres = ['s_school_1','s_school_2','s_school_3']
      .filter(k=>s[k] && FAVOURED_FRAG_SPHERES.includes(s[k]))
      .map(k=>s[k]);
    notesHTML = sec('Favoured Vocation Notes', `
      <div style="font-size:13px;color:var(--color-text-secondary);line-height:1.6">
        ${row('Type', `${favData.group} (${s.vocation})`)}
        ${row('Cost Table', `${favData.group} skill costs applied`)}
        ${favData.exclusiveSphere ? row('Exclusive Sphere', favData.exclusiveSphere) : ''}
        ${fragSpheres.length ? row('Frag Surcharge Spheres', fragSpheres.join(', ') + ` (+${fragSpheres.length * 100} frags)`) : ''}
      </div>`);
  }

  return header + coreStats + identity + magicHTML + racialHTML + occHTML + skillsHTML + notesHTML;
}

// ============================================================
// ---- Spell Summary Print ----
function sbPrintSummary(){
  const spheres = sbGetSpheres();
  const charName = s.name || 'Unnamed Character';
  const level = document.getElementById('st-level')?.textContent || '?';
  const atts = s.elementalAttunements && s.elementalAttunements.length ? s.elementalAttunements.join(', ') : null;

  let html = `<h2 style="font-size:1.25rem;font-weight:700;color:var(--color-text-primary);margin:0 0 0.25rem">❆ Spell List — ${charName}</h2>`;
  html += `<div style="font-size:12px;color:var(--color-text-tertiary);margin-bottom:1.5rem">Level ${level}`;
  if(spheres.length) html += ` &middot; Spheres: ${spheres.join(', ')}`;
  if(atts) html += ` &middot; Attunements: ${atts}`;
  html += `</div>`;

  if(!spheres.length){
    html += `<p style="color:var(--color-text-tertiary);font-style:italic">No spheres of magic selected.</p>`;
  } else {
    let hasAny = false;
    for(let lvl=1; lvl<=9; lvl++){
      const count = sbGetSlotCount(lvl);
      if(!count) continue;
      hasAny = true;
      html += `<div style="margin-bottom:1.25rem">`;
      html += `<div style="font-size:13px;font-weight:700;color:var(--color-text-warning, #c9a84c);border-bottom:0.5px solid var(--color-border-tertiary);padding-bottom:4px;margin-bottom:8px">${ordinal(lvl)} Circle — ${count} slot${count!==1?'s':''}</div>`;
      html += `<table style="width:100%;border-collapse:collapse;font-size:12px">`;
      html += `<colgroup><col style="width:32px"><col style="width:38%"><col><col style="width:28%"></colgroup>`;
      html += `<thead><tr style="color:var(--color-text-tertiary);font-size:10px;text-transform:uppercase;letter-spacing:0.5px">
        <th style="text-align:center;padding:3px 6px">#</th>
        <th style="text-align:left;padding:3px 6px">Spell</th>
        <th style="text-align:left;padding:3px 6px">Incantation</th>
        <th style="text-align:left;padding:3px 6px">Sphere</th>
      </tr></thead><tbody>`;
      for(let slot=1; slot<=count; slot++){
        const val = sbSelections[lvl+'-'+slot];
        let spellName = '<span style="color:var(--color-text-tertiary);font-style:italic">unassigned</span>';
        let incant = '';
        let sphere = '';
        if(val){
          const parts = val.split('|');
          const sp = SB_SPELLS.find(x=>x.sphere===parts[0]&&x.name===parts[1]&&x.level===lvl);
          if(sp){
            spellName = sp.name;
            incant = sbResolveIncant(sp);
            sphere = sp.sphere;
          }
        }
        const bg = slot%2===0 ? 'background:var(--color-background-secondary)' : '';
        html += `<tr style="${bg}">
          <td style="text-align:center;padding:5px 6px;color:var(--color-text-tertiary)">${slot}</td>
          <td style="padding:5px 6px;color:var(--color-text-primary);font-weight:500">${spellName}</td>
          <td style="padding:5px 6px;color:var(--color-text-secondary);font-style:italic">${incant}</td>
          <td style="padding:5px 6px;color:var(--color-text-tertiary)">${sphere}</td>
        </tr>`;
      }
      html += `</tbody></table></div>`;
    }
    if(!hasAny) html += `<p style="color:var(--color-text-tertiary);font-style:italic">No spell slots purchased.</p>`;
  }

  document.getElementById('spell-summary-body').innerHTML = html;
  document.getElementById('print-area').innerHTML = html;
  window.print();
}

// ============================================================
// SPELL LIST BUILDER
// ============================================================

const SB_SPELLS = [
  // Elemental
  {sphere:"Elemental",level:1,name:"Elemental Missile",incant:"I invoke <type> to inflict Missile. 10 Magic <type>!",desc:"This spell will create a small Elemental Missile that will do 10 Magic <type> upon a successful hit."},
  {sphere:"Elemental",level:1,name:"Swampwalk",incant:"I invoke <type> to inflict Swampwalk.",desc:"This spell causes the earth beneath the target's feet to become viscous and muddy. For the duration of the spell, the target's movement is slowed to one step every three seconds. The effect follows the target until the spell ends. This spell in no way affects anyone other than the target."},
  {sphere:"Elemental",level:2,name:"Elemental Affinity",incant:"I invoke <type> to grant Affinity <type(s)>.",desc:"This self-cast spell will grant the caster affinity with Elementals of any and all of their attuned elements. Any Elementals of an attuned type will treat the caster as a friend so long as the caster does not engage in any activity that the Elemental would deem hostile. The caster can state \"Active Elemental Affinity <type(s)>\" when approaching Elementals to indicate this."},
  {sphere:"Elemental",level:2,name:"Elemental Rebuke",incant:"I invoke <type> to inflict Elemental Rebuke. 1 Magic <type>!",desc:"This spell will push a single target with the strength of +5 total (10 feet) and do 1 Magic <type> damage. The target will be pushed away in the opposite direction of the caster. It may be stopped with equal or greater strength. Although the push has a physical effect, it is considered magical in nature, in regards to defenses. Any strength bonus the caster has is not added to the total strength of the spell. This spell cannot be used to rip the target from any bindings; it is a pushing effect, not a ripping effect."},
  {sphere:"Elemental",level:3,name:"Elemental Blade",incant:"I invoke <type> to grant Blade.",desc:"This spell sits on the target's Spirit and will cause the target's next three weapon strikes to become imbued with the caster's Element. It will add +5 damage to the weapon's normal damage and will change the damage type to \"Magic <type>\" for the next three strikes. The target must call the altered damage when they strike. Example: \"7 Magic Stone\". This effect will remain on the target's Spirit for the duration of the spell and must be used on the next three physical strikes that they make."},
  {sphere:"Elemental",level:3,name:"Elemental Vulnerability",incant:"I invoke <type> to grant Elemental Vulnerability.",desc:"This self-cast spell will imbue the caster's next spell from the Elemental Battle Magic sphere with a numeric damage amount to do x2 its normal damage. The next spell must be cast within 10 minutes of the Vulnerability. If the caster's next spell allows the caster to do numeric damage multiple times, the x2 damage only applies to the first attack which successfully strikes the target. The caster should call the appropriate x2 damage, as the target will not be aware that it needs to be doubled. This spell is caster only."},
  {sphere:"Elemental",level:4,name:"Control Lesser Elemental",incant:"I invoke <type> to inflict Control Lesser Elemental.",desc:"This spell will grant control over any Lesser Elemental of the types the caster is attuned to. The Elemental will do anything the caster desires, including suicidal actions. Only one command may be followed at a time. This spell will function as an Elemental Affinity against Greater Elementals."},
  {sphere:"Elemental",level:4,name:"Elemental Shield *",incant:"I invoke <type> to grant Elemental Shield.",desc:"This spell will protect the recipient from the next Elemental-based attack which hits them, so long as it employs the word \"Elemental\" in its call."},
  {sphere:"Elemental",level:5,name:"Elemental Conduit",incant:"I invoke <type> to grant Elemental Conduit.",desc:"This spell allows one memorized spell from the Elemental Battle Magic sphere to be cast as a Spellstrike. Once Elemental Conduit is cast, the caster has 10 minutes to use one of their memorized Elemental spells in Spellstrike form. To use a Spellstrike, the caster must strike with a melee weapon and call \"Spellstrike <spell name>\". If the weapon hits, the spell has struck the target as it if was touch cast or hit the target with a packet. A memorized spell used in this way is lost from memory as if it had been cast normally."},
  {sphere:"Elemental",level:5,name:"Elemental Strike",incant:"I invoke <type> to inflict Strike. 25 Elemental <type>!",desc:"This spell causes an Elemental Strike of <type> to leap from the caster's fingertips, inflicting 25 Elemental <type> damage to any target it hits. Elemental damage cannot be defended against with a Shield Magic; it requires an Elemental Shield."},
  {sphere:"Elemental",level:6,name:"Elemental Sunder",incant:"I Invoke <type> to inflict Sunder.",desc:"This spell will inflict 50 Magic damage on a target but will only damage the target's armour. Body points will remain unharmed. Any type of armour will be affected. If the target has less than 50 armour, the extra damage will be lost."},
  {sphere:"Elemental",level:6,name:"Greater Elemental Blade",incant:"I invoke <type> to grant Greater Blade.",desc:"This spell will act as an Elemental Blade but the duration is extended to all the attacks on one specific opponent. There is no limit to the number of physical attacks that the Greater Elemental Blade will alter, so long as the spell's target does not change opponents. If the spell's target, at any time, switches opponents, the spell will terminate. If the user leaves the battle for more than one minute, the spell will terminate. The battle is considered over when one of the two people fighting becomes unconscious or dead, or they spend more than one minute without attacking."},
  {sphere:"Elemental",level:7,name:"Advanced Elemental Shield *",incant:"I invoke <type> to grant Advanced Elemental Shield.",desc:"This spell acts like Elemental Shield, except that the wearer of this spell may choose what attack to defend against. When this spell defense is used the target must call out \"Advanced Elemental Shield\", and a visible flash of white energy can be seen as the spell protection dissipates. Only one Elemental Shield or Advanced Elemental Shield may be worn at any given time. It will not protect the wearer from any damage that contains the suffix \"Magic\" in its damage call. Since the choice to activate this defense is a conscious one, it will not function against surprise attacks."},
  {sphere:"Elemental",level:7,name:"Elemental Chain",incant:"I invoke <type> to inflict Elemental Chain. 30 Magic <type>, 20 Magic <type> 10 Magic <type>!",desc:"This spell will allow the caster to throw three spell packets total (or touch cast three times), the first of which does 30 Magic damage, then 20 Magic damage and finally 10 Magic damage. No target may be hit with more than one of the three packets. If there are fewer than three targets available, the remaining parts of the chain are lost. No more than three seconds may pass between each chain."},
  {sphere:"Elemental",level:8,name:"Elemental Storm",incant:"I invoke <type> to inflict Storm. 5 Magic <type>, 5 Magic <type>, 5 Magic <type> \u2026 (Repeat)",desc:"The caster must plant their feet when this spell is cast. As long as neither foot is moved, the caster may throw packets doing 5 Magic <type> each. The spell will end if the caster moves their feet, is hit with a Dispel Magic or takes damage to Body."},
  {sphere:"Elemental",level:8,name:"Greater Elemental Vulnerability",incant:"I invoke <type> to grant Greater Elemental Vulnerability.",desc:"This spell acts the same as the Elemental Vulnerability spell, except that it does x4 rather than x2 damage, and will also change the damage type from Magic to Elemental. This spell does not stack with Elemental Vulnerability. Elemental damage cannot be defended against with a Shield Magic; it requires an Elemental Shield."},
  {sphere:"Elemental",level:9,name:"Elemental Annihilation",incant:"I invoke <type> to inflict Elemental Annihilation!",desc:"This spell will cause a target that has been successfully struck to enter their Bleed Count. If the target successfully uses a defense against the Elemental Annihilation, they will not enter their Bleed Count but will suffer a 5 second magical stun effect. No defenses below ritual level may be used to avoid the stun. While stunned, a victim is unable to take any action, including blocking, moving and the use of skills, minus the ability to call \"interrupt\" against Killing Blows and any counts against them. Automatic defenses such as Shield Magic will still operate, but ones requiring conscious thought such as Advanced Shield Magic will not."},
  {sphere:"Elemental",level:9,name:"Elemental Tempest",incant:"I invoke <type> to inflict Tempest. 50 Magic <type>!",desc:"This spell causes a bolt of magical energy to rush from the caster's hands, inflicting 50 Magic damage on any target it strikes."},
  // Healing
  {sphere:"Healing",level:1,name:"Recover",incant:"I invoke Healing to grant Recover.",desc:"This spell can only be cast on a wounded target that is at less than 2 Body. Doing so will raise their Body points to 2. This does not function on those in their Death Counts or on Undead."},
  {sphere:"Healing",level:1,name:"Repel Undead",incant:"I invoke Healing to inflict Repel Undead.",desc:"This spell applies a repel effect to a target Lesser Undead for 10 minutes. During this time the targeted Undead is physically pushed away from the caster if it attempts to get closer than 10 feet. The Undead may cast spells and throw weapons or other objects at the caster. If the repelled Undead cannot retreat any further and the caster approaches the Undead within 10 feet, the spell will end. The caster must hold out one of their hands with the palm out (as a policeman's \"stop\" signal) and must maintain this gesture if the spell is to remain in effect. This spell has no effect against the living."},
  {sphere:"Healing",level:2,name:"Cleanse",incant:"I invoke Healing to grant Cleanse.",desc:"This spell will cure any disease except those that have specific cures. It will also cure nausea and plague. Diseases cured can be mundane and magical but the spell will not affect powerful diseases such as lycanthropy, vampirism, etc."},
  {sphere:"Healing",level:2,name:"Cure Wounds",incant:"I invoke Healing to grant Cure Wounds. 5 Healing!",desc:"This spell will heal the recipient by 5 Body points. It will not add Body points beyond the target's maximum Body. It will heal a target out of its Bleed Count, but will have no effect on someone in their Death Count. Cure Wounds will cause 20 points of Body damage to any Undead creature."},
  {sphere:"Healing",level:3,name:"Potion of Sweetwater",incant:"I invoke Healing to create Potion of Sweetwater.",desc:"This spell creates a Potion of Sweetwater, which has two possible uses. First, it will turn any liquid (including alchemy and other potions) into pure, clean drinking water. One potion of Sweetwater will convert one pint-sized container into water. Additional Potions of Sweetwater may be combined to change larger volumes of liquid. The second use of Potions of Sweetwater is to store Healing spells by creating healing potions. Once a Potion of Sweetwater has been created, any other curative spell within the Battle Magic Healing sphere of 8th level or lower may be cast on it. Doing so will convert the Sweetwater potion into a potion with the same effect of the spell that was cast on it. This new potion will last three months. Both the Potion of Sweetwater tag and the healing spell tag should be affixed to the potion together. The following spells may be turned into potions this way: Recover, Cleanse, Cure Wounds, Recuperate, Cure Serious Wounds, Bolster, Restore Limb, Cure Mortal Wounds, Heal and Purify."},
  {sphere:"Healing",level:3,name:"Recuperate",incant:"I invoke Healing to grant Recuperate.",desc:"This spell will heal 5 Body points every 5 minutes until the target reaches full health, or takes damage to Body. The first 5 points of healing will occur after the first 5 minutes' pass. Then every 5 minutes after that another 5 Body will be healed. This spell has no effect on Undead. The maximum duration of Recuperation is 5 days. While under its effects the target must state \"Visibly Regenerating\" every minute and whenever a new person approaches them."},
  {sphere:"Healing",level:4,name:"Cure Serious Wounds",incant:"I invoke Healing to grant Cure Serious Wounds. 10 Healing!",desc:"This spell will heal the recipient by 10 Body points. It will not add Body points beyond the target's maximum Body. It will heal a target out of its Bleed Count, but will have no effect on someone in their Death Count. Cure Serious Wounds will cause 40 points of Body damage to any Undead creature."},
  {sphere:"Healing",level:4,name:"Dawnblade",incant:"I invoke Healing to grant a Dawnblade.",desc:"This spell will allow the caster's weapons to \"Spellstrike Dawnblade. 20 Magic Body!\" damage three times within 10 minutes. These strikes will only harm Undead and have no effect against the living. This spell is caster only."},
  {sphere:"Healing",level:5,name:"Bolster *",incant:"I invoke Healing to grant Bolster.",desc:"This caster-only spell will heal the caster 15 Body points. Additionally, any healing that exceeds the caster's maximum Body points will grant them temporary Body points equal to the excess. These additional Body points can be dispelled and, if damaged, the temporary Body is removed before any other Body points. Once depleted, or after 5 days, the effect ends. These Body points cannot be healed by any means. Temporary Body point effects from any source cannot stack. Bolster is considered a spell protection and healers may select it as pre-cast during logistics, allowing them to enter game with 15 additional temporary Body. This spell has no effect on Undead, Gargylen, or Fauns."},
  {sphere:"Healing",level:5,name:"Restore Limb",incant:"I invoke Healing to grant Restore Limb.",desc:"This spell will restore one severed, fractured or missing limb from the target immediately. Thereafter it will restore another missing limb (if any) every 5 minutes until either all limbs are restored or until the duration expires. Only limbs which were missing at the time of casting will be restored. Once a limb is restored, the original detached limb will crumble to dust."},
  {sphere:"Healing",level:6,name:"Cure Mortal Wounds",incant:"I invoke Healing to grant Cure Mortal Wounds. 20 Healing!",desc:"This spell will heal the recipient by 20 Body points. It will not add Body points beyond the target's maximum Body. It will heal a target out of its Bleed Count, but will have no effect on someone in their Death Count. Cure Mortal Wounds will cause 80 points of Body damage to any Undead creature."},
  {sphere:"Healing",level:6,name:"Peaceful Repose *",incant:"I invoke Healing to grant a Peaceful Repose.",desc:"Once cast, Peaceful Repose will remain on the target's spirit for 5 days. If, during that time, the target enters their Death Count, Peaceful Repose will activate at the final second of that count and will extend the count by one additional minute. A secondary effect of Peaceful Repose is that will grant protection against any Necromantic \"Raise Undead\" spells and effects once during the initial Death Count, but will not provide that protection in the final \"additional\" minute of Death Count granted by the spell. If Peaceful Repose protects against a Raise Undead spell during the first 5 minutes, it will not grant an additional minute to the Death Count. It will only protect against \"Raise Undead\" effects once. When either effect is triggered, the spell will end."},
  {sphere:"Healing",level:7,name:"Death Ward *",incant:"I invoke Healing to grant a Death Ward.",desc:"This spell will act as a defense against the next effect with \"Death\" in its name that strikes the wearer. Death Ward may be stacked with other types of spell defenses and will activate automatically when the next appropriate effect strikes the wearer."},
  {sphere:"Healing",level:7,name:"Healing Hands",incant:"I invoke Healing to grant Healing Hands.",desc:"This spell is cast on a target. The next appropriate spell that is used on that target will be spread to anyone else holding that target's hands. This may continue to chain to an unlimited amount of targets, as long as they are all holding hands. Once this occurs, the spell will end. This spell may not be cast on Undead targets. Healing transferred in this manner does not multiply if more than one person in the chain touches a single person - the healing done will always mirror the amount provided by the original spell. Spells which may be used with Healing Hands are: Recover, Cleanse, Cure Wounds, Recuperate, Cure Serious Wounds, Restore Limb, Cure Mortal Wounds, Heal, Purify, and Life. Healing Hands does not pass through dying targets, so if someone in the chain is in their Death Count, the spell will affect them (if applicable) but not spread further."},
  {sphere:"Healing",level:8,name:"Heal",incant:"I invoke Healing to grant Heal.",desc:"This spell will restore the target to their full Body points. It will destroy any Lesser Undead and inflict 25 Healing/100 Magic Body damage on Greater Undead."},
  {sphere:"Healing",level:8,name:"Purify",incant:"I invoke Healing to grant Purify.",desc:"This spell will cure the target of certain magical, alchemical and mundane ailments. Afflictions cured are limited to silence, blindness, sleep, paralysis, and all toxins and diseases. Purify will not remove curses, Ritual-level afflictions or effects which require numerical healing to be cured. The target must be willing for this spell to work."},
  {sphere:"Healing",level:9,name:"Life",incant:"I invoke Healing to grant Life.",desc:"This spell will bring one creature back from the dead so long as it is in its Death Count. It will bring the creature back to fully Body points, removing any physical injuries, toxins, and diseases which do not normally persist through resurrection or require a specific cure. Should the body be in more than one piece, the spell must be cast on the majority of the body and the recipient will be brought back in that location. When Life is cast, the body reforms with the Spirit and all other pieces of the body elsewhere crumble to dust. The Spirit must be present with the body or body part when Life is cast for it to take effect. Life will have no effect on Undead, only on creatures which are living."},
  {sphere:"Healing",level:9,name:"Safeguard",incant:"I invoke Healing to grant a Safeguard.",desc:"This spell requires a 10-ft diameter circle to be drawn on the ground prior to use. A rope may be used. So long as the caster remains in the centre of the circle, Safeguard will pulse 1 Magic Healing to everyone in the circle every second that passes. The circle is not a barrier and anyone is free to enter and exit. This healing will inflict 4 Magic Body points of damage against Undead within the circle every second. If the caster moves from the center of the circle, the spell will end prematurely."},
  // Nature
  {sphere:"Nature",level:1,name:"Goodberry",incant:"I invoke Nature to create Goodberry.",desc:"This spell will transform up to three pieces of non-Magical fruit into health-giving Goodberries. The caster must have at least one to three pieces of edible fruit, no bigger than a grape, at the time of casting. These Goodberries will last 1 hour, or until eaten. Each Goodberry will bring an unconscious person currently in their Bleed Count to 1 Body point immediately if ingested. Be mindful if the target has food allergies and never feed anybody anything if they are not aware of what it is, nor should you place items in people's mouths OOG. You do not have to actually eat the Goodberry rep OOG if you don't want to."},
  {sphere:"Nature",level:1,name:"Snare",incant:"I invoke Nature to inflict Snare.",desc:"This spell causes a magical vine to emerge from the ground and wrap itself tightly around the target's right foot, forcing the target to keep that foot upon the ground, unable to move. The vines may be cut through with a two minute count. The Snare may be ripped free from by the victim if a +2 or greater strength is used. This however, will cause them to take 2 points of damage straight to Body regardless of threshold. It takes three seconds to rip free from the Snare."},
  {sphere:"Nature",level:2,name:"Charm Animal",incant:"I invoke Nature to inflict Charm Animal.",desc:"This spell will act as a Charm spell against any natural animal. During the spell's duration, the Charmed animal will respond to the caster as if it was a \"friend\", pack member or master. The exact relationship will depend on the animal in question, for example a wolf would consider the caster a member of its pack, a soldier ant will see the caster as worker ant, and other animals may see the caster as a parent or cub. The type of relationship that appears upon casting is random."},
  {sphere:"Nature",level:2,name:"Repel",incant:"I invoke Nature to inflict Repel.",desc:"This spell causes the target to be pushed away from the caster to a distance of 10 feet. The target may throw spells, weapons, or other objects at the caster, but may not cross the 10 foot boundary by any means (phasing, teleporting, etc.) so long as the caster maintains concentration. The caster must hold out one of their hands with the palm out (as a policeman's \"stop\" signal) and must maintain this gesture if the spell is to remain in effect. While doing this, the caster may move freely but may not engage in combat or use any skill, ability, or spell. If a repelled creature cannot retreat any further and the caster approaches the creature within the ten feet, the spell will fail and is lost. Note that some creatures that possess the ability \"Innate Repel\" may use both hands on two separate targets."},
  {sphere:"Nature",level:3,name:"Claws",incant:"I invoke Nature to grant Claws.",desc:"This spell causes the target to grow a vicious set of claws. These claws act as natural weapons, cannot be disarmed and grant the natural ability to use them. They swing for 2 Normal and may be used to block, as well as attack. Strength bonuses, either natural or spell-granted, will add to the damage as well, but nothing else will affect the damage of the Claws. If this spell is cast on another the caster is responsible for providing the weapon reps or the spell fails, likewise if the claw reps are dropped the spell will end. The target may refuse the weapon reps, which will cause the spell to fail. Magic may be cast while claws are active, however spells cannot be touch-cast through the claws. You may temporarily release a claw rep in order to cast spells via packets. The Claws spell is stackable. If a second set is cast while the first is still active, the duration will not reset but the claws will gain +1 damage and become silver. If a third set is cast while the second is still active, they again another +1 damage and become magical. Additional castings will each add another +1, but the duration will always be equal to the original casting."},
  {sphere:"Nature",level:3,name:"Moonlight Mantle *",incant:"I invoke Nature to grant Moonlight Mantle.",desc:"This caster-only spell envelops the caster in an invisible cloak of Magical Body points, providing an additional 10 temporary Body points. For all intents and purposes, these Body points behave entirely like real Body points except for the fact that they can be dispelled. Once they are gone, they cannot be healed and the spell ends. There are no flashes or any other perceptual indications that a Moonlight Mantle is present in combat. Such mantles count as Body when the recipient is struck by effects that bypass armour. Additionally, a Moonlight Mantle may be intentionally used-up in order to heal a target victim (as per Healing Magic). The Mantle will heal an amount in Body points equal to how many points remain within the Mantle. The Mantle may not be partially used in this manner; it is all or nothing. Once the Mantle has been used to heal someone the spell is terminated and the Mantle is gone. The incant to transfer a Moonlight Mantle is \"Transfer Moonlight Mantle\" and may only be touch-cast."},
  {sphere:"Nature",level:4,name:"Bind",incant:"I invoke Nature to inflict Bind.",desc:"This spell causes the target to have their hands pulled to their side and be bound there by a glowing white band of Druidic energy one inch in thickness. The band is impervious to damage from weapons or spells, but it may be negated with a Dispel Magic (which will also affect the person who is bound). The Bind may be cut through with a 4 minute count. The bound target may rip free from the Bind with +4 Strength or greater. Doing so will cause the target to take 4 points of damage straight to Body regardless of threshold. It takes three seconds to rip free. While bound, a person may walk, run, and otherwise move freely. They cannot however, use their hands in any means and therefore cannot cast, fight, or use the vast majority of their skills. The Magic of the Bind also shorts out any attempts by the target to touch cast on themselves, but Magic items may be used."},
  {sphere:"Nature",level:4,name:"Root Lance",incant:"I invoke Nature to inflict Root Lance. 15 Normal!",desc:"This spell will cause a sharp, barbed root to tear from the ground and up into the target's body. This packet-delivered attack will cause 15 points of Normal damage upon a successful strike and if damages the target into Body it will also affect them with a Magic Snare. Root Lance cannot be cast upon stone floors, inside man-made buildings or wherever there is no dirt, earth or soil."},
  {sphere:"Nature",level:5,name:"Regeneration",incant:"I invoke Nature to grant Regeneration.",desc:"This healing spell will restore 1 Body point per minute for a period of 10 minutes. The first Body point is healed 60 seconds after the spell is cast, the next 60 after that, etc. Although this spell will not give the target more Body points than their maximum, if during the 10 minutes the target reaches full Body and is wounded again, the regeneration will continue for the remaining duration. Regeneration will still continue to work if the target drops into their Bleed Count but not the target's Death Count. While under its effects the target must state \"Visibly Regenerating\" every minute that they heal a Body point from the spell and whenever a new person approaches them."},
  {sphere:"Nature",level:5,name:"Swarm",incant:"I invoke Nature to inflict Swarm.",desc:"This spell surrounds the target with a swarm of biting insects. These insects will cause the target to be unable to cast spells. Any damage calls from the target will be reduced by 1, to a minimum of 1 damage, and every 10 seconds the target will take 1 Body damage. These effects will continue until the target (or an ally) spends ten seconds batting away the insects. Multiple targets swatting will not lower this count. This spell has no effect against non-living targets, such as Undead, golems and incorporeal Spirits."},
  {sphere:"Nature",level:6,name:"Release",incant:"I invoke Nature to grant Release.",desc:"This spell will immediately release the target from any magical or natural bindings that are physically constricting the target in any manner. All bindings will be removed, even if more than one has been applied. It does not function against \"man-made\" bindings such as manacles, nooses or chains and will not open doors."},
  {sphere:"Nature",level:6,name:"Strength of the Bear",incant:"I invoke Nature to grant Strength of the Bear.",desc:"This spell will grant its target +3 Strength for an hour. This strength bonus will stack with any other strength bonus the target may have, but cannot be stacked with itself."},
  {sphere:"Nature",level:7,name:"Barkskin *",incant:"I invoke Nature to grant Barkskin.",desc:"This spell gives the target 40 points of Magical armour. This armour is Magical in nature and may not be Refit. Magical armour is removed before physical armour. While the target has Barkskin on their spirit, they suffer from a x2 vulnerability to Fire damage. If the armour is Breached the remaining fire damage will carry over to the target."},
  {sphere:"Nature",level:7,name:"Web",incant:"I invoke Nature to inflict Web.",desc:"This spell creates a Magical Web that immobilizes the target from the neck down. Creatures so trapped are unable to do anything with the exception of talking, reading, and skills that require no movement. Trapped creatures may also activate Magical items if the items are touching them, though few items would be beneficial, for the victim cannot use their hands to direct the activated item by throwing packets. Creatures with a Strength bonus of +6 may rip free from the web, taking three seconds and doing 6 Body in the process regardless of threshold; otherwise they may be cut out which takes 6 minutes of time to completely remove the sticky strands. Webbed creatures cannot be moved."},
  {sphere:"Nature",level:8,name:"Nature's Restoration",incant:"I invoke Nature to grant Nature's Restoration.",desc:"This spell affects any living creature which can be put to sleep. The creature must be willing unless they are a normal animal, in which case the spell works regardless. If successful, the spell puts the target into a restorative sleep for 10 minutes. If the target sleeps for the full 10 minutes, they are completely healed, cured of any diseases or toxins and may restore one lost or fractured limb. While asleep, any diseases or toxins in their system will be paused and will resume as normal after the target wakes up prematurely. Physicians may operate on the target without waking them. This spell does not halt a Bleed Count or a Death Count. The target may be awoken by any means that will wake someone from a magical sleep."},
  {sphere:"Nature",level:8,name:"Polymorph Other",incant:"I invoke Nature to inflict Polymorph Other <Type>.",desc:"This spell will briefly turn its target (and all their possessions) into a small animal in size and appearance. The caster may choose what kind of animal in <Type>, but it should be roughly the size of a chicken or a small dog. This, understandably, causes the mind of the target to become muddled. The target must sit down for the duration of the spell and can use no skills. The target may interrupt killing blows, and other forcible gestures that require a count, but cannot otherwise move or defend themselves. The target will keep their normal Body but for the duration of the spell they will have no armour. This spell only works on living creatures."},
  {sphere:"Nature",level:9,name:"Faerie Fire",incant:"I invoke Nature to inflict Faerie Fire.",desc:"This spell causes an aura of light to instantly be created around the struck target. The light emanates from the victim, thereby following them wherever they go, lasting 10 minutes in duration. The light inflicts the cumulative effects of x2 damage from all attacks, the inability to be healed in any form, and also causes blindness."},
  {sphere:"Nature",level:9,name:"Suspension",incant:"I invoke Nature to grant Suspension.",desc:"Suspension places a target that is in their Death Count in a state of suspended animation until the spell has ended or until the caster wishes to terminate the spell. Dispel Magic will continue the Death Count where it left off. This spell does not make the target immune to magic, so a Life spell will work on it. This spell does not prevent the target from forfeiting their Death Count at any time and choosing to resurrect immediately."},
  // Protections
  {sphere:"Protections",level:1,name:"Mage Robes *",incant:"I invoke Protection to grant Mage Robes.",desc:"This spell will surround the caster in a semi-transparent robe of armour. This robe is Magical in nature and may be Dispelled as normal. Mage Robes grants the caster +10 Magical Armour Points. This bonus armour will not stack with the Mage Leathers or Mage Plate spells but may stack with any other armour the caster is wearing. Magical armour is removed before physical armour. While the caster has Mage Robes on their spirit, they suffer from a x2 vulnerability to Lightning damage. If the armour is Breached the remaining Lightning damage will carry over to the target. This spell is caster only."},
  {sphere:"Protections",level:1,name:"Magic Shield",incant:"I invoke Protection to grant Magic Shield.",desc:"This spell calls into existence a Magical Shield, usable only by the caster. It also gives the caster the Shield skill-proficiency for the duration of the spell. The size of the shield must be chosen upon casting and must be larger than a buckler but no larger than the maximum size of a physical shield. The shield is spirit linked to the caster and will remain with the caster until the duration expires or the caster wills the spell to end. This Magic Shield will have every benefit and detriment of a real shield, with the exception that it cannot be shattered (destroyed), disarmed by any skill, and any Slay that strikes it will remain active. It can, however, be Dispelled. If possible, the shield should have white tape visible on its surface to represent that it is Magical."},
  {sphere:"Protections",level:2,name:"Magic Armour *",incant:"I invoke Protection to grant Magic Armour.",desc:"This spell protects the target from the next single physical strike or spell packet attack with the prefix \"physical\" in its damage call. It cannot be saved and will go off on the first successful hit, even if the recipient does not wish it to. When this spell defense is used, the target must call out \"Magic Armour,\" and a visible flash of white energy can be seen as the spell-protection dissipates. A Magic Armour will not protect against the physical touch of a touch cast spell or a Spellstrike. It will not protect the wearer from any damage that contains the suffix \"Elemental\" in its damage call. Only one Magic Armour or Advanced Magic Armour may be worn at any given time."},
  {sphere:"Protections",level:2,name:"Ward Stone",incant:"I invoke Protection to create a Ward Stone.",desc:"This spell will turn a normal stone into a Ward Stone, granting the bearer a 1 Normal Threshold. Once cast, the Ward Stone will become spirit linked to the first creature that touches it. That spirit link and the Ward Stone itself will become dispelled after the spell's duration expires or the creature dies. Ward Stones may be stacked with other Ward Stones and with thresholds granted by other Protections spells and rituals. For example, four Ward Stones will give the bearer a 4 Normal Threshold. Ward Stones must have the spell tag affixed to them and therefore must be large enough for this to be done."},
  {sphere:"Protections",level:3,name:"Render Weapon",incant:"I invoke Protection to create Render Weapon.",desc:"The Render Weapon spell will allow a targeted weapon to resist the next magical, alchemical or physical attempt to shatter or destroy it by stating \"Render\". Once an effect has been resisted, the spell ends. A weapon may only have one Render Weapon spell cast on it at any given time."},
  {sphere:"Protections",level:3,name:"Stone Form",incant:"I invoke Protection to grant Stone Form.",desc:"This spell turns the target into a statue for as long as the target remains motionless. As soon as the target chooses to move, the spell is broken. For the duration of the spell, the target is immune to all non-Magical physical attacks, or spell packets with the prefix \"physical\". They are also immune to all non ritual-magic sources of forced movement. While the spell is in effect, the target may not speak or use any skills. All other attacks, such as spells or Magic, affect the target normally. Due to safety concerns, you cannot use this spell in a manner which would trap someone else's limbs."},
  {sphere:"Protections",level:4,name:"Mage Leathers *",incant:"I invoke Protection to grant Mage Leathers.",desc:"This spell will surround the caster in semi-transparent leather armour. These leathers are Magical in nature and may be Dispelled as normal. Mage Leathers grants the caster +20 Magical Armour Points. This bonus armour will not stack with the Mage Robe or Mage Plate spells but may stack with any other armour that the caster is wearing. While the caster has Mage Leathers on their spirit, they suffer from a x2 vulnerability to Lightning damage. If the armour is Breached the remaining Lightning damage will carry over to the target. This spell is caster only."},
  {sphere:"Protections",level:4,name:"Tenacity *",incant:"I invoke Protection to grant Tenacity.",desc:"This spell will allow the target to carry on with an incantation through adversity. If the target accidentally miscants or has their concentration interrupted by Body damage or any other interruption, they may call \"Tenacity!\" and re-incant the spell. Only one Tenacity may be worn at any given time."},
  {sphere:"Protections",level:5,name:"Hold Portal",incant:"I invoke Protection to create Hold Portal.",desc:"A Hold Portal spell creates a Magical barrier surrounding any target window or doorway. The entire portal is covered by an impermeable field that is visible to all. Nothing besides normal air may pass through the barrier, although astral beings may do so. Once cast, the portal will be held until it is dispelled (via Dispel Magic), the duration expires, or the caster chooses to end it. This barrier will not block gaze-attacks. The target window or doorway does not need to have a windowpane or door present for this to function; an archway or window hole will suffice. The caster must attach a white H to the portal to indicate that the spell is active. Only one Hold Portal may be cast on a window or doorway at a time."},
  {sphere:"Protections",level:5,name:"Shield Magic *",incant:"I invoke Protection to grant Shield Magic.",desc:"This spell will protect the target once from the next Battle Magic spell or spell-like attack with 'Magic' in the call. It will protect the target from Spellstrikes but not weapon strikes, even those with 'Magic' in the call. It cannot be saved and will activate even if the target wishes to accept the spell. The only exception to this is if the spell is touch cast onto the target and the target chooses to accept it, such as in the case of most healing spells. Unconscious or incapacitated targets cannot choose to accept a touch cast spell. When this spell defense is used the target must call out \"Shield Magic\", and a visible flash of white energy can be seen as the spell-protection dissipates. Only one Shield Magic, Advanced Shield Magic, or Reflect Magic may be worn at any given time. It will not protect the wearer from any damage that contains the suffix \"Elemental\" in its damage call."},
  {sphere:"Protections",level:6,name:"Advanced Magic Armour *",incant:"I invoke Protection to grant Advanced Magic Armour.",desc:"This spell acts like a Magic Armour, except that the wearer of this spell may choose what attack to defend against. When this spell defense is used the target must call out \"Advanced Magic Armour\", and a visible flash of white energy can be seen as the spell-protection dissipates. Only one Magic Armour or Advanced Magic Armour a may be worn at a time."},
  {sphere:"Protections",level:6,name:"Dispel Magic",incant:"I invoke Protection to inflict Dispel Magic.",desc:"This spell will terminate any spell of ninth level or lower, unless specifically stated otherwise in the description. A Shield Magic or Reflect Magic will protect a living target from a Dispel Magic. If the spell is cast on a creature, all active spells on the creature are lost. Magic items that contain Battle Magic spells, Healing potions and Battle Magic scrolls are inoperative for 10 minutes. Dispel Magic has no effect on ritual magic."},
  {sphere:"Protections",level:7,name:"Mage Plate *",incant:"I invoke Protection to grant Mage Plate.",desc:"This spell will surround the caster in semi-transparent plate armour. This plate is Magical in nature and may be Dispelled as normal. Mage Plate grants the caster +30 Magical Armour Points. This bonus armour will not stack with the Mage Robe or Mage Leathers spells but may stack with any other armour the caster is wearing. While the caster has Mage Plate on their spirit, they suffer from a x2 vulnerability to Lightning damage. If the armour is Breached the remaining Lightning damage will carry over to the target. This spell is caster only."},
  {sphere:"Protections",level:7,name:"Reflect Magic *",incant:"I invoke Protection to grant Reflect Magic.",desc:"This spell behaves exactly like Shield Magic, except that when Reflect Magic is triggered, the magical effect that hit the user will be reflected back at the attacker. When this spell defense is used the target must call out \"Reflect\" and the attacker will be struck automatically with the reflected magic. When a magical effect is successfully reflected, the user of Reflect Magic becomes the caster of the reflected spell as if they had cast it themselves. The spell and its target (the original caster) cannot be changed, but things like its duration become under the control of the new caster. Only one Reflect Magic, Shield Magic, or Advanced Shield Magic may be worn at any given time."},
  {sphere:"Protections",level:8,name:"Advanced Shield Magic *",incant:"I invoke Protection to grant Advanced Shield Magic.",desc:"This spell acts like a Shield Magic, except that the wearer of this spell may choose what attack to defend against. When this spell defense is used the target must call out \"Advanced Shield Magic\", and a visible flash of white energy can be seen as the spell-protection dissipates. Only one Reflect Magic, Shield Magic, or Advanced Shield Magic may be worn at any given time. It will not protect the wearer from any damage that contains the suffix \"Elemental\" in its damage call."},
  {sphere:"Protections",level:8,name:"Iron Skin",incant:"I invoke Protection to grant Iron Skin.",desc:"This spell grants the target a 5 Normal threshold for ten minutes. Any attack that does 5 or fewer points of Normal damage is replied to with \"No Effect\". The target takes no damage from these attacks. This spell also makes the target immune to Saps for the duration of the spell. All attacks that are not normally damaging in nature (e.g. sleep) affect the target normally."},
  {sphere:"Protections",level:9,name:"Anti-Magic Field",incant:"I invoke Protection to grant Anti-Magic Field.",desc:"This spell will make the caster immune to all Battle Magic spells, so long as the caster holds both arms out to their sides and palms facing outwards. During this time, the caster can speak but must otherwise maintain Concentration. While in this position, the caster calls \"No Effect\" to all Magic that targets them, both positive and negative. This Anti-Magic Field will not protect against any Magic spell with the suffix \"Elemental\" in its damage call."},
  {sphere:"Protections",level:9,name:"Circle of Protection",incant:"I invoke Protection to create Circle of Protection.",desc:"This spell creates a 10-foot diameter spherical barrier, centered on the caster. This barrier will continue into the ground to complete a magical sphere around the caster, with the caster in the exact center. This barrier is frictionless and cannot be dispelled by Battle Magic spells. The Circle of Protection must be visually represented by a rope, a heavily drawn circle in the dirt, or any other method which distinctly creates a visible circle. This physical representation must be placed before the spell is cast or the spell will fail. If, during the casting, a creature or object is on the barrier wall, the caster will decide if they are pushed out or pulled in as the Circle wall raises. After the Circle is successfully cast, no physical object may pass through the barrier, including the caster. The caster may choose to end the spell at any time. If the caster's spirit leaves the circle for any reason, the spell will end. Once active, the Circle of Protection will act as a physical barrier preventing the passage of all physical objects (including gas, liquid, etc.) and Battle Magic spells. This barrier functions in both directions. Gaze attacks and ritual magic will pierce through the circle as well as other powerful ritual-level effects. Multiple castings by the same caster can be used to increase the size of the Circle by an additional 10 feet at any time after the initial Circle is cast. A Circle of Protection will not function as a ritual circle."},
  // Psionics
  {sphere:"Psionics",level:1,name:"Ego Whip",incant:"By force of will I inflict Ego Whip. 2 Magic Body!",desc:"This spell will do 2 points of Magic Body damage. This spell deals x4 damage to Angelic / Demonic creatures, but will not affect Undead, or other non-living creatures."},
  {sphere:"Psionics",level:1,name:"Sense Angelic / Demonic",incant:"By force of will I grant Sense Angelic / Demonic.",desc:"This spell will allow the caster the ability to sense whether any Angelic or Demonic creatures are in the area. Once the spell has been cast, the caster has the duration of the spell to \"Sense Angelic / Demonic\" once before the spell ends. The caster must choose either Angelic or Demonic at the time of the spell-casting. The \"Sense\" must be said in a normal speaking voice. Any Angelic or Demonic creatures in the area will respond with \"here\" if they are within hearing range."},
  {sphere:"Psionics",level:2,name:"Ethereal Walk",incant:"By force of will I grant Ethereal Walk.",desc:"This spell will allow the caster to disappear from their current location and reappear 10 feet away. At the time of casting, the caster must put their weapon or hand on their head (to show they are out-of-game), then walk 10 feet in a straight line at a normal walking pace and immediately go back in-game. There is no hold called for this spell. The time it takes for the caster to walk 10 feet is the time it takes to Ethereally Walk. The caster must immediately pick a direction and begin walking in a straight line. This spell does not allow the caster to bypass any obstacle that would normally impede their walk. If the caster cannot continue walking normally in a straight line due to an obstacle, then the spell immediately ends and the caster reappears. The caster will still set off any traps they set off during their walk and, if the trap would affect the person who triggered it, they will be damaged and the Ethereal Walk will end. While in this brief ethereal state, the player cannot speak, cast, use abilities or do anything else other than walk. Ethereal Walk cannot break line of sight."},
  {sphere:"Psionics",level:2,name:"Mind Meld",incant:"By force of will I grant Mind Meld.",desc:"Mind Meld may be used to communicate telepathically as long as the caster is touching the temples, forehead or shoulders of the target and concentrates on the task. The Meld takes 10 seconds to initiate. Once established, either participant may choose to convey speech in the form of words, emotions or pictures. Both participants may choose to fabricate any thought, emotion or picture. There is no way to confirm the validity of either participant's actions, through the use of Mind Meld. No other actions by either party may be taken while a Mind Meld is in effect. Mind Meld is not able to cause erasure or editing of memory. During a Mind Meld, the caster may choose to heal the target's Body points by casting Psionic \"Ego\" spells through the meld. These spells must be touch cast properly, including the incant, but the damage is converted to healing instead. The caster cannot break free of the Mind Meld during the initiation period, although if the target breaks the link, the Meld is terminated. If, during the Meld, the target or caster is rendered unconscious or dead, the link is considered to have been terminated by the target. Mind Meld cannot be forced upon a target. If the target is not willing, the spell simply fails. The target may terminate the Mind Meld at any time, without penalty, and the caster may terminate it likewise, at any time after the 10 seconds has elapsed."},
  {sphere:"Psionics",level:3,name:"Hallucinate",incant:"By Force of will I inflict Hallucinate.",desc:"This spell causes wild and unrealistic hallucinations to flood the mind of its victim. It is up to the victim to roleplay these hallucinations. For example, victims might miscant, swing at enemies that are not there, or fail to recognise their friends. The effect can only be removed by a Dispel Magic or by waiting ten minutes. The victim does not realise this spell was cast on them until the effect ends. This effect stacks. For each additional Hallucinate the victim is hit with, the hallucinations will become more vivid, more disturbing, encompass more senses, etc. Each time the victim is hit with another stack of Hallucinate, the duration will be reset to 10 minutes and the victim will experience the full number of stacks for the remainder of the duration. Hallucinate will stack with other forms of Hallucinate, such as Hallucinoid alchemy, up to a maximum of 5 stacks. 1 stack: The victim experiences visual hallucinations, seeing things that are not there. 2 stacks: The victim experiences auditory and physical hallucinations, such as hearing voices or feeling like something is touching them. 3 stacks: The victim has difficulty speaking or understanding complex speech and may begin to speak in gibberish at times. 4 stacks: The victim cannot distinguish friend from foe, seeing everyone around them as entirely different people. 5 stacks: The victim's reality is entirely replaced by a hallucination, putting them in a completely different world with different people and objects, and so on."},
  {sphere:"Psionics",level:3,name:"Psionic Knife",incant:"By force of will I create Psionic Knife.",desc:"This spell focuses the caster's mental energy into one small, blade-shaped force, which can be used in combat. Once the spell is cast, the caster may wield a dagger-sized phys-rep (blue) swinging for 2 Magic. This does no extra damage to demons, but does affect Undead. While this spell is in effect, the caster may not cast any spells. At any time during the duration of this spell, the caster may channel any Psionic spell currently in memory through the weapon by calling \"Spellstrike <Spell-Name>\". This reduces the damage that the knife can swing for by 1. If the damage of the knife is reduced to zero, the hour runs out, or the caster wishes, the spell ends. Should the caster drop the weapon or become disarmed, the weapon will dissipate and the spell will end. The caster is responsible for bringing their own blue weapon phys-rep, the spell will fail without the proper rep. Summoned weapons may be used with natural weaponry like Savar'Aving Claws, but will not grant the user the Florentine skill needed to fight with both. Purchasing an Exotic Weapon Specialization: Summoned Weapons will increase the damage of any weapon conjured by this spell by 1 per purchase, but the summoned weapon will still dissipate when a number of Spellstrikes equal to its base damage are used."},
  {sphere:"Psionics",level:4,name:"Ego Flay",incant:"By force of will I inflict Ego Flay. 5 Magic Body!",desc:"This spell will do 5 points of Magic Body damage. This spell deals x4 damage to Angelic / Demonic beings but will not affect Undead, or other non-living creatures."},
  {sphere:"Psionics",level:4,name:"Sleep",incant:"By force of will I inflict Sleep.",desc:"This spell causes the target to fall instantly into a deep sleep. The person will sleep for the duration of the spell, unless someone shakes them continuously for one minute, or if they take damage into Body. The target will awaken enough only to interrupt Killing Blows then fall back into deep sleep. The target will not snore. This spell has no effect on Undead or non-living creatures."},
  {sphere:"Psionics",level:5,name:"Ego Rend",incant:"By force of will I inflict Ego Rend. 10 Magic Body!",desc:"This spell will do 10 points of Magic Body damage. This spell deals x4 damage to Angelic / Demonic beings but will not affect Undead, or other non-living creatures."},
  {sphere:"Psionics",level:5,name:"Silence",incant:"By force of will I inflict Silence.",desc:"While under the effects of Silence, the target cannot make any sound that comes out of their head, including speech, grunting, coughing or the use of wind instruments. Casting spells becomes impossible; although the player must still call out any damage they may do using weapons. This spell may be countered with Dispel Magic."},
  {sphere:"Psionics",level:6,name:"Charm",incant:"By force of will I inflict Charm.",desc:"This spell causes the target to treat the caster as their best friend. Although it does not turn the target into a mindless automaton that follows every order the caster gives, the target will be required to stay with their \"friend\" and listen to any \"suggestions\" the caster may give. If the caster attacks the Charmed individual, the spell will be broken. However, friends of the caster may attack the victim and the spell may remain intact if the caster can give adequate reason as to why they are not defending the target. A Charmed creature will not attack their old friends unless given enough reason. However, if the target is told to \"defend me\" and their old friends attack the caster; this would be considered adequate reason. This spell will not force the target to act in a way that is contrary to their nature (a pacifist killing someone, etc.). The spell will not force the target to tell the truth or reveal secrets, unless it is already in their nature to do so to their best friend. This spell will not force the target to do anything obviously suicidal unless it would be in the target's nature to do so. This spell will not work on Undead or other mindless creatures. A target may be Charmed to multiple people at the same time. If this would cause a conflict, the most recent Charm will override any previous Charms. This does not cure the previous Charms; it only makes them inactive as long as they are in conflict with the most recent Charm. The victim does not realise this spell was cast on them until the effect ends."},
  {sphere:"Psionics",level:6,name:"Ego Burn",incant:"By force of will I inflict Ego Burn. 15 Magic Body!",desc:"This spell will do 15 points of Magic Body damage. It will do x4 damage if the target is Angelic / Demonic. This spell will not harm Undead."},
  {sphere:"Psionics",level:7,name:"Circle of Protection: Demonic / Angelic",incant:"By force of will I create Circle of Protection: Demonic (or) Angelic.",desc:"This spell will summon into existence a Circle of Protection. This is protection against either the Demonic or the Angelic (chosen at the time of casting). It will affect both Lesser and Greater demons/angels. This Circle must be physically represented by the caster and cannot be larger than 10 feet in diameter. While this Circle is up, no creature of the chosen type can enter or leave. This Circle can be used to trap as well as repel. If the Circle is used to trap a creature, it will last for 5 days for a Lesser demon/angel or 1 hour for a Greater demon/angel, or until the creature is killed. The Circle is immune to all spells and effects originating from the chosen creature type including Dispel Magic. This does not apply to any other creatures that can dispel the circle normally. The caster may leave the circle."},
  {sphere:"Psionics",level:7,name:"Psionic Blade",incant:"By force of will I create Psionic Blade.",desc:"This spell acts exactly as the Psionic Knife spell, except as follows: the caster may use a phys-rep up to Sword size, the Psionic Blade's starting damage is 4 Magic and the caster may Spellstrike any spell memorized regardless of Sphere. Should the caster drop the weapon, or become disarmed, the weapon will dissipate and the spell will end."},
  {sphere:"Psionics",level:8,name:"Forget",incant:"By force of will I inflict Forget.",desc:"Forget causes the target's memory to be erased of all that occurred within the last 10 minutes. If a Dispel Magic is cast on the target or the target receives a Charm Break within one hour, the memories will be restored. One hour after the casting, the effects are permanent and cannot be restored save via Ritual Magic. If the victim dies (not just enters their Death Count) before the hour has ended, the Forget is cured. This spell can be freely resisted by any conscious target. The target will be fully aware their memories have been removed but will have no idea how, why or by whom. Multiple Forget spells can be cast at once to increase the duration. Each casting will add 10 minutes to the period the victim forgets."},
  {sphere:"Psionics",level:8,name:"Paralysis",incant:"By force of will I inflict Paralysis.",desc:"The spell Paralysis will immobilize the target, rendering them unable to move at all. This spell will not work on creatures which have no nervous system such as Undead, Golems, Elementals, etc."},
  {sphere:"Psionics",level:9,name:"Exorcism",incant:"By force of will I inflict Exorcism.",desc:"This spell will destroy any lesser Demon or Angel, sending it back to the plane from whence it came, trapping it there for a year and a day. Against greater Demons and Angels, this spell will do 216 points of Magic Body damage. This spell, if cast at a target who is possessed by a Demon, will only affect the Demon, and not the target. This spell will also send a ghost from a Haunt fully back to the Deadlands, removing their foothold in the physical world."},
  {sphere:"Psionics",level:9,name:"Mimic",incant:"By force of will I grant Mimic.",desc:"This spell allows the caster to copy a spell whose incantation they have heard, other than a Mimic spell. Within 1 minute of hearing the spell they wish to mimic, the caster must incant the Mimic spell. Within the next 3 seconds, they can cast the spell as if it was one of their own. The caster may mimic a spell that they originally cast. The caster does not need to know the sphere that they are mimicking. This spell may only mimic Battle Magic spells from the core rulebook. It cannot be used to imitate magic items, Spellstrikes, monster abilities, or anything else that does not use the full, spoken incant of a spell."},
  // Dark
  {sphere:"Dark",level:1,name:"Bless *",incant:"I channel <God> to grant Blessing.",desc:"This spell calls down upon the target the blessing of whichever God the caster worships. If the caster casts Bless on themselves, it will function as a Shield Magic versus the next Divine or Draconic Battle Magic spell to strike the caster. From time to time a character with a Bless on their spirit may find favour with the God(dess) that the caster serves. This can sometimes, decided by a Shaper, have a small positive effect happen to or around them. This could be anything from a small warning of danger to minor healing or even minor miracles. The caster may not force a Bless upon a person and it may be resisted without using up a spell-protection, such as Shield Magic. One can only be Blessed if one chooses to be and only one Bless can be active at a time. A person can choose to allow a new Bless spell to replace an old one if they wish. They may also end a Bless on themselves any time they choose, but this may offend the god."},
  {sphere:"Dark",level:1,name:"Siphon",incant:"I channel <God> to inflict Siphon.",desc:"This spell can only be targeted at someone who is currently in their Bleed Count. If successfully cast, the spell will cause the target to enter their Death Count, bypassing their Bleed Count completely, and grant the caster 5 Body points in healing or infliction, by caster's choice. This cannot exceed the caster's maximum Body point total nor can it be thrown or transferred to another."},
  {sphere:"Dark",level:2,name:"Divine Ward",incant:"I channel <God> to create Divine Ward.",desc:"Divine Ward requires the caster to plant or otherwise display their holy symbol foci for the duration of the spell. During this time, the symbol may not be used to cast other Dark spells. The symbol does not have to remain on the person of the caster and, in fact, may be hung upon a door, placed upon a tree or otherwise, so long as it remains stationary. Placing the spell tag next to the symbol is encouraged. While the symbol is being used in this way, creatures possessing a spirit may not approach within 10 feet of the symbol unless they are wearing a Bless spell of the deity represented by the Divine Ward. When the spell is cast, anyone not wearing a Bless spell of the appropriate deity will be pushed out of the Ward. If a creature already in the Ward cannot retreat any further, the spell will fail and is lost. This barrier may be resisted with Shield Magic, Resist Magic or similar anti-magic defenses spell, and it may also be resisted by expending an active Bless spell from any God or Goddess. Doing so makes the user immune to the effects of this Divine Ward for 10 minutes. If the symbol is physically moved the spell ends. The caster of Divine Ward is immune to the effects of the spell."},
  {sphere:"Dark",level:2,name:"Soul Whip",incant:"I channel <God> to inflict Soul Whip. 3 Dark Drain!",desc:"This spell will summon a black, wispy tendril to strike out at the target, causing 3 Dark points of damage and mending the caster the same amount. Any Mending that exceeds the caster's maximum Body points grants them temporary Body points equal to the excess, up to a maximum of double the caster's original Body points. Temporary Body points gained from this ability lasts 1 hour. If the target resists the spell or is otherwise unaffected by the damage, the spell fails."},
  {sphere:"Dark",level:3,name:"Death Aura",incant:"I channel <God> to grant Death Aura.",desc:"This spell will hide the target's spirit in an aura of Undeath. While Death Aura is active the target will not be detectable via Sense Life."},
  {sphere:"Dark",level:3,name:"Mass: Blessings",incant:"I channel <God> to grant Mass Blessing.",desc:"This area-of-effect spell requires the caster to give a powerful Mass to their flock, calling on their God to Bless those the caster touches. To initiate Mass: Blessings the caster must roleplay a sermon to their God, speaking to those present about their deity's tenets, beliefs and how they relate to the situation at hand for at least one minute. After that minute has passed they may then, while continuing their sermon, touch the foreheads of any who have heard it. One person may be touched in this manner every 10 seconds so long as the sermon continues or the maximum duration of 10 minutes is reached. Each person who is touched by the caster in this manner will take the effect of a Bless spell. A maximum of 10 Blessings may be granted. Each person may only receive one Blessing per Mass. The caster may not \"force\" the effects of this mass to take place upon anyone, including the unconscious, dying, or otherwise incapacitated."},
  {sphere:"Dark",level:4,name:"Banner of the Faithful",incant:"I channel <God> to create Banner of the Faithful.",desc:"This spell creates a magic \"flag\" or banner which lasts one hour's time. During that time, any character that has a Bless spell of the same God on their spirit may gain access to the Banner's full abilities. The Blessed character must touch the Banner and speak the God's name. Once done, they may attack for +0 Magic damage so long as the Banner stays within their line of sight. This bonus includes ranged weapons. The flag is considered a non-spirited item with 1 Body and may be destroyed by any weapon damage, Acid, or Elemental damage. Anyone holding the Banner will take whatever damage it takes. If the banner leaves the target's line of sight for more than 10 seconds, the effect is lost until the Banner is back in their line of sight. The banner must be visible as well, which means that it may be necessary to illuminate a banner used in the dark. A Banner may be any shape so long as it is a minimum 2.5' x 1' and no greater than 4'x 6' and must be mounted on a pole with a minimum length of 4' and a maximum of 6'. The holy symbol of the God worshipped must be represented on the Banner. When the banner is first created, the caster must state \"Banner up - <God's name>!\". When the banner ends for any reason, the caster must then state \"Banner down - <God's name>!\". The caster of Banner of the Faithful is always under the Banner's effect while it exists."},
  {sphere:"Dark",level:4,name:"Control Mindless",incant:"I channel <God> to inflict Control Mindless.",desc:"This spell grants the caster control over one non-sentient creature. Non-sentient creatures are limited to mindless Undead, lesser mindless constructs, natural animals and victims of Feeblemind. This spell will not work on a target with an active Bless or Dragon Mark but will work on children too young to resurrect, though this is considered abhorrent by most. This control will allow the caster to command the target to do anything, including suicidal actions. Control will last for 1 minute, unless the target is undead in which case it will last 10 minutes. If Control Mindless is used on a living target it will leave a scar of the Cleric's God's holy symbol somewhere on its body. The scar will fade after one year or may be removed early through divine intervention."},
  {sphere:"Dark",level:5,name:"Mass: Relic",incant:"I channel <God> to grant Relic.",desc:"This 10 minute mass magically enhances an item, typically a weapon, in the name of the God of the caster. Once the mass is complete, the object or weapon is made rendered as per the spell and is given a Magic aura. The weapon or object will become attuned to the first creature bearing the Bless of the caster's God that touches it after the mass is completed. If the item is dropped by the attuned creature or passed off to another creature, the spell ends and the item will revert back to its normal form. The effects on the object last for 24 hour, starting at the completion of the mass."},
  {sphere:"Dark",level:5,name:"Wave of Pain",incant:"I channel <God> to inflict Wave of Pain, Wave of Pain, Wave of Pain.",desc:"Before this spell is cast, the caster must plant both feet and then incant. They may then do 5 Dark via packet, touch cast, or a combination, up to five times. Each damage call must be preceded by the phrase \"Wave of Pain\". If the caster moves either foot or is struck for damage to Body, any remaining waves are lost and the spell ends."},
  {sphere:"Dark",level:6,name:"Dark Lore",incant:"I channel <God> to grant Dark Lore.",desc:"This spell allows the caster to summon a Ghost or lost spirit and ask a series of questions in which it is bound to answer truthfully. The caster should have a topic of questioning in mind before casting the spell. Spirits summoned in this manner will arrive as soon as they possibly can but no later than 12 hours after casting. During this wait the caster should attempt to find a Shaper at their earliest convenience. The first few questions are set and must be spoken verbatim after the spirit arrives. These questions are: \"Spirit before me I bind you and command you to identify yourself.\" \"I bring you no ill will; do you wish my spirit harm?\" \"I seek the knowledge in death regarding <Subject>.\" \"I release you of your binding, you are free to go. Will you leave peacefully?\" OR \"I release you of your binding but request additional information if it pleases you. Will you stay?\" If the Cleric fails or incorrectly speaks these questions the spirit may not arrive or may arrive hostile. If the Cleric succeeds, the spirit is bound to answer truthfully, to the best of its knowledge, the four questions asked. After this point the caster may continue asking questions of the spirit if the spirit is willing. The limit of questions is random, generally depending on the demeanor and sensitivity of the caster toward the spirit. Some spirits are simply uninterested in speaking to the living and will leave after the required questions are answered. The quality of answers will greatly depend upon the spirit called, which in general terms is beyond the ability of the caster's control. The use of Dark Lore is not considered Necromantic in nature although it may be mistaken as such to the uneducated."},
  {sphere:"Dark",level:6,name:"Unholy Armour *",incant:"I channel <God> to grant Unholy Armour.",desc:"This spell gives the target 25 points of Magical amour. This armour is Magical in nature and may not be Refit. Magical armour is removed before physical armour. This spell cannot be stacked with itself. While the Unholy Armour is active, the target will Sense as Demonic, Undead, Wytchcraft, Necromancy and Dark, though they will not be changed into any of those things."},
  {sphere:"Dark",level:7,name:"Corruption",incant:"I channel <God> to inflict Corruption.",desc:"This spell will cause its target to take x2 damage from all physical weapon attacks for 10 minutes. Additionally, any spell thrown by the caster of Corruption at the target will receive an Echo effect for each spell. This Echo effect will allow the caster to strike the target an additional time with the same spell if the first spell was successfully defended against in any way. This is done by calling \"Echo!\" immediately after the spell was defended against."},
  {sphere:"Dark",level:7,name:"Dark Bolt",incant:"I channel <God> to inflict Dark Bolt. 20 Dark",desc:"This spell causes a bolt of darkness to spring from the caster's fingers towards the target. The spell will take full effect on Undead creatures and living creatures alike. The bolt does 20 points of Dark damage straight to Body. This damage will be halved if the target has any active Bless spell on their person."},
  {sphere:"Dark",level:8,name:"Chains and Bonds",incant:"I channel <God> to inflict Chains and Bonds.",desc:"This spell creates magical chains, hooks and locks that wrap around the target. These chains will Silence their victim. Their legs are bound together and their arms forced against the sides of their body, making actions impossible. Creatures with a Strength of 6 may break free from the chains. Doing so takes 3 seconds and causes the victim to take 6 Body in the process. Creatures bound in this way can be picked up and moved."},
  {sphere:"Dark",level:8,name:"Unholy Warrior",incant:"I channel <God> to summon an Unholy Warrior.",desc:"This powerful spell will allow the Cleric to call upon their God to send forth an Unholy Warrior to strike down one who has wronged them. The Cleric must offer up a sacrifice of a catalyst or an object worth at least 1 gold in value appropriate to the Cleric's god. Once cast, the offering is consumed and a being of pure shadow and darkness will manifest before the Cleric within the next 12 hours. When the Unholy Warrior has arrived the Cleric then needs to speak the name of the target as they know it, visualize the target's identity for one minute and finally state how the target has wronged the Cleric or their God. During this count, the Unholy Warrior cannot be the target of spells or effects, nor will they defend the Cleric or themselves until the spell prerequisites are completed. If the Cleric does not complete these requirements within two minutes of their arrival, the Unholy Warrior will leave. If the requirements are met, the Unholy Warrior will then dissipate, becoming undetectable to even the most powerful of magic. For the next hour the Unholy Warrior will hunt the target, searching tirelessly and with the innate ability to sense that target's spirit at will. When the target is found, the Unholy Warrior will phase in nearby with a 3-count. It will state to the target that they have wronged a Cleric of <God> and that their life is forfeit. The Unholy Warrior will attack that target to the best of its ability and will not cease until it is destroyed or the target has ended its Death Count. An Unholy Warrior will be equal to the level and power of the Cleric who is summoning it. Should the Cleric speak the True Name of the target to the Unholy Warrior or use a Discord catalyst as the offering, that level will increase to the Cleric's level +5. The Unholy Warrior's Occupation is determined randomly by the God of the Cleric. Once the target has been destroyed the Unholy Warrior will return to the Cleric and announce its success. Should the Cleric decide after successfully casting the spell that they made a mistake and wish to cancel the Unholy Warrior's summoned duty, they may do so by expending their own bless spell. Ending the spell in this manner will incur a very harsh repercussion. As punishment for wasting the Dark God's power, the Cleric will find themselves the target of their own Unholy Warrior. No creature may be the target of this spell by the Cleric more than once per month, nor will the Unholy Warrior attack any creature that carries a Bless of the Clerics God. The Unholy Warrior is Celestial in Nature."},
  {sphere:"Dark",level:9,name:"Avatar",incant:"I channel <God> to grant Avatar.",desc:"This spell turns the Cleric into an \"Avatar\" of their deity, morphing their body into a shadowy dark form. After the spell is cast, the Cleric's shape will change over the course of a 3-count as they grow two feet in height; their physical features become shadowy black and their eyes glow blood red. This spell will also summon into existence either a two-handed Dark melee weapon or a one-handed Dark melee weapon and shield. The two-handed Dark weapon has a base damage of 10 Magic, while the one-handed weapon's base damage is 5 Magic. The shield has a 60 Magic threshold. The spell also grants the proficiency in Exotic Weapon: Dark <Weapon> and the Shield skill, as long as they are holding the summoned weapons. The Cleric can choose which weapon combination they would like at the time of casting. In Avatar form, the Cleric also has the ability to Spellstrike 10 Dark through their summoned weapon of choice a total of three times. They also gain a temporary health boost of 50 Body. Any Body Damage the Cleric receives is removed from the bonus 50 Body points first and this Body cannot be healed. The weapons and/or shield will instantly dissipate if the Cleric drops them, is rendered unconscious, or incapacitated. These items may be used with natural weaponry, like a Savar'Aving's Claws. The Cleric may not cast any spells while in Avatar form. When the Avatar ends, the Cleric will perform a 3-count to exit the form."},
  {sphere:"Dark",level:9,name:"Death",incant:"I channel <God> to inflict Death.",desc:"Death causes the spirit of the target to be ripped forcibly from the Body, putting the target into their Death Count, dropping their Body points to -1 and bypassing their Bleed Count completely."},
  // Draconic
  {sphere:"Draconic",level:1,name:"Divine Shield *",incant:"I call upon <Dragon> to grant Divine Shield.",desc:"Divine Shield functions like a \"Shield Magic\" spell against any spell from the Dark or Light Spheres of Magic. It can be stacked with Shield Magic or Advanced Shield Magic but will have no effect against Divine Ritual Magic. If wearing both Shield Magic and Divine Shield simultaneously and struck with a Divine spell, the Divine Shield will always activate first."},
  {sphere:"Draconic",level:1,name:"Mark of the Firstborn *",incant:"I call upon <Dragon> to grant Mark of the Firstborn.",desc:"This spell causes the symbol of the Firstborn (served by the Dragon Knight who cast it) to appear upon the target. The target must be willing or the spell fails without affect. The mark will appear on the cheek of the target and may be drawn to represent this. The symbol must be clearly visible and cannot be hidden. If the Dragon Knight casts Mark of the Firstborn on themselves, it will function as a Shield Magic versus the next divine spell to strike the Dragon Knight. The target may end this mark any time they choose, but this may offend the Firstborn."},
  {sphere:"Draconic",level:2,name:"Dragon Hide",incant:"I call upon <Dragon> to grant Dragon Hide.",desc:"This spell will grant the target an immediate repair of damaged 10 armour points. It will only repair armour pieces, not other things which might be repaired by a Blacksmith with Shaper approval. It will not work on Gargylen."},
  {sphere:"Draconic",level:2,name:"Sign of the Firstborn",incant:"I call upon <Dragon> to create Sign of the Firstborn.",desc:"Sign of the Firstborn requires the caster to place a symbol of the Dragon they serve at a location of their choice. This symbol can be a banner, flag or simple drawing. Once cast, this symbol cannot be moved. While active, no creature with a spirit may approach within 10 feet of the symbol unless wearing a Mark of the Firstborn. This barrier may be resisted with a Shield Magic or similar spell and if resisted the target becomes immune to the effects of Sign of the Firstborn for 10 minutes. If the symbol is physically moved the spell ends. The caster is not immune to the effects of the spell and must be wearing a Mark of the Firstborn to pass."},
  {sphere:"Draconic",level:3,name:"Enlightenment of the Firstborn",incant:"I call upon <Dragon> to grant Enlightenment of the Firstborn.",desc:"This spell works like a Mark of the Firstborn but over a greater range of targets. Immediately after casting this spell, the Dragon Knight must lead a 10 minute discussion or debate on any topic relating to the Firstborn, their followers or the fight against Gods. After the first minute has passed the Dragon Knight may anoint those present with their symbolic weapon of choice, bestowing onto them the Mark of the Firstborn served. The Dragon Knight must continue the debate while bestowing the Mark and if they stop the spell will fail and all Marks granted will become dispelled. A Dragon Knight may grant the Mark to one target every 10 seconds or until the 10 minute duration has been reached. A maximum of 10 Marks may be granted. Dragon Knights may not force the Mark an unwilling subject or those who are unconscious, dying or otherwise incapacitated."},
  {sphere:"Draconic",level:3,name:"Scales *",incant:"I call upon <Dragon> to grant Scales.",desc:"This spell will protect the caster from the next Body Damage attack that strikes them. If stacked with a Magic Armour, Scales will always activate first. It will only protect against physical Body attacks delivered via a weapon strike. When this defense is triggered, the caster must call \"Scales!\""},
  {sphere:"Draconic",level:4,name:"Shadow of the Firstborn",incant:"I call upon <Dragon> to grant Shadow of the Firstborn.",desc:"For the next hour after casting, the caster will become immune to all \"Sense\" type effects such as \"Sense Life\" from Undead creatures."},
  {sphere:"Draconic",level:4,name:"Strength of the Firstborn",incant:"I call upon <Dragon> to grant Strength of the Firstborn.",desc:"This spell will grant the target a +3 Strength bonus for 1 hour. This spell will stack with other strength bonuses but not itself."},
  {sphere:"Draconic",level:5,name:"Dragon Fear",incant:"I call upon <Dragon> to inflict Dragon Fear.",desc:"This spell will cause the affected target to flee in fear. If line of sight between the target and caster remains broken for one minute, the fear effect will end. While under the effects of fear, a victim will do everything in their power to escape the line of sight with the caster. At first they may simply attempt to flee, but if physically held within the fear range or are otherwise forced to confront the caster, their reaction will escalate to violence. After the one minute duration has expired, the target will still be unable approach or interact with the caster or come within 100 feet of them, for the next 10 minutes. Removing or dispelling the effect of Dragon Fear will negate both the fear and the aversion that follows."},
  {sphere:"Draconic",level:5,name:"Dragon's Regeneration",incant:"I call upon <Dragon> to grant Dragon's Regeneration.",desc:"While uninterrupted concentration is continued by the caster, they will gain 1 Body point of healing every 60 seconds, for up to 10 minutes. The 1 Body of healing will take effect at the end of each 60 second count, not the beginning. If the caster uses any other skill or breaks concentration, the spell will end. Any person with a Mark of the Firstborn may concentrate along with the caster to gain the benefits of this healing as well. The caster must keep concentrating in order for others to do this, even if they are at full Body."},
  {sphere:"Draconic",level:6,name:"Breath of the Firstborn",incant:"I call upon <Dragon> to inflict Breath of the Firstborn. 25 Elemental <Type>!",desc:"This spell will do 25 points of Elemental damage. The elemental type is determined by the caster but there is otherwise no difference in the effects. Should this spell drop the target to negative Body points, the target will forgo their Bleed Count and directly enter their Death Count as per typical elemental damage calls. If their target successfully defends against this spell, the Dragon Knight can cause it to strike a second time in an attempt to bypass defenses. The Dragon Knight may then call \"Innate Echo!\", causing the target to be instantly hit by the spell again, although they may still defend against it if possible."},
  {sphere:"Draconic",level:6,name:"Dragon's Intuition",incant:"I call upon <Dragon> to grant Dragon's Intuition.",desc:"This spell requires 10 minutes of concentration by the caster. At the end of those 10 minutes, the caster will gain insight into the levels of Divine energy in the surrounding lands, typically defined as a five mile radius. It will grant a general impression of powerful Divine beings, sources of Divine energy and concentrations of followers but will not give details beyond which God(s) are behind this influence. For example, it may indicate a powerful Divine creature adherent to Raze moving through the area but will not give a description of that creature, or it may state that a concentration of followers of a Cassandra are nearby but not where or who they are."},
  {sphere:"Draconic",level:7,name:"Dragon's Toughness *",incant:"I call upon <Dragon> to grant Dragon's Toughness.",desc:"This spell will grant 30 of temporary Body points to the caster. These extra Body points will be counted down first when damage is taken, before the caster's natural Body points. This spell cannot be stacked. All lightning based attacks that strike the caster do x2 damage."},
  {sphere:"Draconic",level:7,name:"Elemental Fragility",incant:"I call upon <Dragon> to inflict Elemental Fragility <type>.",desc:"This spell will cause its target to suffer x4 damage from one elemental type for 10 minutes, chosen at casting. The caster will receive 1/2 damage from that element for 10 minutes."},
  {sphere:"Draconic",level:8,name:"Fury of the Firstborn",incant:"I call upon <Dragon> to grant Fury of the Firstborn.",desc:"After casting Fury of the Firstborn the caster may state \"Sense Bless\". Every creature with an active Bless spell within earshot must respond \"Here!\" For each person that responds, the caster of Fury of the Firstborn will gain +1 damage for 10 minutes. The caster will also gain an immunity to all numeric Dark and Light damage for the duration of the spell. This spell may be combined with Talons of the Firstborn and Spirit of the Firstborn to deadly effect."},
  {sphere:"Draconic",level:8,name:"Talons of the Firstborn",incant:"I call upon <Dragon> to grant Talons of the Firstborn.",desc:"This spell will change the caster's hands into powerful talons. The talons will be claw size or smaller. Each talon swings for 5 Magic Body, which cannot be augmented by any means, including benefits that apply to summoned weapons, except Fury of the Firstborn. While the talons exist no other weapons or skills which require the hands can be used. No weapon skills can be combined with the talons. Talons of the Firstborn may be combined with Spirit of the Firstborn and Fury of the Firstborn to deadly effect. This spell is caster only."},
  {sphere:"Draconic",level:9,name:"Life of the Firstborn *",incant:"I call upon <Dragon> to grant Life of the Firstborn.",desc:"This spell functions as a Contingency Life spell. Contingency spells remain on the spirit and automatically activate when certain conditions are met. Life of the Firstborn will activate when the caster has one second left in their Death Count. At this time, the spell will cast Life on the caster, bringing the caster back to full Body points instantly. This spell is caster-only and cannot be stacked with itself or any other Contingency Life spell. When activated, the caster should state \"Draconic Contingency Life\"."},
  {sphere:"Draconic",level:9,name:"Spirit of the Firstborn",incant:"I call upon <Dragon> to grant Spirit of the Firstborn.",desc:"This spell infuses the caster with small piece of the spirit of the dragon they serve. Ethereal draconic wings will erupt from the casters back for a brief second before vanishing, as the caster is empowered with the might of the Firstborn on a 3-count. This spell will grant the caster +75 temporary Body, two claws which swing for \"2 Magic\" and the ability to throw one packet of \"50 Elemental <type>\", with the type being the caster's choice. If the Dragon Knight casts Talons of the Firstborn, those claws may be used instead. Any Body Damage the Dragon Knight receives is removed from the bonus Body points first and this Body cannot be healed. If the caster is dropped to -1 Body while the spell is active, it will end. When Spirit of the Firstborn ends, the Dragon Knight will perform a 3-count to exit the form. If their target successfully defends against the 50 Elemental <type> packet, the Dragon Knight can cause it to strike a second time in an attempt to bypass defenses. The Dragon Knight may then call \"Innate Echo!\", causing the target to be instantly hit by the 50 Elemental <type> again, although they may still defend against it if possible."},
  // Dredgecraft
  {sphere:"Dredgecraft",level:1,name:"Grog",incant:"I call the Deep to grant Grog.",desc:"This spell increases the alcoholic strength of a bottle. The spell must be touch-cast onto a bottle phys-rep, either with or without an alcohol tag already attached. Each Grog tag on the bottle increases the Stamina damage of each serving by 1, up to the first 5 servings maximum. Servings beyond the 5th will not be affected. Each time this spell is cast on a drink it becomes a little more foul but remains surprisingly refreshing, and by the 5th cast no one is drinking it for the flavour. The spell tag must be taped to the bottle and if concentration is broken before the tag is affixed, the spell fails. An untagged bottle is treated as having 5 servings. Once the tag is attached to the bottle, the effect will last for 1 year after casting."},
  {sphere:"Dredgecraft",level:1,name:"Riptide",incant:"I call the Deep to inflict Riptide.",desc:"This spell causes a magical current of energy to pull the target down and away. The target is pushed back 10 ft and must kneel on one knee for 3 seconds. During this time the target is unable to move but may still perform actions normally."},
  {sphere:"Dredgecraft",level:2,name:"Punch Drunk *",incant:"I call the Deep to grant Punch Drunk.",desc:"This spell will protect the caster from the next source of numerical damage to their Body, converting Body damage into Stamina damage. This includes damage that armour fails to block and therefore strikes Body, damage that strikes straight to Body, and magic from Battle Magic spells which goes to Body. This does not prevent additional effects from the attack, if there were any. Punch Drunk will not activate if the damage would have been multiplied due to a racial weakness or other effect such as being hit with fire damage while wearing a Barkskin."},
  {sphere:"Dredgecraft",level:2,name:"Tread Water",incant:"I call the Deep to grant Tread Water.",desc:"This spell will cause the target to feel as though they are treading in water that only they can feel. While this spell is active, they can move no faster than walking pace (1 step per second) and will be unimpeded by effects below ritual level which slow a person down, such as a Hamstring, Dismember or Swampwalk. This does not allow them to ignore effects which prevent them from moving entirely, such as a Snare or Paralysis."},
  {sphere:"Dredgecraft",level:3,name:"Dram",incant:"I call the Deep to grant Dram.",desc:"This caster only spell will allow the caster to receive the effects of a single Ingested alchemy without consuming the tag. This spell does not work on Chemistry or alchemy which costs more than 24 RM to create. Using this spell will taint the alchemy, causing it to expire in 5 days. The caster should indicate this by affixing the spell tag to the alchemy tag."},
  {sphere:"Dredgecraft",level:3,name:"Sea Legs",incant:"I call the Deep to grant Sea Legs.",desc:"The first time the target of this spell receives Stamina damage, they will instead receive Healing equal to the Stamina damage taken."},
  {sphere:"Dredgecraft",level:4,name:"Alestorm",incant:"I call the Deep to inflict Alestorm. [X] Magic!",desc:"This spell will sober up the caster at the same time as damaging their target. The damage this spell does is however much Stamina the caster is missing, up to 20. The caster regains that much Stamina."},
  {sphere:"Dredgecraft",level:4,name:"Curse of Breathless Lung *",incant:"I call the Deep to grant Curse of Breathless Lung.",desc:"This spell grants the recipient a Lesser Curse which acts as a contingency defence. When triggered by the target needing to breathe but being unable to do so (such as when a person is drowning or being strangled), for the next 10 minutes the target will be Silenced but will not need to breathe. During this time, they must call \"No Effect\" to effects which are based on causing someone not to breathe, like Garrotte. The curse ends once the contingency is triggered."},
  {sphere:"Dredgecraft",level:5,name:"Curse of the Captain",incant:"I call the Deep to grant Curse of the Captain.",desc:"This touch-cast spell must be cast on a conscious, willing target. The target will be Charmed to the caster of the spell for the duration and gain +2 Strength. The effect of this Charm compels the target to see the caster not necessarily as a friend, but as a superior. While they are not magically compelled to satisfy every order they are given, they will feel considerable pressure to comply and should act as they would act in the presence of a respected superior. If the target is already cursed with one or more Lesser Curses from this sphere, they may choose to replace one of those curses with Curse of the Captain. This spell is a Charm effect."},
  {sphere:"Dredgecraft",level:5,name:"Parley",incant:"I call the Deep to grant Parley.",desc:"This spell will make the target believe that any conflict with the caster can and should be resolved verbally. While Parley is active, the target may not attempt to physically harm the caster or instruct others to do so, although they may still feel hostile towards them. If the caster is physically hostile towards the target or instructs others to be, the spell will end and the caster will take a Magic Charm effect towards the original target of the spell for 10 minutes. This spell is a Charm effect."},
  {sphere:"Dredgecraft",level:6,name:"Cat o' Nine",incant:"I call the Deep to create Cat o' Nine.",desc:"This spell is caster-only and requires the use of a 1-handed weapon with which the caster is proficient. The weapon must be held by the caster when the spell is cast. The spell turns the weapon into a spectral cat o' nine tails whip. The weapon rep should be sheathed and is considered out of game for the duration of the spell. While the cat o' nine tails is active, packets may be thrown as a physical attack with the same damage and type as the underlying weapon, adding the prefix \"Physical\" to the call. For example, if the caster swung a weapon which did 3 Iron damage normally, the call would become \"Physical 3 Iron\". The packet may be blocked in the same way as any physical attack. This spell is stackable. With two stacks, the weapon will do Silver damage or, if it already did Silver or Magic damage, will do +1 damage. With three stacks, the weapon will do Magic damage or, if it already did Magic damage, will do +1 damage. Any additional stacks will increase the weapon damage by +1. The duration will always be equal to the original casting. Tagged skills and abilities, including other spells, cannot be used with the Cat o' Nine, nor can Criticals. The spell will end early if the caster takes Body damage, falls asleep or unconscious, or casts a spell other than Cat o' Nine."},
  {sphere:"Dredgecraft",level:6,name:"Curse of the Bloated Corpse",incant:"I call the Deep to inflict Curse of the Bloated Corpse.",desc:"The target of this curse feels their gut distend painfully as the fluids of death swell within. They take an immediate nausea effect, making them unable to run or use tagged skills for 10 minutes. The target may end their nausea by roleplaying vomiting for an uninterruptible 10 count. Further, for the hour after the target is cursed, if they enter their Death Count, their body will erupt with magical effluvial liquid and everyone within 5 ft will take 10 Magic damage. The target's Death Count continues normally afterwards."},
  {sphere:"Dredgecraft",level:7,name:"Curse of the Albatross",incant:"I call the Deep to inflict Curse of the Albatross.",desc:"This spell may be touch-cast on an object on the person of a willing target, or packet delivered otherwise. If the spell is packet delivered, the caster must declare the intended object after the incant, such as \"Sword, left hand\", and the object must be either a weapon or shield on the target's person. The targeted item is now linked to the curse and to the target person, who now has the Lesser Curse of the Albatross. While cursed, the targeted item is now spirit-linked to the targeted person and they will behave as if they had the skill Cold Dead Hands for that object only. If the object ever leaves their person, their maximum Body is reduced to 2. If the object is returned to them, their maximum Body goes back to normal, but they are not healed for the difference. The curse will end early if the object is destroyed."},
  {sphere:"Dredgecraft",level:7,name:"Hornswoggle",incant:"I call the Deep to grant Hornswoggle.",desc:"If the caster hears a miscant which is not saved by Tenacity, including of a spell they themselves cast, they may cast Hornswoggle within 1 minute. This allows the caster of the miscanted spell to refresh 1 memorised spell already cast from memory, up to and including 7th circle spells. If the miscant came from the Deep caster themselves, they can only refresh a spell of a circle up to the circle of the miscanted spell, up to 7. This spell cannot be refreshed by itself."},
  {sphere:"Dredgecraft",level:8,name:"Curse of the Coward",incant:"I call the Deep to inflict Curse of the Coward.",desc:"The target of this spell gains the Lesser Curse of the Coward, cursing them with a reluctance to fight which causes their hands to numb at the prospect of battle. The target takes a chill effect, rendering them unable to use their hands to wield weapons or cast magic until they perform a 10 second count to warm them up. The chill effect can be resisted as either a cold effect or a fear effect. This part of the curse will end after 10 minutes if the target does not take the time to warm their hands up. For the full duration of the curse, the target's Strength is reduced by 2, which lowers their weapon damage by -1 (to a minimum of 1) and they cannot willingly be the first to swing a weapon or cast a spell which would start a fight."},
  {sphere:"Dredgecraft",level:8,name:"Keelhaul",incant:"I call the Deep to inflict Keelhaul. 10 Magic Body Stun!",desc:"This spell will cause magical ropes to appear in the target's mind, dragging them under the keel of an illusionary ship so real that the target can feel the scrape of the barnacles and the stabbing of splintered wood, dealing them 10 Magic Body and stunning the target for 5 seconds as they are trapped in the illusion."},
  {sphere:"Dredgecraft",level:9,name:"Curse of the Black Spot *",incant:"I call the Deep to grant Curse of the Black Spot.",desc:"This spell will protect the caster with a Lesser contingency curse. If the caster enters their Bleed Count or Death Count via a weapon strike or spell, the attacker will be inflicted with the Curse of the Black Spot. As soon as possible, they should phys-rep the black spot on the back of the hand which was holding the weapon or casting the spell that struck down the caster. The spot and curse last until the cursed character dies or the curse is removed. Those suffering from the Curse of the Black Spot take 1 Magic damage each time they swing, block, or use an active skill with the hand with the spot on it and they cannot cast through that hand. This effect does not stack."},
  {sphere:"Dredgecraft",level:9,name:"Watery Grave",incant:"I call the Deep to inflict Watery Grave.",desc:"This spell causes the target to plunge into the ground beneath their feet as though it were the sea itself and they find themselves in the inky black of the ocean deep, surrounded by a crushing emptiness. Nothing has ever felt so vast, empty, and smothering as this does. The target goes out of game for 1 minute as they have been engulfed by the deep. After 1 minute, they will reappear in the same location but, unless they can breathe water or do not need to breathe, they will return in their Death Count if they weren't already."},
  // Light
  {sphere:"Light",level:1,name:"Bless *",incant:"I channel <God> to grant Blessing.",desc:"This spell calls down upon the target the blessing of whichever God the caster worships. If the caster casts Bless on themselves, it will function as a Shield Magic versus the next Divine or Draconic Battle Magic spell to strike the caster. From time to time a character with a Bless on their spirit may find favour with the God(dess) that the caster serves. This can sometimes, decided by a Shaper, have a small positive effect happen to or around them. This could be anything from a small warning of danger to minor healing or even minor miracles. The caster may not force a Bless upon a person and it may be resisted without using up a spell-protection, such as Shield Magic. One can only be Blessed if one chooses to be and only one Bless can be active at a time. A person can choose to allow a new Bless spell to replace an old one if they wish. They may also end a Bless on themselves any time they choose, but this may offend the god."},
  {sphere:"Light",level:1,name:"Illumination",incant:"I channel <God> to create Illumination.",desc:"This spell will create a light source, so long as it is cast on any small object of no larger than 6x6x6 cubic inches in area. The spell will last for 12 hours, until it is dispelled, or until the caster wishes to terminate the light. A flashlight may be used, but the light produced must be diffused significantly using a gel or cloth so that there is no directional beam. An out-of-game, luminescent, physical representation is required for this spell to be used as a light source. If desired, this spell may be used offensively. If cast via spell packet or touch cast on a target, it will blind the target for 10 seconds, so long as it is a creature that relies on sight. It will have no effect on creatures that do not, such as golems, Undead and slimes."},
  {sphere:"Light",level:2,name:"Divine Ward",incant:"I channel <God> to create Divine Ward.",desc:"Divine Ward requires the caster to plant or otherwise display their holy symbol foci for the duration of the spell. During this time, the symbol may not be used to cast other Light spells. The symbol does not have to remain on the person of the caster, and in fact may be hung upon a door, placed upon a tree or otherwise, so long as it remains stationary. Placing the spell tag next to the symbol is encouraged. While the symbol is being used in this way, creatures possessing a spirit may not approach within 10 feet of the symbol unless they are wearing a Bless spell of the deity represented by the Divine Ward. When the spell is cast, anyone not wearing a Bless spell of the appropriate deity will be pushed out of the Ward. If a creature already in the Ward cannot retreat any further, the spell will fail and is lost. This barrier may be resisted with Shield Magic, Resist Magic or similar anti-magic defenses spell, and it may also be resisted by expending an active Bless spell from any God or Goddess. Doing so makes the user immune to the effects of this Divine Ward for 10 minutes. If the symbol is physically moved the spell ends. The caster of Divine Ward is immune to the effects of the spell."},
  {sphere:"Light",level:2,name:"Pin Evil",incant:"I channel <God> to inflict Pin Evil.",desc:"This spell has two effects. Firstly, the spell will release the target from any binding effect which pins the target's foot to the ground and requires +2 or lower Strength to rip free from. The second effect works only against Lesser Undead and Lesser Demons. When cast, it will cause the target to keep one foot on the ground, unable to move. The creature may rip free on a 3-count if they have +5 or greater Strength. Ripping free will cause them to take 5 Magic Body damage."},
  {sphere:"Light",level:3,name:"Mass: Blessings",incant:"I channel <God> to grant Mass Blessing.",desc:"This area-of-effect spell requires the caster to give a powerful Mass to their flock, calling on their God to bless those that the caster touches. To start Mass: Blessings the caster must actively roleplay a sermon to their God speaking to those present about their deity's tenets, beliefs and how they relate to the situation at hand, for one minute. After that minute has passed they may then, while continuing their sermon, touch the foreheads of any who have heard it. One person may be touched in this manner every 10 seconds so long as the sermon continues or the maximum duration of 10 minutes is reached. Each person who is touched by the caster in this manner will take the effect of a Bless spell. A maximum of 10 Blessings may be granted. Each person may only receive one Blessing per Mass. The caster may not \"force\" the effects of this mass to take place upon anyone, including the unconscious, dying, or otherwise incapacitated."},
  {sphere:"Light",level:3,name:"Wave of Healing",incant:"I channel <God> to grant Wave of Healing, Wave of Healing, Wave of Healing.",desc:"The caster must plant both feet and then cast this spell. They may then do 5 Magic Healing via packet, touch cast, or a combination, up to five times. If the target has a Bless from the same God as the caster, the healing is raised to 10 Magic Healing. Each Healing call must be preceded by the phrase \"Wave of Healing\". If the caster moves either foot or is struck for damage to Body, any remaining Healing is lost."},
  {sphere:"Light",level:4,name:"Banner of the Faithful",incant:"I channel <God> to create Banner of the Faithful.",desc:"This spell creates a magic \"flag\" or banner which lasts one hour's time. During that time, any character that has a Bless spell of the same God on their spirit may gain access to the Banner's full abilities. The Blessed character must touch the Banner and speak the God's name. Once done, they may attack for +0 Magic damage so long as the Banner stays within their line of sight. This bonus includes ranged weapons. The flag is considered a non-spirited item with 1 Body and may be destroyed by any weapon damage, Acid, or Elemental damage. Anyone holding the Banner will take whatever damage it takes. If the banner leaves the target's line of sight for more than 10 seconds, the effect is lost until the Banner is back in their line of sight. The banner must be visible as well, which means that it may be necessary to illuminate a banner used in the dark. A Banner may be any shape so long as it is a minimum 2.5' x 1' and no greater than 4'x 6' and must be mounted on a pole with a minimum length of 4' and a maximum of 6'. The holy symbol of the God worshipped must be represented on the Banner. When the banner is first created, the caster must state \"Banner up - <God's name>!\". When the banner ends for any reason, the caster must then state, \"Banner down - <God's name>!\". The caster of Banner of the Faithful is always under the Banner's effect while it exists."},
  {sphere:"Light",level:4,name:"Freedom",incant:"I channel <God> to grant Freedom.",desc:"This spell is an area effect spell that will function on all targets within hearing range who wear a Bless of the same God as the caster. It grants three benefits: 1) it will release the targets from any magical or alchemical (but not physical) bindings instantly, 2) it will awaken sleeping targets and 3) it will remove any active stun effects. If a target chooses to be affected by Freedom, it will end their active Bless spell."},
  {sphere:"Light",level:5,name:"Destroy Lesser Undead",incant:"I channel <God> to inflict Destroy Lesser Undead.",desc:"This packet delivered attack spell will cause 50 points of Magic damage to Greater Undead and will destroy lesser Undead outright."},
  {sphere:"Light",level:5,name:"Mass: Relic",incant:"I channel <God> to grant Relic.",desc:"This 10 minute mass magically enhances an item, typically a weapon, in the name of the God of the caster. Once the mass is complete, the object or weapon is made rendered as per the spell and is given a Magic aura. The weapon or object will become attuned to the first creature bearing the Bless of the caster's God that touches it after the mass is completed. If the item is dropped by the attuned creature or passed off to another creature, the spell ends and the item will revert back to its normal form. The effects on the object last for 24 hours, starting at the completion of the mass."},
  {sphere:"Light",level:6,name:"Dark Lore",incant:"I channel <God> to grant Dark Lore.",desc:"This spell allows the caster to beseech a lost spirit who served their God in life and ask a series of questions. Sprits summoned in this manner will arrive as soon as they possibly can but no later than 12 hours after casting. During this waiting time, the caster should attempt to find a Shaper at their earliest convenience. The first few questions are set and must be spoken verbatim after the spirit arrives. These questions are: \"Spirit before me, I ask that you identify yourself.\" \"I bring you no ill will; do you wish my spirit harm?\" \"I seek the knowledge in death regarding <Subject>.\" \"I release you of your binding, you are free to go. Will you leave peacefully?\" OR \"I release you of your binding but request additional information if it pleases you. Will you stay?\" If the caster fails or incorrectly speaks these questions, the spirit may not arrive or may arrive hostile. If they succeed, the spirit is bound to answer truthfully, to the best of its knowledge, those four questions. After this point the caster may continue asking questions of the spirit if the spirit is willing. The limit of questions is random, generally depending on the demeanor and sensitivity of the caster toward the spirit. Some spirits are simply uninterested in speaking to the living and will leave after the required questions are answered. The quality of answers will greatly depend upon the spirit called which, in general terms, is beyond the ability of the caster's control. The use of Dark Lore is not considered Necromantic in nature."},
  {sphere:"Light",level:6,name:"Shield of Light",incant:"I channel <God> to create Shield of Light.",desc:"This spell will summon into being a shield. While in existence, this shield will act as a normal metal shield, granting the caster the ability to use it. If the shield is hit by a packet delivered Dark, Draconic, Necromancy or Wytch spell, it will act like a Shield Magic once. The caster may not determine when to use the Shield Magic capabilities; it will simply react to the first spell of the spheres listed that strike it directly. The shield will NOT act as a Shield Magic if it is not directly hit by the spell or if the spell is not from one of the spheres listed. If the shield is dropped by the caster or they are rendered unconscious or incapacitated, the shield will dissipate and the spell will end. The shield may be used with natural weaponry like Savar'Aving Claws."},
  {sphere:"Light",level:7,name:"Beacon of Light *",incant:"I channel <God> to grant Beacon of Light.",desc:"The next time the target of this spell enters their Bleed or Death Count, a light will hover over their body until they are restored to life or their spirit departs to resurrect. The player may represent this with a liquid light or LED light and may state out \"Visible Beacon of Light\" in a normal speaking voice no more than once every 10 seconds. The player must remain where they are. They cannot sit or stand unless lying down would be unsafe. The light cannot be covered. It will shine through any attempts to hide it."},
  {sphere:"Light",level:7,name:"Light Bolt",incant:"I channel <God> to inflict Light Bolt. 20 Light!",desc:"This spell causes a bolt of light to spring from the caster's fingers toward the target. The spell will take full effect on Undead creatures and living creatures alike. The bolt does 20 points of Light damage straight to Body. This damage will be halved if the target has any active Bless on their person."},
  {sphere:"Light",level:8,name:"Holy Warrior",incant:"I channel <God> to summon a Holy Warrior.",desc:"This powerful spell will allow the Cleric to call upon their God to send forth a Holy Warrior to strike down one who has wronged the Cleric in some manner. The Cleric must offer up a sacrifice of a catalyst or an object worth at least 1 gold in value appropriate to the Cleric's god. Once cast, the offering is consumed and a being of pure light and energy will manifest before the Cleric within the next 12 hours. Once the Holy Warrior has arrived, the Cleric then needs to speak the name of the target as they know it, visualize the targets identity for one minute, and finally state how the target has wronged the Cleric or their God. During this count, the Holy Warrior cannot be the target of spells or effects, nor will they defend the Cleric or themselves until the spell prerequisites are completed. If the Cleric does not complete these requirements within two minutes of their arrival, the Holy Warrior will leave. If the requirements are met, this Holy Warrior will then dissipate, becoming undetectable to even the most powerful of magic. For the next hour the Holy Warrior will hunt the target, searching tirelessly and with the innate ability to sense that targets spirit at will. When the target is found, the Holy Warrior will phase in with a 3-count. It will state to the target that they have wronged a Cleric of <God> and that their life is forfeit. The Holy Warrior will attack that target to the best of its ability and will not cease until it is destroyed or that target has ended its Death Count. A Holy Warrior will be equal in level and power to the Cleric who is summoning it. Should the Cleric speak the True Name of the target to the Holy Warrior or use a Discord catalyst as the offering, that level increases to the Cleric's level +5. The Holy Warrior's Occupation is determined randomly by the God of the Cleric. Once the target has been destroyed the Holy Warrior will return to the Cleric and announce its success. Should the Cleric decide, after successfully casting the spell, that they made a mistake and wish to cancel the Holy Warrior's summoned duty, they may do so by expending their own bless spell. Ending the spell in this manner will incur a very harsh repercussion. As punishment for risking the life of an innocent the Cleric will find themselves the target of their own Holy Warrior. No creature may be the target of this spell by the same Cleric, more than once per month nor will the Holy Warrior attack any creature that carries a Bless of the Cleric's God. The Holy Warrior is a Celestial creature."},
  {sphere:"Light",level:8,name:"Tooth for a Tooth",incant:"I channel <God> to grant Tooth for a Tooth.",desc:"For 10 minutes after this spell has been cast, the Cleric may activate the spell to reflect the next 3 weapon, packet or touch-cast effects or attacks which strike them by stating \"Activate Tooth for a Tooth\". This will function for 3 effects in a row from the time the spell is activated, and then will end. The caster will still take the effect of these effects, but so will the attacker. The Cleric must state \"Tooth for a Tooth Reflect!\" for each of the 3 effects individually. The Cleric cannot activate the spell as a reaction to an attack which has hit them. The tag for this spell should not be destroyed until the duration expires. At any time after the spell has been activated, the Cleric may choose to bestow one of the 3 reflects onto a target individual who has a Bless of the same God. The duration is the same as the Cleric's original duration; however long the Cleric has left is the duration of the target. This will allow the target to reflect the next effect which hits them as per the normal effect of Tooth for a Tooth. Accepting one of the uses will expend the target's Bless. A target who is not the Cleric may have only a single use at a time."},
  {sphere:"Light",level:9,name:"Avatar",incant:"I channel <God> to grant Avatar.",desc:"This spell turns the Cleric into an \"Avatar\" of their deity, morphing their Body into a glowing light form on a 3-count. After the spell is cast, the caster's body will pulse energy and they must state \"Active Avatar\" out-of-game to anyone who sees them. This spell will also summon into existence either a two-handed Light melee weapon or a one-handed Light melee weapon and shield. The two-handed Light weapon has a base damage of 10 Magic, while the one-handed weapon's base damage is 5 Magic. The shield has a 60 Magic threshold. The spell also grants the proficiency in Exotic Weapon: Light <Weapon> and the Shield skill, as long as they are holding the summoned weapons. The Cleric can choose which weapon combination they would like at the time of casting. In Avatar form, the Cleric also has the ability to Spellstrike 10 Light through their summoned weapon of choice a total of three times. They also gain a temporary health boost of 50 Body. Any Body Damage the Cleric receives is removed from the bonus 50 Body points first and this Body cannot be healed. The weapons and/or shield will instantly dissipate if the Cleric drops it, is rendered unconscious, or incapacitated. Summoned weapons may be used with natural weaponry like Savar'Aving Claws. The Cleric may not cast any spells while in Avatar form. When the Avatar ends, the Cleric will perform a 3-count to exit the form."},
  {sphere:"Light",level:9,name:"Cleansing Light",incant:"I channel <God> to grant Cleansing Light.",desc:"This spell will act as a Life spell, with a couple of exceptions. Cleansing Light does not share Life's restriction on casting only on targets in their Death Count. It can be cast on a person with just a single point of Body Damage or one in their Bleed Count or Death Count and each would receive its full benefit. This spell also places a Bless of the Cleric's deity upon the recipient, if they desire it."},
  // Necromancy
  {sphere:"Necromancy",level:1,name:"Black Plague",incant:"I invoke Necromancy to inflict Black Plague.",desc:"The spell will inflict the victim with a magic plague. The target cannot run, is sickened with disease, and should role-play accordingly. The target can only heal up to 1 Body, no matter the source of healing, until the disease is cured. If the target is over 1 Body when plagued, any additional healing attempted will have no effect. The duration of this effect is 5 days. While active, the victim will slowly bleed from the eyes, nose, ears and mouth."},
  {sphere:"Necromancy",level:1,name:"Feign Death",incant:"I invoke Necromancy to grant Feign Death.",desc:"This spell makes the caster appear to be dead (final death). The spell will fool all skills, abilities and spells that relate to determining the health status of the target or detecting the living. The caster may choose to end the spell at any time during the duration. This spell is caster only."},
  {sphere:"Necromancy",level:2,name:"Control Lesser Undead",incant:"I invoke Necromancy to inflict Control Lesser Undead.",desc:"This spell will temporarily over-ride any existing control over a lesser Undead. For one hour, that Undead will obey all commands of the necromancer, including suicide. Commands must be simple, such as \"Defend me!\", \"Kill them!\" or \"Don't allow anyone to pass\". At the end of the hour the control fades."},
  {sphere:"Necromancy",level:2,name:"Leech",incant:"I invoke Necromancy to inflict Leech. 10 Body Drain!",desc:"This spell will transfer 10 Body from any lesser Undead to the caster via Mending. The caster does not need to be in control of the Undead for it to function. Any Body that exceeds the caster's maximum Body points grants them temporary Body points equal to the excess, up to a maximum of double the caster's original Body points. Temporary Body points gained from this ability lasts 1 hour. Lesser Undead will not notice its casting and will not respond as if it had been the target of a hostile spell, however Leech will still activate defenses on the target such as Resist Magic and Shield Magic. If a defense is activated, the Undead will respond as if the caster attacked them."},
  {sphere:"Necromancy",level:3,name:"Necrotic Bolt",incant:"I invoke Necromancy to inflict Necrotic Bolt. 5 Infliction!",desc:"This purple and black bolt of raw infliction energy does 5 points of Infliction damage to the target. This bolt will heal Undead by 5 points, but not past their current maximum Body point total. The Bolt will deal x2 damage (10) directly to the Body of any living target it strikes."},
  {sphere:"Necromancy",level:3,name:"Wake the Dead",incant:"I invoke Necromancy to inflict Wake the Dead.",desc:"This spell must be cast on a target still within its Death Count. If successful, the caster will be able to bend the corpse's spirit to their will for a short time and force it to answer a single question. This is extremely painful for the spirit as it is twisted and forced into its dead body. The spirit may be unwilling but is forced to answer as if affected by a Charm effect. The spell will not force the target to tell the truth or reveal secrets, unless it is already in their nature to do so to their best friend. While someone is affected by Wake the Dead, their Death Count will continue and they may be Lifed as normal. The target of this spell will not remember the interaction. This spell will fail if used on a target who is Manifesting or whose soul is more than 10 ft from their body."},
  {sphere:"Necromancy",level:4,name:"Carnivorous Worms",incant:"I invoke Necromancy to inflict Carnivorous Worms.",desc:"This spell shoots forth a wriggling mass of necrotic worms at the target. The magic worms immediately dig themselves into the skin of the target, chewing and eating as they go. The spell can be resisted by effects that resist diseases. The worms eat the target from the outside, dealing 1 Magic Body damage per minute. Damage begins 1 minute after the target is struck by the spell. The target will suffer from -2 Strength immediately. The only way to remove the worms is by removing the disease via magic or a Physician, Dispel Magic or entering one's Death Count. A Physician cannot pause the damage while removing the disease. This spell can be stacked. If the target enters their Death Count while this spell is active, the caster can eat the worms to mend themselves 5 Body. The worms can be consumed up to 1 minute after the target's body dissipates. If the target dissipates to resurrect, the worms will still infest the clothing and belongings they left behind for 1 minute. Should anyone besides the caster touch the worms after the original target enters their Death Count, they too will be infected with Carnivorous Worms. The target should stay there, out of game, for this minute to marshal any possible infections. If the spell was stacked, anyone else who is infected receives the stacked version. If the target receives a Life effect during their Death Count, the worms will be killed."},
  {sphere:"Necromancy",level:4,name:"Vampiric Blade",incant:"I Invoke Necromancy to create a Vampiric Blade.",desc:"This spell summons a magic dagger (purple) that gleams with Necrotic energy. The weapon deals \"1 Magic Body Drain\" and Mends the caster for the equivalent amount of damage dealt. Any Body that exceeds the caster's maximum Body points grants them temporary Body points equal to the excess. Temporary Body points gained from this ability lasts 1 hour. This Temporary Body, like all Temporary Body, does not stack. In order to Mend the wielder, Body damage must be done with the strike. This damage cannot be increased or augmented by any means and no skills may be used with the blade. The dagger, if wielded by someone other than the caster, or if it's dropped, disarmed, or dispelled will dissipate. The caster is responsible for bringing their own purple dagger phys-rep; the spell will fail without the proper rep."},
  {sphere:"Necromancy",level:5,name:"Fracture",incant:"I invoke Necromancy to Fracture your <limb>",desc:"Fracture will cause a limb of the caster's choice (arm or leg) to break and become useless. If the caster does not specify which limb is to be broken, then the victim is free to choose. The broken limb may be used for nothing, not even locomotion. On humanoids, arms or legs count as limbs although pincers, tentacles etc. qualify as limbs on many other creatures. This spell can be countered by Restore Limb, but not Dispel Magic, or may be treated with non-magical means such as medical skills."},
  {sphere:"Necromancy",level:5,name:"Raise Skeleton",incant:"I invoke Necromancy to Raise a Skeleton.",desc:"This spell must be cast on a target still within its Death Count. If successful, it will raise a mindless Mortal Lesser Skeleton under the control of the caster. The control over the Undead is absolute, including self-destructive orders, and must be simple one sentence commands given by the caster. Any new commands will override the last. Though mindless, the Skeleton is empowered by this spell, and can fight effectively. It can wield weapons and wear armour to augment its capabilities. This special Skeleton is a Physical Undead with 40 Body, +2 Strength, Undead State, and a +0 Magic Threshold. It swings all weapons for base \"2 Magic\" or \"2 Magic Body\" if it is using a Body weapon. After one hour, the Skeleton will turn to dust and the spell's target will depart to resurrect. While the target is raised as a Skeleton, their Death Count will continue. If the Skeleton is reduced to 0 Body during the target's Death Count, they may receive a Life effect as normal. Otherwise, the target must resurrect as normal. Because of the nature of this spell, the target can't choose to resurrect as an Undead."},
  {sphere:"Necromancy",level:6,name:"Enhance Undead",incant:"I invoke Necromancy to grant Enhance Undead.",desc:"This spell, when cast on an Undead, will grant it +4 Strength and one Lesser Resist Magic. It will mend the Undead up to 50 Body. It will have no effect on targets that are not lesser Undead. This enhancement will last as long as the Undead does."},
  {sphere:"Necromancy",level:6,name:"Necrotic Blast",incant:"I invoke Necromancy to inflict Necrotic Blast. 10 Infliction!",desc:"This purple and black bolt of raw infliction magic does 10 points of Infliction damage to the target."},
  {sphere:"Necromancy",level:7,name:"Death's Grasp",incant:"I Invoke Necromancy to inflict Death's Grasp.",desc:"After casting this spell and successfully striking, the Necromancer must hold his arm toward the target, make a fist and concentrate on maintaining the spell. The target struck is immediately affected by a Garrotte attack that can only be countered by interrupting the caster by dealing Body damage, casting a Dispel Magic on the necromancer or target, or the target breaking out of the spell with +2 or greater Strength. The caster must keep his arm forward for the entire duration (20 seconds) and count the Garrotte attack as if they were using the skill (Garrotte 1, Garrotte 2 ...). If 20 seconds pass, the target has been killing-blowed and enters their Death Count. The spell will succeed even if the target is wearing a gorget."},
  {sphere:"Necromancy",level:7,name:"Raise Netherwisp",incant:"I invoke Necromancy to Raise a Netherwisp.",desc:"This spell must be cast on a target still within its Death Count. If successful, it will create a semi-incorporeal Lesser Undead Netherwisp under the control of the caster. The target's body remains where it is but will now require two Life effects to take it out of its Death Count. The target is immune to further castings of Raise Netherwisp for the next hour. The Netherwisp takes on a skeletal or wraith-like form of the Necromancer's choosing, no bigger than a housecat. While the spell is active the Netherwisp must be represented by a doll or stuffed toy appropriate to this appearance. The Netherwisp has high animal intelligence. It is Spirit Linked to the Necromancer, senses as both Undead and Necromancy, cannot speak or make any sound, has no Spirit, and cannot die unless the Necromancer themselves dies and resurrects. Although it has no Body Points and cannot be physically harmed via numerical damage, it can be affected by magic that targets Lesser Undead such as Destroy Undead effects and barriers which bar entry to Undead. If the Necromancer avoids resurrection via the Requiem spell, the Netherwisp reappears with them. Only one Netherwisp may be active at a time. The caster may choose to end the spell at any time before it automatically ends after 5 days."},
  {sphere:"Necromancy",level:8,name:"Unlife",incant:"I invoke Necromancy to grant Unlife.",desc:"This spell will temporarily infuse the caster's spirit with necromancy, granting them Undead style abilities. The caster does not become genuinely Undead. It can only be cast between the hours of 6 PM - 6 AM. The caster gains the following: Healed via Infliction magic; x4 Magic Body damage from Healing, regardless of Sphere (this is not considered a racial vulnerability); +0 Magic Threshold; Immune to all poisons, diseases, and alchemy/chemistry, with the exception of Acid damage, Sticky Paste, Rusting Dust, and any alchemy/chemistry that can be applied to a weapon to increase its damage; Immune to Charm and Sleep Effects but not mind altering effects such as Paralysis or Ego Whip; Immune to physical effects that target vital organs, such as Execute, Vital Blow, Disembowel, etc., but not external body parts such as Hamstring, Dismember, Decapitate, etc.; No spells or abilities that specifically target Undead will function on them, except Control Greater Undead which will act like a Charm spell; Senses as Undead and not as Living, as well as sensing as Necromancy; Most mindless Lesser Undead will ignore them if no hostile action is taken against them; The caster will be recognizable as an Undead version of themselves. The caster can end the spell at any time, but if they are under the effect of Control Greater Undead, they can only end the spell if directed to."},
  {sphere:"Necromancy",level:8,name:"Walk the Deadlands",incant:"I invoke Necromancy to grant Walk the Deadlands.",desc:"In order for this spell to function the Necromancer must killing blow themselves and enter a five minute Death Count. During those five minutes, the Necromancer gains the Mysticism skill \"Manifest\" with one single exception - they are not anchored to their corpse. Able to walk freely in the Deadlands, the player must use an orange glowstick to represent their altered status. They are invisible to mortal eyes while in this state unless seen by a Mystic with the Dead Sight ability. While in the Deadlands the necromancer's corpse remains in the mortal plane, slowly dying. Everything in the mortal plane will be visible to them and they can hear sounds as well. No physical or magical barriers may stop them unless that barrier is specifically designed to stop ghosts or Undead. However, while in the Deadlands, nothing on the mortal plane can be manipulated and all sounds the Necromancer makes will not be heard by the living. If the necromancer returns to their corpse's location and ends the spell before the five minutes expire, the body will gasp and shudder, returning to life with 2 Body points but suffering no other ill effect. If for whatever reason the necromancer does not or cannot return to their corpse before the spell ends their spirit becomes lost in the Deadlands and they must resurrect. The Death Count during this ability will last for five minutes regardless of race and nothing will extend it or stop the Necromancer from resurrecting if they do not return in time."},
  {sphere:"Necromancy",level:9,name:"Requiem",incant:"I invoke Necromancy to grant Requiem.",desc:"In order to prepare this spell, the Necromancer must do 1 Body point of damage to themselves and spill their blood on the ground in a small circle. The spell is then cast with one foot inside that circle and remains on the necromancer for one hour. During that hour, if the Necromancer's spirit leaves their body through death via any means, their body will explode into maggots and worms. Instead of resurrecting they will appear at the circle of blood without having taken a death. For 10 minutes the Necromancer will remain unconscious and vulnerable with 1 Body point. If the Necromancer is moved away from the circle of blood, they will enter their Death Count and only a Life effect will revive them. At the end of the 10 minutes they will awaken with 2 Body. Items will not travel with the necromancer; they remain behind as if they had been slain. The player must write the time that the Requiem was cast on its spell tag."},
  {sphere:"Necromancy",level:9,name:"Wasting Death",incant:"I Invoke Necromancy to inflict Wasting Death. 50 Infliction!",desc:"This powerful necromantic spell causes the target to suffer 50 Infliction damage. If this puts the target into their Bleed Count, they instead skip their Bleed Count and immediately enter their Death Count."},
  // Sigil
  {sphere:"Sigil",level:1,name:"Sigil of Rest",incant:"I craft a Sigil of Rest.",desc:"Once this Sigil is cast, the target must rest unmoving for one minute. After that time they are affected by \"2 Healing\" and a full restore of all lost Stamina points. If the target moves, is moved or takes additional Body damage, the spell will end."},
  {sphere:"Sigil",level:1,name:"Sigil of Shock",incant:"I craft a Sigil of Shock.",desc:"Once activated this Sigil will allow its wearer to touch cast \"1 Magic Lightning!\" damage once every 10 seconds, for a period of 10 minutes. This magic slowly builds up a charge its wearer's hands and cannot be used more than once every 10 seconds, nor can it be packet-delivered. It cannot be combined with other skills or spells, including hand to hand damage. If less than 1 minute has passed since activating Sigil of Shock, the wearer can expend the remainder of the Sigil to Spellstrike 10 Magic Lightning once."},
  {sphere:"Sigil",level:2,name:"Sigil of Armour",incant:"I craft a Sigil of Armour.",desc:"This Sigil will reduce all incoming damage by 1 from all sources, to a minimum of 1. This damage reduction will only apply to damage done to armour points, it does not reduce incoming body damage. This Sigil can be drawn multiple times to reduce the damage further but requires a separate casting for each reduction of 1. There can be no more than five active Sigils of Armour on any one person. This reduction applies before any thresholds."},
  {sphere:"Sigil",level:2,name:"Sigil of Bravery *",incant:"I craft a Sigil of Bravery.",desc:"This Sigil will protect its wearer from Fear effects. If struck with such an attack, the Sigil wearer may declare \"Sigil: Bravery!\" and take no effect. The Sigil will vanish when used."},
  {sphere:"Sigil",level:3,name:"Sigil of the Forge",incant:"I craft a Sigil of the Forge.",desc:"This Sigil will instantly repair 10 armour points worn by the target at the time of casting. Every minute after casting, it will repair an additional 10 armour points until the target reaches full armour points, takes a single point of damage to their armour, or 10 minutes pass. It will also mend Gargylen at the same rate a basic Blacksmith would, for up to 10 minutes, but will end if the target takes any damage or falls into their Bleed count."},
  {sphere:"Sigil",level:3,name:"Sigil of the Pocket *",incant:"I craft a Sigil of the Pocket.",desc:"This Sigil acts like a magic pocket with a size of at most 6x6x3 inches. Items touching this Sigil will vanish into it. It can hold no more than a normal sized pouch and if the Sigil is dispelled or the duration expires, the items will appear at the feet of the caster. If an item does not fit into the pouch, nothing will happen. The caster must possess an OOG pouch and write \"SIGIL POCKET\" on the outside. All items placed into the Sigil Pocket must be placed into the OOG pouch. Items inside a Sigil Pocket cannot be sensed. Only one pouch can be active at a time."},
  {sphere:"Sigil",level:4,name:"Sigil of the Barrier *",incant:"I craft a Sigil of the Barrier.",desc:"Once cast, this Sigil will reduce the incoming damage done by the next single crossbow bolt, arrow, thrown weapon, or numerical packet-delivered physical attack. When they are struck with such an effect, the Sigil wearer states \"Minimize!\" The Sigil will vanish when used."},
  {sphere:"Sigil",level:4,name:"Sigil of the Bound Man",incant:"I craft a Sigil of the Bound Man.",desc:"Once the Sigil is drawn and the spell is cast, the target's arms are held stiffly behind their backs as if tied. The caster may command them to sit, stand, and walk as directed. They may not make the target run and cannot make them walk over a cliff or into an environmental condition that will damage them/kill them. They could, however, make them walk up a gallows, or in front of an executioner's block. This is a charm effect and can be resisted as such. When the caster casts the spell, the target may choose to use any spell defenses or resistances they may have. If attacked or damaged in any way, the spell will end."},
  {sphere:"Sigil",level:5,name:"Sigil of the Lizard",incant:"I craft a Sigil of the Lizard.",desc:"This Sigil will restore all severed and fractured limbs after the target rests quietly for five minutes. Once the Sigil is drawn and the spell is cast, the target must rest for five minutes. During that time, they cannot use any skills, cannot defend themselves, or move farther than 10 feet from the spot it was activated. After that time, they will heal 5 Body and all lost or fractured limbs will be restored. If the target is not affected by healing magic (like a Gargylen) but still affected by restore limb, then the restore limb effect will still take place."},
  {sphere:"Sigil",level:5,name:"Sigil of the Weapon Master",incant:"I craft a Sigil of the Weapon Master.",desc:"This Sigil will grant its wearer the weapon proficiency skill of the weapon that is drawn as the Sigil, with the exception of Exotic weapons. If its wearer already possesses the weapon skill the Sigil will grant +1 damage instead. A second stack will allow the wearer to pick either an extra +1 damage, or cause the weapon to swing for Silver damage for the duration. A third stack will allow the wearer to pick either an extra +1 damage, or cause the weapon to swing for Magic damage for the duration. Even if the weapon is already silver or the wearer already has the weapon proficiency, no stack step may be skipped. This spell may be stacked a maximum of three times. This spell will not create a weapon, merely grant proficiency."},
  {sphere:"Sigil",level:6,name:"Sigil of Flechette",incant:"I craft a Sigil of Flechette.",desc:"Once active, this Sigil allows its wearer to touch the Sigil and draw forth up to three magical throwing weapons. They do not all need to be drawn forth at the same time. These summoned weapons do 10 Magic Body each and dissipate upon impact. Purchasing an Exotic Weapon Specialization: Summoned Weapons will increase the damage of the Flechettes by 1 per purchase. No other means will augment the damage. Weapon reps for Sigil of Fletchette can be any thrown type and should be blue in colour to indicate they cannot be picked up once thrown."},
  {sphere:"Sigil",level:6,name:"Sigil of Inversion *",incant:"I craft a Sigil of Inversion.",desc:"This Sigil will reverse the next non-divine or non-Draconic damaging spell or magical effect to hit the target's Body and turn it into Mending appropriate for the wearer's race. This effect triggers whenever the effect would hit Body (even partially) on the Sigil bearer but will not if it only damages armour. Eg: if the Sigil wearer was a Gargylen who wore 15 points of armour, or none at all, and was hit by an Elemental Strike, instead of taking 25 points of Magic damage, the full 25 points of damage would be converted to Mending because at least some of the damage hit to Body points. This spell can be stacked with other magical protections such as Shield Magic and, if it is, the wearer may decide which activates first. When this Sigil is used its wearer must state \"Sigil Inversion!\""},
  {sphere:"Sigil",level:7,name:"Sigil of Dispel",incant:"I craft a Sigil of Dispel.",desc:"This Sigil will function as a Dispel Magic spell and will terminate any spell of ninth level or lower, unless specifically stated otherwise in the description. All active spells are lost. Magic items that contain Battle Magic spells, potions extended by Sweetwater and Battle Magic scrolls are inoperative for 10 minutes. Sigil of Dispel has no effect on ritual magic."},
  {sphere:"Sigil",level:7,name:"Sigil of Hatred",incant:"I craft a Sigil of Hatred.",desc:"For the duration of this spell, the Sigil wearer will do +2 Magic damage to members of the racial group drawn. If a member of this race performs a Killing Blow on the Sigil wearer, they will take a \"Sigil Contingency: Magic Death\" on the second to last second of the Killing Blow. The racial group will be one of the following: Angels/Demons, Animals, Bestial, Brood, Constructs, Draconic, Dwarves, Elementals, Elves, Fae, Goblinoids, Humanoids, Magical Beasts, Plants, Spirit, Undead (excluding vampires), Vermin. This Sigil will not stack with itself."},
  {sphere:"Sigil",level:8,name:"Sigil of Delay *",incant:"I craft a Sigil of Delay.",desc:"Upon being hit by an instantaneous Battle Magic spell effect, the wearer may declare \"Sigil of Delay!\" and postpone the spell's effect for 1 minute. Once the full minute has passed, the effect carries on as normal. Any new protective spells gained in this minute will resolve before the delayed effect if applicable. While a spell is stored, a Dispel Magic may be cast on the Sigil to dispel both the Sigil as well as the captured spell."},
  {sphere:"Sigil",level:8,name:"Sigil of Warding",incant:"I craft a Sigil of Warding.",desc:"This Sigil must be drawn on the arm where it is intended to be used. If that arm becomes dismembered, the Sigil will end. This spell allows the wearer of the Sigil to use the selected arm from the elbow down as a shield, negating all physical damage from melee weapon strikes that strike the arm between the wrist and elbow. Grabbing weapons will still inflict Body damage. Damage greater than 30 will break through the Sigil, causing the Sigil to end and the wearer to take the full damage of that strike. While active, the wearer's forearm will glow blue and the wearer must state \"Active Warding\" to those that see them. The wearer may wear a bracer on the selected arm, as long as the Sigil is visible as well. The selected arm's hand may still be used for other activities, like wielding a weapon or spellcasting, while this Sigil is active."},
  {sphere:"Sigil",level:9,name:"Sigil of Magical Storage",incant:"I craft a Sigil of Magical Storage.",desc:"When this Sigil is activated, for the next 10 minutes it will absorb the first spell that is touch-cast on the Sigil itself. This spell will then be available for the Sigil wearer to use for 24 hours. Any spell levels 1 to 9 from Sigil or any core rulebook sphere can be absorbed in this fashion and the wearer simply needs to state \"Activate Sigil: <Spell Name>\". The spell operates like normal and the Sigil wearer is considered to be the caster. When this Sigil absorbs a spell that spell is considered to have been cast and is lost from the caster's memory. Only one spell can be absorbed per Sigil of Magical Storage and only one of these Sigils can be active on any one person at a time. Spells absorbed with this sigil will fail if the target already possesses an active version on their spirit. Eg: You cannot store a Magic Armour spell if you are wearing an active Magic Armour."},
  {sphere:"Sigil",level:9,name:"Sigil of the Phoenix *",incant:"I craft a Sigil of the Phoenix.",desc:"While active, this Sigil will have one of two possible effects: 1) This Sigil can be activated to allow its wearer to swing for 5 Magic Fire with any weapon they are holding for 60 seconds. Activating the Sigil in this manner will also heal its wearer of all lost Body points, remove all toxins, restore all limbs, remove any charms and dispel any negative magical effects on their spirit. It will not cleanse ritual magic or toxins with specific antidotes. 2) If the wearer of this Sigil falls into their Bleed Count, the Sigil will immediately activate granting the same bonus as #1 including the full healing. This effect will also activate automatically during the final \"count\" of a killing blow. Eg: If the killing blow is a 10 second version, it will activate at the 10th second. When either of these uses are activated the wearer must state \"Sigil: Phoenix!\". Once one of the effects is activated, the Sigil ends."},
  // Wytchcraft
  {sphere:"Wytchcraft",level:1,name:"Blood Curse",incant:"I summon a Hex to inflict a Blood Curse.",desc:"A Wytch in possession of your blood is a terrible thing indeed. A Wytch with both your blood and True Name is something beyond terror. Once this spell is cast on a target, any additional spells cast on the same target will allow the Wytch to Echo the spell if the Wytch knows their True Name. This Echo effect will allow the caster to strike the target an additional time with the same spell if the first spell was successfully defended against in any way. This is done by calling \"Echo!\" immediately after the spell was defended against. This second spell happens automatically and does not require the Wytch to expend a spell slot. This Echo effect continues to occur for every spell cast by the Wytch on the target until the curse is removed. Blood Curse is a Lesser Curse. In addition, if the Wytch possesses one liter of the target's blood and has it on their person, any spells cast on the target of a Blood Curse will gain the Penetrating prefix - allowing the spell to ignore all non-ritual protections, all non-racial defenses and all armour. Doing so will consume one liter of the target's blood for each use of Penetration. Penetration may be combined with the Echo effect above, but may only be used once per liter of blood possessed. The blood may be obtained prior to casting the spells and follows standard blood rules."},
  {sphere:"Wytchcraft",level:1,name:"Talisman *",incant:"I summon a Hex to create a Talisman.",desc:"This spell allows the Wytch to create a protective talisman out of any item that could be worn as jewellery. While being worn, this talisman grants the target 5 points of Magical Armour and wards the bearer against certain evil spirits. This armour cannot be repaired but can stack with other physical or Magical Armour. The talisman is not destroyed when the armour is used up, but the magical effect on it dissipates. This talisman can be worn or given freely by the Wytch. Multiple castings of this spell cannot be stacked on the same item at the same time. Multiple talismans may be worn at the same time and the Magical Armour will stack. The Player must attach this spell tag to the item after casting. Once the Magical Armour is consumed, the tag is to be destroyed."},
  {sphere:"Wytchcraft",level:2,name:"Blindness",incant:"I summon a Hex to inflict Blindness.",desc:"With spit and malice, a Wytch may cause the target's eyes to grow milky white, filling with cataracts. With a successful attack, the Wytch causes blindness in the target. This will blind the target for ten seconds, forcing the target to close their eyes OOG for the duration of the effect. Players in an unsafe or unstable environment (e.g. fighting near a fire pit) may keep their eyes open, but must look down at their feet and away from their attacker for the skill's duration."},
  {sphere:"Wytchcraft",level:2,name:"Curse of Evil Eye",incant:"I summon a Hex to inflict Curse of Evil Eye. Power Word: Directed <Target>.",desc:"One of the Wytch's most feared powers is the Evil Eye. With a glance, the Wytch can cause terrible luck in some and despair in others. By staring intensely at a target, the Wytch can curse those with misfortune causing them to take an additional point of damage from all sources directed at them. This additional damage is counted by the Wytch for all sources of damage regardless of source or where it strikes. In order to use this spell the Wytch must be able to see the target, although it is not necessary that the target see the Wytch. The Wytch must then incant the spell and point at the target. Although no spell packet is required to be thrown, once the incant and point has been completed, the target is considered to be stuck by a packet automatically. Evil Eye does not require a spell packet to use. Curse of Evil Eye is a Lesser Curse."},
  {sphere:"Wytchcraft",level:3,name:"Repulsion",incant:"I summon a Hex to inflict Repulsion <item>.",desc:"This spell attacks the target's mind, and forces them to believe that an item they are holding becomes a writhing pile of maggots, worms, and bugs. If successful, this spell will cause a target to drop the item identified in the incant and retreat away from it at least ten feet. Nothing short of a Dispel Magic will force a target to believe otherwise. The target cannot be forced to touch the item and will defend himself to the best of his abilities to maintain his distance. Repulsion is considered a Fear effect and can be resisted as such, along with standard anti-magical defenses."},
  {sphere:"Wytchcraft",level:3,name:"Curse of Weakness",incant:"I summon a Hex to inflict Curse of Weakness.",desc:"This spell will penetrate a victim's muscles and bones, making them weak and feeble. Weakness will sap the strength from a target causing a loss of -8 Strength, which lowers the target's weapon swings by -4 (to a minimum of 1). This effect can be stacked with multiple castings. Curse of Weakness is a Lesser Curse."},
  {sphere:"Wytchcraft",level:4,name:"Horror",incant:"I summon a Hex to inflict Horror.",desc:"This fear-based spell influences the mind of the target, causing it to view the Wytch as hideous and offensive, causing the target to avoid the Wytch at all costs. Under the effect of Horror, the target may not come within ten feet of the Wytch and, while aware the Wytch is there, will not attack the Wytch for any reason. If the Wytch approaches the target, the target will retreat if possible. If no retreat is possible, the spell is not broken, but the target will move away at the next opportunity. If the Wytch takes any hostile gesture toward the target, such as attacking them or casting spells at them, the spell will end."},
  {sphere:"Wytchcraft",level:4,name:"Requital",incant:"I summon a Hex to grant Requital.",desc:"This spell allows the Wytch to draw life energy from a distant source and use it to heal themselves. By casting this spell, the Wytch can Mend themself of all missing Body points. However, doing so has a cost: every casting negatively affects the local area the Wytch is in. A mother may deliver a stillborn baby, a calf may die, a hailstorm may destroy some crops, etc. The actual effect is decided by plot and likely unknown to the Wytch. The negative effect will never be one that gives irrefutable proof that the Wytch is at fault. All castings of this spell must be reported to a plot member the next time they see one. It is not necessary to go out of game for this."},
  {sphere:"Wytchcraft",level:5,name:"Contingency: Sleep *",incant:"I summon a Hex to create a Contingency Sleep.",desc:"This spell allows the Wytch to imbue any non-magical object with a powerful sleep enchantment. This enchantment will activate when a set contingency happens. At that point, the target of the contingency will be affected by a magical sleep. The call for contingency activating is \"Wytchcraft Contingency: Sleep\". This sleep spell will drop the target into a deep slumber for the duration of 10 minutes. They will not snore. The victim can be woken via Dispel Magic, Body damage or one minute of vigorous shaking. The condition of the contingency is decided by the Wytch upon casting. Only one contingency condition may be set on the item and that condition must be activated by a creature touching the item and possessing a spirit. The condition may not exceed ten words and must involve the item being damaged, destroyed or consumed in some manner. Once activated, the contingency is used up and must be cast again on the item."},
  {sphere:"Wytchcraft",level:5,name:"Curse of Tongue Rot",incant:"I summon a Hex to inflict Curse of Tongue Rot.",desc:"This powerful Lesser Curse will cause the victim's tongue to rot in their mouth, dissolving into a disgusting black chunky liquid. The target takes one Magic Body and is silenced. If the damage is negated the target will not be silenced and the spell will fail."},
  {sphere:"Wytchcraft",level:6,name:"Eye for an Eye *",incant:"I summon a Hex to grant Eye for an Eye.",desc:"This spell envelops the Wytch in a pulsing black aura which will duplicate any physical attack and its damage, along with its effects (if any) back onto the target that struck the Wytch, once. The damage type duplicated on the attacker will always be \"Normal\" damage regardless of the damage type the attacker used, though Body damage will be returned as Body damage. Eg: If the attacker strikes with Wytch with \"10 Magic Body\", they will receive \"10 Normal Body\" reflected back at them, regardless of the attacker's armour points. Eye for an Eye is considered an Advanced Defense, meaning that it may be used at any time the Wytch chooses and does not automatically activate on the first strike. Even though the damage is duplicated back to the target, the Wytch will still take the damage and effects of the attack by default, but may choose to defend against it like normal in hopes of negating it, if they so desire. This spell will not duplicate spells or abilities which do no physical damage. The source of the rebounded damage is considered to be the Wytch, not the person striking them. To use this spell, the Wytch must state clearly \"Eye for an Eye reflect!\". This spell is caster only."},
  {sphere:"Wytchcraft",level:6,name:"Trap Demonic / Angelic",incant:"I summon a Hex to create a Trap.",desc:"Tapping into their Demonic power, the Wytch can temporarily trap a Lesser Demonic or Angelic creature inside a circle of blood. After casting this spell, the Wytch has one minute to spill one Body Point worth of their own blood into the form of a circle. Once the circle is complete, the next Lesser Demonic or Angelic creature that steps or is summoned inside will be trapped for one hour's time. The creature will be unable to leave the circle or cast/attack through the circle. This spell gives no control over the trapped creature. Once a creature is successfully trapped, the Wytch has three options. 1) They may ask the Lesser Angel/Demon one question which the Angel/Demon must answer truthfully. Once answered, the spell immediately ends and the creature is released. 2) The Wytch may choose to banish the Angel/Demon, sending it back to its own plane of existence for 1 year. 3) The Wytch may choose to simply leave the Angel/Demon in the trap for the duration of the spell. Should the circle be crossed or breached by anything or anyone, the spell will end and anything trapped inside will be freed. The Wytch may drop this circle at any time. The circle perimeter must be represented by a rope or a similarly identifying prop."},
  {sphere:"Wytchcraft",level:7,name:"Control Lesser Demon / Angel",incant:"I summon a Hex to inflict Control Lesser Demon (or) Angel.",desc:"This spell grants the caster control over one Lesser Angel or Demon. For the hour, the target will do anything asked of it, including sacrificing itself. The specific abilities and limitations of command will depend upon the type of creature controlled. It has no effect against Greater Demons or Angels."},
  {sphere:"Wytchcraft",level:7,name:"Dark Entrails",incant:"I summon a Hex to grant Dark Entrails.",desc:"By digging through the entrails of a living being, the Wytch can gain insight into their own future. This spell requires a living creature with a spirit which is currently in their Bleed Count. After casting the spell, the Wytch has one minute to find a living creature that is in their Bleed Count. By digging through the flesh of the target's stomach, the Wytch can remove the entrails and glean from them a vision of the future. The act of reading takes ten seconds and will cause the target to enter their Death Count, bypassing their Bleed Count completely. For the next 5 days, the Wytch has one dodge which they may use to avoid any one attack. This dodge ability will have no effect on surprise or AOE (Area of Effect) attacks. The Wytch may not have more than one dodge on their spirit at a time. The defensive call is \"Dodge.\""},
  {sphere:"Wytchcraft",level:8,name:"Curse of Pain",incant:"I summon a Hex to inflict Penetrating Curse of Pain.",desc:"This spell is considered both a Penetrating spell as well as a Lesser Curse. For the duration of this spell, the target will take 5 Magic damage whenever they use a tag skill, or whenever they swing a weapon for damage. All other actions, such as blocking attacks with a shield, drinking potions or running away will not cause the damage to occur."},
  {sphere:"Wytchcraft",level:8,name:"Race Change: Toad",incant:"I summon a Hex to inflict Race Change: Toad.",desc:"This spell allows the Wytch to temporarily polymorph their target to that of an ugly, wart-covered toad. This polymorph is considered a temporary race change for the target. While in the form of a toad, the target may not use any skills or abilities. This includes any racial abilities they may have possessed in their previous form. The target toad has 5 Body and may only move by hopping. All items and clothing are polymorphed with the target and cannot be accessed until the spell has expired or the magic dispelled. Licking the toad will cause alchemical hallucinations effects similar to the Alchemy Hallucinoid. This spell will only work on creatures with a spirit and the creature may be no larger than an Ogre."},
  {sphere:"Wytchcraft",level:9,name:"Dark Pact",incant:"I summon a Hex to grant a Dark Pact.",desc:"With this spell, a Wytch tries to convince a dying target to strike a deal with the devil. If a target has entered their Death Count, the Wytch may cast this spell on their body. The spell itself offers to grant the target a Life spell in exchange for the target's full True Name. The decision to accept or deny this request is done by the target's spirit. The target may choose to deny the offer and continue on their way towards resurrection. If the target denies the offer, the spell slot is returned to the Wytch. If the target chooses to accept the offer, the target's True Name will be revealed to the Wytch and the target automatically. No deception can be made by the target as the spell binds them to speak the truth and only the Wytch can hear the target speak. Regardless of whether or not the target consciously knows their own True Name, their spirit always knows. If the target accepts the Pact, they know that the spell has been cast on them, but not who cast it. Once the name has been revealed, the target immediately takes the effect of a Life spell and is returned to the world of the living. Once Lifed, the target who accepted the Dark Pact must write their character's True Name on the Dark Pact spell tag and then sign it, out-of-game. This becomes the Wytch's proof that they know the name in-game. This spell will pause the target's Death Count for 30 seconds to give the target time to decide. The Wytch may only cast this spell on a particular target once every 24 hours."},
  {sphere:"Wytchcraft",level:9,name:"Shatter Your Skull",incant:"I summon a Hex to Shatter Your Skull.",desc:"This is perhaps most powerful Battle Magic spell in a Wytch's arsenal. By summoning the Demonic powers of the abyss, the Wytch is able to project a massive force of Demonic Magic capable of instantly shattering a target's skull. Once shattered, the target immediately drops into their Bleed Count, which will only last 10 seconds, regardless of how long their Bleed Count would normally last."},
];



// Spell builder state — prefixed sb_ to avoid collision with main builder state
let sbShowIncants = false;
let sbSelections = {}; // {"level-slot": "sphere|name"}

function openSpellBuilder(){
  // Pre-populate from character's purchased spheres and slot counts
  sbRenderSpheresBar();
  sbRenderTable();
  sbUpdateSummary();
  document.getElementById('spell-builder-overlay').style.display = 'flex';
}

function closeSpellBuilder(){
  document.getElementById('spell-builder-overlay').style.display = 'none';
}

function sbGetPrimaryAttunement(){
  return (s.elementalAttunements && s.elementalAttunements.length > 0) ? s.elementalAttunements[0] : null;
}

function sbResolveIncant(spell){
  if(spell.sphere !== 'Elemental') return spell.incant;
  const att = sbGetPrimaryAttunement();
  if(!att) return spell.incant;
  return spell.incant.replace(/<[Tt]ype>/g, att);
}

function sbGetSpheres(){
  // Read spheres from the main builder's state
  const spheres = new Set();
  if(s.s_school_1) spheres.add(s.s_school_1);
  if(s.s_school_2) spheres.add(s.s_school_2);
  if(s.s_school_3) spheres.add(s.s_school_3);
  return [...spheres];
}

function sbGetSlotCount(level){
  // Read from main builder's owned spell slots
  return s.owned.filter(o=>o._spellSlot && o._spellSlotLevel===level).length;
}

function sbRenderSpheresBar(){
  const spheres = sbGetSpheres();
  const el = document.getElementById('sb-spheres-display');
  if(!spheres.length){
    el.textContent = 'None — select spheres in the Magic panel';
    el.style.color = 'var(--color-text-tertiary)';
  } else {
    const atts = s.elementalAttunements && s.elementalAttunements.length ? ` <span style="font-size:10px;color:var(--color-text-tertiary)">[${s.elementalAttunements.join(', ')}]</span>` : '';
    el.innerHTML = spheres.map(sp=>`<span style="display:inline-block;padding:2px 10px;border-radius:100px;background:var(--color-background-tertiary);border:0.5px solid var(--color-border-secondary);font-size:11px;color:var(--color-text-primary);margin-right:4px">${sp}${sp==='Elemental'?atts:''}</span>`).join('');
  }
}

function sbToggleIncants(){
  sbShowIncants = !sbShowIncants;
  const btn = document.getElementById('sb-incant-btn');
  const th = document.getElementById('sb-incant-th');
  const cells = document.querySelectorAll('.sb-incant-cell');
  if(sbShowIncants){
    btn.textContent = '📜 Hide Incantations';
    btn.style.background = 'var(--color-background-info, #1a2a4a)';
    btn.style.color = 'var(--color-text-info, #85b7eb)';
    if(th) th.style.display = '';
    cells.forEach(c=>c.style.display='');
  } else {
    btn.textContent = '📜 Show Incantations';
    btn.style.background = 'var(--color-background-tertiary)';
    btn.style.color = 'var(--color-text-secondary)';
    if(th) th.style.display = 'none';
    cells.forEach(c=>c.style.display='none');
  }
}

function sbOnSpellSelect(level, slot, selectEl){
  const val = selectEl.value;
  const key = level+'-'+slot;
  if(val) sbSelections[key] = val;
  else delete sbSelections[key];
  // Update incant cell
  const incantCell = document.getElementById('sb-incant-'+level+'-'+slot);
  if(incantCell){
    if(val){
      const parts = val.split('|');
      const spell = SB_SPELLS.find(sp=>sp.sphere===parts[0]&&sp.name===parts[1]&&sp.level===level);
      incantCell.textContent = spell ? sbResolveIncant(spell) : '';
      // Update description panel
      sbShowDesc(spell);
    } else {
      incantCell.textContent = '';
      sbClearDesc();
    }
  }
  sbUpdateSummary();
}

function sbShowDesc(spell){
  if(!spell) { sbClearDesc(); return; }
  const panel = document.getElementById('sb-desc-content');
  if(!panel) return;
  const resolvedIncant = sbResolveIncant(spell);
  panel.innerHTML = `
    <div style="font-size:13px;font-weight:600;color:var(--color-text-primary);margin-bottom:2px">${spell.name}</div>
    <div style="font-size:10px;color:var(--color-text-tertiary);margin-bottom:8px">${spell.sphere} · ${ordinal(spell.level)} Circle</div>
    <div style="font-size:11px;color:var(--color-text-warning, #c9a84c);font-style:italic;margin-bottom:8px;padding:6px 8px;background:var(--color-background-tertiary);border-radius:4px;line-height:1.5">"${resolvedIncant}"</div>
    <div style="font-size:11px;color:var(--color-text-secondary);line-height:1.6">${spell.desc||'No description available.'}</div>
  `;
}

function sbClearDesc(){
  const panel = document.getElementById('sb-desc-content');
  if(panel) panel.innerHTML = '<span style="color:var(--color-text-tertiary);font-style:italic;font-size:12px">Select a spell from the table to see its description and incantation.</span>';
}

function sbRenderTable(){
  const spheres = sbGetSpheres();
  const tbody = document.getElementById('sb-body');
  const noMsg = document.getElementById('sb-no-sphere');
  const tableWrap = document.getElementById('sb-table-wrap');

  if(!spheres.length){
    noMsg.style.display = 'block';
    tableWrap.style.display = 'none';
    document.getElementById('sb-summary').style.display = 'none';
    tbody.innerHTML = '';
    return;
  }

  noMsg.style.display = 'none';
  tableWrap.style.display = 'block';

  let html = '';
  for(let lvl=1; lvl<=9; lvl++){
    const count = sbGetSlotCount(lvl);

    // Level header row
    const hasSlots = count > 0;
    html += `<tr style="background:var(--color-background-secondary);border-top:0.5px solid var(--color-border-secondary)">
      <td colspan="4" style="padding:6px 12px">
        <div style="display:flex;align-items:center;gap:10px">
          <span style="font-size:13px;font-weight:700;color:var(--color-text-warning, #c9a84c);min-width:60px">${ordinal(lvl)} Circle</span>
          <span style="font-size:11px;color:var(--color-text-tertiary)">${count} slot${count!==1?'s':''} available</span>
        </div>
      </td>
    </tr>`;

    if(!hasSlots){
      html += `<tr><td colspan="4" style="padding:6px 12px 8px;font-size:12px;color:var(--color-text-tertiary);font-style:italic">No slots at this level</td></tr>`;
      continue;
    }

    // Get available spells sorted by sphere then name
    const available = SB_SPELLS.filter(sp=>sp.level===lvl&&spheres.includes(sp.sphere));
    available.sort((a,b)=>a.sphere<b.sphere?-1:a.sphere>b.sphere?1:a.name.localeCompare(b.name));

    for(let slot=1; slot<=count; slot++){
      const key = lvl+'-'+slot;
      const savedVal = sbSelections[key]||'';
      // Validate saved selection still applies to current spheres
      let currentVal = '';
      if(savedVal){
        const parts = savedVal.split('|');
        if(available.some(sp=>sp.sphere===parts[0]&&sp.name===parts[1])) currentVal = savedVal;
        else delete sbSelections[key];
      }

      let opts = `<option value="">— Select spell —</option>`;
      let lastSphere = null;
      available.forEach(sp=>{
        if(sp.sphere !== lastSphere){
          opts += `<optgroup label="${sp.sphere}">`;
          lastSphere = sp.sphere;
        }
        const sel = (sp.sphere+'|'+sp.name===currentVal) ? ' selected' : '';
        opts += `<option value="${sp.sphere}|${sp.name}"${sel}>${sp.name}</option>`;
      });

      const incantText = (() => {
        if(!currentVal) return '';
        const parts = currentVal.split('|');
        const sp = SB_SPELLS.find(x=>x.sphere===parts[0]&&x.name===parts[1]&&x.level===lvl);
        return sp ? sbResolveIncant(sp) : '';
      })();

      const rowBg = slot%2===0 ? 'background:var(--color-background-secondary)' : '';
      html += `<tr style="${rowBg};border-bottom:0.5px solid var(--color-border-tertiary)">
        <td style="padding:6px 12px;text-align:center;font-size:13px;font-weight:700;color:var(--color-text-warning, #c9a84c)">${slot===1?lvl:''}</td>
        <td style="padding:6px 12px;text-align:center;font-size:12px;color:var(--color-text-tertiary)">${slot}</td>
        <td style="padding:5px 12px">
          <select onchange="sbOnSpellSelect(${lvl},${slot},this)"
            style="width:100%;padding:5px 8px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-sm, 4px);background:var(--color-background-secondary);color:var(--color-text-primary);font-family:var(--font-sans);font-size:12px;cursor:pointer">
            ${opts}
          </select>
        </td>
        <td id="sb-incant-${lvl}-${slot}" class="sb-incant-cell" style="${sbShowIncants?'':'display:none'};padding:6px 12px;font-size:11px;color:var(--color-text-tertiary);font-style:italic">${incantText}</td>
      </tr>`;
    }
  }

  tbody.innerHTML = html;
  // Keep incant header in sync
  const th = document.getElementById('sb-incant-th');
  if(th) th.style.display = sbShowIncants ? '' : 'none';
}

function sbUpdateSummary(){
  const spheres = sbGetSpheres();
  const panel = document.getElementById('sb-summary');
  const grid = document.getElementById('sb-summary-grid');
  if(!spheres.length){ panel.style.display='none'; return; }

  let hasAny = false;
  let html = '';
  for(let lvl=1; lvl<=9; lvl++){
    const count = sbGetSlotCount(lvl);
    if(!count) continue;
    const filled = [];
    for(let slot=1; slot<=count; slot++){
      const val = sbSelections[lvl+'-'+slot];
      if(val){
        const parts = val.split('|');
        const sp = SB_SPELLS.find(x=>x.sphere===parts[0]&&x.name===parts[1]&&x.level===lvl);
        if(sp) filled.push(sp);
      }
    }
    hasAny = true;
    const pct = Math.round(filled.length/count*100);
    html += `<div style="background:var(--color-background-secondary);border:0.5px solid var(--color-border-${filled.length===count?'secondary':'tertiary'});border-radius:var(--border-radius-md);padding:8px 12px">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:4px">
        <span style="font-size:12px;font-weight:600;color:var(--color-text-warning, #c9a84c)">${ordinal(lvl)} Circle</span>
        <span style="font-size:10px;color:${filled.length===count?'var(--color-text-success)':'var(--color-text-tertiary)'};background:var(--color-background-tertiary);padding:1px 7px;border-radius:100px">${filled.length}/${count}</span>
      </div>
      ${filled.length===0
        ? `<div style="font-size:11px;color:var(--color-text-tertiary);font-style:italic">No spells chosen</div>`
        : `<ul style="list-style:none;padding:0;margin:0">${filled.map(sp=>`<li style="font-size:11px;color:var(--color-text-primary);padding:1px 0;display:flex;justify-content:space-between;gap:6px;border-bottom:0.5px solid var(--color-border-tertiary)"><span>${sp.name}</span><span style="color:var(--color-text-tertiary);font-size:10px;white-space:nowrap">${sp.sphere}</span></li>`).join('')}</ul>`}
    </div>`;
  }

  panel.style.display = hasAny ? 'block' : 'none';
  grid.innerHTML = html;
}

function resetCharacter(){
  if(!confirm('Reset all character selections? This cannot be undone.')) return;
  s = { name:'', race:'', culture:'', occupation:'', vocation:'', blankets:0, owned:[], openCats:{General:false, 'Frag Skills':false, Production:false, Scholar:false, 'Scholar Class Frag Skills':false, Warrior:false, 'Warrior Class Frag Skills':false, Rogue:false, 'Rogue Class Frag Skills':false, Racial:false}, hovered:null, s_school_1:'', s_school_2:'', s_school_3:'', elementalAttunements:[] };
  // Reset all input elements
  const nm = document.getElementById('inp-name'); if(nm) nm.value = '';
  const bl = document.getElementById('inp-blankets'); if(bl) bl.value = '0';
  const rc = document.getElementById('sel-race'); if(rc) rc.value = '';
  const cu = document.getElementById('sel-culture'); if(cu) cu.value = '';
  const oc = document.getElementById('sel-occ'); if(oc) oc.value = '';
  const vo = document.getElementById('sel-voc'); if(vo) vo.value = '';
  // Reset detail panel
  const detail = document.getElementById('detail-panel');
  if(detail) detail.innerHTML = '<div class="detail-empty">Hover a skill to see details</div>';
  render();
}

render();
</script>

<div id="print-area"></div>
</body>
</html>
