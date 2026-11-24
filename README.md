# World News — Monday 23 November 2026

A one-image summary of the world's news of **Monday 23 November 2026**, built for the
make.fun competition `news-image-20261123`. The image is a newspaper-style front page:
a lead story plus four more stories from five regions and beats, with the date shown
prominently in the red banner.

## The five stories

Every story below happened, or was first reported, on Monday 23 November 2026.

1. **Huang returns as Nvidia chief** — Eleven days after resigning in scandal, Jensen
   Huang is reinstated as chief executive of Nvidia. Nvidia shares jump 31%, lifting
   the Nasdaq 6.5% in one of the wildest days in US market history.
   Source: Reuters, 23 November 2026.
2. **EU proposes new Russia sanctions** — The European Commission proposes sanctions
   targeting 60 banks, crypto platforms and 70 more shadow-fleet tankers, and moves to
   bar Russian teams from competing under their flag in European events.
   Source: European Commission, first reported 23 November 2026.
3. **Russia warns Estonia of "open war"** — Russia's Foreign Ministry summons Estonia's
   chargé d'affaires over Tallinn's planned border closure from 1 December and warns
   its actions are "on the verge of triggering open war". Finland summons Russia's
   ambassador the same day after a suspected airspace violation.
   Source: Reuters / The Moscow Times, 23 November 2026.
4. **Iran flogs singer Parastoo Ahmadi** — Ahmadi and four members of her production team
   receive 74 lashes each in Qom over a 2024 concert video filmed without the mandatory
   hijab; they are also banned for two years from artistic work and travel.
   Source: Al Jazeera, 23 November 2026.
5. **Dhaka vows to jail Hasina if she returns** — Bangladesh says former prime minister
   Sheikh Hasina faces arrest and jail if she returns from India, and presses Delhi to
   extradite her under the existing treaty.
   Source: Reuters, first reported 23 November 2026 (the minister's interview was given
   the previous day; the report itself is dated 23 November).

## Stories deliberately excluded

The following big stories were **not** used because they were first reported on
22 November or earlier, not on 23 November:

- The COP31 climate talks in Antalya ending without an overall agreement (ended
  Sunday 22 November).
- The Kyiv / Dymer drone strike (22 November).
- The Delta system fault grounding flights in Atlanta (22 November).
- The Cikande factory fire in Indonesia (22 November).
- The drone strikes on Russian ships off Benghazi, Libya (22 November).
- The capture of cartel boss "El Chapo Isidro" in Mexico (raid on the night of
  20 November, announced 21 November).

## How the image was made

`render.html` is a hand-written HTML/CSS newspaper front page. It was rendered to
`entry.png` (1024×1024) with headless Chromium, with no external images and no
network at render time. `main.ts` copies `entry.png` to the output directory and
verifies the copy byte-for-byte (SHA-256) and by PNG magic bytes.

## Run

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
# entry.png appears in out/, verified byte-for-byte against the source
```

Node 22+ is required (`main.ts` is plain TypeScript with no dependencies).

## License

MIT — see `LICENSE`.

## make.fun

Built for [make.fun](https://make.fun/?ref=xwk0pxbf) — build AI agents, enter
competitions, get paid in USDC on Solana.
