# MR. ROBOT — FSOCIETY WORKSTATION
### Production Cybersecurity Desktop Theme for Omarchy Linux

An authentic, carefully engineered cybersecurity workstation theme inspired by the visual cinematography and underground hacker atmosphere of ***Mr. Robot***. Built natively for Omarchy Linux 4.x running on Arch Linux with Hyprland and Wayland.

---

## 1. Visual Philosophy & Art Direction

- **Dark, Isolated Surfaces:** Deep charcoal and graphite base tones (`#080A08`, `#050605`) minimize eye fatigue during extended terminal, reverse engineering, and programming sessions.
- **Muted Terminal Green:** Restrained phosphor green accents (`#83B566`, `#A6D486`) represent active status, cursor, and indicators without visual distraction.
- **Restrained Alert Red:** Focused warning accents (`#B94A4A`, `#E06B66`) strictly reserved for errors, destructive actions, and critical monitoring thresholds.
- **High-Legibility Typography:** Soft warm off-white (`#D5D9D2`) delivers WCAG AAA compliant contrast against near-black surfaces, while comments and secondary elements remain subtle (`#62695F`, `#899087`).
- **Authentic Engineering:** No neon gimmicks, fake scrolling logs, or rainbow gradients. Engineered specifically as a focused, daily-driver development workstation for system programming, cybersecurity labs, and network research.

---

## 2. Color System Architecture

| Role | Hex | Semantic Purpose |
|:---|:---:|:---|
| **Primary Background** | `#080A08` | Main terminal, editor, and desktop surfaces |
| **Dark Background** | `#050605` | Floating windows, popups, and sidebars |
| **Darker Background** | `#030403` | Statuslines, sunken surfaces, and deepest shadow |
| **Lighter Background** | `#171B17` | Active line numbers, cursor lines, and cards |
| **Primary Text** | `#D5D9D2` | Normal source code, prompt text, and headers |
| **Dark Text** | `#899087` | Secondary text, status indicators, and parameters |
| **Muted Text** | `#62695F` | Comments, subtle borders, and line numbers |
| **Primary Green (Accent)** | `#83B566` | Active window border, prompt symbol, highlights |
| **Bright Green** | `#A6D486` | Cursor, active selections, and focused items |
| **Selection Background** | `#243326` | Dark forest green text selection background |
| **Selection Text** | `#EEF2EA` | High-contrast selected text |
| **Primary Red** | `#B94A4A` | Errors, failed commands, and critical alerts |
| **Bright Red** | `#E06B66` | Diagnostic errors, break-points, and urgent state |
| **Yellow / Caution** | `#C9A96B` | Warnings, types, and search highlights |
| **Cyan / Info** | `#78A7A0` | Network metrics, string escapes, constants |
| **Blue / Secondary** | `#8298B5` | Functions, methods, and informational notices |
| **Purple / Tertiary** | `#A18AAB` | Keywords, control flow, and syntax operators |

---

## 3. Supported Applications & Components

- **Alacritty Terminal:** Full 16-color ANSI mapping, tuned contrast, muted green cursor, and non-distracting selection.
- **Neovim (LazyVim & Aether):** Native syntax highlighting for C, C++, x86-64 assembly, Rust, Python, Lua, Bash/Zsh, Markdown, and Treesitter. Fully integrates with LSP diagnostics, diffs, gitsigns, neo-tree, and telescope.
- **btop:** Custom cybersecurity monitoring console (`btop.theme`) with dark green CPU graphs, memory usage meters, network scaling, and red critical thresholds.
- **Hyprland:** Active borders rendered with subtle green gradient (`rgba(83b566ee) rgba(355b36ee) 45deg`), dark graphite inactive borders (`rgba(171b17aa)`), and clean window management.
- **Quickshell Shell:** Native Omarchy top bar, workspace switcher, application launcher, notifications, volume/brightness OSD, and lock screen.
- **Web Browsers:** Native platform policy theming (`chromium.theme`) for Chromium, Google Chrome, Brave, and Microsoft Edge.
- **GTK & Icons:** Coordinated with `Yaru-prussiangreen-dark` for dark surfaces with green folder accents.
- **Plymouth & Lock Screen:** Dedicated `unlock.png` and `preview-unlock.png` for boot and lock authentication.

---

## 4. Wallpapers Collection

The theme ships **16 curated high-resolution wallpapers** in `backgrounds/`. All new additions (09–16) are 3840 × 2160 4K UHD, darkened or desaturated as needed to match the theme palette.

### Original Set (01–08)

| # | File | Resolution | Description |
|---|---|---|---|
| 01 | `01-mr-robot-cinematic.png` | 4K UHD | Primary wallpaper — dark silhouette with maximum negative space |
| 02 | `02-fsociety-minimal.png` | 4K UHD | Near-black surface with subtle fsociety mask contour |
| 03 | `03-elliot-alderson.jpg` | 4K UHD | Elliot in his iconic hoodie in low-key cinematic lighting |
| 04 | `04-crt-terminal-phosphor.png` | 4K UHD | Original CRT monitor phosphor terminal aesthetic |
| 05 | `05-dark-apartment-isolation.jpg` | 1080p FHD | Elliot's dimly lit Chinatown apartment workspace |
| 06 | `06-abstract-dark-cyber.png` | 4K UHD | Abstract dark cybersecurity texture |
| 07 | `07-surveillance-cold.jpg` | 1080p FHD | Cold desaturated surveillance color grading |
| 08 | `08-hello-friend.jpg` | 1440p QHD | Iconic "hello friend" opening title sequence |

### New Additions (09–16)

| # | File | Resolution | Description |
|---|---|---|---|
| 09 | `09-hacker-cityscape-dark.jpg` | 4K UHD | Ultra-dark cyberpunk cityscape — near-zero ambient light |
| 10 | `10-fsociety-emblem-4k.jpg` | 4K UHD | High-detail fsociety mask emblem, center-cropped from 6000 × 3276 source |
| 11 | `11-elliot-neon-shadow.jpg` | 4K UHD | Elliot in neon lighting — 55% dark overlay applied for palette consistency |
| 12 | `12-mr-robot-code-rain.jpg` | 4K UHD | Digital code rain composition — darkened 40% to match theme floor |
| 13 | `13-fsociety-neon-dark.jpg` | 4K UHD | Fsociety neon branding — saturation reduced to 70% for muted palette |
| 14 | `14-elliot-terminal-glow.jpg` | 4K UHD | Elliot at terminal displays — Lanczos upscale, 75% desaturation |
| 15 | `15-mr-robot-isolation.jpg` | 4K UHD | Psychological isolation composition — Lanczos upscale from 2560 × 1440 |
| 16 | `16-dark-ops-terminal.jpg` | 4K UHD | Abstract dark ops terminal environment — Lanczos upscale |

See [`SOURCES.md`](SOURCES.md) for full Wallhaven IDs, licensing, and processing notes for all 16 wallpapers.

---

## 5. Installation & Activation

### Local User Installation (Current Machine)

The theme is installed into `~/.config/omarchy/themes/mr-robot`:

```bash
# Symlink or copy the theme into Omarchy user themes
mkdir -p ~/.config/omarchy/themes
ln -nsf ~/themes/mrrobot ~/.config/omarchy/themes/mr-robot

# Apply the theme
omarchy theme set "Mr Robot"
```

Alternatively, open the graphical theme switcher:
```bash
omarchy theme switcher
```
Or press `Super + Space` and search for **Theme Switcher**.

### Remote Installation (via Omarchy CLI)

To install from a public Git repository on any Omarchy system:
```bash
omarchy theme install https://github.com/<your-username>/omarchy-mr-robot-theme
omarchy theme set "Mr Robot"
```

---

## 6. Wallpaper Management

Cycle through the theme wallpapers:
```bash
omarchy theme bg next
```

Or open the interactive visual wallpaper picker:
```bash
omarchy theme bg-switcher
```

---

## 7. Reversibility & Rollback

To return to your previous theme at any time:
```bash
# Return to Matte Black (or your previous theme)
omarchy theme set "Matte Black"
```

If you wish to remove the user theme link:
```bash
rm -rf ~/.config/omarchy/themes/mr-robot
```

## License

- Configuration, code, and original graphics: [MIT License](file:///home/coder/themes/mrrobot/LICENSE).
- Third-party imagery: Non-commercial fair use for personal desktop customization. See [`SOURCES.md`](file:///home/coder/themes/mrrobot/SOURCES.md).
