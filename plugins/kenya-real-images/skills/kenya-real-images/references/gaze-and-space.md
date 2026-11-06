# Gaze, pointing and room layout

Two problems make otherwise good images feel wrong at a glance:
1. **Eyes that don't land.** Two people are meant to look at each other, but their eyes slide past, look slightly off, or one of them seems to look at nothing.
2. **Rooms that don't add up.** One table sits at a diamond angle in a square room, chairs face nowhere, floor lines run one way and a table edge another, so one part of the image feels "off".

Both happen because the model is told what people do, but not where everything is in space. Fix it by placing people and objects first, then saying who looks at what.

## Part 1: Gaze that lands

### 1. Place people before you say where they look
Give each main person a position in the scene and a direction their body faces, then the gaze.
- Weak: "the trainer talks to a participant, who listens."
- Strong: "The trainer stands on the left, facing right. The participant sits on the right at the table, his chair turned to face left toward the trainer. They are about two metres apart."

### 2. Lock head, eyes and body to the same target
Off-looking eyes usually come from the head pointing one way and the eyes another. Say all three:
- "Her shoulders, head and eyes all turn toward him; her eyes look straight at his face."
- "He looks back at her eyes, head turned fully toward her."

### 3. Write both ends of every eye line
If A looks at B, say what B looks at too. If B looks back, say "they make eye contact". If B looks at something else, name it.

### 4. Choose a camera angle that shows eye contact clearly
Eye contact reads clearly when the two faces are seen in profile or three-quarter view from the side. It looks wrong when both faces are turned toward the camera while "looking at each other".
- For two people talking: "camera to the side, so we see both faces in three-quarter profile, facing each other".
- Avoid: "camera in front of both of them" for eye contact.

### 5. Downward gazes are safest
Looking down at a task (a phone, a book, food, a document, hands at work) almost always reads as natural. Use it for most people in a group, and save direct eye contact for the 1-2 people who matter.

### 6. Keep eye-line faces large enough
Eyes in small, mid-distance faces often look wrong. If eye contact matters, frame the two people closer (waist-up or tighter). For wide shots, have people look at clearly readable targets (a screen, a speaker at the front) rather than at each other.

### 7. One speaker, many listeners
- Put the speaker in a named position: "at the front of the room on the left".
- Say the audience's bodies face that position: "chairs in rows facing the front-left where the speaker stands; most heads turned toward her".
- Give 1-2 listeners a different, specific action (writing notes, whispering to a neighbour) so the crowd isn't a wall of identical stares.

### 7b. Spectators watching something
When people watch a race, match, parade or performance, they all watch the same thing:
- Name the one target and its position in the frame, and say every spectator's head and eyes follow it: "all spectators face the road and their heads turn to follow the car as it passes".
- Show watching with real actions: filming on a raised phone, shading their eyes, leaning forward, cheering, a hand over the mouth.
- Nobody faces away from the action or chats with their back to it. At most one person glances at a neighbour, and only while still mostly facing the action.
- Spectators stand close to the barrier, facing the action.

### 8. Pointing
Arm, finger, eyes and target must line up:
- Name the target and make sure it is in the frame.
- Put the fingertip close to the target (within a hand's width) so the direction is unambiguous.
- Say that the pointer and the listener both look at the target, not at each other.
- Example: "He points with his right index finger at the second row of the spreadsheet on her screen, fingertip almost touching the screen; both of them look at that row."

### 9. Holding things
State orientation for anything with a front and back:
- Phones: "screen facing her", or "held flat and face up so all three look down at it".
- Books, documents, tablets: which side faces whom.
- Cameras: what they are aimed at.

## Part 2: Rooms and arrangements that add up

### 1. Name the room's shape and the layout
- "A rectangular classroom; desks in four straight rows, parallel to the front wall, all facing the whiteboard."
- "A square boardroom with one long rectangular table in the middle, parallel to the walls, chairs on both long sides."
- "A hotel conference room with round tables evenly spaced in a grid."
- "A U-shaped arrangement of tables open toward the screen."
- "A small sitting room: a three-seater sofa against the back wall, a coffee table centred in front of it, two armchairs facing the sofa."

### 2. Say everything is aligned
Add this line to every indoor scene with furniture:
"All furniture is aligned to the room: tables and desks are square to the walls (never rotated at a diagonal unless stated), chairs face the table they belong to, rows are straight and evenly spaced, and everything stands flat on the floor."

### 3. Pick the camera view so perspective stays simple
- **Square-on view:** camera faces one wall straight on; the floor and ceiling lines run toward one point in the middle. Best for classrooms, halls, rows of desks, boardrooms seen from the end.
- **Corner view:** camera stands in a corner; two walls visible, lines run toward two points on the left and right. Best for offices and sitting rooms.
- Say which: "camera at the back of the room facing the front wall straight on" or "camera standing in the doorway corner looking diagonally across the room".
- Add: "one consistent perspective: the floor, walls, ceiling, table edges and windows all follow the same vanishing points."

### 4. Keep the camera level
A tilted camera makes the model bend furniture and tables into diamond shapes. Keep the camera level and get the "real photo" feel from off-centre framing, foreground objects and imperfect light instead of tilt. (The realism block already says this.)

### 5. Keep scale consistent
"People, chairs and tables are in correct proportion to each other and get smaller evenly with distance." Watch for oversized chairs or tiny tables in the back.

### 6. Less clutter, fewer errors
Every extra object is another chance to misplace something. Name only the furniture and objects the scene needs; let the rest stay simple.

### 7. Outdoors
- Name the ground line and layout: "a straight pavement running from the bottom left toward the back right", "market stalls in two straight rows on either side of a central path".
- Vehicles on the road, not at odd angles across it.
- Buildings stand upright; vertical lines stay vertical.

## Part 3: Quick check before you accept an image

1. Follow each person's eyes: does their gaze land on what the prompt says?
2. For each pointing finger: draw a line from the shoulder through the fingertip. Does it hit the target?
3. Look at every table and desk: is it square to the walls and to its neighbours? Do the chairs face it?
4. Follow the floor and ceiling lines: do they head to the same point(s)?
5. Is anything floating, sinking into the floor, or much too large or small for its distance?

If any check fails, regenerate with a sentence that names the exact fix, for example: "the round table in the back left was rotated; all tables must sit in a straight grid parallel to the walls" or "her eyes look past him; her head and eyes must turn fully to his face".
