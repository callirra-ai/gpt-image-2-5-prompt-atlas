# Rice Grain Micro Typography

![A heap of rice with a circular inset magnifying one grain, which carries the tiny text "wOw"](preview.jpg)

Nineteen words that ask for an impossible scale: a pile of rice, and three characters of type on one single grain. Use it for typography-limit tests, print and editorial covers, and any brief about scale — the smallest legible thing next to the largest.

## Try the prompt

```text
A massive pile of rice, and on one single grain of rice there is tiny text that reads "wOw"
```

[Copy plain text](prompt.txt) · [Full-size image](full.jpg)

## Make it your own

- **Change the object, keep the ratio.** A grain of rice, a grain of sand, a coin edge, a snowflake. What matters is one tiny surface inside a huge mass.
- **Choose your three characters carefully.** Short words survive. This one reads `wOw` because a three-letter palindrome is unmistakable at any size.
- **Expect the model to solve visibility for you.** See the note below — it added a magnifier on its own. If you want a pure photograph, say so explicitly.

## Settings and result

`openai/gpt-image-2.5-sunburst` · quality `xhigh` · 1:1 · **3122 image tokens** · 78 s · $0.0938

The three characters are **exactly right** — lowercase `w`, uppercase `O`, lowercase `w` — in a serif face, printed once on a single translucent grain.

**The model added a circular magnifier inset that the prompt never asked for.** It read the brief, decided the type would be invisible at frame size, and solved it. That is a real editorial decision made on your behalf: good if you want the joke to land in a thumbnail, wrong if you wanted a straight macro photograph. Add `no magnifier, no inset, no callout` to suppress it.

The setting is a kitchen — a `RICE` sack, jars, a plant — not a studio backdrop. Nineteen words leave the model a lot of room.

> **Source.** Prompt reproduced verbatim from the [GPT Image Prompt Library](https://cyberbara.com/gpt-image-prompt-library). The frame below was generated for this repository and is not the source image.

---

<!-- CTA_CASE -->

[← Back to the gallery](../../README.md)
