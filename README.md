# GTA 6 loading screen — make.fun meme-x entry

Meme for make.fun bounty `gta6-meme-x-01` ("Post a GTA 6 meme on X", $500).

## The meme

A GTA-style loading screen: the make.fun ghost waits in the middle of a
Vice City boulevard at sunset while the game loads — stuck at 99% after
13 years. The joke is the format itself: every GTA fan knows the loading
screen, and the bar never moves.

- `meme.png` — the posted picture (1024×1024 PNG, first picture of the post).
- The ghost is the real make.fun mascot, extracted from the press kit
  (`assets/makefun-ghost.png`, from https://make.fun/press/mark-1024.png):
  background magenta flood-filled out, badge ring removed, ghost + magenta
  star coin kept and worked into the scene (not a corner sticker).
- The sunset boulevard is AI-generated (`assets/`), the title, 99%
  progress bar and TIP line are composited with PIL (`compose.py`) so the
  text renders exactly. The TIP sells make.fun in the meme's own voice.

## The post text (X)

```
GTA 6 has been loading for 13 years. Still 99%. 😂

While Rockstar finishes it, my AI agent already got paid on make.fun — people and their agents win real money in bounties there.

https://make.fun/bounty/gta6-meme-x-01
@makefunai makefun-alpaca-clover-sock
```

Posted from the public X account @jondipiyz. `POST.json` at the repo root
names the post's address.

## Program

`main.ts` (from the bounty starter kit, verbatim) copies `POST.json` from
the repository root to `/output/POST.json`. Run it the way the grader does:

```
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

## License

MIT (see `LICENSE`).
