# Artemis to RPCS3 Patch Converter

**Community-driven Artemis → RPCS3 YAML patch converter.**

> Chicago Dreams. Global Knowledge.

---

## 🚀 Project Status

**Current:** Alpha  
**Next Release:** 🔥 **Version 1.0 — Coming Soon**

Version 1.0 will mark the first stable community release of this tool, focused on reliability, clarity, and open knowledge sharing.

---

## 🌍 Mission

This project exists for one simple reason:

> **Emulation knowledge belongs to everyone.**

No gatekeeping.  
No paywalls.  
No locked communities.

This tool is built to help convert Artemis NCL cheat databases into modern **RPCS3 1.2 YAML patch format**, making PS3 cheat research accessible to everyone.

---

## 🎯 What This Tool Does

- Converts Artemis `.ncl` cheat files to RPCS3 YAML patch format  
- Supports multiple game serials and versions  
- Preserves cheat names, structure, and metadata  
- Allows optional PPU hash usage  
- Enables bulk database importing  
- Creates clean, readable RPCS3-compatible patch files  

---

## 🛠 Supported Platforms

- RPCS3 (PS3)
- Artemis Cheat Databases
- Future expansion planned

---

## 📦 Planned for Version 1.0

✔ Plugin-ready architecture  
✔ Cleaner UI layout  
✔ Improved database handling  
✔ Better YAML validation  
✔ Community template support  
✔ Documentation polish  
✔ Bug fixes and stability pass  

---

## 🧠 Philosophy

This is not just a converter.

This is a **learning tool**, a **research platform**, and a **community foundation** for PS3 emulation cheat development.

Every feature is built to help users understand what they are converting — not just press a button.

---

## 📂 Example YAML Output

```yaml
PPU-0000000000000000000000000000000000000000:
  "Infinite Health":
    Games:
      "Example Game":
        BLUS12345: ["01.00"]
    Author: "Community"
    Notes: "Converted from Artemis NCL format"
    Patch Version: "1.2"
    Patch:
      - [ be32, 0x00123456, 0x60000000 ]

---

##🤝 Community

YouTube: Chidreams Emulation Gameplay](https://www.youtube.com/c/ChidreamsEmulationGamePlay

GitHub: https://github.com/chidreams

Discord: discord.gg/CUUva5FPzu

---

##🔥 Version 1.0 Vision

Version 1.0 is not about perfection.

It’s about giving the community a solid foundation to grow from.

---

##📜 License

MIT License — Free for community use.
