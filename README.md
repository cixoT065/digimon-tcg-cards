# digimon-tcg-cards

Backup copies of the card pictures used by the [digimon-tcg](https://github.com/cixoT065/digimon-tcg) simulator,
so the app still shows cards if the sites it normally loads them from go away.

- `cards/<card number>.webp`: the normal printing, for example `cards/BT1-010.webp`
- `cards/<card number>_<art>.webp`: an alternate art, for example `cards/BT12-070_P4.webp`
- `missing.txt`: alternate arts listed in the card data that no source hosts (the app shows the normal printing)

All pictures are 430 × 601 WebP (quality 70) with transparent rounded corners, converted from the official
English card list (world.digimoncard.com), or from images.digimoncard.io where that has none. Pre-Release
stamps and promos the official site doesn't show come from TakaOtaku's card app (web-garage.takaotaku.de,
taken from the Digimon Card Game Fandom wiki); a few of those only exist with a SAMPLE watermark.

**Update after a new set:** run `python3 tools/mirror-images.py ../digimon-tcg-cards` from the app repo
(it only downloads pictures that aren't here yet), then commit and push this repo.

Card images © Akiyoshi Hongo, Toei Animation and Bandai. This is an unofficial fan project, not affiliated
with Bandai, and the pictures are here only so the simulator can display cards.
