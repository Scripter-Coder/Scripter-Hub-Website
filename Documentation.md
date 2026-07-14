markdown
# 📚 ScripterHub Website - Complete Documentation

Welcome to ScripterHub! This guide explains how to edit everything on your website.

---

## 📁 File Structure
Scripter-Hub-Website/
├── index.html # Main hub
├── status.html # Status page
├── scripts.html # Scripts library
├── Documentation.md # This file
└── Images/ # Game images

text

**Live Website:** `https://Scripter-Coder.github.io/Scripter-Hub-Website/`


---

## 📜 Adding a New Script (scripts.html)

**Step 1:** Open `scripts.html`

**Step 2:** Find the `scriptsData` array and add:
```javascript
{
  name: "Your Game",
  gameId: "1234567890",
  image: "Images/YourGame.png",
  gameUrl: "https://www.roblox.com/games/1234567890/Your-Game",
  script: `loadstring(game:HttpGet("YOUR_SCRIPT_URL"))()`,
  youtube: "https://youtube.com/@yourchannel",
  discord: "https://discord.gg/yourinvite",
  status: "Working | OP ⭐"
}
```

**Step 3:** Upload image to Images/ folder

**Step 4:** Add to status page (status.html):

```html
<div class="script-row">
  <span class="script-name">Your Game</span>
  <span class="script-status status-soon">Soon</span>
</div>
```

🎨 Status Colors (status.html)
Status	CSS Class
Working | OP ⭐	 = status-working-op
Working (EXPERIMENTAL) = status-experimental
Soon = status-soon
Not Working	= status-notworking
Working	= status-working
Updating = status-updating
Discontinued = status-discontinued

🔧 Editing Executors (status.html)
Add new executor:

```html
<div class="executor-item">
  <span class="exe-name">ExecutorName</span>
  <span>
    <span class="exe-type">Free</span>
    <span class="exe-status exe-green">🟢</span>
  </span>
</div>
```

Colors:
exe-green → 🟢 Working
exe-red → 🔴 Down
exe-blue → 🔵 Unknown

🏠 Main Hub (index.html)
Change title text:
```html
<span>Hello Player,<br>What Are You Looking For?</span>
```
Add/Edit button:
```html
<a href="page.html" class="btn">🎮 Button Name</a>
```
Lock a button:
```html
<button class="btn btn-locked" disabled>🔒 Feature (Soon)</button>
```

🖼️ Images
Path: Images/YourGame.png
Requirements:

PNG or JPG
400×200 pixels recommended
Upload to Images/ folder

🚀 Publishing Changes
Commit changes on GitHub
Wait 1-2 minutes
Refresh: https://Scripter-Coder.github.io/Scripter-Hub-Website/

❓ Quick Fixes
Issue	Solution
Images not showing = Check path Images/YourGame.png
Changes not showing	= Clear cache (Ctrl+Shift+R)
Button not working = Check href="..." is correct
Script not copying = Check script URL is valid

🎯 Button Actions
Button	What it does
🎮 Game	Opens Roblox game page
📋 Script	Copies script to clipboard
▶️ YouTube	Opens YouTube
💬 Discord	Opens Discord

