# MotionWAM Project Page

Static project page for **MotionWAM: Towards Foundation World Action Models for Real-Time Humanoid Loco-Manipulation** (CoRL 2026 submission), styled after the DiT4DiT project page.

## Structure

```
homepage/
├── index.html               # Main page
├── static/
│   ├── css/                 # Bulma + custom DreamDojo-style stylesheet (index.css)
│   ├── fonts/               # Computer Modern Serif
│   ├── fontawesome/         # FontAwesome icons
│   └── js/
└── media/
    ├── figures/
    │   ├── arch.png         # Method overview (copied from paper/sections/images)
    │   └── suc_rate.png     # Per-task success-rate chart (copied from paper)
    └── videos/              # ⚠️ Empty — drop the video files listed below
```

## Videos to add to `media/videos/`

`index.html` references these video files. Drop the corresponding `.mp4` files into `media/videos/` to make the page complete:

- `teaser.mp4` — used both as the hero background and as the top-of-page demo reel.
- Per-task demos (one each):
  - `kick_soccer.mp4`
  - `load_cart.mp4`
  - `retrieve_item.mp4`
  - `wipe_board.mp4`
  - `do_laundry.mp4`
  - `lift_basket.mp4`
  - `toss_garbage.mp4`
  - `task_9.mp4` — placeholder slot for the 9th task; rename to whatever the final task is and update `index.html`.

If you don't yet have a hero video, you can temporarily replace the `<video class="hero-bg-video">` element with a static `<img>` background, or simply drop in any task clip as `teaser.mp4`.

## Action-button links to update

The four buttons under the title (`Paper`, `arXiv`, `Code`, `Thread`) currently point to `#`. Update the `href` values in `index.html` once the corresponding URLs are available.

## Local preview

```
cd homepage
python3 -m http.server 8000
# open http://localhost:8000
```
