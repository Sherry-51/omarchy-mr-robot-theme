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

The theme includes 8 curated high-resolution wallpapers in `backgrounds/`:

1. `01-mr-robot-cinematic.png` (4K UHD) — Primary wallpaper with dark silhouette and negative space.
2. `02-fsociety-minimal.png` (4K UHD) — Near-black surface with subtle fsociety mask contour.
3. `03-elliot-alderson.jpg` (4K UHD) — Elliot in his iconic hoodie in low-key lighting.
4. `04-crt-terminal-phosphor.png` (4K UHD) — Original CRT monitor phosphor aesthetic.
5. `05-dark-apartment-isolation.jpg` (1080p FHD) — The dimly lit apartment workspace.
6. `06-abstract-dark-cyber.png` (4K UHD) — Abstract dark cybersecurity texture.
7. `07-surveillance-cold.jpg` (1080p FHD) — Cold surveillance color grading.
8. `08-hello-friend.jpg` (1440p QHD) — Iconic "hello friend" opening title sequence.

See [`SOURCES.md`](file:///home/coder/themes/mrrobot/SOURCES.md) for full licensing, sources, and attribution.

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

---

## 8. Publishing to GitHub & Omarchy Themes Directory

### Step 1: Push to GitHub

1. Create a new public repository on GitHub named:
   ```
   omarchy-mr-robot-theme
   ```
2. Link your local repository and push:
   ```bash
   cd ~/themes/mrrobot
   git remote add origin https://github.com/<your-username>/omarchy-mr-robot-theme.git
   git push -u origin main
   ```

### Step 2: Submit to Omarchy Themes Directory

To list your theme on the official Omarchy community catalog ([omarchythemes.dev](https://omarchythemes.dev) & [omarchy.org/themes](https://omarchy.org/themes/)):

1. Open the [Omarchy Theme Registry](https://github.com/omacom/omarchy-theme-registry) on GitHub.
2. Click **New Issue** and select the theme submission form.
3. Paste your repository URL:
   ```
   https://github.com/<your-username>/omarchy-mr-robot-theme
   ```
4. **Automated Validation:**
   - The registry validation bot automatically verifies your theme structure (`colors.toml`, `backgrounds/`, and `preview.png`).
   - If everything passes, the bot opens a Pull Request automatically for maintainers to merge.
   - If changes are needed, commit the fixes to your repository and comment `/recheck` on the issue.
5. **Continuous Updates:**
   - Once merged, the catalog updates automatically every few hours.
   - Future commits pushed to your `main` branch are automatically synced without needing new pull requests.

---

## License

- Configuration, code, and original graphics: [MIT License](file:///home/coder/themes/mrrobot/LICENSE).
- Third-party imagery: Non-commercial fair use for personal desktop customization. See [`SOURCES.md`](file:///home/coder/themes/mrrobot/SOURCES.md).
