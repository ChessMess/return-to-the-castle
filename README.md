# Return to the Castle

**Play:** https://chessmess.github.io/return-to-the-castle/

"Return to the Castle" by James Wood, published as a type-in listing in *80 Micro*, April 1983,
for the TRS-80 Color Computer (16K, Extended Color BASIC).

`castle.bas` is the original listing, transcribed and verified on XRoar. `index.html` runs it
on a small Extended Color BASIC / MC6847 emulation in the browser, with timing, graphics
and keyboard behaviour matched against XRoar. The only change to the listing is one added line,
`31 FORTI=1TO780:NEXTTI`, which holds the stats screen about a second longer.

Keys: D drink · F fish · G gold · S slay · ← → arrows · ENTER · ESC = BREAK (then `RUN` or `LIST`).

Note: line 13076 in the published listing is missing a space (`TCTHEN`), so buying food from a
stranger stops with `?SN ERROR IN 13076`, exactly as on a real CoCo. To fix it, type at the `OK` prompt:

```
13076 IFA$="F"THENIF FC>TC THENGOTO13200ELSETC=TC-FC:S=S+7:GOTO13300
```
