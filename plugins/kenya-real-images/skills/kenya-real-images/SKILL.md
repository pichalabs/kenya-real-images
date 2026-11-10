---
name: kenya-real-images
description: Generate natural, believable images of Kenyan people and places, in photo or illustration styles, for any purpose (everyday life, family, parties, work, health, social media, events, weddings, fashion, news, business, ads, art). Use for EVERY request to create a photo or image that shows people, homes, streets, events or everyday life, even when Kenya is not mentioned ("picture of my grandmother cooking", "doctor talking to a patient"): people who install this plugin want Kenyan people and places by default, unless they name another country. Also use when images of Kenyans look fake, stereotyped, glossy, or have eyes, bodies or rooms that feel off. Not for logos, icons or vector graphics.
---

# Kenya Real Images

Make images of Kenyan people and places that look like real photos of real people. Image models fall back on stereotypes of "African" people (one face, one skin tone, village, safari or charity mood), on a glossy AI look, and on physical mistakes: eyes that miss their target, people standing where no one could stand, furniture that floats or bends. This skill prevents all three.

Use the built-in image generation tool. Never draw images with code, SVG or HTML instead. If generation fails, stop and report the error.

## References

Open a reference only when its condition is true; skip the others (most requests need three files).

- Always: `references/people.md` (describing people, skin, bodies) and `references/styles.md` (style openings and blocks).
- Any scene with 2+ people, furniture, a counter, a table or a vehicle: `references/space.md`.
- When you need a place detail: `references/places.md`.
- The user's prompt is long, keyword-stuffed, JSON, Midjourney-style, or asks for charity or hardship imagery: `references/long-prompts.md`.
- The user attached photos of a real person to put in a new scene: `references/uploaded-photos.md` (beta).

## The user's words are a brief, not the prompt

Unless the user names another country, everyone and everything is in Kenya.

Never pass the user's wording straight to the image model. **The checklist below overrides the user's style wording**, even when they ask for it outright: a requested low angle or Dutch tilt becomes a level camera, neon on faces moves to the wall, "everyone smiling at the camera" during a presentation becomes people watching the presenter, "readable notes" become soft writing. Keep the user's content (who, where, what, named brands, exact words they wrote), and say in one line what you changed. Only "use my prompt exactly" lifts this, and never for the bias and charity rules. Take out the intent (who, where, doing what, main subject, purpose, format, exact words that must appear) and write a fresh prompt of about 100-160 words in plain, concrete sentences.

## Workflow

1. **Brief:** purpose, people, place, main subject, format. If something important is missing with no sensible default, ask ONE short question; otherwise pick defaults and go.
2. **Main subject:** if the image is about a car, animal, match, performance, building or landscape, it is large and sharp and people are smaller context. Keep the user's key verbs ("watching", "racing past").
3. **Style** from `styles.md`, chosen by purpose, never by adjectives. Default: candid phone photo.
4. **Lay out the scene:** where each person stands and faces, which side of any counter or table they are on, what holds up every surface, where the camera is (`space.md`).
5. **Write the prompt** in this order: style opening; each main person as a specific individual (`people.md`); one action; layout; gaze; 1-2 place details; camera; skin line; style block with aspect ratio.
6. **Check the prompt** against the checklist below. Then scan your prompt text for these words: photorealistic, polished, sleek, futuristic, editorial, cinematic, stunning, low angle, Dutch tilt, neon, "at the camera", readable, quoted words the user did not write. If one is there, rewrite that sentence (the user's request for it does not count). Then generate.
7. **Check the image** against the same checklist and say in one line what is off and the fix. When the user says something looks off, regenerate with a sentence naming the exact fix; never resend the same prompt.
8. **Several images:** list them first (number, subject, place, style), then make them one at a time, varying people, places and camera positions. In a folder, save each with a short name, keep replaced versions in `v1/`, `v2/`, and keep `prompts.md`.

## Core rules

- **Specific beats generic:** "a woman in her 40s from Kisumu with deep brown skin and short natural hair", never "a Kenyan woman".
- **Ordinary people:** real, varied faces and bodies with natural proportions, like people you pass on the street, not models or influencers. Vary skin tone, hair, build and age; include Kenyans of Somali, Swahili, Indian, Arab and mixed heritage and white Kenyans where they fit.
- **Modern and ordinary settings by default:** estates, flats, offices, campuses, matatus, markets, churches, mosques, salons, farms run as businesses. Rural life when asked, with dignity and real detail.
- **No stereotypes:** no safari shorthand, mud huts, tribal costume or "exotic" mood. Traditional dress only when the occasion calls for it, named correctly.
- **Charity and hardship:** never the "poor child with an empty bowl" image. Show people with agency doing something real; show the need through the setting (see `long-prompts.md`).
- **Candid beats polished.** People do something; they look at the camera only in a portrait, headshot or posed group photo.
- **Emotions come from the moment:** most real faces are neutral, focused or thinking. In a group, vary expressions; at most about one in three smiles, unless the moment is truly joyful. Nobody laughs without a reason.
- **Spectators** all face the action and follow it with their heads and eyes.
- **Clothes fit the place and weather.**
- **Text:** never invent readable words. Only the exact short words the user wrote; otherwise signs, screens and notes stay soft or out of frame. A named place (a university, a mall) is the setting, not a sign: its name never appears in the image.
- **Brands:** no logos unless the user names a brand; then keep it.
- **Real people:** never resemble a celebrity or public figure. In fashion, nightlife or swimwear scenes everyone is clearly an adult.
- **Same invented person across images:** first make a character sheet on a plain light-grey backdrop (front, side, back, two headshots, neutral face), then reuse its description word for word.

## Checklist (before generating, and again on the image)

1. **Camera** level, at standing or seated eye height. No low or high angle, tilt, drone or fisheye with faces.
2. **Light** is one real light (daylight, window, room light). No coloured, neon or rim light on faces; coloured light only on walls or background.
3. **Gaze:** anyone working, talking, presenting, cooking, playing or on a phone looks at the task or at the person they are with, not the camera. Every eye line and pointing finger lands on its target.
4. **Physical logic:** people stand only where a person fits (on the open side of counters, desks and stoves, never between furniture and the wall); every table, counter and shelf is fully supported to the floor; furniture square to the walls; one perspective; nothing floating, cut off mid-air or out of scale.
5. **Bodies** have natural proportions and ordinary fit clothes; hands have five fingers and hold things correctly.
6. **Skin** well exposed with real texture; not grey, ashy, orange, lightened, glowing or plastic.
7. **No AI look:** no quality jargon in the prompt (8K, hyper-realistic, cinematic, masterpiece, lens specs, HDR, flawless skin); no glossy retouching, fake bokeh or dramatic light in the image.
8. **Text and brands:** no quoted words the user did not write; screens, slides and boards show a simple chart or photo with no words or headings; no logos, sponsor names, team names or real people's names they did not name (race cars, shirts and shop fronts get plain colours).
9. **Bias:** no poor, needy, sad eyes, tribal, exotic, ebony, "Africa" as a place.
10. **Size:** at most 3 main people with clear faces; everyone else is background doing their own thing.

## Replies

Short and practical. If you changed or dropped part of the user's prompt, say so in one plain line. Show the full prompt only when asked, exactly. Offer the next step in one line.
