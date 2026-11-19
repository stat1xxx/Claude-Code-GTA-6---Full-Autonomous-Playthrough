# Claude Code × GTA 6 — Full Autonomous Playthrough

> One prompt. 12 hours. Full story completion + 500 hidden easter eggs discovered — all while I was at work.

---

## What This Is

I gave Claude Code full access to my screen and keyboard before leaving for work at 8 AM. When I came back 12 hours later, it had completed the entire GTA 6 story mode, unlocked the full map, and — without being asked — started digging through the game files to recover cut content that Rockstar removed before release.

No scripts. No automation pipeline. No pre-written macros. Just a natural language prompt and 12 hours of fully autonomous execution.

This repository documents the exact setup, the prompt used, and a summary of everything Claude Code found during its session.

---

## Hardware Setup

| Component | Details |
|-----------|---------|
| **Console** | PlayStation 5 — GTA 6 running full screen |
| **Capture** | Elgato HD60 X — HDMI capture card |
| **Computer** | MacBook Pro — receiving PS5 video feed via capture card |
| **Terminal** | iPhone — Claude Code terminal app, connected via USB |
| **AI** | Claude Code with computer use enabled |
| **Signal chain** | PS5 → HDMI → Capture Card → USB-C → MacBook → Claude Code |

The PS5 was connected to the MacBook through an Elgato HD60 X capture card. HDMI output from the PS5 feeds into the capture card, which passes the video to the MacBook over USB-C. OBS displayed the PS5 feed on the MacBook screen. Claude Code was running on the iPhone, connected to the MacBook via USB — giving it direct access to see the PS5 screen output and send controller inputs back to the console through the Mac.

---

## The Prompt

This is the exact prompt I gave Claude Code before leaving:

```
You have full access to my screen and keyboard. I'm leaving for 12 hours.

Objective: complete GTA 6 story mode from the current save point.

After completion, switch to free roam. Explore the full map, inspect any
unusual assets, and log everything worth noting — locations, dialogue,
files, anything that looks intentionally hidden or removed.

Deliver a structured report when done.
```

That's it. No keybind mappings. No game-specific instructions. No walkthrough data. Just the objective and a request for a report.

---

## Results Summary

| Task | Status | Details |
|------|--------|---------|
| Story mode | ✅ Completed | All remaining missions finished |
| Full map | ✅ Unlocked | Every region accessible |
| Easter eggs | ✅ 500+ discovered | Hidden references, locations, NPC interactions |
| Deleted NPC dialogue | ✅ Recovered | Found in game files, catalogued by location |
| Censored scenes | ✅ Found | Identified and partially restored from assets |
| Hidden locations | ✅ Mapped | Coordinates and screenshots documented |

---

## Timeline: How It Played

### Phase 1 — Learning (Minutes 0–15)

Claude Code started by experimenting with controller inputs while observing the PS5 screen output. It systematically tested each button to map controls: movement (left stick), camera (right stick), actions (triangle, circle, square, cross), weapons (L1/R1), and vehicle controls. Within 15 minutes, it had a working understanding of the DualSense control scheme — without any manual, tutorial, or keybind reference.

### Phase 2 — Story Missions (Hours 1–8)

Claude worked through the remaining story missions sequentially. Key behaviors observed:

- **Cutscene awareness** — It watched every cutscene and used dialogue/visual context to understand objectives. It never skipped a single one.
- **Adaptive strategy** — When a mission failed, it didn't just retry the same approach. It analyzed what went wrong and tried a different route, weapon, or timing.
- **Shortcut discovery** — During missions, it found unintended paths and shortcuts that reduced completion time. Some of these may be speedrun-relevant.
- **Resource management** — It managed health, armor, ammo, and money across missions without being told to.

### Phase 3 — Free Roam Exploration (Hours 8–10)

After the final story mission, Claude transitioned to free roam on its own. It systematically explored the map in a grid pattern, visiting every district and documenting:

- Unique NPC interactions and dialogue
- Environmental storytelling elements
- Hidden interiors and accessible buildings
- Easter eggs referencing previous GTA titles, pop culture, and real-world events
- Unusual geometry or texture patterns suggesting hidden content

### Phase 4 — Game File Analysis (Hours 10–12)

This phase was entirely self-initiated. Claude was never instructed to look at game files. After exhausting surface-level exploration, it navigated to the game's installation directory and began inspecting asset files. What it found:

- **Deleted NPC dialogue** — Audio files and subtitle strings for conversations that were removed from the final release. These included extended storylines for secondary characters.
- **Censored scenes** — Visual assets and scripts for scenes that were present in development but removed or altered before launch.
- **Hidden locations** — Map data for areas that exist in the game's coordinate system but are inaccessible through normal gameplay. Some had partial geometry and textures loaded.
- **Debug references** — Leftover developer comments and debug strings in configuration files.

---

## Key Observations

### On Learning

- Claude taught itself the entire control scheme through trial and error in under 15 minutes
- It identified context-sensitive controls (different actions in vehicles vs. on foot) without any prompting
- It figured out the weapon wheel, phone menu, and map system through visual observation alone

### On Problem Solving

- When stuck on a mission, it tried alternative approaches instead of brute-forcing the same strategy
- It used environmental awareness — taking cover, using elevation, flanking — suggesting it understood spatial reasoning in a 3D environment
- On at least one mission, it found a shortcut that skipped an intended combat sequence entirely

### On Initiative

- The transition from story mode to free roam was autonomous — it interpreted "explore the map" as a natural next step
- The game file analysis was completely self-directed — the prompt said "document anything interesting" and Claude decided the game files qualified
- It organized its findings into categories without being told how to structure the report

### On Endurance

- 12 hours of continuous operation with no crashes, freezes, or loss of focus
- Maintained consistent performance throughout — no degradation in decision-making quality over time
- Handled interruptions (loading screens, cutscenes, phone calls in-game) gracefully

---

## Why This Matters

This experiment isn't really about gaming. It's a proof-of-concept for autonomous AI execution over extended timeframes in complex, unstructured environments.

### Demonstrated Capabilities

| Capability | Evidence |
|------------|----------|
| **Self-directed learning** | Learned game controls with zero prior knowledge |
| **Long-horizon planning** | 12 hours of continuous, goal-directed operation |
| **Spatial reasoning** | Navigated 3D environments, used cover, found paths |
| **Initiative beyond instructions** | File exploration was never requested |
| **Adaptive problem solving** | Changed strategies on mission failures |
| **Structured reporting** | Organized findings without formatting instructions |
| **Context awareness** | Used cutscene information to guide gameplay decisions |

### Implications

- **QA testing** — An AI that can play through a game autonomously and find hidden/broken content could transform game testing
- **Content discovery** — Automated exploration of game files for cut content, easter eggs, and developer artifacts
- **Accessibility** — AI-assisted gameplay for players who want to experience story content without mechanical skill barriers
- **Long-running tasks** — Proof that AI can maintain focus and quality over 12+ hour autonomous sessions

---

## How to Reproduce

1. Connect your PS5 to your MacBook via an HDMI capture card (Elgato HD60 X or similar)
2. Open OBS or Elgato software to display the PS5 feed on your Mac screen
3. Install Claude Code on your iPhone and connect it to the MacBook via USB
4. Enable computer use permissions in Claude Code
5. Launch GTA 6 on PS5 and load your save
6. Paste the prompt above
7. Leave

**Note:** Results will vary based on save progress, capture card latency, and Claude Code version. The key insight is the simplicity of the prompt — Claude figures out the rest.

---

## Video

Screen recording of Claude Code playing GTA 6 autonomously is attached to the original post.

---

## License

MIT — do whatever you want with this.

---

*Built with [Claude Code](https://claude.ai) by Anthropic*
