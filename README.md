# CampOS Linux

CampOS Linux is a lightweight Linux desktop distribution concept inspired by glamorous desktop aesthetics and built for early-2000s hardware.

## Vision

CampOS combines expressive visual design with practical performance:

- **Desktop**: XFCE (fast and low-memory)
- **Included apps**: LibreOffice and Firefox
- **Visual identity**:
  - Glam-inspired wallpaper and splash screens
  - Deluxe stationery-inspired icon set
  - Press-on-fingernail-inspired cursor theme
  - Stylish, personality-driven error messages
- **Target hardware**: vintage computers from the early 2000s

## Design Pillars

1. **Lightweight first**: responsive on Pentium 4 / Athlon-era systems with modest RAM.
2. **Fashion-forward UI**: strong visual personality without sacrificing readability.
3. **Practical defaults**: office suite + browser out of the box.
4. **Delightful feedback**: errors and system messages should feel polished and human.


# Theme System Specification

## Visual Direction

CampOS visual language should balance glam styling with usability.

## Wallpaper + Splash

- **Wallpaper**: glam-inspired color palette and textured gradients.
- **Boot splash**: matching brand palette with minimal animation for low-end GPUs.
- **Login screen**: simplified variant to reduce rendering cost.

## Icon Theme (Deluxe Stationery)

Icon motifs should borrow from stationery aesthetics:

- Polished paper textures
- Metallic accents
- Label/tab shapes for folders

The theme must preserve standard icon naming to maintain compatibility.

## Cursor Theme (Press-On Fingernail Inspired)

- Shape language: rounded, glossy, high-contrast edge.
- Keep hotspot alignment exact to avoid click precision issues.
- Provide fallback to a classic cursor pack if theme fails to load.

## Error and Warning Styling

Error dialogs should be visually polished but clear:

- Use concise, direct language.
- Add personality without being vague.
- Preserve technical details behind an expandable "Details" section.

### Example Error Tone

> "Oops, glamour malfunction. Your document couldn't be saved yet. Check disk space and try again."

## Performance Constraints

All theme assets should optimize for early-2000s systems:

- Prefer static assets over expensive effects.
- Minimize alpha-heavy compositing.
- Keep icon and cursor frame counts low.
- Avoid Transparency PNG effects.
- 
# Hardware Target Specification

## Primary Target Class

Early-2000s desktop and laptop hardware.

## Baseline Profile

- CPU: Single-core x86 (Pentium 4 / Athlon XP era)
- RAM: 512 MB minimum
- Storage: IDE HDD
- GPU: Integrated graphics with limited acceleration

## Recommended Profile

- CPU: Dual-core x86
- RAM: 1-2 GB
- Storage: SSD via adapter or fast HDD

## Optimization Strategy

- Keep desktop effects optional and off by default.
- Use lightweight services and avoid background bloat.
- Favor compressed but low-overhead assets.
- Ensure office + browser workflows remain functional under memory pressure.
- 
## Next Steps

- Build and package an XFCE profile seed.
- Produce first-pass icon and cursor assets.
- Create a Plymouth splash and lightweight GTK theme.
- Define an installer profile and ISO build pipeline.
