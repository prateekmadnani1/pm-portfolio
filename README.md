# Prateek Madnani, portfolio

A career drawn as a transit map. Five lines (Work, Case studies, Projects, Writing, Foundations) run to one terminus, "Get in touch". Every stop is a role, a case study, a project, a piece of writing or a credential. Click a stop to read it, ride a line with Previous and Next (or the arrow keys), and switch to the Timetable view for a plain list. On phones the Timetable is the default.

Plain HTML, CSS and JavaScript in one file. The font is embedded. No build step, no dependencies, no tracking.

## Run it locally

    python3 -m http.server 8000

Then open http://localhost:8000.

## Edit the content

Open `index.html` and find the block that starts with `EDIT ME` near the top of the `<script>`. It holds:

- `PERSON`: name, role, intro, facts, email, links and portrait.
- `LINES`: the five lines and the track each one follows, as grid points (x 0 to 11, y 0 to 7). Keep turns at 45° or 90°.
- `ZONES`: the three dotted career phases along the top.
- `LINKS`: pairs of stops joined by an interchange capsule (a role and its case study).
- `STATIONS`: every stop. `at` is where it sits on its line, `lbl` is the map label (`\n` makes two lines), `label` is the side the label goes (n, s, e, w, ne, nw, se, sw), `cta` adds link buttons, and `video` (`src`, `poster`, `title`) adds a "Watch the video" button that opens the player.

If a stop is more than a few pixels off its line the browser console says so.

Line colours are the `--l1` to `--l5` tokens at the top of the CSS, with light and dark values.

## Deploy

Settings, then Pages, then Deploy from a branch, branch `main`, folder `/ (root)`.

Live at https://prateekmadnani1.github.io/pm-portfolio/

## Files

- `index.html`: the whole site
- `in-n-out-case-study.html`: the case study deck
- `in-n-out-case-study-video.mp4`, `in-n-out-case-study-poster.jpg`: its video walkthrough
- `uniqlo-case-study-video.mp4`, `uniqlo-case-study-poster.jpg`: the Uniqlo case study video walkthrough
- `portrait.jpg`: the cropped portrait on the "You are here" card
- `user_profile.jpg`: the full portrait, used for link previews
- `favicon.svg`: the tab icon
