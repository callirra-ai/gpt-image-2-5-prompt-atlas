# 16-Bit Town at Dusk

![A 16-bit pixel art game screen showing a small walled town at dusk, with a river and a stone bridge](preview.jpg)

A 16-bit console-era game screen: a small walled town at dusk with a clock tower, a windmill, a river under a two-arch bridge and one tiny traveller sprite on the road. Use it for game art, retro branding, album covers, and anything that has to look genuinely pixel-drawn rather than photographed and filtered.

## Try the prompt

```text
Pixel art in the style of a 16-bit console role-playing game, 16:9 landscape, showing a small walled town at
dusk seen from a slight raised angle, as a single game screen.

THE PIXEL GRID — this is the whole style
The image is built from large, visible square pixels at one consistent size across the entire frame, roughly the
scale of a 320 by 180 pixel image enlarged for display. Every edge in the picture is a hard staircase of whole
pixels: there is no anti-aliasing, no sub-pixel smoothness, no soft blending and no blurred edge anywhere.
Diagonal edges step in visible blocks. Curves are chunky. Nothing in the image is smaller than one pixel, and
nothing has a detail finer than the pixel grid. Colour transitions happen by dithering — ordered checkerboard
and scattered-dot patterns of two palette colours — never by a smooth gradient.

PALETTE — exactly twenty-four colours and no more
A dusk palette of twenty-four fixed colours: four blues for the sky, two deep purples for the far hills, three
greens for foliage, two browns for wood and earth, three greys for stone and the road, four warm ambers and
oranges for lit windows and lanterns, one off-white for highlights, one near-black for outlines and one muted
red for roof tiles. Every colour in the image is one of these twenty-four; no colour is blended, faded or
tinted outside the palette.

THE TOWN
A low stone wall with a square gatehouse runs across the middle of the frame, the gate standing open. Behind it,
fifteen or so small buildings with steeply pitched red-tiled roofs crowd together along two narrow streets;
windows are small and most of them are lit warm amber. A square tower with a single clock face stands above the
roofs at the left, and a windmill turns slowly on a low hill at the right. A cobbled road enters through the
gate and runs toward the viewer, widening in the foreground. A stone well with a wooden frame stands in the
small square just inside the gate.

THE LANDSCAPE
Behind the town, three stepped bands of hills recede in increasingly dark purples, undulating rather than
smooth. On the far left, a river runs down from the hills and passes under a two-arch stone bridge, its surface
drawn as horizontal bands of two blues with dithered highlights, and it catches a few dither-speckled glints of
the dying light. Three conical pine trees stand on the near bank and four on the far bank, all the same size
and drawn from the same four or five pixels of shape.

THE SKY
Late dusk: the sky is a vertical gradient built entirely from dithered bands of the four blues, from a deeper
blue at the top to a warm orange band at the horizon, with no smooth blend anywhere. Eight small stars are
placed in the upper third, each a single off-white pixel with no glow. One low cloud sits in the middle of the
sky, a flat two-colour shape with a dithered lower edge.

THE FIGURE
A single small sprite of a traveller stands on the cobbled road just inside the gate, facing away from the
viewer. The sprite is about twelve pixels tall, drawn from the same palette, with a visible dark outline around
its whole silhouette. It is the only figure in the scene and casts no shadow.

CONSTRAINTS
The whole image must read as pixel art, not as a photograph or painting with a pixel filter applied over it:
no photographic texture, no painted brushwork, no smooth gradients, no 3D rendering, no depth of field. No text
anywhere: no signposts, no shop signs, no town name, no window lettering, no watermark. Do not add a second
figure, animals, carts, vehicles, laundry, banners or smoke. Do not add modern elements. Keep the horizon
straight and place it in the upper third of the frame.
```

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **Specify the pixel grid, not the style name.** "Large visible square pixels at one consistent size, hard staircase edges, no anti-aliasing, nothing smaller than one pixel" is what produces pixel art. "Pixel art style" produces a photograph with a mosaic filter over it, and you can always tell.
- **Ban smooth gradients by name and demand dithering.** Every colour transition has to happen through ordered checkerboard or scattered-dot patterns of two palette colours. That single instruction is the difference between a 16-bit screen and a modern illustration.
- **Fix the palette count.** Twenty-four colours, listed by role. A limited palette is what forces the chunky, deliberate shapes that make the style read, and it stops the image drifting into photographic colour.

## Settings and result

`gpt-image-2.5-sunburst` · 2K requested · 16:9 · **2736 × 1536 px** · 36.1 s

This is genuine pixel art rather than a filter: the pixels are large, square and consistent across the whole frame; every edge is a hard staircase with no anti-aliasing; the sky gradient is built entirely from dithered bands rather than a smooth blend; and the eight stars are single off-white pixels with no glow.

The scene holds everything in the brief. The low stone wall and its square open gatehouse run across the middle; fifteen-odd buildings with steep red-tiled roofs crowd behind it with their small windows lit warm amber; the clock tower with its single clock face stands above the roofs at the left; the windmill turns on the low hill at the right; the cobbled road enters through the gate and widens toward the viewer; and the stone well with its wooden frame sits in the square just inside the gate. Behind, three stepped bands of purple hills recede, and on the far left the river runs down under the two-arch bridge with its surface drawn as horizontal bands of two blues carrying dithered glints of the last light. The pine trees repeat at one size. The single twelve-pixel traveller stands on the road just inside the gate with a dark outline and no shadow.

There is no text, no photographic texture and no modern elements anywhere, and the horizon sits in the upper third as specified. The 2K render was enough here for the same reason the watercolour case used it: the picture has no small type and no fine engraved structure, and extra resolution would add nothing the pixel grid can use.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
