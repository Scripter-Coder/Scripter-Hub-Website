markdown
# 📚 ScripterHub Website - Complete Documentation

Welcome to ScripterHub! This guide explains how to edit everything on your website.

---

## 📁 File Structure
Scripter-Hub-Website/
├── index.html # Main hub page
├── status.html # Scripts & Executors status
├── scripts.html # Scripts library with search
├── Documentation.md # This file
└── Images/ # Folder for game images
├── SlapBattles.png
├── Doors.png
└── ... (more images)

text

**Live Website:** `https://Scripter-Coder.github.io/Scripter-Hub-Website/`

---

## 🏠 1. Main Hub (`index.html`)

### Change the Title Text
Find this line:
```html
<span>Hello Player,<br>What Are You Looking For?</span>
Change the text between <span> tags.

Change Button Links
html
<a href="status.html" class="btn">📊 Scripts/Executors Status</a>
Edit href="..." to point to a different page.

Lock/Unlock Buttons
Locked (not clickable):

html
<button class="btn btn-locked" disabled>🔒 Wiki (Soon)</button>
Unlocked (clickable):

html
<a href="wiki.html" class="btn">📖 Wiki</a>
Add a New Button
html
<a href="yourpage.html" class="btn">🎮 New Button</a>
Change Background Speed
Find this in CSS:

css
.animated-bg {
  animation: colorPulse 12s ease-in-out infinite;
}
Change 12s to 8s (faster) or 16s (slower).

📊 2. Status Page (status.html)
Edit Script Status
Find a script entry:

html
<div class="script-row">
  <span class="script-name">Slap Battles</span>
  <span class="script-status status-working-op">Working | OP ⭐</span>
</div>
Status Color Classes
Status	CSS Class
Working | OP ⭐	status-working-op
Working (EXPERIMENTAL)	status-experimental
Soon	status-soon
Not Working	status-notworking
Working	status-working
Updating	status-updating
Discontinued	status-discontinued
Add a New Script
html
<div class="script-row">
  <span class="script-name">Your Game</span>
  <span class="script-status status-soon">Soon</span>
</div>
Edit Executors
Find an executor entry:

html
<div class="executor-item">
  <span class="exe-name">Solara</span>
  <span>
    <span class="exe-type">Free</span>
    <span class="exe-status exe-green">🟢</span>
  </span>
</div>
Executor Colors:

exe-green → 🟢 (Working)

exe-red → 🔴 (Down)

exe-blue → 🔵 (Unknown)

📜 3. Scripts Library (scripts.html)
Script Data Structure
Find the scriptsData array and add/edit scripts:

javascript
{
  name: "Slap Battles",
  gameId: "6403373529",
  image: "Images/SlapBattles.png",
  gameUrl: "https://www.roblox.com/games/6403373529/Slap-Battles",
  script: `loadstring(game:HttpGet("SCRIPT_URL"))()`,
  youtube: "https://youtube.com/@yourchannel",
  discord: "https://discord.gg/yourinvite",
  status: "Working | OP ⭐"
}
How to Get Game ID
From the Roblox URL: https://www.roblox.com/games/6403373529/Slap-Battles
The number 6403373529 is the Game ID.

Add a New Script
Copy this template and fill in your details:

javascript
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
Delete a Script
Find the script in scriptsData and delete the entire block including the { } and comma.

Change YouTube/Discord Links
javascript
youtube: "https://youtube.com/@YOUR_CHANNEL",
discord: "https://discord.gg/YOUR_INVITE"
🖼️ 4. Images Folder (Images/)
How to Add Images
Create a folder called Images/ in your repository

Upload PNG/JPG files there

Name them like SlapBattles.png

Reference them as "Images/SlapBattles.png"

Image Requirements
Format: PNG or JPG

Recommended size: 400×200 pixels

Naming: Use game name (e.g., Doors.png)

🔧 5. How to Edit Everything
Edit Text
Open the HTML file

Find the text

Change it between the <tag> and </tag>

Edit Colors
Find CSS like this and change the hex color:

css
.status-working-op { color: #66d9a0; }
Common colors:

#ff0000 = Red

#00ff00 = Green

#0000ff = Blue

#ffff00 = Yellow

#ffffff = White

#000000 = Black

Add Emojis
Use any emoji in text:

html
🚀 Launch
🎮 Game
📜 Script
🔒 Locked
⭐ Star
🚀 6. Publishing Changes
Update Your Website
Make changes to files

Click "Commit changes" on GitHub

Wait 1-2 minutes

Refresh your website

Your Website URL
text
https://Scripter-Coder.github.io/Scripter-Hub-Website/
❓ 7. Troubleshooting
Images Not Showing
✅ Check path: "Images/YourGame.png"

✅ Verify image is in Images/ folder

✅ Check file extension (.png, .jpg)

✅ Refresh page (Ctrl+F5)

Button Not Working
✅ Check href="..." points to correct file

✅ Remove disabled and btn-locked for unlocked buttons

✅ Verify file exists

Changes Not Showing
✅ Wait 1-2 minutes for GitHub Pages

✅ Clear browser cache (Ctrl+Shift+R)

✅ Check you committed changes

Search Bar Not Finding Scripts
✅ Script is in scriptsData array

✅ No extra commas in array

✅ Check spelling

Script Copy Not Working
✅ Script URL is valid

✅ Uses loadstring(game:HttpGet("..."))()

📝 8. Quick Reference
File Purposes
File	Purpose
index.html	Main landing page
status.html	Scripts & Executors status
scripts.html	Script library with search
Button Actions
Button	Action
🎮 Game	Opens Roblox game page
📋 Script	Copies script to clipboard
▶️ YouTube	Opens YouTube channel
💬 Discord	Opens Discord server
Status Page Colors
Status	Color
Working | OP ⭐	🟢 Green-Aqua
Working (EXPERIMENTAL)	🟡 Dark Yellow
Soon	🟣 Purple
Not Working	🔴 Red
Working	🟢 Green
Updating	🟡 Yellow
Discontinued	🔵 Blue
Executor Status
Symbol	Meaning
🟢	Working/Online
🔴	Down/Not working
🔵	Unknown
🎯 9. Common Tasks Checklist
Add a New Script
Upload image to Images/ folder

Add script entry in scriptsData (scripts.html)

Add script entry in status page (status.html)

Commit changes

Test on live website

Change a Script's Status
Update in status.html (change the status- class)

Update in scripts.html (change the status field)

Commit changes

Add a New Button
Add button HTML to index.html

Create target page (if new)

Link with href="page.html"

Commit changes

Documentation Version: 1.0
Created: 2026
Website: ScripterHub
