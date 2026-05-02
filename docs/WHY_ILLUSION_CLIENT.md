# 💠 Why Illusion Client

<div align="center">

![Java](https://img.shields.io/badge/Java-17+-orange?style=flat-square)
![Minecraft](https://img.shields.io/badge/Minecraft-1.21.11-brightgreen?style=flat-square)
![Engine Optimized](https://img.shields.io/badge/Engine-Optimized-8A2BE2?style=flat-square)
![PvP Focused](https://img.shields.io/badge/PvP-Focused-FF5555?style=flat-square)

**A next‑generation performance & PvP client engineered for Minecraft 1.21.11**

</div>

---

## 📌 Overview

Illusion Client is **not** a modpack, preset, or template.  
It is a **fully engineered Fabric client** built for players who take PvP seriously — with real engine‑level optimizations, real mixins, real UI code, and real anti‑tamper protection.

Where other clients flip a few settings, Illusion Client modifies the **actual game engine** and UI pipeline to deliver measurable, repeatable improvements you can feel in combat.

---

## ⚡ Engine‑Level Performance (Real Optimizations)

Illusion Client implements **real engine changes**, not placebo toggles.

### ✔ ParticleEngineMixin  
Caps particle creation at runtime → **instant GPU relief**.

### ✔ LevelRendererMixin (Entity Culling)  
Skips rendering entities outside the frustum → **real FPS gains** in crowded areas.

### ✔ GameRendererMixin (Fullbright)  
Overrides gamma at the engine level → **clean, stable fullbright**.

### ✔ FpsBoostModule  
Writes directly to Minecraft’s internal options API for 1.21.11:
- Clouds  
- Shadows  
- Smooth lighting  
- Particle mode  
- Lighting engine toggles

These are **engine calls**, not UI tricks.

---

## 🎯 PvP Modules Built in Real Java

Every PvP feature is a real class with real logic — not a preset or overlay.

- CPS Counter  
- Keystrokes HUD  
- Armour Durability  
- Potion Timer  
- Reach Display  
- Sprint Toggle  
- Combo Counter (event‑driven)  
- Hit Flash (mixin‑based)

Modules read **live game values** and update in real time.

---

## 🎨 A Custom UI Framework (Not a Template)

Illusion Client ships a hand‑coded UI system with production polish:

- Animated Right‑Shift menu  
- Violet active‑tab underline  
- Lerp‑animated toggle pills  
- Hover highlights  
- Smooth open animation (scale + alpha)  
- Updated drawText usage for 1.21.11  
- Full settings architecture (IllusionConfig)

It looks and feels like a native client UI, not a copied template.

---

## 🧠 Smart Configuration System

- **Gson‑backed config** stored in `.minecraft/illusion/`  
- Auto‑save on every toggle  
- Per‑module settings and profiles  
- Real‑time updates — no restart required

This behaves like a proper application configuration system.

---

## 🛡️ Anti‑Copying Protection (Real IP Protection)

Illusion Client includes multiple protection layers to protect your compiled builds:

### 🔐 ProGuard Obfuscation  
Class and method names are obfuscated; line numbers removed.

### 🔑 XOR String Encryption  
Visible strings are stored encrypted and decoded at runtime.

### 🧬 Cryptographic Watermark  
Each build contains a SHA‑256 fingerprint tied to your private seed and build metadata so you can prove ownership.

These measures protect the distributed JAR from trivial copying and decompilation.

---

## 🧱 Built for Minecraft 1.21.11

This release is targeted and tested for:

- **Fabric Loader:** 0.18.4  
- **Fabric API:** 0.141.1+1.21.11  
- **Loom:** 1.14  
- **Yarn:** 1.21.11+build.1

All API changes for 1.21.11 have been handled (HudRenderCallback, Options API, drawText signature, gamma API, etc.).

---

## 🔧 Fully Implemented Features

### ✔ Working now
- FPS Boost  
- Particle limiter  
- Fullbright  
- Sprint toggle  
- Zoom  
- HUD modules (FPS, Ping, CPS, Keystrokes)  
- Config system  
- UI animations

### ✔ Completed fixes
- Entity culling with frustum check  
- Frame cap slider UI and logic  
- Smooth FPS smoothing logic  
- Chunk animation toggle  
- Combo counter event hook  
- Hit flash effect  
- Custom crosshair rendering

Everything in the menu now performs the action it advertises.

---

## 🛠️ Developer‑Grade Build System

- Full Gradle project with Loom  
- ProGuard integration for obfuscation  
- Mixins and fabric.mod.json  
- IntelliJ project structure and genSources steps  
- Build tutorial and troubleshooting guide  
- Version‑locked dependencies for reproducible builds

This is a professional codebase, not a hobby folder.

---

<div align="center">

**🔥 Built for players who take PvP seriously.**

</div>
