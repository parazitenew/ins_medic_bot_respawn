# ins_medic_bot_respawn
Insurgency (2014) plugin to add MEDIC feature and bots reinforcement
# Improved Medical & Bot Reinforcement Plugin (Fork of Jared Ballou's Plugin)

This plugin is a modified and improved version of the original plugin created by **Jared Ballou** and improved by **Naong**.  
I decided to create this fork because I encountered several issues with the original version on my server, especially regarding message display and overall clarity.

---

## ✨ Why This Fork Exists

While using the original plugin, I experienced a few problems that affected gameplay and server usability:

### **1. Reinforcement Timer Message Would Never Disappear**
The plugin displays reinforcement information (enemy bot wave timer).  
Originally:
- The message appeared **every 10 seconds**.
- The message itself **stayed on screen for 10 seconds**.
- Result: the message **never disappeared**, permanently blocking the center of the screen.

### **2. Reinforcement Message Was Only Displayed in the Center of the Screen**
The information was not visible in the chat at all, which made it annoying for players and created visual clutter.

### ✔️ What I changed
- Increased the reinforcement update interval from **10 seconds to 30 seconds**.
- Disabled the **center-screen hint text** for regular updates.
- Reinforcement info now appears **in the chat** instead of blocking the middle of the screen.
- When reinforcements are **less than 10 seconds away**, the countdown:
  - appears **every second**
  - shows up **in the center of the screen**, so players clearly notice it.

This keeps the screen clean while still warning players when it actually matters.

---

## ✨ Additional Improvements

### **3. Plugin Renamed for Better Clarity**
The original plugin’s name did not include any reference to “medic”, “healing”, or “reinforcements”.  
It took me **weeks** to find a functioning medic plugin simply because its filename gave no indication of what it actually did.

To fix this, I renamed the plugin so its purpose is **clear and intuitive**.

### **4. Two Main Features in One Plugin**
This plugin provides:
- **A medic system**: allowing the Medic class to heal teammates.
- **A reinforcement system**: spawning enemy bot waves based on configurable timers.

The new name reflects both functions, making the plugin easy to find and understand.

---

## 📁 Installation

Installation is very simple:

1. Download the release archive or clone the repository.
2. **Keep the exact folder structure provided** in this repository.
3. You need the plugins folder with both .smx files, the gamedata and the translations. The configuration file of the plugin will be generated in **........./nsurgency/cfg/sourcemod/respawn.cfg** once you start the server.

## 🛠️ Compilation

Compile using the standard SourceMod compiler (`spcomp`), or use the compiler included with your server.  
Only the main `.sp` file needs to be compiled.  
Includes are already provided or referenced correctly in the repository.

---

## 🙏 Credits

- Original plugin by **Jared Ballou**
- Contributor: (Daimyo, naong, parazitenew (Imed))

---

## 📜 License

This fork respects the original plugin’s license.  
You may modify and redistribute it as long as credit is preserved.

