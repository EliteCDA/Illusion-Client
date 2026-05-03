# ILLUSIONCLIENT — PROPRIETARY LICENSE

**Version:** 1.0.0  
**Platform:** Minecraft 1.21.11 • Fabric Mod  
**Copyright:** © 2026 IllusionDev — All Rights Reserved  
**Status:** CONFIDENTIAL LEGAL DOCUMENT

---

## NOTICE

This is a **proprietary software license**. You may use the compiled software, but you may not copy, modify, distribute, or access the source code.

By installing, downloading, or using IllusionClient, you expressly agree to all terms and conditions outlined below. If you do not agree, you must cease all use immediately.

---

## 1. DEFINITIONS

For clarity, the following terms are defined as follows:

- **"Software"** — The IllusionClient Fabric mod, including all compiled JAR files, binaries, and executable code.
- **"Source Code"** — All Java source files, configuration files, design documents, and architectural specifications.
- **"Derivative Works"** — Any modified version, fork, port, or adaptation of the Software or its components.
- **"IllusionDev"** — The original author and copyright holder of the Software.
- **"User"** or **"You"** — Any individual or entity that downloads, installs, or uses the Software.
- **"Compiled JAR"** — The distributed, obfuscated binary form of the Software.
- **"Unauthorized Access"** — Any attempt to reverse engineer, decompile, or inspect the Software beyond normal gameplay use.

---

## 2. OWNERSHIP & COPYRIGHT

IllusionClient ("the Software") is an original work created exclusively by IllusionDev.

Ownership includes, but is not limited to:

- All source code and compiled bytecode
- All configuration files and resources
- All GUI layouts, HUD systems, and module designs
- All algorithms, logic, and architecture
- All documentation and design specifications

**Copyright © 2026 IllusionDev. All Rights Reserved.**

The Software is protected under international law, including:

- The Berne Convention for the Protection of Literary and Artistic Works
- The Digital Millennium Copyright Act (DMCA), 17 U.S.C. § 1201
- The UK Copyright, Designs and Patents Act 1988
- EU Directive 2009/24/EC on Software Protection
- All applicable national copyright and intellectual property laws

---

## 3. PROTECTED WORKS

The following components are protected intellectual property and may not be reused, modified, or distributed without written consent.

### 3.1 Source Code

- Java source files under `com.illusion.client.*`
- Mod entry point and lifecycle code
- IllusionConfig system and configuration handlers
- IllusionMenuScreen GUI system with animations
- All Mixin classes and mixins
- HudModule base class and HudRenderer architecture
- PvP modules (CPS Counter, Keystrokes, Armour Durability, Potion Timer, Reach Display, Sprint Toggle, Combo Counter)
- Performance modules (FPS Boost, FPS Counter, Ping HUD)
- Security package (XOR encryption, watermark system, anti-tampering mechanisms)

### 3.2 Architecture & Design

- Two-tab animated toggle-pill menu design
- HudModule/HudRenderer architecture and interaction patterns
- ModuleManager system and module loading pipeline
- JSON configuration schema and format
- XOR string obfuscation algorithm and implementation
- SHA-256 build watermarking and verification system

### 3.3 Build Configuration

- Gradle build scripts and configurations
- ProGuard obfuscation pipeline and automation
- ProGuard obfuscation rules and optimization rules
- Fabric mod descriptor (`fabric.mod.json`)
- Mixin configuration files

---

## 4. PROHIBITED ACTIONS

The following actions are **strictly prohibited** without prior written consent from IllusionDev:

- Copying or duplicating any part of the source code
- Decompiling, disassembling, or reverse engineering the compiled JAR
- Using decompiled or reverse-engineered code in any form
- Creating derivative works, including forks, ports, or modified versions
- Distributing, selling, or sublicensing the Software
- Removing, disabling, or bypassing the watermark or protection systems
- Publishing, sharing, or leaking the source code
- Rebranding the Software or removing copyright notices
- Reusing GUI design, HUD layout, color scheme, or visual elements
- Using the Software as a reference implementation for similar projects
- Circumventing technical protection measures (TPMs)
- Uploading the Software to public mod repositories without permission
- Using the Software on public servers or commercial game servers

**Any violation of these terms constitutes copyright infringement and may result in legal action, injunctions, and statutory damages.**

---

## 5. PERMITTED ACTIONS

The following uses are **explicitly permitted**:

- **Personal Use:** Installing and using the compiled JAR for private, single-player gameplay
- **Private Server Use:** Using the Software on private servers where you hold administrative control (not public or commercial servers)
- **Personal Sharing:** Sharing the compiled JAR (unmodified) with personal friends or family for personal use only, provided this license remains intact and visible
- **Bug Reports:** Reporting bugs, security vulnerabilities, or issues to IllusionDev
- **Content Creation:** Creating videos, screenshots, livestreams, or streams featuring the Software for entertainment purposes
- **Commentary & Review:** Referencing the Software by name in reviews, commentary, or discussion

**Important:** Any use not explicitly listed as permitted is prohibited.

---

## 6. TECHNICAL PROTECTION MEASURES (TPMs)

IllusionClient includes multiple technical protection measures designed to prevent unauthorized copying and modification:

### 6.1 Cryptographic Watermark

Each build contains a unique SHA-256 fingerprint that:
- Survives decompilation and repacking
- Identifies the exact build version and release date
- Is verified against known legitimate builds
- Triggers warnings if tampering is detected

### 6.2 String Encryption

- All string constants are XOR-encrypted using a multi-fragment private key
- Encryption prevents static analysis of code functionality
- Keys are distributed in a manner that prevents extraction

### 6.3 ProGuard Obfuscation

- The compiled JAR is heavily obfuscated to prevent reverse engineering
- Method names, class names, and variable names are scrambled
- Control flow is modified to prevent analysis
- Obfuscation rules are proprietary and not disclosed

### 6.4 Anti-Tampering Detection

- The Software verifies its own integrity on startup
- Modified or repacked JARs are detected and flagged
- Unauthorized modifications may trigger safeguards

**DMCA Compliance:** Circumventing, disabling, or attempting to bypass any TPM is a separate and independent legal violation under the Digital Millennium Copyright Act, 17 U.S.C. § 1201, with penalties of $200–$2,500 per work, regardless of whether copyright infringement occurs.

---

## 7. LICENSE REVOCATION & SUSPENSION

IllusionDev reserves the absolute right to revoke or suspend this license at any time for:

- Violation of any term in this license
- Reverse engineering or decompilation attempts
- Unauthorized distribution or modification
- Use on public or commercial servers
- Circumventing technical protections
- Any other misuse as determined by IllusionDev

**Revocation is effective immediately upon notice.** Upon revocation, all rights to use the Software terminate immediately, and you must cease all use and delete all copies of the Software in your possession.

---

## 8. DISCLAIMER OF WARRANTIES

THE SOFTWARE IS PROVIDED **"AS-IS"** WITHOUT WARRANTIES OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO:

- Warranties of merchantability
- Warranties of fitness for a particular purpose
- Warranties of non-infringement
- Warranties of uninterrupted service or availability

**IllusionDev makes no guarantee that:**

- The Software will function without errors or interruptions
- The Software will be compatible with all Minecraft versions or mod loaders
- The Software will not conflict with other mods
- Your account will not be flagged or banned by anti-cheat systems
- Any data or configurations will be preserved

**Your use of the Software is at your own risk.**

---

## 9. LIMITATION OF LIABILITY

**IN NO EVENT SHALL ILLUSIONCLIENT OR ILLUSIONCLIENT BE LIABLE FOR:**

- Indirect, incidental, consequential, special, or punitive damages
- Loss of data, saves, or user accounts
- Loss of revenue, profits, or goodwill
- Account bans, suspensions, or restrictions
- Damage to hardware or software
- Third-party claims or disputes

**This limitation applies even if IllusionDev has been advised of the possibility of such damages.**

---

## 10. ENFORCEMENT & LEGAL REMEDIES

IllusionDev reserves the right to enforce these terms through any legal means, including:

- DMCA takedown notices and demands
- Removal of infringing copies from hosting platforms
- Civil litigation and injunctive relief
- Recovery of statutory damages ($150–$30,000 per work, or up to $150,000 for willful infringement)
- Recovery of actual damages and profits from infringement
- Recovery of legal fees and court costs
- Reporting violations to law enforcement agencies
- Platform reporting and account suspension cooperation

### Evidence of Ownership

IllusionDev retains exclusive ownership evidence including:

- Original source code repositories and version history
- Build logs and release records
- Private watermark seeds and verification keys
- Original design documents and architectural specifications

---

## 11. DMCA PROCEDURE & TAKEDOWN NOTICES

If you discover an unauthorized copy or derivative work of IllusionClient, you may report it via DMCA or contact IllusionDev directly.

A valid DMCA notice must include:

- Identification of the copyrighted work (IllusionClient, version number)
- URL or identification of the infringing material
- Build fingerprint or watermark evidence (if available)
- Your contact information (name, email, phone)
- Statement of good-faith belief that use is unauthorized
- Statement of accuracy under penalty of perjury
- Your signature (physical or electronic)

**DMCA notices may be submitted to:** Discord: **elite_original**

Platforms receiving valid DMCA notices must act promptly under 17 U.S.C. § 512(c) and the EU Copyright Directive.

---

## 12. THIRD-PARTY COMPONENTS

IllusionClient incorporates third-party components under their respective open-source licenses. These licenses apply **only** to their respective components and do not extend to IllusionClient's original code.

| Component | License | Copyright |
|-----------|---------|-----------|
| Minecraft | Proprietary EULA | © Mojang Studios / Microsoft Corporation |
| Fabric Loader | Apache 2.0 | © Fabric Project |
| Fabric API | Apache 2.0 | © Fabric Project |
| Yarn Mappings | CC0 (Public Domain) | © Fabric Project |
| Mixin | MIT | © SpongePowered |
| Gson | Apache 2.0 | © Google |
| ProGuard | GPLv2 | © Yakov Fain |
| LWJGL | BSD-3-Clause | © Lightweight Java Game Library |

**IllusionDev's copyright applies exclusively to original code not covered by the above licenses.**

---

## 13. MINECRAFT EULA & PLATFORM COMPLIANCE

This license operates independently but does **not override** Minecraft's End User License Agreement (EULA) or any platform's Terms of Service.

You must comply with:

- **Minecraft EULA:** Modifications (including mods) are permitted for personal use only under Mojang's EULA
- **Microsoft Services Agreement:** All Minecraft-related terms and policies
- **Platform-Specific Terms:** Terms of your game launcher (Fabric, MultiMC, CurseForge, etc.)
- **Server Rules:** Rules of any server or community where you use the Software

If this license conflicts with any platform policy, the most restrictive terms apply.

---

## 14. GOVERNING LAW & JURISDICTION

This License is governed by the laws of the **United Kingdom**, specifically England and Wales, without regard to conflicts of law principles.

All legal proceedings, disputes, and claims arising from this License or the use of the Software shall be:

- **Exclusive Jurisdiction:** Brought exclusively in the courts of England and Wales
- **Venue:** Subject to the exclusive venue of the High Court of Justice or Courts of England and Wales
- **Dispute Resolution:** Any party waives the right to jury trial

By using IllusionClient, you consent to personal jurisdiction and venue in these courts.

---

## 15. COMPLIANCE AUDIT & INSPECTION

IllusionDev reserves the right to audit your use of the Software to ensure compliance with this license.

**Upon reasonable written notice, you agree to:**

- Provide evidence of authorized use and installation
- Allow inspection of the Software installation directory
- Certify in writing that no unauthorized modifications, copies, or distributions have occurred
- Respond to compliance inquiries within 14 calendar days

**Failure to comply with an audit request within 14 days constitutes a material breach of this license and may result in immediate revocation.**

---

## 16. SEVERABILITY

If any provision of this License is found to be invalid, unenforceable, or illegal by a court of competent jurisdiction, that provision shall be modified to the minimum extent necessary to make it valid and enforceable, or severed from this License.

All other provisions remain in full force and effect.

---

## 17. ENTIRE AGREEMENT

This License constitutes the entire agreement between you and IllusionDev regarding the Software. It supersedes all prior negotiations, agreements, and understandings, whether written or oral.

No modification, waiver, or amendment to this License is valid unless made in writing and signed by both parties.

---

## 18. CONTACT & SUPPORT

For inquiries, licensing requests, or DMCA notices, contact:

**IllusionDev**  
Discord: **elite_original**
Discord Server: https://discord.gg/99fyCrFUxg

---

## FINAL NOTICE

**By installing, downloading, copying, or using IllusionClient, you acknowledge that:**

1. You have read and understood all terms in this License
2. You agree to be bound by all provisions herein
3. You understand the legal consequences of violations
4. You take full responsibility for your use of the Software
5. You will not hold IllusionDev liable for any damages

**Unauthorized use, modification, distribution, reverse engineering, or circumvention of technical protections is strictly prohibited and will be vigorously enforced.**

---

**END OF LICENSE**

*Last Updated: May 2, 2026*  
*Version: 1.0.0*
