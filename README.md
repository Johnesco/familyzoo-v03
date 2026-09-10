# Family Zoo — v03: Scenery

Fences, flower beds, hay, a waterfall, a toucan. Scenery is what makes a room feel like a place rather than a list of exits — present to examine, refused when taken.

Step 3 of sixteen in the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial for [Chord](https://sharpee.net/chord/), the authoring language of the [Sharpee](https://sharpee.net) interactive fiction engine.

## What this step adds

- `scenery` blocks taking without any refusal message of your own
- Several scenery things sharing one room
- Writing descriptions that reward a second look
- `aka` on scenery so EXAMINE FENCE and EXAMINE IRON FENCE both work

## The source

The whole step is one file: [`familyzoo-v03.story`](./familyzoo-v03.story) — the step before it plus the ideas above. The chapter that walks through it is [`docs/v03-scenery.md`](./docs/v03-scenery.md).

## Playing and testing

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v03.tests.json
python ../tools/build.py familyzoo-v03 --force
```

## Engine

Pinned to `@sharpee/*` **5.3.0** (Chord 3.6.0), held there by an `overrides` block: 5.3.1 publishes broken subpath exports and breaks `sharpee test`.

The 0.9.x TypeScript edition this replaced is kept in [`legacy/`](./legacy).
