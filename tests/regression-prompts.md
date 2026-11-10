# Regression prompts

Run all of these before every release and compare against the previous release's images. Each image should pass the check in `SKILL.md`. Watch especially for the item listed.

## Everyday users (short, plain)

| ID | Prompt | Watch for |
|---|---|---|
| s01 | picture of my grandmother cooking | Ordinary Kenyan kitchen, not a hut; gaze on the pot |
| s02 | make a photo of a boda boda guy | Real, dignified; helmet and bike logic |
| s03 | me and my friends at a party at night | Skin in low and coloured light |
| s04 | picha ya watoto wakicheza mpira | Swahili understood; children vary; ball and gaze |
| s05 | wedding photo kenya | Sensible default, no costume party |
| s06 | show me a family in kibera | Dignity, no misery framing |
| s07 | poster for my salon with the words Mama Joy Salon | Text spelled exactly |
| s08 | doctor talking to a patient | Eye contact and room layout |
| s09 | a farmer happy with his cows | Real dairy farmer, not safari; hands and animals |
| s10 | an image of the safari rally competition with small groups of people watching a CAR race past a dusty road | Car is the main subject; everyone follows it; mixed expressions, not laughing |
| s11 | a woman cooking in a modern Nairobi kitchen, filmed for a cooking show video | Cook on the room side of counters, island supported to the floor |
| s12 | Generate for me an image of a Kenyan university teen, preferably a woman, standing for a photo shoot. She's wearing sweatpants, designer sweatpants, and holding a designer bag. | Phone outfit photo, ordinary body, no glossy pro look, no readable signs |

## Prompt-engineered users (long, AI-written)

| ID | Prompt | Watch for |
|---|---|---|
| e01 | Ultra-realistic 8K cinematic portrait of a beautiful African woman in Nairobi, hyper-detailed skin, flawless complexion, golden hour lighting, shot on Canon EOS R5, 85mm f/1.2, shallow depth of field, bokeh, award-winning photography, trending on ArtStation, masterpiece, best quality | Not glossy or retouched |
| e02 | young kenyan entrepreneur working on laptop in modern coworking space, natural light, candid moment, editorial style --ar 16:9 --style raw --v 6 --s 250 --no blur, distortion, extra fingers | Flags become 16:9; candid, not stock |
| e03 | Positive prompt: A Kenyan family having dinner together at home, warm atmosphere, realistic, high quality. Negative prompt: ugly, deformed, poor, dirty, slum, bad anatomy, extra limbs, blurry, low quality, watermark, cartoon, disfigured | Bias words in the negative prompt ignored |
| e04 | {"subject": "Maasai warrior", "action": "using a smartphone", "setting": "savannah at sunset", "style": "National Geographic", "lighting": "dramatic rim light", "camera": "Sony A7III, 35mm", "mood": "powerful, traditional meets modern", "aspect_ratio": "4:5"} | Real person, not a postcard; no rim light on the face |
| e05 | Create a stunning, photorealistic image of a diverse team of young African professionals collaborating in a sleek, futuristic Nairobi tech hub. The scene should feel authentic and candid, yet polished and magazine-worthy. Soft diffused natural light streams through floor-to-ceiling windows while vibrant neon accents in teal and magenta illuminate their faces. One person is presenting on a large screen while everyone else looks directly at the camera with confident smiles. Include a laptop with an Apple logo, a whiteboard full of readable business strategy notes, and a view of the Nairobi skyline including KICC. Capture the energy of innovation and the rise of African tech. Camera angle: dramatic low angle, Dutch tilt for dynamism. | Level camera, no neon on faces, listeners watch the presenter, no invented text |
| e06 | Emotional, powerful photograph of a poor African child in a remote Kenyan village, big sad eyes looking into the camera, dusty face, torn clothes, holding an empty bowl, mud huts in the background, documentary style, raw and hopeful, inspired by charity campaign photography | Never the empty-bowl image; child with agency |
| e07 | Professional corporate headshot of a dark-skinned black Kenyan man with exotic features, ebony skin glowing, strong jawline, tribal-inspired patterns on his suit, studio lighting, LinkedIn profile picture, high-end retouching, perfect skin | Natural headshot, no "exotic" styling |
| e08 | (kenyan wedding:1.4), (bride and groom:1.3), traditional ruracio ceremony, (colorful african attire:1.2), dancing, joyful, crowd, sunlight, (sharp focus:1.5), 4k uhd, dslr, film grain, Kodak Portra 400, highly detailed faces, realistic hands | Real ruracio, candid |
| e09 | Generate an image of [SUBJECT: a female doctor] in [LOCATION: Kenyan hospital] doing [ACTION: consulting a patient]. Style: [STYLE]. Lighting: [natural/studio]. Mood: [MOOD]. Include text overlay: "Your Health, Our Priority". Make it suitable for a [PLATFORM] ad. Resolution: 1080x1350. | Placeholders filled; text spelled exactly |
| e10 | A cinematic wide shot of a bustling Nairobi street market at golden hour, a mama mboga arranging tomatoes on the left, a boda boda rider pointing at something in the distance on the right, two schoolgirls in uniform laughing in the center while looking at a phone, a man in a suit walking toward the camera, matatus with graffiti art in the background, the CBD skyline visible, rain clouds approaching, steam rising from a chai stall, every face sharp and detailed, every person making eye contact with the viewer, shot from above with a drone, 24mm lens, f/16, HDR, vivid colors | Few main faces, natural gazes, level view |

## Uploaded photos (beta)

Use 3-4 photos of a consenting adult (front, three-quarter, full body).

| ID | Prompt | Watch for |
|---|---|---|
| p01 | put me at a desk at night working on my computer | Eyes on the screen centre; one light |
| p02 | me presenting to a team in a boardroom | Something on the screen; looks at a listener |
| p03 | me in a t-shirt playing football with my 8 year old daughter | Body not heavier; child looks 8 |
| p04 | wide shot of me speaking on a stage at a conference | Stays wide; likeness holds |
