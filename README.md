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

/* ================= Notice ================= */
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

<h1>UKBRUM</h1>

<div class="tabs">
    <button class="tab-btn active" onclick="openTab(0)">📋 Messages</button>
    <button class="tab-btn" onclick="openTab(1)">Active Notice</button>
</div>

<!-- ================= TAB 1 ================= -->
<div class="tab active">

<h2></h2>

<div class="box"><div class="copy-container">
<textarea>This Website has been discontinued due to the fact that "Panther_cattreats" has retired from UKBRUM's staff team, any inquiries about this topic don't hesitate to DM me privately! Panther_cattreats.
</div></div>
    
</body>
</html>
