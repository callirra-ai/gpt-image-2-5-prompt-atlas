# The Wizard's Study

![A dense, cluttered wizard's study lit by a green-shaded lamp, a fire and one shaft of moonlight](preview.jpg)

A maximalist interior: a wizard's study where every surface is occupied, with **forty-four separately listed objects** all present at once. Use it for game environment art, illustration portfolios, book interiors, and as a stress test for any claim that a model "can't hold a lot of instructions at the same time".

This is the densest case in the atlas, and the reason it exists is the count. The prompt numbers all forty-four objects, and the note at the bottom records how many of them actually arrived.

## Try the prompt

```text
A dense interior painting of a wizard's study, 3:2, seen from standing height at the doorway looking in, lit by
lamplight and a fire. This is a maximalist picture: every surface is occupied and the eye should find something
new on the fourth look. Forty-four separate objects are listed below and all forty-four must appear.

THE ROOM
A stone-walled study about four metres square, one small deep-set leaded window high on the left wall with the
night beyond it, a low arched fireplace on the right wall, a timber ceiling with exposed joists, and a floor of
worn dark boards partly covered by a threadbare patterned rug.

THE DESK — twelve objects
1. A long oak desk across the middle of the room, its surface scarred and ink-stained.
2. A brass desk lamp with a green glass shade, lit, throwing a warm pool onto the desk.
3. An open leather grimoire on a wooden cradle, its pages yellowed, one red silk ribbon.
4. A second closed book with brass corner pieces and a clasp, lying flat.
5. A stack of three smaller books at different angles.
6. A crystal ball on a brass ring stand, one bright point of light inside it.
7. A stone mortar with green residue in it and its pestle laid across the rim.
8. A rack of nine small glass vials, each holding a different coloured liquid.
9. A brass astrolabe with visible graduated rings.
10. A scroll in an open leather tube, with a corner of a star chart unrolled beside it.
11. A quill standing in a brass inkwell, and two loose quills lying beside it.
12. A pair of brass dividers resting on a wooden ruler.

THE LEFT SHELF WALL — nine objects
13. A tall open-fronted shelf unit leaning against the left wall.
14. A mounted armillary sphere on a wooden base.
15. The horned skull of a large animal, hung on the wall above the shelf.
16. A glass jar of dried beetles.
17. A glass jar of pale root slices.
18. A brass balance scale with its pan and four stacked weights.
19. A magnifying lens on a turned handle.
20. A small hourglass, half run through.
21. A chipped ceramic bowl holding three large seed pods.

THE FIREPLACE AND HEARTH — eight objects
22. The low arched fireplace with a live fire banked low, glowing embers visible.
23. A black iron cauldron on a three-legged trivet, steam rising from it.
24. A long iron poker and a pair of tongs leaning against the stone.
25. A stack of split firewood in a wicker basket beside the hearth.
26. A string of dried red peppers hanging on the wall beside the chimney.
27. A brass candelabra with three candles, all lit.
28. A single tall wax candle standing in a holder on the mantel.
29. A broken mantel clock, its face open, its hands stopped.

THE CEILING AND CORNERS — seven objects
30. A rack of dried herbs hanging head-down from a ceiling joist.
31. A bundle of dried roots suspended beside them.
32. A wicker basket of mushrooms on the floor beneath the herbs.
33. A birdcage on a stand with a small sleeping songbird inside.
34. An owl perched on a wall bracket, awake and watching.
35. Cobwebs filling the upper right corner.
36. Dust suspended in the shaft of light falling from the high window.

THE FLOOR AND FURNITURE — eight objects
37. A tall-backed wooden chair with one elbow worn through, pulled back from the desk.
38. A wingback armchair beside the fire with a patchwork blanket on it.
39. A grey cat asleep in the armchair.
40. A small iron-bound chest against the wall, its lid closed.
41. A padlocked strongbox sitting on top of the chest.
42. A lute leaning in the far corner beside the window.
43. A spilt pile of white salt on the boards, swept halfway into a drift.
44. A chalk diagram, half erased, drawn on the boards beside the desk.

WALLS AND FURNISHINGS
A framed chart of an unfamiliar coastline hangs on the wall behind the desk. A heavy tapestry, rolled and
leaning in the corner, its colours faded. A rack of long wooden spoons and a small teapot on a side table.

LIGHT AND PALETTE
Three sources only: the lamp with its warm green-tinted pool on the desk; the fire, low and orange, from the
right; and one cold shaft of moonlight through the high window, striking the floor and the board wall on the
left. Each source keeps its own colour and its own shadow direction: lamp from above the desk, fire from the
right at knee height, moon from upper left. The palette is warm — amber, oak, brass, deep greens and blacks —
with the cold moon shaft and the crystal ball's point as the only cool notes.

CONSTRAINTS
All forty-four listed objects must be present, each visible and identifiable, and no object may appear twice.
No text anywhere: no legible lettering on any book page, spine, chart, clock face or label, and no runes,
sigils or symbols anywhere. Do not add a second person; the room is empty of people. Do not add a second cat,
a second owl or a second bird. Do not add hanging chains, floating objects, spell effects, glowing runes or any
magical light. No watermark. Keep the room believable: every object rests on a surface or hangs from a fixing,
and nothing floats.
```

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **Number the objects and state the total.** This is the whole technique. "A cluttered study full of magical objects" produces a tidy room with four things in it. A numbered list of forty-four with the sentence *all forty-four must appear* produces a cluttered study full of magical objects — and makes the result countable, so you can check it.
- **Group the list by zone, not by importance.** Desk, shelf wall, hearth, ceiling, floor. Zones give the objects somewhere to be, which is what stops them all piling onto the desk.
- **Three light sources, each with its own direction.** A warm desk lamp from above, a fire from the right at knee height and a cold moon shaft from the upper left. Three colours with three directions is what keeps a dense room readable instead of muddy.

## Settings and result

`gpt-image-2.5-sunburst` · 4K requested · 3:2 · **3520 × 2336 px** · 51.3 s

**All forty-four listed objects are present and individually identifiable**, which is the entire purpose of the case. Verified by quadrant at full size:

| Zone | Objects found |
|---|---|
| Desk (12) | oak desk · green-shaded brass lamp, lit · open grimoire with its red silk ribbon · closed book with brass corners · stack of three books · crystal ball with a bright point inside · stone mortar and pestle · nine-vial rack · brass astrolabe · scroll in its tube with an unrolled star chart · quill in a brass inkwell plus two loose quills · dividers and wooden ruler |
| Shelf wall (9) | open shelf unit · armillary sphere · horned skull above the shelf · jar of dried beetles · jar of pale root slices · brass balance scale with weights · magnifying lens · hourglass · chipped bowl of seed pods |
| Hearth (8) | arched fireplace with live fire · cauldron on its trivet with steam rising · poker and tongs · basket of firewood · string of dried red peppers · three-candle candelabra · tall candle in its holder · broken mantel clock with its face open |
| Ceiling and corners (7) | herbs hanging from the joist · bundle of dried roots · basket of mushrooms · birdcage with its sleeping bird · owl on its bracket · cobwebs in the corner · dust in the window's light shaft |
| Floor and furniture (8) | tall-backed chair with the worn elbow · wingback armchair with the patchwork blanket · grey cat asleep in it · iron-bound chest · padlocked strongbox on the chest · lute in the corner · spilt pile of white salt · half-erased chalk diagram on the boards |

The three furnishing items beyond the numbered list are present as well — the framed coastal chart, the rolled tapestry in the corner, the wooden spoon rack and the brass teapot.

The lighting holds its discipline at this density, which is what keeps the room readable rather than muddy: warm green-tinted lamp pool on the desk, orange fire from the right at knee height, and one cold moonlight shaft from the upper left striking the floor and the wall. There is no legible lettering anywhere, including on the open grimoire and the star chart, and no spell effects, floating objects or magical glows. Two small duplications are worth noting if you adapt this: the hourglass appears twice on the shelf, and the mortar's residue reads grey rather than green.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
