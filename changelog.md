# Changelog
All notable changes to this Minecraft 1.21.11 PvP/Optimization client will be documented here.  
This project follows Semantic Versioning: **MAJOR.MINOR.PATCH**
 
---
 
# [1.0.3] - 2026-05-08
 
## ⚡ Performance Improvements
- Optimized HUD rendering with minimal text-only displays (no panels/shadows for FPS/Ping)
- Reduced visual clutter by removing complex HUD modules by default
- Streamlined Title Screen to remove excessive visual effects
 
## 🎯 PvP Features
- **Reach Highlight HUD**: Completely redesigned with animated pulsing ring around crosshair
  - Distance-based color coding (red = closest, green = farthest)
  - Ring only appears when aiming at target (within 30° of crosshair)
  - Shows target name when within 2 blocks
  - Smooth sine-wave pulse animation
- **Arrow Count HUD**: Shows total arrows in inventory (PvP essential)
- **Held Item Durability HUD**: Shows durability of currently held item with color coding
  - Green (50%+ durability), Yellow (25-50%), Red (<25%)
- **Crit Visuals**: Visual feedback system for critical hits
- **W-Tap Helper**: Sprint reset assistance for PvP
 
## 🖥️ HUD Modules Added
- **ReachHighlightHUD**: Distance-aware target indicator with ring animation
- **ArrowCountModule**: Inventory arrow counter
- **HeldItemDurabilityModule**: Real-time durability display
- **FpsCounterModule**: Minimal text FPS display with color coding
- **PingHudModule**: Text-based ping display
- **PingGraph**: Historical ping visualization
- **CritVisualsModule**: Critical hit feedback system
 
## 🧠 Engine / System Tweaks
- **ModuleManager Refactor**: Separated HUD-visible modules from background-only modules
  - HUD modules appear in drag-drop editor (H key)
  - Background modules run without visual representation
- **Config System**: Added comprehensive settings for all new features
  - All PvP features enabled by default
  - Non-essential features disabled by default
- **Removed MouseMixin**: Fixed crash by removing problematic mixin
 
## 🎨 UI / UX
- **Title Screen**: Simplified to minimal clean design
  - Reduced color palette to blue/gray theme
  - Removed complex visual effects (aurora, scan lines, glitches)
  - Clean button styling with minimal accent colors
- **Right Shift Menu (IllusionMenuScreen)**: Reorganized and simplified
  - Reduced panel size: 440×400 → 400×350
  - Three organized tabs: COMBAT, VISUALS, ENGINE
  - Removed emoji icons from tab labels
  - Simplified color scheme (blue accent instead of purple)
  - Added all new PvP features to appropriate tabs
- **HUD Layout**: Compact positioning for minimal screen coverage
  - Top-left: FPS, Ping, Arrow Count, Pearl/Rod Cooldowns
  - Bottom-left: KeyStrokes
  - Right side: Target HUD, Item Durability
 
## 🛠 Bug Fixes
- Fixed Reach Highlight to only show when actually aiming at target
- Fixed various HUD positioning conflicts
- Fixed Title Screen color compatibility issues
 
## 🧹 Removed / Deprecated
- **CPS Counter**: Removed from HUD registration (unreliable measurement)
- **Coordinates HUD**: Removed (not needed for PvP)
- **Timer HUD**: Removed (not needed for PvP)
- **Speed HUD**: Removed (not needed for PvP)
- **Sprint Indicator**: Removed (not needed for PvP)
- **Biome HUD**: Removed (not needed for PvP)
- **Pearl Cooldown HUD**: Removed due to Minecraft API incompatibility
- **Rod Cooldown HUD**: Removed due to Minecraft API incompatibility
- **Hotbar Scroll Protection**: Removed due to private field access issues
- **Complex Title Screen Effects**: Removed aurora, scan lines, glitches, orb particles
- **Non-essential HUDs**: Disabled by default (Target HUD, Inventory HUD, Armour HUD, Potion HUD)
 
---
 
# [1.0.2] - 2026-05-04
 
## ⚡ Performance Improvements
- Optimized JAR file size by removing embedded texture resources (prevents memory/GPU crashes)
- Reduced texture atlas load time on startup
 
## 🎯 Input & Responsiveness
(No changes in this version)
 
## 🖥️ Rendering & Visual Optimization
- Removed problematic Armor Texture mixin (caused black screen crashes in 1.21.11)
- Removed built-in resource pack registration (Fabric API incompatibility, caused startup failures)
 
## 🧠 Engine / System Tweaks
- Resource Manager now uses external pack fallback (manual resource pack enabling)
- Added `disableDamageTilt` config option (defaults to `true`)
- Simplified texture loading to prevent EXCEPTION_ACCESS_VIOLATION crashes
 
## 🎨 UI / UX
- Increased menu panel height to fix toggle overflow in VISUALS tab
- Removed non-functional texture toggles (blocks/items/fonts/armor) from UI
- Cleaned up menu to only show working features
 
## 🌐 Networking / Ping Stability
(No changes in this version)
 
## 🛠 Bug Fixes
- Fixed black screen crash caused by ArmorTextureMixin injection failure
- Fixed GPU memory crash from embedded high-res textures (91MB PvP pack)
- Fixed Smooth FPS to respect configured `frameCap` instead of hardcoded 60
- Fixed font path errors (invalid path: `illusion:font/` → moved to `minecraft:font/`)
- Fixed corrupted PNG texture signatures (removed broken bed textures)
 
## 🧹 Removed / Deprecated
- **ArmorTextureMixin**: Removed due to Minecraft 1.21.11 API incompatibility (no matching method `getTexture`)
- **Built-in Resource Pack**: Removed automatic pack registration (Fabric 1.21.11 unreliable)
- **Embedded Textures**: Removed 300+ embedded textures causing GPU crashes
  - PvP pack textures (blocks, items, font)
  - Armor pack textures
- **Resource Pack Toggles**: Removed from UI (blocks, items, fonts, armor, GUI toggles)
  - Use external resource packs instead: `§7§lPVP-zegarn (1.21.9-1.26).zip` 
  - Armor pack: `Swight_armour_pack.zip` (enable manually in Options → Resource Packs)
- **ResourcePackMixin**: Removed unused mixin class
- **ArmorTextureMixin entry**: Removed from `illusionclient.mixins.json` 
 
---
 
# [1.0.1] - Previous Release
 
## ⚡ Performance Improvements
- Added FPS Boost mode toggle (disables entity shadows & clouds)
- Added Smooth FPS option for frame pacing
- Added Entity Culling toggle for render optimization
 
## 🎯 Input & Responsiveness
(No changes in this version)
 
## 🖥️ Rendering & Visual Optimization
- Added Fullbright toggle for maximum brightness
- Added Hit Flash effect toggle
- Added Custom Hit FX toggle
 
## 🧠 Engine / System Tweaks
- Refactored module registration system to separate HUD-visible vs background-only modules
- Auto-sprint now runs as background feature (no HUD positioning needed)
 
## 🎨 UI / UX
- Complete Title Screen redesign: Scrolling starfield background, parallax effect, modern white button styling with colored accent bars
- Complete Menu Screen redesign (Right Shift):
  - New 440×320 panel layout with sidebar tabs
  - Three organized categories: ⚔ COMBAT, 🎨 VISUALS, ⚡ ENGINE
  - Smooth animated toggles with lerp transitions
  - Clean dark theme with purple accent colors
  - Removed problematic scale animations (API compatibility)
  - Standardized button sizing (200×28) and spacing
  - Updated footer text styling with fade-in animations
 
## 🌐 Networking / Ping Stability
(No changes in this version)
 
## 🛠 Bug Fixes
- Fixed config field name references (case sensitivity: fullbright, smoothFPS, fpsBoostMode)
- Fixed clearAndInitWidgets() compatibility issue (changed to clearChildren())
- Fixed MatrixStack.scale() API incompatibility by removing transform operations
 
## 🧹 Removed / Deprecated
- HUD Changer (H key): Removed non-positionable modules from drag-drop editor:
  - Armor Customization (auto-enabled background feature)
  - Weapon Customization (auto-enabled background feature)
  - Auto-sprint (always-on utility)
- Removed unused palette constants (C_GLASS, C_BTN_BASE, C_BTN_OUTLINE, etc.)
- Removed grid background effect from title screen (simplified to stars only)
- Removed chromatic glitch logo effect
 
---
