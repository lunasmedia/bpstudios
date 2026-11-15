# BP Studios — website

Single-page bilingual (FR / EN) website for **BP Studios**, film & photo studio spaces for hire in Kinshasa, DR Congo.

## Before going live

Open `index.html`, find the `CONFIG` block near the bottom, and fill in:

```js
const CONFIG = {
  email: "bookings@yourdomain.cd",   // booking inbox
  whatsapp: "243XXXXXXXXX",          // international format, digits only
  address: "Kinshasa, République Démocratique du Congo"
};
```

Leave a value empty to hide that contact option. The booking form opens the visitor's email app or WhatsApp with the enquiry pre-filled.

Also review the four space descriptions (Studio A–C and the dressing rooms) and the FAQ answers so they match the real studio.

## Brand assets (`assets/`)

| File | Use |
|---|---|
| `bp-studios-logo-full.png` | Master 3D cream logo, transparent, high-res (for print / other uses) |
| `bp-studios-logo-3d.webp`, `-700.webp` | Same logo for the web — hero, About & footer |
| `logo/*.webp` | The hero logo split into layers (roof, BP, STUDIOS, tagline) for the animated 3D version |
| `bp-studios-logo.webp` | Compact version without the tagline — header |
| `favicon.ico`, `icon-512.png`, `apple-touch-icon.png` | Browser / phone icons |
| `og-image.jpg` | Social sharing preview |
| `terracotta-texture.webp` | Background texture |

Use the transparent logos on dark or terracotta backgrounds only, and never stretch, skew or recolour them.

## Language

French is the default and is written directly in the HTML; English translations live in the `EN` object in the script. Visitors can switch with the FR / EN toggle, and their choice is remembered. You can link to a specific language with `?lang=en`.

## Animated logo

The homepage logo is built from the layers in `assets/logo/`. On load, the roof line draws in, the BP letters rise, STUDIOS spreads out, the tagline fades up, and the two spotlights flicker on. A light sweep then passes across the letters every few seconds. On computers the logo tilts in 3D to follow the mouse; on phones it floats gently. Visitors who have "reduce motion" turned on see the static logo.
