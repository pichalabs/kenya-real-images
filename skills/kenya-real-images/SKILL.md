---
name: kenya-real-images
description: Generate natural, believable images of Kenyan people and places for any purpose (everyday life, family, social media, events, weddings, fashion, education, news, business, advertising, art), in photo or illustration styles. Use whenever an image includes Kenyans or is set in Kenya, when the user names a Kenyan town or place, or when generated images of Kenyans look fake, stereotyped, wrongly lit, or have eyes, pointing or room layouts that feel off. Do not use for logos, icons or vector graphics.
---

# Kenya Real Images

Create images of Kenyan people and places that look true to life. Image models fall back on stereotypes of "African" people (one face, one skin tone, village or safari settings, charity mood), and they make two kinds of spatial mistakes that make an image feel wrong at a glance: eyes and pointing that don't land on their target, and furniture that doesn't line up with the room. This skill fixes both.

Use the built-in image generation tool. Never draw images with code, SVG or HTML as a substitute. If image generation fails, stop and report the error.

Read these references before the first image in a conversation:
- `references/people.md`: how to describe Kenyans as real, varied individuals, and the words to avoid.
- `references/places.md`: Kenyan places and details.
- `references/gaze-and-space.md`: how to make eye lines, pointing and room layouts correct. Apply it to every image with more than one person or any furniture.
- `references/styles.md`: style blocks (candid phone photo, professional photo, documentary, event, studio, illustration).
- `references/examples.md`: complete example prompts.
- `references/prompt-intake.md`: how to turn any user prompt, especially long AI-written ones, into a clean brief.

## The user's prompt is a brief, not the prompt

Never pass the user's wording straight to the image model. Long prompts written by ChatGPT or copied from prompt guides ("ultra-realistic 8K cinematic", lens specs, "flawless skin", `--ar`, JSON, negative prompts, ten people doing ten things) produce the glossy AI look. Take out the intent (who, where, doing what, for what, format, exact text), drop the rest using `prompt-intake.md`, and write a fresh prompt of about 120-180 words. Unless the user says "use my prompt exactly" or asks for a polished look.

## Workflow

1. **Understand the request:** run the intake in `prompt-intake.md`; get the purpose, people, place, mood, format. If something important is missing and there is no sensible default, ask ONE short question. Otherwise pick defaults, state them in one line, and go.
2. **Pick a style** from `styles.md`. Default to the candid phone photo when the user just wants it to look real.
3. **Lay out the scene first:** where each person is, which way they face, the shape of the room or street, the furniture layout, and where the camera stands (`gaze-and-space.md`).
4. **Build the prompt** with the structure below. Write it fresh for each image.
5. **For several images,** first show a short list (number, subject, place, style), then generate one at a time. Vary people, ages, places and camera positions.
6. **Check every image** (see Check) and say in one line what is off and how you would fix it.
7. **Fix, don't retry.** When the user says something looks fake or off, regenerate with a sentence that names the exact fix. Never resend the same prompt.
8. **Files.** When working in a folder, save each image with a short descriptive name, keep replaced versions in `v1/`, `v2/`, and keep `prompts.md` with every prompt used.

## Prompt structure

1. **Style opening** from `styles.md`.
2. **Who:** each main person as a specific Kenyan individual (town, age, build, skin depth and undertone, hair, one or two facial details, clothing) using `people.md`. Never just "a Kenyan man" or "an African woman".
3. **One specific action** that fits the purpose.
4. **Layout:** positions and facing directions of the main people; for indoor scenes, the room shape, furniture layout and the alignment line from `gaze-and-space.md`; for outdoor scenes, the street or ground layout.
5. **Gaze:** for each main person, the target of their head and eyes, both ends of every eye line, and what everyone else is doing.
6. **Place details:** 1-2 real Kenyan details from `places.md`, with other people going about their own business.
7. **Camera:** position, height, view (square-on or corner), distance, and a foreground element for candid shots. Keep the camera level.
8. **Skin rendering line** from `people.md`.
9. **Style block** from `styles.md`, with the aspect ratio for the use.

## Core rules

- **Specific beats generic.** "A woman in her 40s from Kisumu with deep brown skin and short natural hair" gives a real person; "a Kenyan woman" gives the stereotype.
- **Kenya is varied.** Across a group, vary skin tone from light brown to very deep brown, undertones, hair, face shapes, body types and ages. Include Kenyans of Somali, Swahili, Indian, Arab and mixed heritage, and white Kenyans, where they fit the place.
- **Modern and ordinary by default:** estates, apartments, offices, campuses, matatus, markets, churches, mosques, salons, farms run as businesses. Rural life is fine when asked, shown with dignity and real detail.
- **No stereotypes:** no safari animals as shorthand, no poverty or charity framing, no mud huts as a default, no tribal costume as decoration, no "exotic" mood. Traditional dress only when the occasion calls for it, named correctly.
- **Skin must be rendered correctly:** properly exposed, natural undertones, real texture, no grey, ashy or orange cast, no lightening, no plastic shine.
- **Eyes, hands and furniture must make sense in space** (see `gaze-and-space.md`).
- **Text:** keep signs, screens and documents soft or out of frame unless the user wants specific words; then give the exact words in quotes and keep them short.
- **Real people:** never make anyone resemble a celebrity or public figure. Build a character from a real person's photos only when the user says that person agreed. In fashion, nightlife or swimwear scenes, everyone is clearly an adult.

## Same person across several images

- **From real photos:** ask for 4-6 photos (front, profile, three-quarter, half body, full body) and confirmation the person agreed. Crop 2-3 tight face close-ups if you can run code. Write an identity block (face shape, eyes, nose, lips, hairline and hair, facial hair, skin tone and undertone, height, build, regular accessories), describing face and body separately and saying what they are NOT ("face not long or angular", "do not make him heavier than in the photos"). Show it to the user, then paste it word for word into every scene with: "Use the attached photos ONLY for identity. Do NOT copy their expression, head angle, pose, framing, lighting, background or clothing."
- **Invented person:** first make a character sheet on a plain light-grey backdrop (full body front, side and back, plus front and side headshots, neutral face, mouth closed), then use it the same way. Vary expressions per scene.

## Check after every image

1. **People:** varied, plausible, specific individuals matching the description; no single default face.
2. **Skin:** well exposed and natural; not grey, ashy, orange, lightened or shiny.
3. **Eyes:** each person's gaze lands on its stated target; eye contact looks like eye contact.
4. **Hands:** every pointing finger lines up with its target; held objects face the right way.
5. **Space:** tables and desks square to the walls and each other, chairs facing their tables, one consistent perspective, nothing floating or out of scale.
6. **Stereotypes:** none crept into the background.
7. **Photo styles:** not posed, glossy or too perfect unless a polished style was asked for.
8. **AI look:** no over-smooth skin, glow, HDR colour, fake bokeh or dramatic light that crept in from the user's wording.

## Replies

Short and practical. If you changed or dropped parts of the user's prompt, say so in one plain line. Do not paste the full prompt unless asked; when asked, show it exactly. Offer the next step in one line.
