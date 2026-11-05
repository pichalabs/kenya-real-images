# Uploaded photos of a person (beta)

Use this when the user attaches one or more photos of a real person and wants that person in a new image. Speed matters: generate ONE image straight away. No character sheet, no preview round. Do all the thinking below silently, then generate. This replaces the prompt intake for these requests, and the final prompt check in SKILL.md still applies.

**Consent:** if the user says the photos are of themselves ("me", "my photo"), go ahead. If they are of someone else, ask once, in one line, whether that person agreed, unless the user already said so. Never use photos of a celebrity or public figure. For a child, only when the user is clearly the parent or guardian, and only in ordinary family, school or everyday scenes.

## 1. Identity block, read from the photos

Write it once and paste it into the final prompt:
- **Face:** shape and width, cheeks, forehead, eyes, brows, nose, lips, ears, teeth, hairline, haircut, exactly where any facial hair grows.
- **Skin:** depth and undertone in plain words.
- **Body as measurements, not adjectives.** Estimate from the photos that show the body: overall height in heads (for example "about 7 heads tall"), shoulder width in head-widths (for example "shoulders about 2.5 head-widths wide"), and how chest, stomach, arms and legs compare to an average person. Say what the body is NOT ("not heavy or bulky, not tall and slim"). Add: "the head is in natural proportion to the body".
- **Casual clothes make bodies drift heavier.** When the new outfit is a t-shirt, hoodie, casual or sportswear, describe the visible parts directly: "arms of an ordinary adult who does not lift weights, waist narrower than the chest, clothes hang loosely".
- **Accessories** and which wrist they are on.
- Do not take clothing from the photos unless the user wants the same outfit.

## 2. Stop the "pasted face"

Reference photos are often studio shots with one smile, one head tilt and one light. Copied onto a new body, the face looks pasted on. Prevent it:
- **Expression:** fits the moment and is different from the reference photos ("mid-sentence, mouth slightly open, eyebrows raised", "concentrating, lips closed"). Never "smiling at the camera" unless asked.
- **Head and body move together:** "head, neck and shoulders turn together in one natural pose".
- **One light for everything:** "the face is lit by the same light as the rest of the scene, from the same direction, with the same colour and softness; no separate studio light on the face".
- End the prompt with: "Use the attached photos ONLY for this person's identity (face, hairline, facial hair, skin tone and body proportions). Do NOT copy their pose, expression, head angle, smile, framing, lighting, background, clothing or any watermark."

## 3. Make the scene logical

Read the user's prompt as a real moment and fix what would not happen in real life, keeping the intent:
- **Someone presenting or explaining** has something to explain: the screen, slide or board shows a simple chart, diagram or photo with no words. Never a blank or switched-off screen. "Blank screen" means "no readable text".
- **Gestures point at the thing being explained,** and gesture and gaze agree.
- **Coloured or brand light** (neon, monitor glow, a brand colour) is an accent on a wall, edge or rim, never across the face.
- **Camera position must be possible:** "behind the shoulder" plus "face clearly visible" becomes "beside and slightly behind at about 45 degrees".
- **Empty space for text:** move large objects to the other side.
- **Wide shots stay wide.** If the user asks for a wide or full scene (a stage, a hall, a field), keep it wide; make the person the sharpest, best-lit and most central figure instead of cropping in.
- **Children's ages by size:** give a size cue with the age ("an 8-year-old girl, her head reaching his chest"), or the model makes children look younger.
- Remove "hyper-realistic", "cinematic", "8k", lens and aperture numbers and similar, unless a polished studio or advertising look is clearly wanted.

## 4. Gaze that lands on its target

**Screens (monitors, laptops, tablets):** put the screen directly in front of the face, about an arm's length away, its centre at eye level, in line with the nose; "eyes fixed on the middle of the screen". Camera from the side (about 90 degrees) or behind and to the side (about 45 degrees), never from in front of the screen. With two monitors, say which one and that the head is turned to it.

**Presenting to people:** the person looks at one named listener ("the woman in the orange blouse at the near left of the table") or at the screen they point at. Listeners look at the presenter or the screen, bodies and chairs facing that way.

**Writing, reading, phones:** eyes down at the page or screen, chin lowered enough for the eyes to reach it.

## 5. Room layout

Name the room shape, the table shape and direction, where the groups sit, where the person stands, and add: "all furniture is aligned to the room, square to the walls, chairs facing the table they belong to, one consistent perspective". Keep the camera level. Keep the person's face at least about a fifth of the frame height when likeness matters, except in wide shots (section 3).

## 6. Final prompt order

Style opening, identity block, action and expression, layout, gaze, place details, camera, light (one light for everything), skin rendering line, style block, format, reference rule.

## 7. Reply

One line on what you changed in the user's prompt, if anything. If the likeness or body looks off, say so and offer one specific fix.
