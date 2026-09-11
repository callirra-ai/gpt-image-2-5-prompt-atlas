# Direct Flash Night Portrait

![A direct-flash night portrait: hard light on the face, a hard shadow on the wall behind — Flare tier](preview-flare.jpg)

![A direct-flash night portrait: hard light on the face, a hard shadow on the wall behind — Sunburst tier](preview-sunburst.jpg)

<sub>Flare (top) and Sunburst (bottom), both rendered from the identical prompt at quality `xhigh`.</sub>

A direct-flash night portrait on a city street: flat hard light on the face, a hard shadow thrown onto the wall behind, background falling to black. Use it for editorial and fashion work, album covers, and any brief built on the on-camera-flash look.

## Try the prompt

```text
35mm color film photography with harsh direct on-camera flash, specular highlights on skin and clothing, strong catchlights in eyes, high contrast flash illumination, authentic film grain and color shift, night street editorial style, close-up portrait, a woman in a black leather jacket leaning back against a shuttered shopfront at 1 AM, one hand pushing her hair back, chin slightly down, gaze just past the lens, hard shadow thrown straight behind her onto the wall, background falling away to black, wet asphalt at the bottom of the frame catching the flash, slight cyan drift in the shadows, no plastic skin, no digital over-sharpening, no airbrushing, no oily skin, no watermark, no text, authentic 35mm direct flash film look
```

[Copy plain text](prompt.txt) · [Full-size Flare](full-flare.jpg) · [Full-size Sunburst](full-sunburst.jpg)

## Make it your own

- **The light is the subject.** One hard on-camera flash, no second source, no fill. Every other decision follows from that.
- **Name the artefacts.** Speculars on the forehead and nose, catchlights in the eyes, a hard shadow behind, film grain, a slight cyan drift. These are what separate a flash photograph from a photograph with flash.
- **Keep the background black.** The moment the street becomes visible the frame stops being about the light.

## Settings and result

`openai/gpt-image-2.5-flare` and `openai/gpt-image-2.5-sunburst` · quality `xhigh` · 3:4 · **2459 image tokens** · 27 s

Both tiers were rendered from the identical prompt. **Flare holds the skin better** — pores, freckles and the oily highlight across the forehead are individually visible — while Sunburst is marginally smoother. Both get the hard shadow and the wet-pavement return.

**The prompt was adapted.** The original asked for a black slip dress, which OpenAI's safety system rejected through OpenRouter; a black leather jacket was substituted. The original wording is in `source.json` under `adaptation`.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
