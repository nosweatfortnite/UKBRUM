<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>UKBRUM Staff Panel</title>

<style>
/* ================= GLOBAL ================= */
body {
    background:#0e0e0e;
    font-family:Arial, sans-serif;
    padding:20px;
    color:#fff;
}

h1 {
    text-align:center;
    color:#ffcc00;
}

/* ================= TABS ================= */
.tabs {
    display:flex;
    gap:10px;
    margin-bottom:20px;
}

.tab-btn {
    padding:10px 18px;
    background:#1e1e1e;
    border:1px solid #444;
    color:#fff;
    cursor:pointer;
    border-radius:6px;
}

.tab-btn.active {
    background:#ffcc00;
    color:#000;
    font-weight:bold;
}

.tab {
    display:none;
}

.tab.active {
    display:block;
}

/* ================= HEADINGS ================= */
h2 {
    color:#ffcc00;
    margin-top:30px;
}

/* ================= MESSAGE BOXES ================= */
.box {
    margin:10px 0;
}

.copy-container {
    display:flex;
    gap:10px;
}

textarea {
    width:100%;
    min-height:70px;
    background:#1a1a1a;
    color:#fff;
    border:1px solid #444;
    border-radius:6px;
    padding:10px;
    resize:vertical;
}

button.copy {
    background:#ffcc00;
    border:none;
    border-radius:6px;
    padding:10px 16px;
    font-weight:bold;
    cursor:pointer;
}

button.copy:hover {
    background:#e6b800;
}

/* ================= PUNISHMENT GUIDE ================= */
table {
    width:100%;
    border-collapse:collapse;
    margin-top:20px;
    background:#f5f5f5;
    color:#000;
    user-select:none;
}

th, td {
    border:1px solid #ccc;
    padding:10px;
    text-align:center;
    color:#000;
}

th {
    background:#e0e0e0;
    font-weight:bold;
}

/* Row types */
.warning { background:#e6f0c8; }
.kick { background:#cfe3f1; }
.ban { background:#f1cfcf; }
.side { background:#eeeeee; }

/* Remove blue selection highlight */
table ::selection {
    background:#ddd;
    color:#000;
}

table ::-moz-selection {
    background:#ddd;
    color:#000;
}

.note {
    margin-top:15px;
    font-style:italic;
    color:#ccc;
}
</style>
</head>

<body>

<h1>UKBRUM Staff Panel</h1>

<div class="tabs">
    <button class="tab-btn active" onclick="openTab(0)">📋 Messages</button>
    <button class="tab-btn" onclick="openTab(1)">⚖️ Punishment Guide</button>
</div>

<!-- ================= TAB 1: MESSAGES ================= -->
<div class="tab active">

<h2>⚠️ Punishment Messages</h2>

<div class="box"><div class="copy-container">
<textarea>You are being verbally warned for [Reason]. If you do this again it will result in a warning and/or kick.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>You are being warned for [Reason]. If caught again it will result in further punishment.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>You are being kicked for [Reason]. Please do not rejoin within the next 30 minutes. You may appeal via UKBRUM communications.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>You are being banned for [Reason]. You may appeal via UKBRUM communications.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<h2>👮 Staff Interaction</h2>

<div class="box"><div class="copy-container">
<textarea>Hello, I am [Name], a [Rank] here at UKBRUM.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>Is there anything else I can assist you with today?</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>Have a great roleplay! If you need staff assistance, don’t hesitate to call a moderator.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<h2>📢 Roleplay / Server Messages</h2>

<div class="box"><div class="copy-container">
<textarea>:h 🚖 Looking for transport? A luxury limousine is available!</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🍔 Three Guys is now open — come grab some food!</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:m 🎮 Please maintain realistic roleplay at all times.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

</div>

<!-- ================= TAB 2: PUNISHMENT GUIDE ================= -->
<div class="tab">

<h2>⚖️ Punishment Guide</h2>

<table>
<tr>
<th>Offence</th>
<th>Action</th>
<th>Side Action</th>
</tr>

<tr><td>Unrealistic Avatar</td><td class="warning">Warning</td><td class="side">Load / Refresh</td></tr>
<tr><td>Interrupting Scenes</td><td class="warning">Warning</td><td class="side">Load / Refresh</td></tr>
<tr><td>RDM / VDM</td><td class="warning">Warning</td><td class="side">None</td></tr>
<tr><td>Cop Baiting / Metagaming</td><td class="warning">Warning</td><td class="side">Load / Refresh</td></tr>
<tr><td>FRP</td><td class="warning">Warning</td><td class="side">Load / Refresh</td></tr>
<tr><td>GTA Driving</td><td class="warning">Warning</td><td class="side">Load / Refresh</td></tr>
<tr><td>No Permissions</td><td class="warning">Warning</td><td class="side">Refresh</td></tr>
<tr><td>Disrespect</td><td class="kick">Kick</td><td class="side">None</td></tr>
<tr><td>NLR</td><td class="warning">Warning</td><td class="side">Refresh</td></tr>
<tr><td>Breaking Priority</td><td class="kick">Kick</td><td class="side">None</td></tr>
<tr><td>Staff Evasion / RDM / VDM</td><td class="kick">Kick</td><td class="side">None</td></tr>
<tr><td>Staff Impersonation</td><td class="ban">Instant Ban</td><td class="side">None</td></tr>
<tr><td>Breaking TOS</td><td class="ban">Instant Ban</td><td class="side">None</td></tr>
</table>

<div class="note">
Kick length and logs are at moderator discretion.<br>
Warnings reset every session and do not carry over.
</div>

</div>

<script>
function copyText(btn) {
    const textarea = btn.previousElementSibling;
    textarea.select();
    navigator.clipboard.writeText(textarea.value);
}

function openTab(index) {
    document.querySelectorAll('.tab').forEach((t,i)=>{
        t.classList.toggle('active', i === index);
    });
    document.querySelectorAll('.tab-btn').forEach((b,i)=>{
        b.classList.toggle('active', i === index);
    });
}
</script>

</body>
</html>
