# How to use a case

Every case ships a complete, filled prompt and the frame it produced. This page is the workflow around them.

## 1. Read the settings line first

Each case records **model · resolution · aspect ratio · measured pixels**. Two of those matter more than any wording:

- **Resolution.** Dense text and fine structure need the headroom of 2K or 4K. A 1K render of a text-heavy layout will fail on legibility no matter how good the prompt is.
- **Aspect ratio.** Choose it for the format — a poster, a story, a hero banner — and make sure the prompt's canvas description matches it. A prompt written for a 2:3 poster rendered at 16:9 will look cropped, because it is.

## 2. Copy the prompt as-is the first time

`prompt.txt` has no placeholders. Run it once unchanged to see the baseline, then adapt. Judging a prompt after three simultaneous edits tells you nothing about which edit helped.

## 3. Fill every variable — always

If you adapt a case and introduce a placeholder of your own, **replace it before you render**.

> A model does not treat `[DATE]` as a blank to preserve. It substitutes something plausible. We learned this the hard way: an early poster rendered with unfilled placeholders came back beautifully typeset with a **fabricated date and a fabricated venue**.

The published frame's visible text must match the text in the prompt. Every time.

## 4. For image-to-image, get the reference order right

The prompt addresses its inputs as `Image 1`, `Image 2`. Attach them in that order. Supplying the right images in the wrong order produces a different image from the same prompt, and there is no way to tell afterwards that the order was the problem.

Also note what each case says about roles: a reference that supplies identity must not also be the source of lighting, or the two average each other and the subject drifts.

## 5. Change what the case tells you to change

Each case lists two to four adaptations and, where it matters, what has to move together with them. Swapping a product means swapping its material behaviour; swapping a climate means rebuilding the architecture. Substituting a noun is not an adaptation.

## 6. Review in this order

1. **Text** — character by character, against the prompt
2. **Protected details** — identity, geometry, label, layout
3. **Composition** — placement, margins, panel counts, circulation
4. **Light and material** — direction, shadow, reflection
5. **Style and polish** — last, because a beautiful frame with the wrong date is a failure

## The failure modes worth knowing

| Symptom | What is usually wrong |
|---|---|
| Result resembles every reference and none of them | More than one input is carrying the same job. Give each exactly one. |
| Text is almost right — one letter swapped | The string was not quoted verbatim, or the case's spell-it-out line was dropped. |
| The frame is technically correct and boring | Composition was never declared. Describe the layout before the subject. |
| Everything is one material | Materials were named instead of described. Say how each surface behaves in the light. |
| A composite reads as pasted | Contact shadow and reflection were not requested, or do not agree with the scene's light direction. |
| The subject drifted across iterations | The preserve list was not repeated, or a reference was swapped rather than kept consistent. |
| Rich prompt, flat result | The prompt accumulated adjectives instead of one decisive structural idea. Cut to the idea and rebuild from it. |

## About the published images

`preview.jpg` is the gallery image. `full.jpg` is the download. Full-resolution masters are kept out of the repository, because thirty-odd 4K frames would make the repository useless to clone — if you need the untouched original of a specific case, open an issue.
