# Changelog

## 1.0.0-beta.3 (2026-11-10)

Fixes images that looked fake or AI-made, and cuts the skill from about 12,300 to 7,200 tokens.

- **Kenya by default:** the skill now runs on everyday requests that don't say "Kenya" ("picture of my grandmother cooking", "doctor talking to a patient"). Before, these skipped the skill and showed non-Kenyan people.
- **New Outfit photo style:** "photo shoot", fashion and outfit requests get a friend's phone photo with an ordinary body and relaxed stance, instead of the glossy "full-frame professional" look. The Professional style is now only for headshots, weddings, products and named campaigns, and no longer mentions full-frame cameras.
- **Physical logic:** people stand only where a person fits (never between a counter and the wall), every table and counter is supported to the floor, bodies have natural proportions.
- **User style wording no longer wins over the realism rules:** requested tilts, neon on faces, "everyone smiling at the camera" and readable notes are rewritten, with a final word scan before every image.
- **No invented names:** no sponsor or team names on cars and kit, no headings on screens, no readable signs for named places.
- **Leaner skill:** references load only when needed (`space.md` replaces gaze-and-space, `long-prompts.md` replaces prompt-intake and loads only for long or charity prompts, examples folded in, uploaded-photos only with photos). Duplicate rules merged into one checklist.

## 1.0.0-beta.2 (2026-11-06)

- **Main subject first:** when an image is about a car, event, animal or place, that thing dominates the frame and people become context.
- **Spectator rule:** people watching something all follow it with their heads and eyes.
- **Natural emotions:** people in a group have different expressions; nobody laughs without a reason.
- **New Sports and action style.** The Event style no longer forces flat, hazy light or laughing.
- Clothes fit the place and weather.

## 1.0.0-beta.1 (2026-11-05)

First public beta.

- Describes Kenyans as real, varied individuals anchored to real places, with correct skin rendering.
- Lays out people, furniture and camera before writing gaze, so eye lines, pointing and room layouts make sense.
- **Prompt intake:** long AI-written prompts (8K, cinematic, lens specs, Midjourney flags, JSON, negative prompts) are turned into a plain brief, so results look like real photos.
- **Style from purpose:** "editorial", "cinematic" or "polished" no longer push images to a glossy stock look; candid wins over polished.
- **Final prompt check** before every image: level camera, no coloured light on faces, nobody staring at the camera mid-activity, no invented readable text, no quality jargon, no bias words.
- **Charity and hardship requests** show people with agency instead of the "empty bowl" stereotype.
- Brand logos only when the user names a brand.
- **Beta: uploaded photos.** Put yourself, or someone who agreed, into a new scene in one fast pass, with fixes for the "pasted face" look, screen gaze and presenter logic.

## Known limits

- Screens and whiteboards can still show words the image model made up.
- A presenter's gaze sometimes lands between listeners instead of on one person.
- With uploaded photos, the body can drift heavier in casual clothes, and likeness varies from image to image.
- Each image takes about 3-8 minutes.
