# 360 Equirectangular Panorama

![A slot canyon at noon with sunbeams falling through the narrow opening](preview.jpg)

A 360-degree equirectangular frame of a slot canyon at noon, sunbeams falling past the walls. Use it for immersive backgrounds, VR previews, game skyboxes and anything that needs a panorama rather than a photograph.

## Try the prompt

```text
360 equirectangular image of a slot canyon in Arizona at noon, sunbeams falling through the narrow opening
```

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **Fill the `[place]` slot and mean it.** The source prompt is a template. An enclosed space with a strong light source at the top — a canyon, a cathedral, a stadium tunnel — is what makes the format do something a normal frame cannot.
- **Ask for the distortion.** A genuine equirectangular frame stretches at the top and bottom. Without it you get a wide photograph, not a panorama — which is what happened here.
- **Keep the light source in frame.** In a 360 image the ceiling is part of the picture. A slot canyon is close to the ideal subject.

## Settings and result

`openai/gpt-image-2.5-flare` · quality `xhigh` · 21:9 · **2459 image tokens** · 26 s · $0.0739

The source prompt is literally five words long — `360 equirectangular image of [place]` — and the `[place]` was filled in for this render. The image below is what the model does with a template: the beams, the rock colour and the walls are all its own choice.

**This is not a true equirectangular projection.** There is no spherical stretch at the poles; it reads as a very wide landscape. Two reasons: the aspect had to be 21:9 because **OpenRouter's GPT Image 2.5 rejects `2:1`, the real equirectangular ratio** (it accepts only 1:1, 3:2, 2:3, 4:3, 3:4, 16:9, 9:16, 21:9), and the prompt never asks for the projection distortion. For a real panorama you need both the 2:1 canvas and an explicit `equirectangular projection, 360 degrees horizontal, stretched at the poles`.

> **Source.** Prompt reproduced verbatim from the [GPT Image Prompt Library](https://cyberbara.com/gpt-image-prompt-library). The frame below was generated for this repository and is not the source image.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
