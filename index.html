<!DOCTYPE html>
<html lang="ku" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="theme-color" content="#0f172a" />
  <title>MyCollege | College Management System</title>
  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-app-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore-compat.js"></script>
  <style>
    :root { --bg:#0b1120; --card:#111827; --card-2:#1e293b; --text:#f8fafc; --muted:#94a3b8; --accent:#38bdf8; --accent-2:#22c55e; --gold:#f59e0b; --silver:#cbd5e1; --bronze:#d97706; --danger:#ef4444; --border:rgba(148,163,184,0.18); --font-scale:1; }
    body.theme-light { --bg:#f1f5f9; --card:#ffffff; --card-2:#e2e8f0; --text:#0f172a; --muted:#475569; --accent:#0284c7; --accent-2:#16a34a; --gold:#d97706; --silver:#64748b; --bronze:#b45309; --danger:#dc2626; --border:rgba(15,23,42,0.14); }
    body.theme-gold { --bg:#090806; --card:#15120c; --card-2:#231e14; --text:#fef9c3; --muted:#cbb88a; --accent:#fbbf24; --accent-2:#34d399; --gold:#facc15; --silver:#e2e8f0; --bronze:#f59e0b; --danger:#f87171; --border:rgba(251,191,36,0.22); }
    * { box-sizing:border-box; margin:0; padding:0; font-family:system-ui,-apple-system,"Segoe UI",Tahoma,Arial,sans-serif; }
    body { background:var(--bg); color:var(--text); min-height:100vh; line-height:1.65; font-size:calc(16px * var(--font-scale)); transition:background .25s,color .25s; }
    header { background:color-mix(in srgb,var(--card) 92%,transparent); backdrop-filter:blur(12px); border-bottom:1px solid var(--border); padding:14px 20px; position:sticky; top:0; z-index:30; display:flex; flex-wrap:wrap; align-items:center; justify-content:space-between; gap:12px; }
    .brand-wrap { display:flex; flex-direction:column; gap:2px; }
    .brand { display:flex; align-items:center; gap:10px; font-weight:800; font-size:1.15em; color:var(--accent); }
    .brand-sub { font-size:.82em; color:var(--muted); }
    .controls, .nav-tabs, .row, .links-group { display:flex; flex-wrap:wrap; align-items:center; gap:8px; }
    select, input, textarea, button { background:var(--card-2); color:var(--text); border:1px solid var(--border); border-radius:10px; padding:9px 12px; font-size:.92em; outline:none; }
    select:focus, input:focus, textarea:focus { border-color:var(--accent); }
    button { cursor:pointer; font-weight:600; transition:.2s; }
    button.primary, .tab-btn.active { background:var(--accent); color:#061220; border:none; }
    button.success { background:var(--accent-2); color:#051b0d; border:none; }
    button.gold { background:var(--gold); color:#1a1203; border:none; }
    button.danger { background:var(--danger); color:#fff; border:none; }
    button.ghost { background:transparent; border:1px solid var(--border); }
    button:hover { opacity:.9; }
    .container { max-width:1140px; margin:22px auto; padding:0 16px 60px; display:grid; gap:20px; }
    .status-bar { display:flex; flex-wrap:wrap; justify-content:space-between; align-items:center; gap:10px; background:var(--card); border:1px solid var(--border); padding:12px 16px; border-radius:14px; font-size:.9em; }
    .badge { padding:4px 10px; border-radius:999px; font-size:.8em; font-weight:700; background:rgba(56,189,248,0.16); color:var(--accent); }
    .badge.live { background:rgba(34,197,94,0.18); color:var(--accent-2); }
    .grid-2 { display:grid; grid-template-columns:repeat(auto-fit,minmax(310px,1fr)); gap:18px; }
    .grid-3 { display:grid; grid-template-columns:repeat(auto-fit,minmax(270px,1fr)); gap:16px; }
    .stats-grid { display:grid; grid-template-columns:repeat(auto-fit,minmax(180px,1fr)); gap:12px; }
    .stat-box, .admin-subject-box, .top-student-card { background:var(--card-2); border:1px solid var(--border); border-radius:14px; padding:14px; display:flex; flex-direction:column; gap:8px; }
    .stat-num { font-size:1.35em; font-weight:800; color:var(--accent); }
    .card, .subject-card { background:var(--card); border:1px solid var(--border); border-radius:16px; padding:18px; display:flex; flex-direction:column; gap:12px; }
    .super-card { border:1px solid color-mix(in srgb,var(--accent) 45%,var(--border)); box-shadow:0 12px 30px rgba(0,0,0,0.18); }
    .card h2, .card h3, .card h4 { color:var(--accent); }
    .muted { color:var(--muted); font-size:.88em; }
    .item { background:var(--card-2); border:1px solid var(--border); border-radius:12px; padding:12px 14px; display:flex; justify-content:space-between; align-items:flex-start; gap:12px; }
    .item-title { font-weight:700; margin-bottom:4px; }
    .rank-1 { border-top:4px solid var(--gold); }
    .rank-2 { border-top:4px solid var(--silver); }
    .rank-3 { border-top:4px solid var(--bronze); }
    .rank-badge { align-self:flex-start; padding:3px 10px; border-radius:999px; font-size:.78em; font-weight:800; background:var(--card); color:var(--gold); border:1px solid var(--border); }
    .subject-header { display:flex; justify-content:space-between; align-items:center; gap:8px; border-bottom:1px solid var(--border); padding-bottom:8px; }
    .subject-num { font-size:.78em; font-weight:800; padding:3px 9px; border-radius:999px; background:var(--card-2); color:var(--accent); }
    .link-pill { display:inline-flex; align-items:center; gap:6px; text-decoration:none; padding:7px 12px; border-radius:10px; font-size:.85em; font-weight:700; background:var(--card-2); color:var(--text); border:1px solid var(--border); }
    .link-pill.pdf { border-color:rgba(56,189,248,0.45); color:var(--accent); }
    .link-pill.img { border-color:rgba(34,197,94,0.45); color:var(--accent-2); }
    .gpa-result { background:var(--card-2); border:1px solid var(--border); border-radius:12px; padding:12px; font-weight:700; }
    .hidden { display:none !important; }
  </style>
</head>
<body>
  <header>
    <div class="brand-wrap">
      <div class="brand"><span>🎓</span><span id="appTitle">MyCollege</span></div>
      <div class="brand-sub" id="headerMetaInfo">Live Firestore Sync</div>
    </div>
    <div class="controls">
      <select id="langSelect" aria-label="Language">
        <option value="ku">کوردی (بادینی)</option>
        <option value="ar">العربية</option>
        <option value="en">English</option>
      </select>
      <select id="roleSelect" aria-label="Role">
        <option value="student" id="optStudent">قوتابی (Student)</option>
        <option value="dept_admin" id="optDeptAdmin">ئەدمینێ بەشێ (Department Admin)</option>
        <option value="super_admin" id="optSuperAdmin">سوپەر ئەدمین (Super Admin)</option>
      </select>
      <input type="password" id="pinInput" class="hidden" placeholder="PIN" style="width:110px;" />
      <button id="unlockBtn" class="primary hidden">چوونە ژوور</button>
      <button id="logoutBtn" class="ghost hidden">دەرچوون</button>
    </div>
  </header>

  <main class="container">
    <div class="status-bar">
      <div><strong id="activeRoleLabel">دۆخێ نووکە: قوتابی (Student)</strong><span class="muted"> — Project: mycollege-b8a6c</span></div>
      <span id="syncStatus" class="badge live">Live Firestore Connected</span>
    </div>

    <div class="nav-tabs">
      <button class="tab-btn active" data-tab="subjectsTab" id="tabSubjectsBtn">٦ مادەیێن بەشی و یەکەمین قۆناغێ</button>
      <button class="tab-btn" data-tab="toolsTab" id="tabToolsBtn">ئامرازێن کۆلیژێ (College Tools)</button>
      <button class="tab-btn" data-tab="settingsTab" id="tabSettingsBtn">ڕێکخستنان (⚙️ Settings)</button>
    </div>

    <section id="adminPanel" class="card super-card hidden">
      <div class="row" style="justify-content:space-between;">
        <div>
          <h2 id="adminPanelTitle">پانێلا تایبەتا ڕێڤەبرنێ (Super Admin & Dept Admin)</h2>
          <p class="muted" id="adminPanelDesc">کۆنترۆڵا تەماما ٦ مادەیان، ٣ یەکەمێن قۆناغێ، زانیاریێن سەرپەرشتیار، و ئاگادارییان.</p>
        </div>
        <span class="badge" id="adminRoleBadge">Admin Unlocked</span>
      </div>

      <div class="stats-grid">
        <div class="stat-box"><span class="muted" id="statSubLabel">مادەیێن چالاک</span><span class="stat-num" id="statActiveSubjects">0 / 6</span></div>
        <div class="stat-box"><span class="muted" id="statAnnLabel">ئاگاداریێن بڵاڤکری</span><span class="stat-num" id="statAnnCount">0</span></div>
        <div class="stat-box"><span class="muted" id="statDeptLabel">تێبینی و بەش</span><span class="stat-num" id="statDeptCount">0</span></div>
        <div class="stat-box"><span class="muted" id="statHonorLabel">یەکەمێن تۆمارکری</span><span class="stat-num" id="statHonorCount">0 / 3</span></div>
      </div>

      <div class="card" style="background:var(--card-2);">
        <h3 id="metaInfoTitle">زانیاریێن سەرپەرشتیار و قۆناغێ</h3>
        <div class="grid-2">
          <input type="text" id="supervisorNameInput" placeholder="ناڤێ سەرپەرشتیار یان بەرپرسی" />
          <input type="text" id="stageLabelInput" placeholder="ناڤێ قۆناغ یان بەشی" />
        </div>
        <div class="row"><button id="saveMetaBtn" class="primary">هەڵگرتنا زانیاریێن سەرپەرشتیاری</button></div>
      </div>

      <div class="card" style="background:var(--card-2);">
        <h3 id="honorAdminTitle">پشتگیرییا قوتابیێن زیرەک (٣ یەکەمێن قۆناغێ)</h3>
        <p class="muted" id="honorAdminDesc">ناڤێ ٣ قوتابیێن یەکەم، تێکڕا، و پەیاما پشتگیریێ بنڤیسە:</p>
        <div id="adminHonorGrid" class="grid-3"></div>
        <div class="row"><button id="saveHonorBtn" class="gold">تۆمارکرنا ٣ یەکەمێن قۆناغێ</button></div>
      </div>

      <h3 id="sixSubjectsAdminTitle">رێکخستنا ٦ مادەیان (PDF & وێنە / تەسویر)</h3>
      <div id="adminSubjectsGrid" class="grid-3"></div>
      <div class="row"><button id="saveAllSubjectsBtn" class="success">تۆمارکرنا هەمی ٦ مادەیان</button></div>

      <hr style="border:0;border-top:1px solid var(--border);margin:4px 0;" />

      <div class="grid-2">
        <div class="card" style="background:var(--card-2);">
          <h3 id="addDeptTitle">زێدەکرنا بەش یان تێبینییەکا گشتی</h3>
          <input type="text" id="deptName" placeholder="ناڤێ بەشی یان تێبینییێ" />
          <input type="text" id="deptCode" placeholder="قۆناغ یان کۆد" />
          <button id="saveDeptBtn" class="success">تۆمارکرن</button>
        </div>
        <div class="card" style="background:var(--card-2);">
          <h3 id="addAnnTitle">بڵاڤکرنا ئاگادارییەکا نوو</h3>
          <input type="text" id="annTitle" placeholder="سەردێڕێ ئاگادارییێ" />
          <textarea id="annBody" rows="3" placeholder="ناڤەرۆکا ئاگادارییێ بنڤیسە..."></textarea>
          <button id="saveAnnBtn" class="primary">بڵاڤکرن</button>
        </div>
      </div>
    </section>

    <div id="subjectsTab" class="tab-content">
      <div class="card" style="margin-bottom:18px;">
        <h2 id="honorPublicTitle">🌟 ٣ یەکەمێن قۆناغێ و پشتگیرییا قوتابیێن زیرەک</h2>
        <p class="muted" id="honorPublicSub">پێزانین و هاندان بۆ قوتابیێن زیرەک و بەردەوام د خواندنێ دا.</p>
        <div id="honorDisplayGrid" class="grid-3"></div>
      </div>

      <div class="card" style="margin-bottom:18px;">
        <h2 id="sixSubjectsTitle">٦ مادەیێن بەشی (PDF & وێنە / تەسویر)</h2>
        <p class="muted" id="sixSubjectsSub">هەر مادەیەکێ فایلێن PDF و وێنەیێن خۆ ب جودا هەنە.</p>
        <div id="subjectsDisplayGrid" class="grid-3"></div>
      </div>

      <section class="grid-2">
        <div class="card"><h3 id="deptListTitle">بەش و زانیاریێن تۆمارکری</h3><div id="deptList" class="muted">...</div></div>
        <div class="card"><h3 id="annListTitle">ئاگاداریێن کۆلێژێ</h3><div id="annList" class="muted">...</div></div>
      </section>
    </div>

    <div id="toolsTab" class="tab-content hidden">
      <div class="grid-2">
        <div class="card">
          <h3 id="gpaTitle">هەژمارکەرێ تێکڕایێ ٦ مادەیان (Average / GPA)</h3>
          <p class="muted" id="gpaDesc">نمرەیێن خۆ یێن ٦ مادەیان (ژ ١٠٠) بنڤیسە:</p>
          <div id="gpaInputsGrid" class="grid-3"></div>
          <button id="calcGpaBtn" class="primary">هەژمارتنا تێکڕایێ</button>
          <div id="gpaOutput" class="gpa-result muted">تێکڕا: —</div>
        </div>
        <div class="card">
          <h3 id="countdownTitle">ژمێرەرێ دەمێ تاقیکرنێ (Exam Countdown)</h3>
          <p class="muted" id="countdownDesc">رۆژا تاقیکرنێ هەلبژێرە:</p>
          <input type="date" id="examDateInput" />
          <button id="calcCountdownBtn" class="gold">پشکنینا ڕۆژێن ماین</button>
          <div id="countdownOutput" class="gpa-result muted">هیشتا رۆژەک نەهاتییە هەلبژارتن.</div>
        </div>
        <div class="card">
          <h3 id="scheduleTitle">خشتەیێ وانەیێن هەفتانە (Weekly Schedule)</h3>
          <p class="muted" id="scheduleDesc">خشتەیێ خۆ یێ هەفتانە بنڤیسە:</p>
          <textarea id="scheduleText" rows="5"></textarea>
          <button id="saveScheduleBtn" class="success">هەڵگرتنا خشتەی</button>
        </div>
        <div class="card">
          <h3 id="notesTitle">تێبینییێن تایبەت (My Notes)</h3>
          <p class="muted" id="notesDesc">تێبینییێن خۆ یێن خواندنێ ل ڤێرە بنڤیسە:</p>
          <textarea id="personalNotesText" rows="5"></textarea>
          <button id="saveNotesBtn" class="primary">هەڵگرتنا تێبینییان</button>
        </div>
      </div>
    </div>

    <div id="settingsTab" class="tab-content hidden">
      <div class="grid-2">
        <div class="card">
          <h3 id="themeSettingTitle">ڕەنگ و شێوازێ شاشەی (Theme & Colors)</h3>
          <p class="muted" id="themeSettingDesc">رەنگێ گونجای بۆ چاڤێ خۆ هەلبژێرە:</p>
          <div class="row">
            <button class="ghost" id="btnThemeDark" onclick="setTheme('dark')">Midnight Blue</button>
            <button class="ghost" id="btnThemeLight" onclick="setTheme('light')">Clean Light</button>
            <button class="ghost" id="btnThemeGold" onclick="setTheme('gold')">Royal Gold & Dark</button>
          </div>
        </div>
        <div class="card">
          <h3 id="fontSettingTitle">قەبارەیێ نڤیسینێ (Font Size)</h3>
          <p class="muted" id="fontSettingDesc">قەبارەیێ نڤیسینێ ب گونجێنە:</p>
          <div class="row">
            <button class="ghost" id="btnFontSmall" onclick="setFontScale(0.92)">بچووک (Small)</button>
            <button class="ghost" id="btnFontNormal" onclick="setFontScale(1)">ئاسایی (Normal)</button>
            <button class="ghost" id="btnFontLarge" onclick="setFontScale(1.14)">مەزن (Large)</button>
          </div>
        </div>
      </div>
    </div>
  </main>

  <script>
    const firebaseConfig = {
      apiKey: "PASTE_YOUR_API_KEY_IF_NEEDED",
      authDomain: "mycollege-b8a6c.firebaseapp.com",
      projectId: "mycollege-b8a6c",
      storageBucket: "mycollege-b8a6c.firebasestorage.app",
      messagingSenderId: "1015075976026",
      appId: "PASTE_YOUR_APP_ID_IF_NEEDED"
    };
    if (!firebase.apps.length) firebase.initializeApp(firebaseConfig);
    const db = firebase.firestore();

    const SUPER_ADMIN_PIN = "8564";
    const DEPT_ADMIN_PIN = "4343";

    const i18n = {
      ku: {
        dir:"rtl", title:"MyCollege", student:"قوتابی (Student)", deptAdmin:"ئەدمینێ بەشێ (Department Admin)", superAdmin:"سوپەر ئەدمین (Super Admin)",
        pinPlaceholder:"کۆدێ PIN", unlock:"چوونە ژوور", logout:"دەرچوون", statusPrefix:"دۆخێ نووکە:",
        tabSubjects:"٦ مادەیێن بەشی و یەکەمین قۆناغێ", tabTools:"ئامرازێن کۆلیژێ (College Tools)", tabSettings:"ڕێکخستنان (⚙️ Settings)",
        adminTitle:"پانێلا تایبەتا ڕێڤەبرنێ (Super Admin & Dept Admin)", adminDesc:"کۆنترۆڵا تەماما ٦ مادەیان، ٣ یەکەمێن قۆناغێ، زانیاریێن سەرپەرشتیار، و ئاگادارییان.",
        statSubLabel:"مادەیێن چالاک", statAnnLabel:"ئاگاداریێن بڵاڤکری", statDeptLabel:"تێبینی و بەش", statHonorLabel:"یەکەمێن تۆمارکری",
        metaTitle:"زانیاریێن سەرپەرشتیار و قۆناغێ", supervisorPh:"ناڤێ سەرپەرشتیار یان بەرپرسی", stagePh:"ناڤێ قۆناغ یان بەشی", saveMeta:"هەڵگرتنا زانیاریێن سەرپەرشتیاری",
        honorAdminTitle:"پشتگیرییا قوتابیێن زیرەک (٣ یەکەمێن قۆناغێ)", honorAdminDesc:"ناڤێ ٣ قوتابیێن یەکەم، تێکڕا، و پەیاما پشتگیریێ بنڤیسە:", saveHonor:"تۆمارکرنا ٣ یەکەمێن قۆناغێ",
        honorPublicTitle:"🌟 ٣ یەکەمێن قۆناغێ و پشتگیرییا قوتابیێن زیرەک", honorPublicSub:"پێزانین و هاندان بۆ قوتابیێن زیرەک و بەردەوام د خواندنێ دا.",
        rankPrefix:"پلەیا", studentNamePh:"ناڤێ قوتابیێ زیرەک", scorePh:"تێکڕا یان پۆینت", supportMsgPh:"پەیاما پشتگیریێ...", noHonorEntry:"هیشتا ناڤێ قوتابی نەهاتییە تۆمارکرن.",
        sixSubjectsAdminTitle:"رێکخستنا ٦ مادەیان (PDF & وێنە / تەسویر)", saveAllSubjects:"تۆمارکرنا هەمی ٦ مادەیان",
        addDept:"زێدەکرنا بەش یان تێبینییەکا گشتی", deptNamePh:"ناڤێ بەشی یان تێبینییێ", deptCodePh:"قۆناغ یان کۆد", save:"تۆمارکرن",
        addAnn:"بڵاڤکرنا ئاگادارییەکا نوو", annTitlePh:"سەردێڕێ ئاگادارییێ", annBodyPh:"ناڤەرۆکا ئاگادارییێ بنڤیسە...", publish:"بڵاڤکرن",
        sixSubjectsTitle:"٦ مادەیێن بەشی (PDF & وێنە / تەسویر)", sixSubjectsSub:"هەر مادەیەکێ فایلێن PDF و وێنەیێن خۆ ب جودا هەنە.",
        deptList:"بەش و زانیاریێن تۆمارکری", annList:"ئاگاداریێن کۆلێژێ", delete:"ژێبرن", wrongPin:"کۆدێ PIN یێ خەڵەتە!", fillFields:"هیڤیە خانەیان پر بکە.", empty:"هیشتا چ داتا نەهاتینە تۆمارکرن.",
        subjectPrefix:"مادەیێ", subjectNamePh:"ناڤێ مادەیێ", pdfLinkPh:"لینکێ PDF", imgLinkPh:"لینکێ وێنەی", openPdf:"ڤەکرنا PDF", openImg:"بینینا وێنەی", noPdf:"PDF نینە", noImg:"وێنە نینە",
        savedSubjects:"هەمی ٦ مادە هاتنە تۆمارکرن!", savedHonor:"٣ یەکەمێن قۆناغێ هاتنە تۆمارکرن!", savedMeta:"زانیاریێن سەرپەرشتیاری هاتنە هەڵگرتن!",
        gpaTitle:"هەژمارکەرێ تێکڕایێ ٦ مادەیان (Average / GPA)", gpaDesc:"نمرەیێن خۆ یێن ٦ مادەیان (ژ ١٠٠) بنڤیسە:", calcGpaBtn:"هەژمارتنا تێکڕایێ",
        gpaDefault:"تێکڕا: —", gpaNoGrades:"هیچ نمرەیەک نەهاتییە نڤیسین.", gpaAvgText:(a,c)=>`تێکڕا: ${a}% (${c}/6 مادە)`,
        countdownTitle:"ژمێرەرێ دەمێ تاقیکرنێ (Exam Countdown)", countdownDesc:"رۆژا تاقیکرنێ هەلبژێرە:", calcCountdownBtn:"پشکنینا ڕۆژێن ماین",
        countdownDefault:"هیشتا رۆژەک نەهاتییە هەلبژارتن.", countdownPickDate:"هیڤیە رۆژەکێ هەلبژێرە.", countdownDaysLeft:(d)=>`${d} ڕۆژ ماینە بۆ تاقیکرنێ.`, countdownToday:"ئەڤرۆ رۆژا تاقیکرنێ یە!", countdownPassed:"ئەڤ مێژووە بوورییە.",
        scheduleTitle:"خشتەیێ وانەیێن هەفتانە", scheduleDesc:"خشتەیێ خۆ یێ هەفتانە بنڤیسە:", schedulePh:"ئێکشەممە: ...\nدووشەممە: ...", saveScheduleBtn:"هەڵگرتنا خشتەی", scheduleSaved:"خشتە هاتە هەڵگرتن.",
        notesTitle:"تێبینییێن تایبەت (My Notes)", notesDesc:"تێبینییێن خۆ بنڤیسە:", notesPh:"تێبینییێن خۆ ل ڤێرە بنڤیسە...", saveNotesBtn:"هەڵگرتنا تێبینییان", notesSaved:"تێبینییێن تە هاتنە هەڵگرتن.",
        themeSettingTitle:"ڕەنگ و شێوازێ شاشەی (Theme)", themeSettingDesc:"رەنگێ گونجای هەلبژێرە:", themeDark:"شینی شەڤێ (Midnight Blue)", themeLight:"ڕۆناهیا پاقژ (Clean Light)", themeGold:"زێڕین و تاری (Royal Gold)",
        fontSettingTitle:"قەبارەیێ نڤیسینێ (Font Size)", fontSettingDesc:"قەبارەیێ نڤیسینێ ب گونجێنە:", fontSmall:"بچووک (Small)", fontNormal:"ئاسایی (Normal)", fontLarge:"مەزن (Large)"
      },
      ar: {
        dir:"rtl", title:"MyCollege", student:"طالب (Student)", deptAdmin:"مسؤول القسم (Department Admin)", superAdmin:"المدير العام (Super Admin)",
        pinPlaceholder:"رمز PIN", unlock:"دخول", logout:"خروج", statusPrefix:"الحالة الحالية:",
        tabSubjects:"المواد الـ 6 وأوائل المرحلة", tabTools:"أدوات الكلية (College Tools)", tabSettings:"الإعدادات (⚙️ Settings)",
        adminTitle:"لوحة الإدارة المتقدمة (Super Admin & Dept Admin)", adminDesc:"تحكم كامل بالمواد الـ 6، أوائل المرحلة، بيانات المشرف، والإعلانات.",
        statSubLabel:"المواد النشطة", statAnnLabel:"الإعلانات المنشورة", statDeptLabel:"الأقسام والملاحظات", statHonorLabel:"الأوائل المسجلون",
        metaTitle:"بيانات المشرف والمرحلة", supervisorPh:"اسم المشرف أو المسؤول", stagePh:"اسم المرحلة أو القسم", saveMeta:"حفظ بيانات المشرف",
        honorAdminTitle:"دعم الطلاب المتفوقين (أوائل المرحلة الـ 3)", honorAdminDesc:"أدخل أسماء الطلاب الـ 3 المتفوقين، المعدل، ورسالة الدعم:", saveHonor:"حفظ أوائل المرحلة الـ 3",
        honorPublicTitle:"🌟 أوائل المرحلة ودعم الطلاب المتفوقين", honorPublicSub:"تكريم وتحفيز للطلبة المتميزين في مسيرتهم الدراسية.",
        rankPrefix:"المركز", studentNamePh:"اسم الطالب المتفوق", scorePh:"المعدل أو التقدير", supportMsgPh:"رسالة دعم أو تهنئة...", noHonorEntry:"لم يتم تسجيل اسم طالب بعد.",
        sixSubjectsAdminTitle:"إدارة المواد الـ 6 (PDF & صور)", saveAllSubjects:"حفظ جميع المواد الـ 6",
        addDept:"إضافة قسم أو ملاحظة عامة", deptNamePh:"اسم القسم أو الملاحظة", deptCodePh:"المرحلة أو الرمز", save:"حفظ",
        addAnn:"نشر إعلان جديد", annTitlePh:"عنوان الإعلان", annBodyPh:"اكتب نص الإعلان...", publish:"نشر",
        sixSubjectsTitle:"المواد الـ 6 للقسم (PDF & صور)", sixSubjectsSub:"كل مادة تحتوي على ملفات PDF وصور خاصة بها.",
        deptList:"الأقسام والمعلومات المسجلة", annList:"إعلانات الكلية", delete:"حذف", wrongPin:"رمز PIN غير صحيح!", fillFields:"يرجى ملء الحقول المطلوبة.", empty:"لا توجد بيانات مسجلة حتى الآن.",
        subjectPrefix:"المادة", subjectNamePh:"اسم المادة", pdfLinkPh:"رابط PDF", imgLinkPh:"رابط الصورة", openPdf:"فتح PDF", openImg:"عرض الصورة", noPdf:"لا يوجد PDF", noImg:"لا توجد صورة",
        savedSubjects:"تم حفظ جميع المواد الـ 6 بنجاح!", savedHonor:"تم حفظ أوائل المرحلة الـ 3!", savedMeta:"تم حفظ بيانات المشرف!",
        gpaTitle:"حاسبة معدل المواد الـ 6 (Average / GPA)", gpaDesc:"أدخل درجاتك للمواد الـ 6 (من 100):", calcGpaBtn:"حساب المعدل",
        gpaDefault:"المعدل: —", gpaNoGrades:"لم يتم إدخال أي درجة.", gpaAvgText:(a,c)=>`المعدل: ${a}% (${c}/6 مواد)`,
        countdownTitle:"عدّاد موعد الامتحان (Exam Countdown)", countdownDesc:"اختر تاريخ الامتحان:", calcCountdownBtn:"فحص الأيام المتبقية",
        countdownDefault:"لم يتم اختيار تاريخ بعد.", countdownPickDate:"يرجى اختيار تاريخ.", countdownDaysLeft:(d)=>`متبقي ${d} يوم على الامتحان.`, countdownToday:"اليوم موعد الامتحان!", countdownPassed:"هذا التاريخ قد مضى.",
        scheduleTitle:"الجدول الأسبوعي للمحاضرات", scheduleDesc:"اكتب جدولك الأسبوعي:", schedulePh:"الأحد: ...\nالإثنين: ...", saveScheduleBtn:"حفظ الجدول", scheduleSaved:"تم حفظ الجدول.",
        notesTitle:"ملاحظاتي الخاصة (My Notes)", notesDesc:"اكتب ملاحظاتك هنا:", notesPh:"اكتب ملاحظاتك هنا...", saveNotesBtn:"حفظ الملاحظات", notesSaved:"تم حفظ ملاحظاتك.",
        themeSettingTitle:"ألوان ومظهر الشاشة (Theme)", themeSettingDesc:"اختر المظهر المناسب:", themeDark:"أزرق ليلي (Midnight Blue)", themeLight:"فاتح نقي (Clean Light)", themeGold:"ذهبي داكن (Royal Gold)",
        fontSettingTitle:"حجم الخط (Font Size)", fontSettingDesc:"اضبط حجم الخط:", fontSmall:"صغير (Small)", fontNormal:"عادي (Normal)", fontLarge:"كبير (Large)"
      },
      en: {
        dir:"ltr", title:"MyCollege", student:"Student", deptAdmin:"Department Admin", superAdmin:"Super Admin",
        pinPlaceholder:"PIN", unlock:"Unlock", logout:"Logout", statusPrefix:"Active Role:",
        tabSubjects:"6 Subjects & Top 3 Honor Roll", tabTools:"College Tools", tabSettings:"Settings (⚙️)",
        adminTitle:"Enhanced Admin Control Center (Super Admin & Dept Admin)", adminDesc:"Full control over 6 subjects, Top 3 honor students, supervisor info, and announcements.",
        statSubLabel:"Active Subjects", statAnnLabel:"Published Notices", statDeptLabel:"Departments & Notes", statHonorLabel:"Honor Students",
        metaTitle:"Supervisor & Stage Info", supervisorPh:"Supervisor or coordinator name", stagePh:"Stage or department label", saveMeta:"Save Supervisor Info",
        honorAdminTitle:"Honor Students Support (Top 3 of Stage)", honorAdminDesc:"Enter top 3 students, score/note, and supportive message:", saveHonor:"Save Top 3 Honor Roll",
        honorPublicTitle:"🌟 Top 3 Stage Achievers & Student Support", honorPublicSub:"Recognition and encouragement for high-performing students.",
        rankPrefix:"Rank", studentNamePh:"Top student name", scorePh:"GPA / Score / Note", supportMsgPh:"Supportive message...", noHonorEntry:"No student recorded yet.",
        sixSubjectsAdminTitle:"6 Subjects Manager (PDF & Images)", saveAllSubjects:"Save All 6 Subjects",
        addDept:"Add Department or Note", deptNamePh:"Department or note name", deptCodePh:"Stage or Code", save:"Save",
        addAnn:"Publish Announcement", annTitlePh:"Announcement title", annBodyPh:"Write announcement details...", publish:"Publish",
        sixSubjectsTitle:"6 Department Subjects (PDF & Images)", sixSubjectsSub:"Each subject has dedicated PDF and image links.",
        deptList:"Registered Departments & Info", annList:"College Announcements", delete:"Delete", wrongPin:"Invalid PIN!", fillFields:"Please fill in the required fields.", empty:"No records found yet.",
        subjectPrefix:"Subject", subjectNamePh:"Subject name", pdfLinkPh:"PDF link", imgLinkPh:"Image link", openPdf:"Open PDF", openImg:"View Image", noPdf:"No PDF", noImg:"No image",
        savedSubjects:"All 6 subjects saved successfully!", savedHonor:"Top 3 honor roll saved!", savedMeta:"Supervisor info saved!",
        gpaTitle:"6-Subject Average / GPA Calculator", gpaDesc:"Enter your grades for the 6 subjects (out of 100):", calcGpaBtn:"Calculate Average",
        gpaDefault:"Average: —", gpaNoGrades:"No grades entered yet.", gpaAvgText:(a,c)=>`Average: ${a}% (${c}/6 subjects)`,
        countdownTitle:"Exam Countdown Timer", countdownDesc:"Select your exam date:", calcCountdownBtn:"Check Remaining Days",
        countdownDefault:"No date selected yet.", countdownPickDate:"Please select a date.", countdownDaysLeft:(d)=>`${d} days remaining until the exam.`, countdownToday:"The exam is today!", countdownPassed:"This date has passed.",
        scheduleTitle:"Weekly Class Schedule", scheduleDesc:"Write your weekly schedule:", schedulePh:"Sunday: ...\nMonday: ...", saveScheduleBtn:"Save Schedule", scheduleSaved:"Schedule saved.",
        notesTitle:"My Personal Notes", notesDesc:"Write your study notes here:", notesPh:"Write your notes here...", saveNotesBtn:"Save Notes", notesSaved:"Your notes have been saved.",
        themeSettingTitle:"Theme & Colors", themeSettingDesc:"Choose a visual theme:", themeDark:"Midnight Blue", themeLight:"Clean Light", themeGold:"Royal Gold & Dark",
        fontSettingTitle:"Font Size", fontSettingDesc:"Adjust text size:", fontSmall:"Small", fontNormal:"Normal", fontLarge:"Large"
      }
    };

    let currentLang = "ku", currentRole = "student", isAdminUnlocked = false;
    let subjectsData = Array.from({ length: 6 }, (_, i) => ({ index: i + 1, name: "", pdfUrl: "", imageUrl: "" }));
    let honorData = [{ rank: 1, name: "", score: "", message: "" }, { rank: 2, name: "", score: "", message: "" }, { rank: 3, name: "", score: "", message: "" }];
    let metaInfo = { supervisor: "", stage: "" };
    let cachedDepts = [], cachedAnns = [];

    const langSelect = document.getElementById("langSelect");
    const roleSelect = document.getElementById("roleSelect");
    const pinInput = document.getElementById("pinInput");
    const unlockBtn = document.getElementById("unlockBtn");
    const logoutBtn = document.getElementById("logoutBtn");
    const adminPanel = document.getElementById("adminPanel");

    function escapeHtml(s) {
      return String(s).replace(/&/g,"&amp;").replace(/</g,"&lt;").replace(/>/g,"&gt;").replace(/"/g,"&quot;");
    }

    function applyLanguage() {
      const t = i18n[currentLang];
      document.documentElement.lang = currentLang;
      document.documentElement.dir = t.dir;
      const mapText = {
        appTitle: t.title, optStudent: t.student, optDeptAdmin: t.deptAdmin, optSuperAdmin: t.superAdmin,
        unlockBtn: t.unlock, logoutBtn: t.logout, tabSubjectsBtn: t.tabSubjects, tabToolsBtn: t.tabTools,
        tabSettingsBtn: t.tabSettings, adminPanelTitle: t.adminTitle, adminPanelDesc: t.adminDesc,
        statSubLabel: t.statSubLabel, statAnnLabel: t.statAnnLabel, statDeptLabel: t.statDeptLabel,
        statHonorLabel: t.statHonorLabel, metaInfoTitle: t.metaTitle, saveMetaBtn: t.saveMeta,
        honorAdminTitle: t.honorAdminTitle, honorAdminDesc: t.honorAdminDesc, saveHonorBtn: t.saveHonor,
        honorPublicTitle: t.honorPublicTitle, honorPublicSub: t.honorPublicSub,
        sixSubjectsAdminTitle: t.sixSubjectsAdminTitle, saveAllSubjectsBtn: t.saveAllSubjects,
        addDeptTitle: t.addDept, saveDeptBtn: t.save, addAnnTitle: t.addAnn, saveAnnBtn: t.publish,
        sixSubjectsTitle: t.sixSubjectsTitle, sixSubjectsSub: t.sixSubjectsSub, deptListTitle: t.deptList,
        annListTitle: t.annList, gpaTitle: t.gpaTitle, gpaDesc: t.gpaDesc, calcGpaBtn: t.calcGpaBtn,
        countdownTitle: t.countdownTitle, countdownDesc: t.countdownDesc, calcCountdownBtn: t.calcCountdownBtn,
        scheduleTitle: t.scheduleTitle, scheduleDesc: t.scheduleDesc, saveScheduleBtn: t.saveScheduleBtn,
        notesTitle: t.notesTitle, notesDesc: t.notesDesc, saveNotesBtn: t.saveNotesBtn,
        themeSettingTitle: t.themeSettingTitle, themeSettingDesc: t.themeSettingDesc,
        btnThemeDark: t.themeDark, btnThemeLight: t.themeLight, btnThemeGold: t.themeGold,
        fontSettingTitle: t.fontSettingTitle, fontSettingDesc: t.fontSettingDesc,
        btnFontSmall: t.fontSmall, btnFontNormal: t.fontNormal, btnFontLarge: t.fontLarge
      };
      Object.entries(mapText).forEach(([id, val]) => { const el = document.getElementById(id); if (el) el.textContent = val; });

      pinInput.placeholder = t.pinPlaceholder;
      document.getElementById("supervisorNameInput").placeholder = t.supervisorPh;
      document.getElementById("stageLabelInput").placeholder = t.stagePh;
      document.getElementById("deptName").placeholder = t.deptNamePh;
      document.getElementById("deptCode").placeholder = t.deptCodePh;
      document.getElementById("annTitle").placeholder = t.annTitlePh;
      document.getElementById("annBody").placeholder = t.annBodyPh;
      document.getElementById("scheduleText").placeholder = t.schedulePh;
      document.getElementById("personalNotesText").placeholder = t.notesPh;

      if (!document.getElementById("gpaOutput").dataset.calculated) document.getElementById("gpaOutput").textContent = t.gpaDefault;
      if (!document.getElementById("countdownOutput").dataset.calculated) document.getElementById("countdownOutput").textContent = t.countdownDefault;

      updateHeaderMeta();
      updateRoleUI();
      renderHonorDisplay();
      renderAdminHonorForm();
      renderAdminSubjectsForm();
      renderSubjectsDisplay();
      renderGpaInputs();
      renderDepts();
      renderAnns();
      updateAdminStats();
    }

    function updateHeaderMeta() {
      const parts = [metaInfo.stage, metaInfo.supervisor].filter((x) => x && x.trim());
      document.getElementById("headerMetaInfo").textContent = parts.length ? parts.join(" • ") : "Live Firestore Sync";
    }

    function updateRoleUI() {
      const t = i18n[currentLang];
      const names = { student: t.student, dept_admin: t.deptAdmin, super_admin: t.superAdmin };
      document.getElementById("activeRoleLabel").textContent = `${t.statusPrefix} ${names[currentRole]}`;
      document.getElementById("adminRoleBadge").textContent = names[currentRole];
      if (currentRole === "student") {
        isAdminUnlocked = false;
        pinInput.classList.add("hidden"); unlockBtn.classList.add("hidden"); logoutBtn.classList.add("hidden"); adminPanel.classList.add("hidden");
      } else if (!isAdminUnlocked) {
        pinInput.classList.remove("hidden"); unlockBtn.classList.remove("hidden"); logoutBtn.classList.add("hidden"); adminPanel.classList.add("hidden");
      } else {
        pinInput.classList.add("hidden"); unlockBtn.classList.add("hidden"); logoutBtn.classList.remove("hidden"); adminPanel.classList.remove("hidden");
      }
    }

    langSelect.addEventListener("change", (e) => { currentLang = e.target.value; localStorage.setItem("mycollege_lang", currentLang); applyLanguage(); });
    roleSelect.addEventListener("change", (e) => { currentRole = e.target.value; if (currentRole === "student") isAdminUnlocked = false; updateRoleUI(); });

    unlockBtn.addEventListener("click", () => {
      const pin = pinInput.value.trim();
      if ((currentRole === "super_admin" && pin === SUPER_ADMIN_PIN) || (currentRole === "dept_admin" && pin === DEPT_ADMIN_PIN)) {
        isAdminUnlocked = true; pinInput.value = ""; updateRoleUI(); renderAdminHonorForm(); renderAdminSubjectsForm(); updateAdminStats(); renderDepts(); renderAnns();
      } else {
        alert(i18n[currentLang].wrongPin);
      }
    });

    logoutBtn.addEventListener("click", () => { isAdminUnlocked = false; currentRole = "student"; roleSelect.value = "student"; updateRoleUI(); renderDepts(); renderAnns(); });

    document.querySelectorAll(".tab-btn").forEach((btn) => {
      btn.addEventListener("click", () => {
        document.querySelectorAll(".tab-btn").forEach((b) => b.classList.remove("active"));
        document.querySelectorAll(".tab-content").forEach((c) => c.classList.add("hidden"));
        btn.classList.add("active");
        document.getElementById(btn.dataset.tab).classList.remove("hidden");
      });
    });

    function setTheme(mode) {
      document.body.classList.remove("theme-light", "theme-gold");
      if (mode === "light") document.body.classList.add("theme-light");
      if (mode === "gold") document.body.classList.add("theme-gold");
      localStorage.setItem("mycollege_theme", mode);
    }

    function setFontScale(scale) {
      document.documentElement.style.setProperty("--font-scale", String(scale));
      localStorage.setItem("mycollege_font_scale", String(scale));
    }

    document.getElementById("saveMetaBtn").addEventListener("click", async () => {
      if (!isAdminUnlocked) return;
      metaInfo = { supervisor: document.getElementById("supervisorNameInput").value.trim(), stage: document.getElementById("stageLabelInput").value.trim() };
      updateHeaderMeta();
      localStorage.setItem("mycollege_meta_info", JSON.stringify(metaInfo));
      try { await db.collection("college_config").doc("meta_info").set({ ...metaInfo, updatedAt: firebase.firestore.FieldValue.serverTimestamp() }); } catch (e) { console.error(e); }
      alert(i18n[currentLang].savedMeta);
    });

    db.collection("college_config").doc("meta_info").onSnapshot((doc) => {
      if (doc.exists) {
        metaInfo = { supervisor: doc.data().supervisor || "", stage: doc.data().stage || "" };
        localStorage.setItem("mycollege_meta_info", JSON.stringify(metaInfo));
        document.getElementById("supervisorNameInput").value = metaInfo.supervisor;
        document.getElementById("stageLabelInput").value = metaInfo.stage;
        updateHeaderMeta();
      }
    });

    function renderAdminHonorForm() {
      const t = i18n[currentLang], medals = ["🥇", "🥈", "🥉"];
      document.getElementById("adminHonorGrid").innerHTML = honorData.map((h, i) => `
        <div class="admin-subject-box">
          <strong>${medals[i]} ${t.rankPrefix} #${i + 1}</strong>
          <input type="text" id="honorName_${i}" value="${escapeHtml(h.name || "")}" placeholder="${t.studentNamePh}" />
          <input type="text" id="honorScore_${i}" value="${escapeHtml(h.score || "")}" placeholder="${t.scorePh}" />
          <input type="text" id="honorMsg_${i}" value="${escapeHtml(h.message || "")}" placeholder="${t.supportMsgPh}" />
        </div>`).join("");
    }

    function renderHonorDisplay() {
      const t = i18n[currentLang], medals = ["🥇", "🥈", "🥉"];
      document.getElementById("honorDisplayGrid").innerHTML = honorData.map((h, i) => `
        <div class="top-student-card rank-${i + 1}">
          <span class="rank-badge">${medals[i]} ${t.rankPrefix} #${i + 1}</span>
          <div class="item-title">${h.name && h.name.trim() ? escapeHtml(h.name.trim()) : `<span class="muted">${t.noHonorEntry}</span>`}</div>
          ${h.score ? `<div class="badge">${escapeHtml(h.score.trim())}</div>` : ""}
          ${h.message ? `<p class="muted">${escapeHtml(h.message.trim())}</p>` : ""}
        </div>`).join("");
    }

    document.getElementById("saveHonorBtn").addEventListener("click", async () => {
      if (!isAdminUnlocked) return;
      honorData = honorData.map((_, i) => ({
        rank: i + 1,
        name: document.getElementById(`honorName_${i}`).value.trim(),
        score: document.getElementById(`honorScore_${i}`).value.trim(),
        message: document.getElementById(`honorMsg_${i}`).value.trim()
      }));
      renderHonorDisplay(); updateAdminStats();
      localStorage.setItem("mycollege_honor_cache", JSON.stringify(honorData));
      try { await db.collection("college_config").doc("honor_roll").set({ topThree: honorData, updatedAt: firebase.firestore.FieldValue.serverTimestamp() }); } catch (e) { console.error(e); }
      alert(i18n[currentLang].savedHonor);
    });

    db.collection("college_config").doc("honor_roll").onSnapshot((doc) => {
      if (doc.exists && Array.isArray(doc.data().topThree) && doc.data().topThree.length === 3) {
        honorData = doc.data().topThree;
        localStorage.setItem("mycollege_honor_cache", JSON.stringify(honorData));
        renderHonorDisplay(); if (isAdminUnlocked) renderAdminHonorForm(); updateAdminStats();
      }
    });

    function renderAdminSubjectsForm() {
      const t = i18n[currentLang];
      document.getElementById("adminSubjectsGrid").innerHTML = subjectsData.map((s, i) => `
        <div class="admin-subject-box">
          <strong>${t.subjectPrefix} ${i + 1}</strong>
          <input type="text" id="subjName_${i}" value="${escapeHtml(s.name || "")}" placeholder="${t.subjectNamePh}" />
          <input type="url" id="subjPdf_${i}" value="${escapeHtml(s.pdfUrl || "")}" placeholder="${t.pdfLinkPh}" />
          <input type="url" id="subjImg_${i}" value="${escapeHtml(s.imageUrl || "")}" placeholder="${t.imgLinkPh}" />
        </div>`).join("");
    }

    function renderSubjectsDisplay() {
      const t = i18n[currentLang];
      document.getElementById("subjectsDisplayGrid").innerHTML = subjectsData.map((s, i) => {
        const name = s.name && s.name.trim() ? s.name.trim() : `${t.subjectPrefix} ${i + 1}`;
        return `
          <div class="subject-card">
            <div class="subject-header"><h4>${escapeHtml(name)}</h4><span class="subject-num">#${i + 1}</span></div>
            <div class="links-group">
              ${s.pdfUrl && s.pdfUrl.trim() ? `<a class="link-pill pdf" href="${escapeHtml(s.pdfUrl.trim())}" target="_blank" rel="noopener noreferrer">📄 ${t.openPdf}</a>` : `<span class="muted">📄 ${t.noPdf}</span>`}
              ${s.imageUrl && s.imageUrl.trim() ? `<a class="link-pill img" href="${escapeHtml(s.imageUrl.trim())}" target="_blank" rel="noopener noreferrer">🖼️ ${t.openImg}</a>` : `<span class="muted">🖼️ ${t.noImg}</span>`}
            </div>
          </div>`;
      }).join("");
    }

    document.getElementById("saveAllSubjectsBtn").addEventListener("click", async () => {
      if (!isAdminUnlocked) return;
      subjectsData = subjectsData.map((_, i) => ({
        index: i + 1,
        name: document.getElementById(`subjName_${i}`).value.trim(),
        pdfUrl: document.getElementById(`subjPdf_${i}`).value.trim(),
        imageUrl: document.getElementById(`subjImg_${i}`).value.trim()
      }));
      renderSubjectsDisplay(); renderGpaInputs(); updateAdminStats();
      localStorage.setItem("mycollege_six_subjects_cache", JSON.stringify(subjectsData));
      try { await db.collection("college_config").doc("six_subjects").set({ subjects: subjectsData, updatedBy: currentRole, updatedAt: firebase.firestore.FieldValue.serverTimestamp() }); } catch (e) { console.error(e); }
      alert(i18n[currentLang].savedSubjects);
    });

    db.collection("college_config").doc("six_subjects").onSnapshot((doc) => {
      if (doc.exists && Array.isArray(doc.data().subjects) && doc.data().subjects.length === 6) {
        subjectsData = doc.data().subjects;
        localStorage.setItem("mycollege_six_subjects_cache", JSON.stringify(subjectsData));
        renderSubjectsDisplay(); renderGpaInputs(); updateAdminStats(); if (isAdminUnlocked) renderAdminSubjectsForm();
      }
    });

    function renderGpaInputs() {
      const t = i18n[currentLang];
      document.getElementById("gpaInputsGrid").innerHTML = subjectsData.map((s, i) => {
        const label = s.name && s.name.trim() ? s.name.trim() : `${t.subjectPrefix} ${i + 1}`;
        return `<input type="number" min="0" max="100" step="0.5" id="grade_${i}" placeholder="${escapeHtml(label)}" />`;
      }).join("");
    }

    document.getElementById("calcGpaBtn").addEventListener("click", () => {
      const t = i18n[currentLang], vals = [];
      for (let i = 0; i < 6; i++) {
        const raw = document.getElementById(`grade_${i}`).value;
        if (raw !== "" && !Number.isNaN(Number(raw))) vals.push(Number(raw));
      }
      const out = document.getElementById("gpaOutput");
      out.dataset.calculated = "1";
      out.textContent = vals.length ? t.gpaAvgText((vals.reduce((a, b) => a + b, 0) / vals.length).toFixed(2), vals.length) : t.gpaNoGrades;
    });

    document.getElementById("calcCountdownBtn").addEventListener("click", () => {
      const t = i18n[currentLang], val = document.getElementById("examDateInput").value, out = document.getElementById("countdownOutput");
      out.dataset.calculated = "1";
      if (!val) { out.textContent = t.countdownPickDate; return; }
      const target = new Date(val + "T00:00:00"), now = new Date(); now.setHours(0, 0, 0, 0);
      const diff = Math.ceil((target - now) / 86400000);
      out.textContent = diff > 0 ? t.countdownDaysLeft(diff) : diff === 0 ? t.countdownToday : t.countdownPassed;
    });

    document.getElementById("saveScheduleBtn").addEventListener("click", () => { localStorage.setItem("mycollege_schedule", document.getElementById("scheduleText").value); alert(i18n[currentLang].scheduleSaved); });
    document.getElementById("saveNotesBtn").addEventListener("click", () => { localStorage.setItem("mycollege_notes", document.getElementById("personalNotesText").value); alert(i18n[currentLang].notesSaved); });

    function updateAdminStats() {
      const activeSubj = subjectsData.filter((s) => (s.name && s.name.trim()) || (s.pdfUrl && s.pdfUrl.trim()) || (s.imageUrl && s.imageUrl.trim())).length;
      const activeHonor = honorData.filter((h) => h.name && h.name.trim()).length;
      document.getElementById("statActiveSubjects").textContent = `${activeSubj} / 6`;
      document.getElementById("statAnnCount").textContent = String(cachedAnns.length);
      document.getElementById("statDeptCount").textContent = String(cachedDepts.length);
      document.getElementById("statHonorCount").textContent = `${activeHonor} / 3`;
    }

    db.collection("departments").orderBy("createdAt", "desc").onSnapshot((snap) => { cachedDepts = snap.docs.map((d) => ({ id: d.id, ...d.data() })); renderDepts(); updateAdminStats(); });
    db.collection("announcements").orderBy("createdAt", "desc").onSnapshot((snap) => { cachedAnns = snap.docs.map((d) => ({ id: d.id, ...d.data() })); renderAnns(); updateAdminStats(); });

    document.getElementById("saveDeptBtn").addEventListener("click", async () => {
      if (!isAdminUnlocked) return;
      const name = document.getElementById("deptName").value.trim(), code = document.getElementById("deptCode").value.trim();
      if (!name) return alert(i18n[currentLang].fillFields);
      await db.collection("departments").add({ name, code, role: currentRole, createdAt: firebase.firestore.FieldValue.serverTimestamp() });
      document.getElementById("deptName").value = ""; document.getElementById("deptCode").value = "";
    });

    document.getElementById("saveAnnBtn").addEventListener("click", async () => {
      if (!isAdminUnlocked) return;
      const title = document.getElementById("annTitle").value.trim(), body = document.getElementById("annBody").value.trim();
      if (!title || !body) return alert(i18n[currentLang].fillFields);
      await db.collection("announcements").add({ title, body, role: currentRole, createdAt: firebase.firestore.FieldValue.serverTimestamp() });
      document.getElementById("annTitle").value = ""; document.getElementById("annBody").value = "";
    });

    async function deleteDocItem(col, id) { if (isAdminUnlocked) await db.collection(col).doc(id).delete(); }

    function renderDepts() {
      const el = document.getElementById("deptList"), t = i18n[currentLang];
      el.innerHTML = cachedDepts.length ? cachedDepts.map((x) => `<div class="item"><div><div class="item-title">${escapeHtml(x.name)}</div><div class="muted">${escapeHtml(x.code || "")}</div></div>${isAdminUnlocked ? `<button class="danger" onclick="deleteDocItem('departments','${x.id}')">${t.delete}</button>` : ""}</div>`).join("") : `<p class="muted">${t.empty}</p>`;
    }

    function renderAnns() {
      const el = document.getElementById("annList"), t = i18n[currentLang];
      el.innerHTML = cachedAnns.length ? cachedAnns.map((x) => `<div class="item"><div><div class="item-title">${escapeHtml(x.title)}</div><div>${escapeHtml(x.body)}</div></div>${isAdminUnlocked ? `<button class="danger" onclick="deleteDocItem('announcements','${x.id}')">${t.delete}</button>` : ""}</div>`).join("") : `<p class="muted">${t.empty}</p>`;
    }

    const sLang = localStorage.getItem("mycollege_lang"); if (sLang && i18n[sLang]) { currentLang = sLang; langSelect.value = sLang; }
    const sTheme = localStorage.getItem("mycollege_theme"); if (sTheme) setTheme(sTheme);
    const sScale = localStorage.getItem("mycollege_font_scale"); if (sScale) setFontScale(sScale);
    const sSched = localStorage.getItem("mycollege_schedule"); if (sSched) document.getElementById("scheduleText").value = sSched;
    const sNotes = localStorage.getItem("mycollege_notes"); if (sNotes) document.getElementById("personalNotesText").value = sNotes;
    try { const m = JSON.parse(localStorage.getItem("mycollege_meta_info")); if (m) { metaInfo = { supervisor: m.supervisor || "", stage: m.stage || "" }; document.getElementById("supervisorNameInput").value = metaInfo.supervisor; document.getElementById("stageLabelInput").value = metaInfo.stage; } } catch (e) {}
    try { const h = JSON.parse(localStorage.getItem("mycollege_honor_cache")); if (Array.isArray(h) && h.length === 3) honorData = h; } catch (e) {}
    try { const s = JSON.parse(localStorage.getItem("mycollege_six_subjects_cache")); if (Array.isArray(s) && s.length === 6) subjectsData = s; } catch (e) {}

    const manifestBlob = new Blob([JSON.stringify({ name: "MyCollege", short_name: "MyCollege", start_url: ".", display: "standalone", background_color: "#0b1120", theme_color: "#0f172a" })], { type: "application/json" });
    const manifestLink = document.createElement("link"); manifestLink.rel = "manifest"; manifestLink.href = URL.createObjectURL(manifestBlob); document.head.appendChild(manifestLink);

    applyLanguage();
  </script>
</body>
</html>
