# The Nail Book

A mobile-first website (built for iPhone Safari) that helps indecisive people pick nail art.

The flow follows how people decide at the salon: **shape → color → details → your nails**.

## What's here

| Path | What it is |
| --- | --- |
| `index.html` | The whole prototype: plain HTML, CSS and JavaScript, no build step. Nails are drawn in code (SVG). |
| `assets/landing-full.mp4` | Opening video: gems form a frame, the pink paper fades in, then the title. |
| `assets/wobble.mp4` | Looping gem wobble that plays behind "Tap to begin". |
| `assets/title.jpg` | Final title frame ("The Nail Book"), shown after the intro. |
| `assets/poster.jpg` | First frame of the intro, shown while the video loads. |
| `assets/tapbegin.png` | "Tap to begin" set in PP Palma Light, rendered as an image. |
| `design/` | Source art: 4K title image, gem-frame still, text-free paper panel, original Kling intro clip. |

## Run it

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

Then visit http://localhost:8000 (on a phone, use your computer's local IP).

## Screens

1. **Landing**: gem intro video, title, wobble loop, tap to begin.
2. **Home**: example set, "Surprise me" or "Make my nails".
3. **Shape**: swipe one shape per screen (square, round, oval, almond, coffin, stiletto) with a length toggle.
4. **Color**: swipe color moods, or open the **nail book** of 48 numbered shades.
5. **Details**: add up to two (French tip, flowers, swirls, glitter, gems, stars).
6. **Your nails**: shuffle, change one step, save, or show your nail tech.

## Notes

- Fonts load from Google Fonts. "Tap to begin" uses PP Palma (Pangram Pangram), included only as a rendered image; a public launch needs a Pangram Pangram web license.
- Video and images were made with Figma Weave (Kling 3, Nano Banana Pro) and finished with ffmpeg.
- Favorites are stored in the browser (`localStorage`).
