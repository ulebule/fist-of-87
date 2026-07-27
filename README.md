# FIST OF '87

A one-on-one fighting game in the browser, in the spirit of the 1987 coin-op
brawlers and the 16-bit home conversions that followed them. Ten challengers
across five countries, three rounds each, and a block-breaking bonus stage
between bouts. Everything is in a single `index.html` — no libraries, no build
step.

**[▶ Play it here](https://ulebule.github.io/fist-of-87/)**

## Not a conversion

This is an original game, not a port of anything. The fighters, their names,
their moves and the artwork are all written for this project; no code, sprite
or character from any published game is used. What it borrows is the shape of
the genre — health bars, a round timer, best of three, a world tour — which the
whole fighting-game canon shares.

## Controls

**Player 1** — `A` `D` move, `W` jump, `S` crouch and guard,
`F` punch, `G` kick, `H` special.

**Player 2** — `←` `→` move, `↑` jump, `↓` crouch and guard,
`,` punch, `.` kick, `/` special (numpad `1` `2` `3` work too).

**Touch** — no on-screen buttons. The left half of the screen steers: drag to
walk, swipe up to jump, drag down to guard. The right half strikes: tap to
punch, swipe up to kick, swipe forward for the special. One player on a phone;
two players need a keyboard.

`ENTER` starts a one-player tour, `2` starts a two-player match, `M` toggles
sound, `L` cycles the language and `N` changes your name.

## The fight

Blocking is holding away from your opponent, as it always was: a guarded hit
costs a sliver of health instead of a chunk and does not stun. Every fighter
has one special move — a thrown energy wave, a rising uppercut or a lunging
dash — plus their own reach, speed, weight and temper. SLUGGER cannot kick;
TANK is slow and hits like a truck; KAGE jumps over almost anything.

A round is 60 seconds. Take two rounds to win the bout, beat all ten
challengers to become world champion. The bonus stage after the fourth and
eighth opponent pays 500 points for a block broken cleanly.

## Score board

Scores are shared online through Firebase, with a top-ten table on the title
and game-over screens. With no connection the game keeps working and falls back
to scores stored in the browser. Two-player matches are friendlies and are not
submitted.

## Languages

English, Slovenian, German, Italian and French, detected from the device and
switchable with `L` or the on-screen button.

## Install it

The game is a PWA: a browser will offer to add it to the home screen (on iOS,
Share → *Add to Home Screen*), and it then opens standalone. A service worker
caches the page, so after the first visit it runs with no connection at all —
the score board naturally needs the network and falls back to local scores.

## Licence

MIT
