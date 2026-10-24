<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Game!Rajya - Free Fire Gaming</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --blue: #008cff;
    --cyan: #00d9ff;
    --bg: #030712;
    --card: #0a1425;
    --text: #f1f5ff;
    --muted: #a5b4cc;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    background: var(--bg);
    color: var(--text);
}

header {
    background: #050c19;
    border-bottom: 1px solid #087aff;
    padding: 18px 5%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
}

.logo {
    font-size: 26px;
    font-weight: 900;
    font-style: italic;
}

.logo span {
    color: var(--blue);
}

nav {
    display: flex;
    gap: 18px;
    flex-wrap: wrap;
}

nav a {
    color: white;
    text-decoration: none;
    font-size: 14px;
}

nav a:hover {
    color: var(--cyan);
}

.hero {
    padding: 75px 7%;
    background:
    radial-gradient(ellipse at 80% 30%, #064a9b 0%, transparent 45%),
    linear-gradient(135deg, #071327, #02050b);
    border-bottom: 1px solid #0756a8;
}

.badge {
    display: inline-block;
    background: #063c70;
    color: var(--cyan);
    padding: 7px 12px;
    border-radius: 5px;
    font-size: 12px;
    font-weight: bold;
    margin-bottom: 18px;
}

.hero h1 {
    font-size: clamp(38px, 8vw, 70px);
    margin-bottom: 15px;
    font-style: italic;
}

.hero h1 span {
    color: var(--blue);
}

.hero p {
    color: var(--muted);
    max-width: 550px;
    line-height: 1.8;
    margin-bottom: 25px;
}

.btn {
    display: inline-block;
    background: linear-gradient(90deg, #006eff, #00aaff);
    color: white;
    border: none;
    border-radius: 8px;
    padding: 13px 22px;
    font-size: 14px;
    font-weight: bold;
    text-decoration: none;
    cursor: pointer;
    transition: .2s;
}

.btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 0 18px #008cff66;
}

.container {
    padding: 35px 5%;
}

.section-title {
    font-size: 25px;
    margin-bottom: 22px;
}

.section-title span {
    color: var(--blue);
}

.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 17px;
}

.card {
    background: linear-gradient(145deg, #0c1b31, #060d19);
    border: 1px solid #163458;
    border-radius: 12px;
    padding: 22px;
    transition: .25s;
}

.card:hover {
    border-color: var(--blue);
    transform: translateY(-4px);
}

.icon {
    font-size: 30px;
    margin-bottom: 12px;
}

.card h3 {
    margin-bottom: 12px;
}

.card p {
    color: var(--muted);
    font-size: 14px;
    line-height: 1.7;
}

.tips-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 15px;
}

.tip {
    background: var(--card);
    border-left: 3px solid var(--blue);
    border-radius: 8px;
    padding: 18px;
}

.tip h3 {
    font-size: 16px;
    margin-bottom: 9px;
}

.tip p {
    color: var(--muted);
    line-height: 1.7;
    font-size: 14px;
}

.tip-number {
    color: var(--cyan);
    font-weight: bold;
    margin-right: 5px;
}

.settings {
    background: var(--card);
    border: 1px solid #163458;
    border-radius: 12px;
    padding: 22px;
    max-width: 650px;
}

.setting {
    margin: 20px 0;
}

.setting label {
    display: flex;
    justify-content: space-between;
    margin-bottom: 10px;
    font-size: 14px;
}

.setting input {
    width: 100%;
    accent-color: var(--blue);
    cursor: pointer;
}

.name-box {
    background: #030a14;
    border: 1px solid #163458;
    border-radius: 8px;
    padding: 15px;
    margin: 15px 0;
    color: var(--cyan);
    font-size: 20px;
    text-align: center;
    overflow-wrap: anywhere;
}

input[type="text"] {
    width: 100%;
    background: #030a14;
    color: white;
    border: 1px solid #163458;
    padding: 13px;
    border-radius: 7px;
    margin: 12px 0;
    outline: none;
}

footer {
    border-top: 1px solid #0756a8;
    background: #050c19;
    padding: 28px 15px;
    text-align: center;
    color: var(--muted);
    line-height: 2;
    font-size: 13px;
}

footer strong {
    color: var(--blue);
}

.small {
    color: var(--muted);
    font-size: 12px;
    margin-top: 12px;
}

@media (max-width: 600px) {
    header {
        justify-content: center;
    }

    nav {
        justify-content: center;
        gap: 13px;
    }

    .hero {
        padding: 55px 6%;
    }

    .container {
        padding: 28px 5%;
    }
}
</style>
</head>

<body>

<header>
    <div class="logo">🎮 Game!<span>Rajya</span></div>

    <nav>
        <a href="#home">Home</a>
        <a href="#tips">FF Tips</a>
        <a href="#sensitivity">Sensitivity</a>
        <a href="#names">Gaming Names</a>
    </nav>
</header>

<section class="hero" id="home">
    <div class="badge">WELCOME TO THE GAMING WORLD</div>

    <h1>Game!<span>Rajya</span></h1>

    <p>
        Improve your Free Fire gameplay with useful tips,
        sensitivity settings and stylish gaming names.
        Your gaming journey starts here!
    </p>

    <a href="#tips" class="btn">🔥 Explore Gaming Tips →</a>
</section>

<section class="container">
    <h2 class="section-title">Explore <span>Game!Rajya</span></h2>

    <div class="grid">
        <div class="card">
            <div class="icon">🎯</div>
            <h3>Headshot Tips</h3>
            <p>Learn aiming, crosshair placement and drag-shot practice.</p>
        </div>

        <div class="card">
            <div class="icon">⚙️</div>
            <h3>Sensitivity</h3>
            <p>Explore adjustable sensitivity settings for your gameplay.</p>
        </div>

        <div class="card">
            <div class="icon">👑</div>
            <h3>Stylish Names</h3>
            <p>Create a unique gaming name for your profile.</p>
        </div>

        <div class="card">
            <div class="icon">🏆</div>
            <h3>Pro Gameplay</h3>
            <p>Improve movement, positioning and decision-making.</p>
        </div>
    </div>
</section>

<section class="container" id="tips">
    <h2 class="section-title">🔥 Free Fire <span>Gaming Tips</span></h2>

    <div class="tips-list">

        <div class="tip">
            <h3><span class="tip-number">01.</span> Headshot Practice</h3>
            <p>
                Keep your crosshair around upper-body level.
                Practise controlled upward drags in the training
                area instead of moving your aim randomly.
            </p>
        </div>

        <div class="tip">
            <h3><span class="tip-number">02.</span> Movement Skills</h3>
            <p>
                Practise strafing, jumping when appropriate and
                changing direction. Avoid standing still while
                fighting in the open.
            </p>
        </div>

        <div class="tip">
            <h3><span class="tip-number">03.</span> Gloo Wall Practice</h3>
            <p>
                Practise placing gloo walls quickly for cover.
                Learn to use them while moving and recovering
                during fights.
            </p>
        </div>

        <div class="tip">
            <h3><span class="tip-number">04.</span> Weapon Selection</h3>
            <p>
                Practise with different weapon types and learn
                their effective ranges. Choose weapons that suit
                your playstyle.
            </p>
        </div>

        <div class="tip">
            <h3><span class="tip-number">05.</span> Smart Positioning</h3>
            <p>
                Use cover, pay attention to the safe zone and
                avoid unnecessary fights when your position
                puts you at a disadvantage.
            </p>
        </div>

        <div class="tip">
            <h3><span class="tip-number">06.</span> Daily Training</h3>
            <p>
                Spend a little time practising aim and movement.
                Review your mistakes and focus on improving
                one skill at a time.
            </p>
        </div>

    </div>
</section>

<section class="container" id="sensitivity">
    <h2 class="section-title">🎯 Sensitivity <span>Settings</span></h2>

    <div class="settings">
        <p class="small">
            Starting suggestions only. Adjust these values to
            your device and comfort; they are not guaranteed
            headshot settings.
        </p>

        <div class="setting">
            <label>General <span id="v1">189</span></label>
            <input type="range" min="0" max="200" value="189"
            oninput="updateValue('v1',this.value)">
        </div>

        <div class="setting">
            <label>Red Dot <span id="v2">187</span></label>
            <input type="range" min="0" max="200" value="187"
            oninput="updateValue('v2',this.value)">
        </div>

        <div class="setting">
            <label>2x Scope <span id="v3">170</span></label>
            <input type="range" min="0" max="200" value="170"
            oninput="updateValue('v3',this.value)">
        </div>

        <div class="setting">
            <label>4x Scope <span id="v4">170</span></label>
            <input type="range" min="0" max="200" value="170"
            oninput="updateValue('v4',this.value)">
        </div>

        <div class="setting">
            <label>Sniper Scope <span id="v5">190</span></label>
            <input type="range" min="0" max="200" value="190"
            oninput="updateValue('v5',this.value)">
        </div>

        <div class="setting">
            <label>Free Look <span id="v6">200</span></label>
            <input type="range" min="0" max="200" value="200"
            oninput="updateValue('v6',this.value)">
        </div>

        <button class="btn" onclick="copySettings()">
            📋 Copy Settings
        </button>
    </div>
</section>

<section class="container" id="names">
    <h2 class="section-title">👑 Stylish <span>Name Generator</span></h2>

    <div class="settings">
        <p class="small">
            Enter your name and generate a decorated version.
        </p>

        <input type="text" id="playerName"
        placeholder="Enter your gaming name">

        <button class="btn" onclick="generateName()">
            ✨ Generate Name
        </button>

        <div class="name-box" id="result">
            Your Gaming Name
        </div>

        <button class="btn" onclick="copyName()">
            📋 Copy Name
        </button>
    </div>
</section>

<footer>
    <h2>🎮 Game!<strong>Rajya</strong></h2>
    <p>Play Smart • Practise Daily • Improve Every Day</p>
    <p>Fan-made gaming tips website.</p>
    <p>Not affiliated with Garena or Free Fire.</p>
    <p>© 2026 Game!Rajya</p>
</footer>

<script>
function updateValue(id, value) {
    document.getElementById(id).textContent = value;
}

function copyText(text) {
    if (navigator.clipboard && window.isSecureContext) {
        navigator.clipboard.writeText(text)
        .then(() => alert("Copied successfully!"))
        .catch(() => fallbackCopy(text));
    } else {
        fallbackCopy(text);
    }
}

function fallbackCopy(text) {
    const area = document.createElement("textarea");
    area.value = text;
    area.style.position = "fixed";
    area.style.left = "-9999px";
    document.body.appendChild(area);
    area.select();

    try {
        document.execCommand("copy");
        alert("Copied!");
    } catch (e) {
        alert("Copy failed. Please select and copy manually.");
    }

    area.remove();
}

function copySettings() {
    const labels = [
        "General", "Red Dot", "2x Scope",
        "4x Scope", "Sniper Scope", "Free Look"
    ];

    const ids = ["v1", "v2", "v3", "v4", "v5", "v6"];

    let result = "Game!Rajya Sensitivity Settings\n";

    labels.forEach((label, i) => {
        result += label + ": " +
        document.getElementById(ids[i]).textContent + "\n";
    });

    copyText(result);
}

function generateName() {
    const input = document.getElementById("playerName");
    const name = input.value.trim();

    if (!name) {
        alert("Please enter your name first!");
        return;
    }

    const styles = [
        "亗 " + name + " 亗",
        "乂" + name + "乂",
        "『" + name + "』",
        "꧁༒" + name + "༒꧂",
        "★彡" + name + "彡★",
        "ツ " + name + " ツ",
        "♛ " + name + " ♛",
        "メ" + name + "メ"
    ];

    const choice = styles[Math.floor(Math.random() * styles.length)];

    document.getElementById("result").textContent = choice;
}

function copyName() {
    const name = document.getElementById("result").textContent;

    if (name === "Your Gaming Name") {
        alert("Generate a name first!");
        return;
    }

    copyText(name);
}
</script>

</body>
</html>
