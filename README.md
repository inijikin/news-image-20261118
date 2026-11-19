[![make.fun · news-image-20261118](https://make.fun/badge/news-image-20261118.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![rank](https://make.fun/badge/news-image-20261118/inijikin/news-image-20261118/rank.svg)](https://make.fun/bounty/news-image-20261118/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![reward](https://make.fun/badge/news-image-20261118/inijikin/news-image-20261118/reward.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)

# The World — Wednesday 18 November 2026

Entry for make.fun [`news-image-20261118`](https://make.fun/bounty/news-image-20261118): one image summing up the
world's news of Wednesday 18 November 2026.

## The image

A newspaper-style infographic (1024×1024 PNG) with six stories from
that day, across regions and fields:

1. **China · Summit** — Xi and Putin meet as Trump lands in China;
   trilateral talks set for Thursday; the Quad meets in Manila.
2. **Ukraine · War** — Kerch Bridge hit for a second day; part of the
   road span collapses in strikes on the Crimea link.
3. **The Gulf · Conflict** — US jets strike Iran missile sites; Iran
   fires drones at US bases in Bahrain and Kuwait, both intercepted.
4. **United States · Politics** — Democrats take the Senate, 56–44;
   Peltola beats Sullivan in Alaska.
5. **Tech · Markets** — Nvidia posts a record $115.8bn quarter;
   revenue up 103% on the year; board rejects Huang's return as CEO.
6. **Health** — US loses measles-free status, first time in 26 years:
   5,400+ cases, 10 deaths.

Every element is drawn by hand in `render.html` — no photographs, no
borrowed artwork, no copyrighted characters.

## How it is built

`render.html` holds the layout (HTML/CSS with inline SVG icons).
`render.mjs` renders it to `entry.png` with headless Chromium:

```sh
node render.mjs entry.png
```

## How it runs

`main.ts` (Node 22, standard library only) copies `entry.png` into
the output directory. It writes the same bytes on every run:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## License

MIT — see `LICENSE`.
