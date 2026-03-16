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

## Repository Layout

- `spec/desktop-profile.md`: XFCE app and panel defaults.
- `spec/theme-system.md`: Wallpaper, splash, icon, cursor, and message style specification.
- `spec/hardware-target.md`: Baseline/recommended hardware profile and optimization strategy.

## Next Steps

- Build and package an XFCE profile seed.
- Produce first-pass icon and cursor assets.
- Create a Plymouth splash and lightweight GTK theme.
- Define an installer profile and ISO build pipeline.
