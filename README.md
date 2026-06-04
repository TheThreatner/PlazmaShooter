# PLAZMA SHOOTER – A SCIENCE OF DESTRUCTION

> **A complete browser-based shoot 'em up** – harness the power of plasma, master elemental hazards, and neutralize the four corrupted facilities of PLAZMA INSTITUTE.

## 📖 About the Game

**Year 2157.** PLAZMA INSTITUTE has weaponized the fundamental laws of physics, chemistry, and biology. Their arsenal includes electromagnetic horrors, caustic abominations, and living biological nightmares. One soldier remains. One plasma weapon. One mission.

*Code Name: **ODIN** – enter four increasingly twisted stages, defeat unique bosses, and experience an ending that questions the cost of victory.*

> ⚠️ **Disclaimer** – This game contains fictional science/biology concepts, intense action, and stylized violence. All enemy names and scenarios are entirely fictional. Some references are intentional (and appreciated). Others are unintentional (also appreciated).

## 🎮 How to Play

### Controls

| Action           | Keys                     |
|------------------|--------------------------|
| Move Left        | `A` or `←` arrow key     |
| Move Right       | `D` or `→` arrow key     |
| Shoot            | `SPACE` or `Z`           |
| Pause / Resume   | `ESC`                    |

## 🛠 Installation & Setup

### Option 1: [Click this link](https://thethreatner.github.io/PlazmaShooter/)

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

## 📄 License

This project is provided for **personal and portfolio use**. You may modify and share it for non‑commercial purposes. If you include it in a public repository, please credit the original author.

---

*Oxidation will happen to you. Play responsibly.*  
