# Family Zoo — v03 — Scenery

Populates every room with environmental detail — fences, flowers, hay bales, waterfalls — that the player can examine but not pick up. Makes the distinction between EntityType.SCENERY as a label and SceneryTrait as the mechanism that actually blocks taking.

Step 3 of the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial — a progressive walkthrough of the [Sharpee](https://sharpee.net) TypeScript interactive fiction engine, from a single room to a full multi-file story.

## What this step teaches

- SceneryTrait to prevent items from being taken
- Distinction between EntityType.SCENERY and SceneryTrait
- Generous alias lists for natural player phrasing
- Guidance on what belongs as scenery vs. portable items
- Scenery-only descriptions that stay hidden from room object listings

## Playing

Open `play.html`, or preview the folder:

```bash
python -m http.server 8000 --directory familyzoo-v03
```

## Building

This is a **frozen 0.9.x TypeScript version**. The built player in this folder is the published artifact; it is re-laid from `browser/` by the workspace build:

```bash
python ../tools/build.py familyzoo-v03
python C:/code/ifhub/tools/ship.py familyzoo-v03
```

The authoring tree for every version lives in the [familyzoo](https://github.com/Johnesco/familyzoo) repo.
