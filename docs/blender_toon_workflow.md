# 100% Free Blender Toon & Anime Animation Workflow

A complete pipeline for solo creators using free and open-source software—zero drawing or manual keyframing required.

---

## The Software Stack

| Tool | License | Purpose |
| :--- | :--- | :--- |
| **Blender 4.x** | GNU GPL (Free Forever) | 3D rendering, lighting, camera and scene assembly |
| **VRoid Studio** | Free (Steam/Mac/PC) | Anime character creator (like an RPG character builder) |
| **Mixamo (Adobe)** | Free with Adobe ID | 10,000+ mocap animations (walking, talking, combat) |
| **Rhubarb Lip Sync** | Open Source Addon | Auto-syncs 3D cartoon mouth shapes directly from audio |
| **Audacity** | Open Source | Audio cleanup and voiceover mastering |
| **CapCut Desktop** | Free | Final timeline assembly, sound effects, auto-captions |

---

## Step-by-Step Setup

### Step 1: Character Creation
1. Open **VRoid Studio**.
2. Customize your character (hair, facial features, clothes).
3. Export as `.vrm` format.
4. Install the free **VRM Addon for Blender** and import your character with 1 click.

### Step 2: Auto-Animation via Mixamo
1. Export your character from Blender as `.fbx` (or use Mixamo's free default characters).
2. Upload to [Mixamo.com](https://www.mixamo.com).
3. Choose animations:
   - *"Menacing Walk"*, *"Panicked Dialogue"*, *"Military Salute"*.
4. Download as **FBX (.fbx)** and import into your Blender scene.

### Step 3: Instant 2D Toon Shader (Eevee)
1. Switch Render Engine to **Eevee Next**.
2. In the Shader Editor, connect:
   `Diffuse BSDF` ➔ `Shader to RGB` ➔ `ColorRamp` (Set mode from *Linear* to **Constant**).
3. The "Constant" setting splits realistic gradients into clean 2-tone cell shadows (classic anime look).

### Step 4: Automated Lip-Sync (Rhubarb)
1. Record your dialogue `.wav` file in Audacity.
2. In Blender, select the character's facial shape keys (`A`, `E`, `I`, `O`, `U`).
3. Run **Rhubarb Lip Sync**; it analyzes speech phonemes and animates the mouth keys frame-by-frame.

### Step 5: Render Settings for Instagram Reels
- **Resolution:** X = 1080px, Y = 1920px (9:16 Vertical)
- **Frame Rate:** 24 fps or 30 fps
- **File Format:** FFmpeg Video (MPEG-4, H.264)
- **Shortcut:** `Ctrl + F12` to render.
