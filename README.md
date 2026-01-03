<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>UKBRUM Staff Panel</title>

<style>
body {
    background:#0e0e0e;
    color:#fff;
    font-family:Arial, sans-serif;
    padding:20px;
}

h1 {
    text-align:center;
    color:#ffcc00;
}

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

h2 {
    color:#ffcc00;
    margin-top:30px;
}

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

/* ================= Punishment Table ================= */
table {
    width:100%;
    border-collapse:collapse;
    margin-top:20px;
}

th, td {
    border:1px solid #444;
    padding:10px;
    text-align:center;
    color:#000; /* FIX: black text for visibility */
}

th {
    background:#1f1f1f;
    color:#ffcc00;
}

.warning { background:#2d3b1f; }
.kick { background:#1f2f3b; }
.ban { background:#2b1f1f; }
.side { background:#2a2a2a; }

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

<!-- ================= TAB 1 ================= -->
<div class="tab active">

<h2>⚠️ Punishment Messages</h2>

<div class="box"><div class="copy-container">
<textarea>You are being verbally warned for [Reason]. If you do this again it will result in a warning and/or kick.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>You are being warned for [Reason]. If caught again it will result in a further punishment.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>You are being kicked for [Reason]. Please do not join back in the next 30 minutes. You can appeal this via our communications UKBRUM.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>You are being banned for [Reason]. You can appeal this via our communications. Code: UKBRUM</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<h2>👮 Staff Interaction</h2>

<div class="box"><div class="copy-container">
<textarea>Greetings! I am [Name], a [Rank] here at UKBRUM. (Late/Void)</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>Is there anything else I can assist you with today?</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>Have an amazing roleplay! If you need any further assistance from staff don’t hesitate to call a moderator.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<h2>📢 Roleplay / Message Commands</h2>

<div class="box"><div class="copy-container">
<textarea>:h 🚖 Looking for a ride? There is a luxurious limousine ready to take you anywhere you want!</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🍔 Three Guys is now open. Head over there for some delicious food.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:m 🎮 We value your roleplay experience! Avoid unnecessary issues to keep things realistic.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:m 🤿 Dive into immersive roleplay with us! Communications Code: UKBRUM</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<h2>📢 Roleplay / Server Messages</h2>

<div class="box"><div class="copy-container">
<textarea>:h 🚖 Looking for a ride? Well the taxi company is now open! Call them.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🚖 Looking for a ride? Well the Metro Bus is now active. Wait at a bus stop to hop on!</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🏀 There is a basketball game happening at the basketball court! Come on over to play!</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h ⛽ River City Gas-N-Go is now open get some gas and food for the road trip.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🔫 River City Guns and Ammo is now open. Get some weapons and use them properly though.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🏦 Bank of River City is now open. Head over there to deposit some money.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🚗 The Mod Shop in River City is now open! Head over there to get an oil change, new paint job, and rims or just repair your car.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🧰 The Tool Store is now open. Grab some tools.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🏥 Need a check-up or need medicine? The hospital is currently open for all of those things!</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 📱 Want a new phone? The Gadget Shack is open!</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🌮 La Mesa is now open. Head over there for some Mexican food.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h ☕ Liberty Cafe is now open. Head over there for some coffee and more.</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 💎 The Jewelry Store Is now open! Get yourself something nice!</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<h2>🛑 Staff Applications</h2>

<div class="box"><div class="copy-container">
<textarea>:h 🛑 Step Up and Make a Difference — Staff Wanted! Communications Code: UKBRUM</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🔊 Be the Voice Behind the Server’s Success! Communications Code: UKBRUM</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h ⚒️ Staff Wanted: Make Moves, Make Impact! Communications Code: UKBRUM</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 🌍 Many Roles, One Goal — Staff Together! Communications Code: UKBRUM</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

<div class="box"><div class="copy-container">
<textarea>:h 💼 Staff Applications are Open! Take your chance today and unlock a world of opportunities! Communications Code: UKBRUM</textarea>
<button class="copy" onclick="copyText(this)">Copy</button>
</div></div>

</div>

<!-- ================= TAB 2 ================= -->
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
<tr><td>RDM / VDM</td><td class="warning">Warning</td><td class="side">No Side Actions</td></tr>
<tr><td>Cop Baiting / Metagaming</td><td class="warning">Warning</td><td class="side">Load / Refresh</td></tr>
<tr><td>FRP</td><td class="warning">Warning</td><td class="side">Load / Refresh</td></tr>
<tr><td>GTA Driving</td><td class="warning">Warning</td><td class="side">Load / Refresh</td></tr>
<tr><td>No Permissions</td><td class="warning">Warning</td><td class="side">Refresh</td></tr>
<tr><td>Disrespect</td><td class="kick">Kick</td><td class="side">No Side Actions</td></tr>
<tr><td>NLR</td><td class="warning">Warning</td><td class="side">Refresh</td></tr>
<tr><td>Not Trained</td><td class="warning">Warning</td><td class="side">Jail / Wanted</td></tr>
<tr><td>Breaking Priority</td><td class="kick">Kick</td><td class="side">No Side Actions</td></tr>
<tr><td>Breaking Safezones</td><td class="kick">Kick</td><td class="side">No Side Actions</td></tr>
<tr><td>Staff Evasion / VDM / RDM</td><td class="kick">Kick</td><td class="side">No Side Actions</td></tr>
<tr><td>Car Blockage</td><td class="warning">Warning</td><td class="side">Jail / Wanted</td></tr>
<tr><td>Staff Impersonation</td><td class="ban">Instant Ban</td><td class="side">No Side Actions</td></tr>
<tr><td>Breaking TOS</td><td class="ban">Instant Ban</td><td class="side">No Side Actions</td></tr>
<tr><td>Major Events</td><td class="ban">Instant Ban</td><td class="side">No Side Actions</td></tr>
<tr><td>L-Tap / NITRP</td><td class="ban">Instant Ban</td><td class="side">No Side Actions</td></tr>
<tr><td>Raiding</td><td class="ban">Instant Ban</td><td class="side">No Side Actions</td></tr>
</table>

<div class="note">
Kick time / log is decided by the moderator depending on the severity of the situation.<br>
All warnings reset each session and will not carry over.
</div>

</div>

<script>
function copyText(btn) {
    const textarea = btn.previousElementSibling;
    textarea.select();
    textarea.setSelectionRange(0, 99999);
    navigator.clipboard.writeText(textarea.value);
}

function openTab(index) {
    document.querySelectorAll('.tab').forEach((t,i)=>t.classList.toggle('active',i===index));
    document.querySelectorAll('.tab-btn').forEach((b,i)=>b.classList.toggle('active',i===index));
}
</script>

</body>
</html>
