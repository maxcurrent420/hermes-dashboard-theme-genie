# Genie Dashboard Theme

A djinn-themed dashboard theme for Hermes Agent with blue and gold accents, and animated smoke wisps.

<img width="1737" height="890" alt="Screenshot from 2026-04-26 23-09-34" src="<img width="1884" height="941" alt="image" src="https://github.com/user-attachments/assets/7ba2c2f8-4aea-40ea-b58e-4b05d1e9ea84" />
" />


## Features

### Color Palette
- **Deep Navy Background**: `#0a1428` — Dark blue-black evoking the midnight sky
- **Gold Accents**: `#f4d03f` — Rich golden highlights
- **Sky Blue Accents**: `#4fc3f7` — Ethereal cyan glow
- **Warm Golden Glow**: `rgba(255, 215, 0, 0.25)` — Subtle ambient lighting

### Typography
- **Display Font**: Cinzel — Elegant serif for headings
- **Body Font**: Playfair Display — Classic serif for readability
- **Monospace**: JetBrains Mono — For code and technical content
- Font loaded from Google Fonts CDN

### Visual Effects

#### Smoke Wisps
- Animated smoke rising from the bottom of the screen
- 5 independent smoke wisp animations at varying positions:
  - Left position (12%, 250px)
  - Center-right (45%, 300px)
  - Header area (25%, 220px)
  - Sidebar positions (60% and 78%)
- Each wisp has unique:
  - Color filter (hue rotation, sepia, brightness adjustments)
  - Size variation (±20% from base)
  - Animation timing (6-7s cycles with staggered delays)
  - Rotation and scale as it rises

#### Golden Glow Effects
- Selected elements have golden box-shadow glow
- Text headers have subtle golden text-shadow
- Cards have gradient shimmer effect

#### Animations
- Floating animation for UI elements (4s ease-in-out)
- Smoke rise animations (6-7s per cycle)
- Smooth fade-in for smoke wisps

## Installation

1. Copy the theme file to your dashboard themes directory:
   ```bash
   mkdir -p ~/.hermes/dashboard-themes
   cp genie.yaml ~/.hermes/dashboard-themes/
   ```

2. Set the theme in your Hermes Agent config:
   ```yaml
   display:
     theme: genie
   ```

3. Restart Hermes Agent to apply the theme

## Requirements

- Hermes Agent with dashboard theme support

## Customization

The theme values can be customized in the YAML file:

- `palette` — Color definitions (background, foreground, accents)
- `typography` — Font families and sizes
- `layout` — Border radius and spacing
- `colorOverrides` — CSS color variable overrides
- `customCSS` — Additional CSS rules (includes smoke animations)

## License

MIT License — See LICENSE file for details.

## Credits

Theme created for Hermes Agent dashboard. Google Fonts (Cinzel, Playfair Display) loaded via Google Fonts API.
