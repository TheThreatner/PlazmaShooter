# PLAZMA SHOOTER – A SCIENCE OF DESTRUCTION

> **A complete browser-based shoot 'em up** – harness the power of plasma, master elemental hazards, and neutralize the four corrupted facilities of AXIOM Corp.

![Game Banner](https://via.placeholder.com/800x200?text=PLAZMA+SHOOTER+%7C+SCIENCE+OF+DESTRUCTION)

## 📖 About the Game

**Year 2157.** PLAZMA INSTITUTE has weaponized the fundamental laws of physics, chemistry, and biology. Their arsenal includes electromagnetic horrors, caustic abominations, and living biological nightmares. One soldier remains. One plasma weapon. One mission.

*Code Name: **ODIN** – enter four increasingly twisted stages, defeat unique bosses, and experience an ending that questions the cost of victory.*

> ⚠️ **Disclaimer** – This game contains fictional science/biology concepts, intense action, and stylized violence. All enemy names and scenarios are entirely fictional. Some references are intentional (and appreciated). Others are unintentional (also appreciated).

## ✨ Features

- **4 Distinct Stages** – Factory Breach → Electric Domain → Chemical Laboratory → Biological Core  
- **Unique Enemy Types** – Grunts, Orb Casters, Laser Mechs, Flamethrower Heavies, Acid Throwers, Rock Golems, Toxic Summoners, and more  
- **3 Brutal Bosses** – **PKING** (physics overlord), **CKING** (chemistry alchemist), **BKING** (bio‑horror)  
- **Challenging Status Effects** – Magnetisation, Freeze, Blindness, Nuclear Bomb, Oxidiser (instant death)  
- **Wave‑Based Combat** – Each stage features multiple waves leading to a climactic boss fight  
- **Autosave & Continue** – Progress is automatically saved after each stage  
- **Fully Adjustable Settings** – Graphics quality, scanlines, particles, master/BGM/SFX volume  
- **Immersive Visuals** – Stage‑specific backgrounds, dynamic particle system, damage numbers, kill flashes, and cinematic death animations (nuclear shredding / oxidisation)  
- **High‑Fidelity Audio** – Placeholder music & sound effects system (Web Audio API) – ready for your own `.mp3` / `.wav` files  

## 🎮 How to Play

### Controls

| Action           | Keys                     |
|------------------|--------------------------|
| Move Left        | `A` or `←` arrow key     |
| Move Right       | `D` or `→` arrow key     |
| Shoot            | `SPACE` or `Z`           |
| Pause / Resume   | `ESC`                    |

### Core Mechanics

- **Survive waves** – Eliminate all enemies in a wave to progress.  
- **Boss Fights** – Bosses have unique attack patterns and special projectiles.  
- **Status Effects**  
  - *Magnetised* – Knife projectiles track your position.  
  - *Frozen* – Movement locked, periodic damage.  
  - *Blind* – Screen obscured for several seconds.  
  - *Nuclear Bomb / Oxidiser* – Instant death on contact (dodge at all costs).  
- **Health & Score** – Your health bar appears at the top. Scoring adds 10 points per hit, 100 per kill.  
- **Autosave** – After completing a stage, your progress is saved. Use **Continue** from the main menu.

## 🛠 Installation & Setup

### Option 1: Click this link

### Option 2: Quick Start (No Audio)

1. Download or copy the `index.html` file to your computer.  
2. Double‑click the file – it will open in your default web browser.  
3. *Note*: Audio will be missing unless you supply the files (see below). The game will run fine without sound, just no SFX/BGM.

### Option 3: Full Experience (with Audio)(later we're still working on it)

Because the game uses the `fetch` API to load audio files, you need to serve the file through a local web server (otherwise CORS restrictions may block audio).

#### Steps

1. Place the `index.html` inside an empty folder.  
2. Create a subfolder named **`audio`** inside that folder.  
3. Add the required audio files (see **Audio File Reference** below).  
4. Start a local HTTP server from that folder:
   ```bash
   # Python 3
   python -m http.server
   
   # or with Node.js (http-server package)
   npx http-server
   ```
5. Open your browser and navigate to `http://localhost:8000` (or the port shown).  
6. Enjoy the full audiovisual experience!

### Audio File Reference

Place the following files inside the `/audio/` directory:

**BGM (background music)** – `.mp3` or `.wav`  
- `menu_bgm.mp3`  
- `story_clip_bgm.mp3`  
- `stage1_bgm.mp3`  
- `stage2_bgm.mp3`  
- `stage3_bgm.mp3`  
- `stage4_bgm.mp3`  
- `pking_theme.mp3`  
- `cking_theme.mp3`  
- `bking_theme.mp3`  
- `end_clip_bgm.mp3`  
- `finish_screen_bgm.mp3`  

**SFX (sound effects)** – `.wav` (preferred)  
- `button_click.wav`  
- `loading_screen.wav`  
- `autosave_notification.wav`  
- `player_shoot.wav`  
- `player_hurt.wav`  
- `electric_orb.wav`  
- `laser_beam.wav`  
- `flamethrower.wav`  
- `blackhole.wav`  
- `nuclear_bomb.wav`  
- `toxic_cloud.wav`  
- `acid_bottle.wav`  
- `rock_impact.wav`  
- `powder_effect.wav`  
- `blindness_effect.wav`  
- `oxidiser.wav`  
- `bacterial_cloud.wav`  
- `snake_attack.wav`  
- `boss_death.wav`  
- `body_deform.wav`  
- `oxidisation.wav`  

> **Tip**: If any file is missing, the game will silently skip that sound – it does not crash. You can add your own custom sounds (keep the same filenames).

## 🖥️ Browser Compatibility

- **Modern browsers required** – Chrome, Firefox, Edge, Safari (latest versions).  
- **WebGL / Canvas 2D** – No external libraries.  
- **Web Audio API** – Needed for sound.  
- **LocalStorage** – For save/continue feature.  

## 🧪 Development Notes

- The entire game is **self‑contained** in a single HTML file (~1000+ lines of CSS, HTML, and JavaScript).  
- Written in **vanilla JavaScript** – no frameworks, no build steps.  
- **Particle system** runs on a separate canvas for performance.  
- **Graphics quality** settings adjust particle counts and scanlines.  
- The game engine includes:  
  - Frame‑based animation loop  
  - Collision detection (AABB & circle)  
  - State management (menu, disclaimer, story, running, pause, death, finish)  
  - Custom death sequences for nuclear and oxidiser kills  
- **Saving** uses `localStorage` – it stores the current stage and score.

## 📄 License

This project is provided for **personal and portfolio use**. You may modify and share it for non‑commercial purposes. If you include it in a public repository, please credit the original author.

---

*Oxidation will happen to you. Play responsibly.*  
[Launch the game](https://yourdomain.com/plazma-shooter) *(if hosted)*
