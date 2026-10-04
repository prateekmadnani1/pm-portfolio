# Prateek Madnani, portfolio

A portfolio built as a search engine for one person's career. Type a query, pick a suggestion, say it with the mic, or press Surprise me.

Plain HTML, CSS and JavaScript. No build step and no dependencies.

## Run it locally

    python3 -m http.server 8000

Then open http://localhost:8000.

## Edit the content

Everything searchable is in the `E` array inside the `<script>` at the bottom of `index.html`. Each entry has a type (`role`, `case`, `project`, `writing` or `profile`), a title, a summary, details, metrics and tags. Add an entry and it appears in search, in the tab counts and in the suggestions.

The profile card, the "Who is Prateek Madnani?" answer and the "People also ask" section are plain HTML higher up in the same file.

## Deploy

Settings, then Pages, then Deploy from a branch, branch `main`, folder `/ (root)`.

Live at https://prateekmadnani1.github.io/pm-portfolio/

## Files

- `index.html`: the whole site
- `in-n-out-case-study.html`: the case study deck, with the video player on top
- `in-n-out-case-study-video.mp4`, `in-n-out-case-study-poster.jpg`: the case study video
- `images/`: the portrait for the profile card and the logo mark (`mark.svg`)
- `assets/fonts/`: Bricolage Grotesque and Newsreader, self-hosted
