# Prompt intake: treat the user's prompt as a brief, not as the prompt

Many users paste prompts written by ChatGPT, Midjourney guides or prompt threads: long paragraphs, keyword lists, JSON, `--ar 16:9`, `(word:1.4)`, negative prompts, camera and lens specs. Image models obey every word, so these prompts pull the image toward the glossy, retouched, staged "AI look", bury the realism instructions, and ask for more than one image can hold.

Never pass the user's wording through to the image model. Read it, take out what the user actually wants, and write a fresh prompt with the structure in SKILL.md. Short, plain prompts ("picture of my grandmother cooking") need almost nothing from this file: just fill in sensible defaults.

## 1. Take out the intent

Keep only these, whatever format the prompt is in:
- **Who:** the people and their roles, ages, relationships.
- **Where:** the place, and the time of day if it matters to the story.
- **Doing what:** the one main action or moment.
- **What it is for:** personal, social media, website, ad, poster, article, book.
- **Format:** aspect ratio or size.
- **Exact text** that must appear in the image, in quotes.
- **A clear style wish** only if the user really wants a non-photo or polished look (illustration, studio portrait, ad campaign).

Everything else (adjectives, quality words, camera gear, lighting jargon, weights) is wording, not intent. Drop it, or translate it with the table below.

## 2. Translate or drop

| User writes | Do this |
|---|---|
| 8K, 4K, UHD, ultra-detailed, hyper-detailed, highly detailed, masterpiece, best quality, award-winning, trending on ArtStation, sharp focus | Drop. |
| hyper-realistic, photorealistic, ultra-realistic, realistic | Drop the word; use the candid phone style, which gives real results. |
| cinematic, epic, dramatic, stunning, breathtaking, magazine-worthy, National Geographic, editorial | Drop. If the purpose is an ad, campaign or fashion shoot, use the professional style; otherwise candid phone. |
| flawless, perfect skin, glowing skin, porcelain, high-end retouching, airbrushed | Replace with "real skin texture, light retouching only". |
| camera models, lens mm, f-stops, ISO, film stocks (Portra, Kodak), bokeh, shallow depth of field | Drop. The style block decides the camera look. |
| golden hour, sunset glow | Keep only as "late afternoon sun" if the time of day matters; avoid it in the candid style. |
| HDR, vivid colours, saturated, high contrast | Drop; ask for natural colour. |
| neon, coloured light, rim light, teal and orange | Keep as an accent on a wall or background only, never across faces. |
| dramatic low angle, Dutch tilt, fisheye, drone shot of faces | Level camera. A drone or high view only for a scene without readable faces. |
| `--ar 16:9`, `1080x1350`, `aspect_ratio` | Use as the aspect ratio. |
| `--v`, `--s`, `--style raw`, `--q`, seeds, `(word:1.4)`, `[word]`, `{word}` | Strip the syntax; keep the word if it is real content. |
| Negative prompt / `--no` | Read it for intent. Keep real quality wishes (no extra fingers, no watermark) as natural sentences. Drop any bias words in it (poor, dirty, slum, ugly) and do not let them shape the scene. |
| JSON or labelled fields | Read each field as part of the brief. |
| Empty placeholders: `[STYLE]`, `[MOOD]`, `[PLATFORM]` | Pick sensible defaults. Never write the brackets into the prompt. |
| "everyone looking at the camera", "perfect smiles", "confident pose" | Only for a group photo or portrait that is meant to be posed. Otherwise people look at each other or at what they are doing. |
| exotic, ebony, tribal, warrior, poor child, sad eyes, mud huts, "Africa" as a place | Apply the avoid-words table in `people.md`, keep the user's real intent (a rural child, a Maasai elder, a village), shown with dignity and specific detail. |
| brand logos, real landmarks, readable notes or strategy boards | Keep a landmark if it really matters (KICC in a skyline). Screens, boards and notes stay soft and unreadable unless the user gave exact short words. |

## 3. Cut it down to one believable photo

A real photo shows one moment. When the prompt asks for more than that:
- **At most 2-3 main people** with visible faces and clear actions. Everyone else is background: further away, seen from the side or behind, busy with their own things.
- **One main action and one light.** If the prompt lists five actions, keep the one that carries the message and let the rest become background detail or drop.
- **Resolve contradictions** by choosing what the user most likely meant: candid or polished (pick one); looking at the camera or at each other; drone view or sharp faces; golden hour or rain. Do not try to satisfy both.
- **Pick a purpose-fitting style:** candid phone by default; professional for ads, headshots, weddings and fashion; documentary for news or charity reports.

## 4. Write the new prompt

- Use the prompt structure in SKILL.md. Keep it to about 120-180 words, however long the user's prompt was.
- Put the style opening first and the style block last, so the realism instruction stays strong.
- Never include the dropped words, not even in a "no ..." sentence (writing "no 8K" still says 8K).

## 5. Tell the user, briefly

After the image, one plain line about what changed, for example: "I kept your market scene but focused it on three people and dropped the 8K, lens and HDR settings so it looks like a real photo." Do not lecture about bias.

## 6. Escape hatch

If the user says "use my prompt exactly", "keep it polished", "keep the cinematic look" or similar, follow their style wording. Still apply the skin rendering line, the bias rules in `people.md`, and the gaze and layout rules.
