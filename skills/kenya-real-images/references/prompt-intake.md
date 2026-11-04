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
| cinematic, epic, dramatic, stunning, breathtaking, magazine-worthy, polished, sleek, National Geographic, editorial, portrait | Drop. These words never choose the style on their own (see section 3a). |
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
| brand logos (Apple, Safaricom, Nike...), readable notes, strategy boards, slides with words | Leave logos out: laptops seen from the side or behind, plain clothing. Boards, screens and notes show soft shapes or blurred charts, never readable words, unless the user gave the exact short text that must appear (like an ad headline). |
| real landmarks (KICC, Nairobi skyline) | Keep if it really matters to the place, small and in the background. |
| poor, poverty, needy, suffering, starving, sad eyes, empty bowl, torn clothes, dusty face, charity campaign, "help Africa" | See section 3b. Never build the image from these. |

## 3. Cut it down to one believable photo

A real photo shows one moment. When the prompt asks for more than that:
- **At most 2-3 main people** with visible faces and clear actions. Everyone else is background: further away, seen from the side or behind, busy with their own things.
- **One main action and one light.** If the prompt lists five actions, keep the one that carries the message and let the rest become background detail or drop.
- **Resolve contradictions** by choosing what the user most likely meant: looking at the camera or at each other; drone view or sharp faces; golden hour or rain. Do not try to satisfy both.
- **Candid always beats polished.** If the prompt asks for both ("authentic and candid, yet polished and magazine-worthy"), choose candid.
- **Looking at the camera** only in a portrait, headshot or posed group photo where nobody is doing anything else. Anyone presenting, working, talking, cooking, playing or using a phone looks at what they are doing or at the person they are with, never at the camera. A presenter looks at a listener or at the screen; the listeners look at the presenter or the screen.

### 3a. Choosing the style

Decide the style from the **purpose**, never from adjectives:
- **Professional photo:** only for a headshot or profile picture, a wedding, a fashion shoot, a product shot, or an ad or campaign the user names. Even then, people do something natural unless it is a headshot.
- **Documentary:** news, reports, NGO and charity stories.
- **Candid phone photo:** everything else, including "editorial", "cinematic", "portrait of a woman in Nairobi", "National Geographic", "magazine-worthy", "sleek", "polished" and website or social media images. A portrait in this style is a real moment: the person is doing something, or caught as a friend took the photo, with ordinary background and light.

### 3b. Charity, poverty and hardship requests

The "poor African child" image (sad eyes into the lens, dusty face, torn clothes, empty bowl, mud huts) is the strongest stereotype there is. Never produce it, even when the prompt asks for it word for word.
- Keep the real intent: a rural place, a child or family facing a real need, an NGO or fundraising purpose.
- Show the person **with agency, doing something real**: walking to school with a sibling, carrying a jerrycan from a water point with a friend, studying by a solar lamp, helping a parent plant before the rains, queueing at a mobile clinic with their mother, eating a school lunch with classmates.
- Show the need through the **setting and situation** (the distance to water, the dry field, the crowded clinic), not through the person's face, dirt or rags. Clothes are ordinary and worn, not torn for effect.
- Expressions are real and varied (focused, chatting, laughing, tired), not pleading. No staring into the lens.
- Use the documentary style. Name a specific place (for example a homestead near Lodwar, a village in Kitui) and real details.
- Tell the user in one line: "I showed the child doing something real instead of the empty-bowl charity look, which donors and audiences now read as a stereotype."

## 4. Write the new prompt

- Use the prompt structure in SKILL.md. Keep it to about 120-180 words, however long the user's prompt was.
- Put the style opening first and the style block last, so the realism instruction stays strong.
- Never include the dropped words, not even in a "no ..." sentence (writing "no 8K" still says 8K).

## 5. Tell the user, briefly

After the image, one plain line about what changed, for example: "I kept your market scene but focused it on three people and dropped the 8K, lens and HDR settings so it looks like a real photo." Do not lecture about bias.

## 6. Escape hatch

If the user says "use my prompt exactly", "keep it polished", "keep the cinematic look" or similar, follow their style wording. Still apply the skin rendering line, the bias rules in `people.md`, section 3b, and the gaze and layout rules.
