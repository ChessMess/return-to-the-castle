# Return to the Castle

**Play:** https://chessmess.github.io/return-to-the-castle/

"Return to the Castle" by James Wood, published as a type-in listing in *80 Micro*, April 1983,
for the TRS-80 Color Computer (16K, Extended Color BASIC).

`castle.bas` is the original listing, transcribed and verified on XRoar. `index.html` runs it
on a small Extended Color BASIC / MC6847 emulation in the browser, with timing, graphics
and keyboard behaviour matched against XRoar. A few small changes make it friendlier to play today:

- line 31 added (`FORTI=1TO780:NEXTTI`): the stats screen stays up about a second longer
- line 1080: the pool stays up ~0.4s longer (700 → 1000); line 1086: the fish window ~0.2s longer
  (200 → 350); line 10100: the road ~0.4s longer (400 → 700)
- line 13076 fixed: the published listing is missing a space (`...TCTHENGOTO...`), which real Extended
  Color BASIC reads as one long variable name, so buying food from a stranger stopped with
  `?SN ERROR IN 13076`; now `IF FC>TC THEN`
- key taps are latched until the program reads them, so a quick tap on an arrow at the dragon or
  crossroads isn't lost between the game's checks

Keys: D drink · F fish · G gold · S slay · ← → arrows · ENTER · SHIFT+ESC = BREAK (then `RUN` or `LIST`).

On phones and tablets, big on-screen keys appear under the screen (beside it in landscape) with every
key the game uses. Hold ← / → at the dragon and crossroads just like the real arrow keys; RUN restarts
after the game ends.
