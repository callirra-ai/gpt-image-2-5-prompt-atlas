# Craft

The prompting principles behind every case in this atlas. They were distilled from the official OpenAI cookbook and prompting guidance, from the strongest community craft notes, and from our own renders — including the ones that failed.

They are ordered roughly by how much damage ignoring them does.

---

## Composition

**1. Canvas before subject.**
Declare the format, the layout and the reading order before you say what anything is. A model that has not been given a structure will invent one, and it will be a centred subject on a plain ground.

**2. Fix the regions, not the mood.**
For anything with panels, bands or zones, give each region a proportional height or width and say it never overlaps its neighbour. "A poster with a title and a date" produces a poster with a title and a date somewhere. "A top band 18% of the height carrying the title, one hairline rule closing it" produces a layout.

**3. One focal point, and a reading order.**
Say which element is largest and where the eye should go first, second and third. If you cannot state the order, the picture does not have one.

**4. Say what is near.**
A foreground element that crops into frame — an out-of-focus edge, a step, a wall — is what creates depth. Without one, everything sits on the same plane no matter how good the light is.

**5. Counts have to close.**
Six panels, seven components, five arches, seven figures. State the number, then make every dependent element match it: one label per component, one leader per label, one callout per part. A count that does not close is the failure a reader notices first.

---

## Light and material

**6. Light before material.**
State the source, its direction, its quality and its colour temperature before you describe what it touches. Materials do not have a look; they have a response.

**7. Materials behave; they are not named.**
"Glass" is a word. "Amber glass with visible thickness at the base, refracting the background and holding one clean specular line" is an instruction. Say how a surface absorbs, reflects, transmits or scatters — never just what it is made of.

**8. Two temperatures beat one.**
A single light source makes a photograph. Two — a cold window and a warm lamp — make a picture. Keep them separate and forbid them from mixing.

**9. Shadow and reflection carry the composite.**
If you place an object into a scene, ask for the contact shadow and the reflection explicitly, at the intensity of the objects already there. Their absence is what makes an image read as pasted.

**10. The background is a decision, not a default.**
Say what the background is, what value it holds, and whether it has a gradient. A background you did not specify is a background you did not choose.

**11. Depth of field is a decision.**
Say whether the frame is sharp throughout, or where the plane of focus falls. "Shallow depth of field" is not an answer; "sharp across the barrel top, soft at both ends" is.

---

## Text

**12. Exact text goes in quotes, verbatim, once each.**
Every string that appears in the image is listed, quoted, and marked as appearing once. Then check it character by character against the render, because the model will get one letter wrong in a way nobody notices until print.

**13. Spell the hard words out.**
Brand names, unusual spellings and short codes should be given letter by letter. It is cheap insurance.

**14. One typographic budget.**
One or two typefaces, a stated number of sizes, one alignment axis. Every extra size and every extra family multiplies the ways the layout can go wrong.

**15. Variables must be filled before you render.**
A bracketed placeholder is not a blank to the model; it is a slot it will fill with something plausible. An unfilled `[DATE]` is how an invented date ends up in a published poster. Replace every one.

**16. Reserve empty space rather than forbidding content.**
"Leave a clean rectangle here for a compliance mark added later" works far better than "do not add a compliance mark". Prohibitions are easy to ignore; a reserved area is a visible thing to keep empty.

---

## Constraints

**17. The preserve list must be longer than the task.**
In any edit, the protected list is the technique. Name the window, the joinery, the camera, the label, the geometry — specifically, one by one. "Keep the room" preserves the layout and quietly replaces the window.

**18. Name the failures you have actually seen.**
A do-not list earns its place by naming real failure modes: the invented certification mark, the mirrored asymmetric detail, the cut-out edge, the drop shadow that disagrees with the light. Generic "high quality" instructions do none of this.

**19. Negation is for strong priors only.**
Do not negate what the model probably would not do anyway. Spend the do-not list on the things it reaches for by default: extra props, glossy plastic, centred subjects, invented text, filled negative space.

**20. Order is semantic.**
With multiple inputs, `Image 1`, `Image 2` means something. State the order, publish the reference files in that order, and keep the highest `Image N` in the prompt equal to the number of references supplied.

**21. One reference, one job.**
Give every input a single responsibility and say what it must *not* supply. The moment two references can both decide the same property, the model averages them and the subject drifts.

**22. State the conflict policy.**
When two inputs can disagree — a person's skin tone from one and the room's colour cast from another — say which wins and why. Without it you get the average of two answers.

---

## Adjustment

**23. A prompt is not a pixel lock.**
Image-to-image preserves layout and content well and finish inconsistently. Prompts can demand alignment; they cannot guarantee it. If a job needs exact alignment, composite it rather than generate it.

**24. When a render misses, name the miss.**
Say what failed, what you changed, and whether it worked. Chasing a failure by re-rolling the same prompt teaches nothing; the pattern is only visible when it is written down.
