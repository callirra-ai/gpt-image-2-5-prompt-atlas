# Contributing

Cases are welcome. The bar exists because a prompt repository is judged by the frames it shows, not by how many files it has.

## What a case has to be

| ✅ Accepted | ❌ Rejected |
|---|---|
| Ships a **rendered frame**, without which the case is not reviewed | prompt only |
| Complete and **filled** — no `[PLACEHOLDERS]` left in `prompt.txt` | `[YOUR PRODUCT HERE]` |
| Composition and layout declared **before** the subject | "a beautiful poster of a cat, 8k, masterpiece" |
| Every visible string **quoted verbatim**, and correct in the frame | "add some text" |
| Materials and light described as separate observable controls | "cinematic, dramatic, premium" |
| An explicit preserve list and an explicit do-not list | no constraints at all |
| Records model, resolution, aspect ratio and **measured pixel size** | no settings |
| For image-to-image: **reference order**, and which reference supplies what | "same product" |
| A short, honest note on what failed or needed a retry | no notes |

There is no minimum length. A short prompt that nails a simple job is better than a long one padded with unobservable words. Equally, a prompt that is short because the constraints were left out is not finished.

## Layout a case must follow

```
cases/<number>-<short-name>/
  README.md          what it is, how to adapt it, what to watch for
  prompt.txt         the complete filled prompt, nothing to substitute
  preview.jpg        gallery image, ~1600 px on the long edge
  full.jpg           full-size download, ~2400 px on the long edge
  generation.json    model, requested settings, prompt hash, task record
  reference-1.jpg    image-to-image cases only, in the order the prompt refers to
```

## How to submit

1. Copy the closest existing case folder and rename it.
2. Write `prompt.txt` first. **Fill every variable** — a model does not preserve bracketed placeholders, it substitutes values of its own invention, which is how invented dates and fake brands end up in published frames.
3. Render the frame. Keep `output.png` locally; publish `preview.jpg` and `full.jpg`.
4. Write the case `README.md`: one-line use case, the prompt inline, two to four adaptations, settings and measured pixels, and an honest result note.
5. Open a pull request. Say which model, which resolution, which aspect ratio, and what you had to retry.

## Image-to-image cases

- The prompt refers to `Image 1`, `Image 2`. **The file order must match.** Renaming files while editing is the most common way a case becomes unreproducible.
- State what each reference supplies and what it must not supply.
- If two references could control the same property, state which one wins.
- Never re-upload someone else's photograph as a reference. Generate your own, or use one you have the rights to.

## Attribution

Adapted work must credit the author by handle and link the original post, and must say what was adapted. Images are never re-uploaded as our own. A removal request is honoured immediately.

## What we do not do

- No fabricated measurements. Model, resolution and pixel size are recorded from the actual run or left blank.
- No derived-from-somewhere-else images passed off as our own renders.
- No case published without a frame that stands up at thumbnail size.

## Review order

1. Does the frame work **at ~400 px** without explanation?
2. Does it survive **full size** — hands, object connections, perspective, reflections, text, edges?
3. Does it meet the case's own stated requirements, judged honestly?
4. Is it **different enough** from the cases already published?
