# DaCaveman Skit: Production Packet

**Tone:** deadpan comedy. Dan treats absurd things (hanging off a mountain, stripping down in a spa) as completely normal. Everyone else overreacts. The laughs come from holding on reactions.
**Target runtime:** about 4 to 5 minutes, roughly 75 shots of 3 to 5 seconds each.
**Stack:** Toonflow handles script import, storyboarding, and the character and location library. ComfyUI runs the models. Wan 2.2 is the quality pick for hero shots and transformations. LTX-Video is the fast pick for drafts, plates, and simple reaction shots.

---

## 1. Character Reference Sheet

Paste each **descriptor block** verbatim into every shot prompt that character appears in. Don't paraphrase it.

### Dan DaCaveman (father, the birthday man)
**Descriptor block:**
> `DAN: a stocky, extremely muscular caveman, 5'5" tall, chiseled jaw, deep-set eye sockets with bright amber eyes, heavy thick eyebrows, long dark-brown beard with a braided goatee, sharp pointed teeth visible when he talks, massive powerful thighs and calves, extremely long thick yellowed ancient fingernails and toenails curved like claws, weathered tan skin, thick dark body hair, age about 60, calm unimpressed expression`

**Wardrobe states**
- **Scene 1:** a rough brown cloth wrapped around the waist covering hips to upper thigh, barefoot, claws exposed.
- **Scene 2:** faded plaid flannel pajamas, nails partly visible, seated in a big worn leather armchair.
- **Scene 3:** a heavy charcoal parka, knit beanie with wild hair bursting out from under it, thick boots, bulky gloves, and a long scarf. The long beard spills over the scarf.
- **Scene 4, human-passing:** the same winter gear with gloves and boots on. Coat comes off at the chair; he's in a plain sweater and sweatpants with hands in gloves. *(Interpretation: the script implies they're disguised before transforming.)*
- **Scene 4, transformed:** brown sackcloth from waist to upper thigh only, bare hairy chest, full claws on hands and feet, fuller hair and brow ridge.

**Reference image prompt (Flux/SDXL):**
> `character reference sheet, [DAN descriptor], brown waist cloth, front view, three-quarter view, side profile, full body, neutral grey studio background, even soft lighting, photorealistic cinematic, consistent face, highly detailed skin texture`

Also make an expression sheet showing deadpan, mild smile, eyes closed in bliss, puzzled, and laughing.

### Tom DaCaveman (son)
**Descriptor block** *(specifics invented for consistency; the script only says he's a younger caveman with a similar build)*:
> `TOM: a muscular young caveman about 30 years old, 5'7" tall, broad shoulders, same deep-set eyes and heavy brow as his father but smoother face, short dark-brown boxed beard with no goatee, shaggy shoulder-length dark hair, sharp teeth, fingernails as long as his fingers and prehistorically thick toenails, warm tan skin, expressive eyebrows, easygoing confident grin`

**Wardrobe states**
- **Scene 1:** a short sackcloth tunic, barefoot.
- **Scene 2:** a hoodie and jeans in his own apartment.
- **Scene 3:** a puffer jacket, beanie, and gloves while driving.
- **Scene 4, human-passing:** a hoodie, joggers, gloves, and sneakers.
- **Scene 4, transformed:** sackcloth across the chest like a tank top and from waist to upper thigh, with nails exposed.

**Reference image prompt:** use the same template as Dan with the TOM block swapped in. Expression sheet: grin, wide-eyed blink, amazement, embarrassed wince.

### Front-Desk Shop Worker
> `DESK: a woman in her late 20s wearing a light-blue nurse-style scrub uniform, short dark hair cut just above the shoulders, small name badge, polite professional smile, standing behind a white reception counter`

### Employee One (male nail tech, the panicker)
> `EMP1: a slim man in his 30s, black scrub top and black pants, short twists hairstyle, thin mustache, nitrile gloves, very expressive face that swings quickly from friendly to horrified`

### Employee Two (nail tech, the frozen one)
> `EMP2: a woman in her 40s, black scrub top, hair in a tight high bun, reading glasses on a chain, stern face, slow-blinking stunned expression`

### The Owner
> `OWNER: a heavyset man in his 50s, bald with a grey horseshoe hairline, rolled-up sleeves on a pink button-down shirt, loosened tie, sweaty forehead, gold watch, dramatic exaggerated facial expressions`

Owner prop: a white handheld bullhorn.

### Female Cavewoman (final button)
- **Human-passing:**
  > `CAVEWOMAN_HUMAN: a confident woman about 40 years old, long thick dark wavy hair, strong brow, warm brown skin, oversized long coat, gloves, knee-high boots, large sunglasses pushed up on her head`
- **Transformed:**
  > `CAVEWOMAN: the same woman transformed into a cavewoman, wilder voluminous hair, heavier brow, brown sackcloth wrapped across the chest and from waist to mid-thigh, extremely long thick ancient fingernails and toenails matching the cavemen, proud joyful grin`

### Minor references
- `ANCHOR: a polished news anchor in a navy suit, seated at a glossy news desk, "BREAKING NEWS" lower-third graphic`
- `GUESTS: two spa customers, a man and a woman in casual shorts and t-shirts, standing in line at reception`
- `CROWD: a diverse crowd of pedestrians on a city sidewalk in winter coats, holding up phones`

### Consistency tips
1. Generate each character's reference sheet with a **fixed seed** and keep the best front and three-quarter images as the canonical references.
2. Make every shot with a named character **image-to-video (I2V)**. First build a still keyframe using the references through IP-Adapter, PuLID, or Toonflow's character assets, then animate it. Use text-to-video (T2V) only for plates and crowds.
3. If faces still drift, train a small character LoRA on 15 to 25 reference images each for Dan and Tom.
4. Keep the descriptor blocks word-for-word, and keep the lighting language consistent within each scene.

## 2. Prompt Conventions

**Wan 2.2 structure:** subject with descriptor block, then action (one continuous motion), then setting, then camera, then lighting, then style.
**LTX-Video variant:** LTX responds best to a single flowing paragraph that leads with the action, describes the camera move explicitly, and stays under about 200 words. When a shot below has no separate LTX note, use the Wan prompt as-is.
**Clip length:** keep each clip to one beat of about 5 seconds, and extend in the edit with holds and cutaways.
**Global style suffix** (append to every prompt): `cinematic 35mm film look, shallow depth of field, natural color grade, photorealistic, comedic timing, subtle film grain`
**Global negative prompt:** `blurry, distorted face, extra fingers, extra limbs, deformed hands, melting features, flicker, text artifacts, watermark, cartoon, nudity, gore, low quality, jitter, morphing between characters`

---

## 3. Scene One: Mountain Treehouse

| # | Shot | Framing | Time | Mode | Dialogue |
|---|---|---|---|---|---|
| 1.01 | Treehouse on the mountain face, Dan hanging off the side | Extreme wide, slow push-in | 5s | T2V | — |
| 1.02 | Dan's toenails dug into the bark, rope dangling unused | Macro close-up, tilt up | 4s | I2V | — |
| 1.03 | Dan sanding the window trim one-handed, totally casual | Medium, slight handheld | 5s | I2V | — |
| 1.04 | Interior through the tall windows: vaulted ceiling, chandeliers, couches, TV | Wide interior, slow dolly | 5s | T2V | — |
| 1.05 | Tom at the base of the tree looking up, arms crossed | Low-angle medium | 3s | I2V | — |
| 1.06 | Tom's line | Medium close-up on Tom | 5s | I2V | "Come on pop. At least hook the rope to your carabiner, for the allusion of safety." |
| 1.07 | Dan looks down, dead-eyed | High-angle close-up on Dan | 4s | I2V | "You being serious right now?" |
| 1.08 | Button: Dan lets go with one hand to wave the rope off; the rope swings | Wide two-shot | 4s | I2V | — |

**1.01 (Wan):** `A huge ancient tree growing out of a sheer mountain cliff, a luxury treehouse built into its trunk with tall glowing windows and crystal chandeliers visible inside, a small muscular caveman figure clinging to the outside wall beside a dangling unused rope, misty pine valley below, golden hour backlight, slow aerial push-in, epic yet comedic, [style]`
LTX: `Slow aerial push-in toward a luxury treehouse built into an ancient tree on a cliff face. Tall windows glow warm with chandeliers inside. A tiny muscular caveman clings to the outside wall while a rope dangles unused beside him. Golden hour, mist below.`

**1.02 (Wan):** `Extreme close-up of [DAN] bare feet, extremely long thick yellowed ancient toenails embedded deep into rough tree bark, toes flexing to grip, a climbing rope swaying loosely in the background untouched, camera slowly tilts up the muscular calf, warm late sunlight, [style]`

**1.03 (Wan):** `[DAN], wearing a brown waist cloth, hangs off the outside of a treehouse wall gripping it only with his toenails, calmly sanding a window frame with one hand and blowing sawdust away, relaxed and focused, rope dangling unused beside him, mountain drop behind, medium shot with gentle handheld sway, golden hour, [style]`

**1.04 (Wan):** `Interior of a luxury treehouse living room: soaring vaulted wooden ceiling, two crystal chandeliers, polished clean wooden floors, plush cream sectional couches, large flat-screen TV mounted on a log wall, tall windows showing mountain sky, slow dolly forward, warm ambient light, architectural photography realism, [style]`

**1.05 (Wan):** `[TOM], wearing a short sackcloth tunic, stands on a rocky ledge at the base of a giant tree, arms crossed, looking up with a skeptical concerned frown, low-angle medium shot, wind moving his hair, golden hour rim light, [style]`

**1.06 (Wan):** `[TOM] cups one hand to his mouth and calls upward, talking with an exasperated expression and pointing at a dangling rope, medium close-up, slight low angle, golden hour, [style]`

**1.07 (Wan):** `[DAN] hangs from the treehouse wall and slowly turns his head to look down at the camera, deadpan unimpressed expression, eyebrows raised, speaking briefly, high-angle close-up, sky behind him, [style]`

**1.08 (Wan):** `Wide shot: [DAN] hangs from a treehouse wall by his toenails and casually lets go with one hand to wave dismissively, the unused rope swinging, [TOM] below throws his hands up in disbelief, golden hour, comedic, [style]`

**Pacing:** Let 1.01 breathe as the scale reveal, cut fast through 1.02 and 1.03, and hold a full beat of silence after 1.07 before the button.

---

## 4. Scene Two: News Broadcast and Phone Call

*Staging fix:* the script mixes up who is where. This version keeps **Dan at home** in his chair and **Tom at his own apartment**, then intercuts the phone call.

| # | Shot | Framing | Time | Mode | Dialogue |
|---|---|---|---|---|---|
| 2.01 | Over Dan's right shoulder: armchair, huge stone fireplace, medieval crock pot, rotisserie pig, TV on | Over-the-shoulder wide | 5s | I2V | — |
| 2.02 | News anchor, breaking-news graphic | Medium, locked-off TV framing | 5s | T2V | "This just in, the illegal Alien Ban has been lifted…" |
| 2.03 | Anchor continues | Same framing, slow push | 5s | T2V | "…All aliens in the U.S. and across the globe are considered legal. You are all free to… (pause) be you!" |
| 2.04 | Celebration montage A: street party | Wide, handheld news footage | 4s | T2V | — |
| 2.05 | Celebration montage B: neighborhood festival with flags | Medium, handheld | 4s | T2V | — |
| 2.06 | Celebration montage C: families dancing in a park | Wide | 4s | T2V | — |
| 2.07 | Tom on his couch watching the same news, slow-blinking | Medium close-up | 4s | I2V | — |
| 2.08 | Tom, surprised, grabs his phone | Medium | 3s | I2V | — |
| 2.09 | Dan's phone rings and he answers, still in pajamas | Medium close-up | 4s | I2V | — |
| 2.10 | Tom on the phone | Close-up | 3s | I2V | "Happy born day pops. What you up to?" |
| 2.11 | Dan, cozy | Close-up | 4s | I2V | "You know me son, sittin around relaxing." |
| 2.12 | Tom | Close-up | 3s | I2V | "Let's go out to eat. Got a birthday surprise for you." |
| 2.13 | Dan, flat | Close-up | 3s | I2V | "You know I hate going out in public." |
| 2.14 | Tom stands and grabs his keys | Medium | 3s | I2V | "Get dressed. I'm on my way." |
| 2.15 | Dan sighs at the pig rotating on the spit | Over-the-shoulder | 3s | I2V | — |

**2.01 (Wan):** `Over-the-shoulder shot from behind the right shoulder of [DAN] in plaid flannel pajamas, sitting in a big worn leather armchair, facing a massive stone fireplace where a whole pig turns on an iron rotisserie spit beside an old medieval iron crock pot, a TV glowing to the side, firelight flicker, cozy cabin interior, static camera, [style]`

**2.02 / 2.03 (Wan):** `[ANCHOR] speaking directly to camera with growing excitement, red "BREAKING NEWS" banner along the bottom, bright studio lighting, broadcast television look, locked-off medium shot, [style]`
LTX: `A news anchor in a navy suit at a glossy desk delivers breaking news straight to camera, a red banner below, bright studio light. The camera holds, then pushes in slightly as the anchor smiles broadly.`

**2.04 to 2.06 (Wan):** use respectful, joyful crowds with no stereotyped costumes.
- 2.04: `Handheld news footage of a joyful diverse crowd dancing in a city street, people of many backgrounds hugging and cheering, confetti, daytime, broadcast news look, [style]`
- 2.05: `Handheld news footage of a lively neighborhood festival, many different national flags waving, people dancing to music, warm afternoon light, [style]`
- 2.06: `Wide shot of multigenerational families dancing together in a sunny park, kids on shoulders, celebration, broadcast news look, [style]`

**2.07 (Wan):** `[TOM] in a hoodie sits on a couch in a modern apartment, lit by a TV, staring at the screen and blinking slowly twice with a stunned, surprised look, medium close-up, cool TV light on his face, [style]`

**2.09 / 2.11 / 2.13 (Wan):** `[DAN] in plaid flannel pajamas sits in a leather armchair holding a phone to his ear, relaxed, warm fireplace glow on his face, speaking calmly with a slight frown, close-up, [style]`

**2.10 / 2.12 / 2.14 (Wan):** `[TOM] in a hoodie holds a phone to his ear, grinning and talking warmly, modern apartment background, soft daylight, close-up, [style]` (for 2.14, add `stands up from the couch and grabs car keys`).

**Pacing:** Play the newscast straight and serious. Hold on Tom's blink (2.07) for comedic timing. Keep the call itself as quick tennis-match cutting.

---

## 5. Scene Three: Car Ride to the Spa

| # | Shot | Framing | Time | Mode | Dialogue |
|---|---|---|---|---|---|
| 3.01 | Tom's car pulls up to Dan's place in winter and honks | Wide exterior | 4s | T2V | — |
| 3.02 | Dan's front door opens and he walks out fully bundled, hair bursting from his hat | Full shot | 5s | I2V | — |
| 3.03 | Dan climbs into the car and they drive off | Wide | 4s | I2V | — |
| 3.04 | Two-shot through the windshield | Front two-shot | 4s | I2V | Tom: "We ain't been out." / Dan: "You know I hate going out in public." |
| 3.05 | Tom reassures him | Side close-up on Tom | 4s | I2V | "Pop, I wouldn't ask you to go out if it wasn't ok." |
| 3.06 | Dan turns serious | Close-up on Dan | 4s | I2V | "So, you mean, it passed?" |
| 3.07 | Tom beams | Close-up | 3s | I2V | "Everyone's excited!" |
| 3.08 | Dan nods gravely | Close-up | 3s | I2V | "They have every reason to be." |
| 3.09 | Tom pitches the mani-pedi | Two-shot | 4s | I2V | "To celebrate, how bout a mani-pedi?" |
| 3.10 | Dan, curious | Close-up | 4s | I2V | "Always wondered about those. What do they do?" |
| 3.11 | Tom explains | Close-up | 5s | I2V | "Well, two good looking women work on your feet and hands at the same time while massaging your calf muscles." |
| 3.12 | Dan leans back, satisfied | Close-up | 5s | I2V | "Sounds good. I'm overdue to be pampered. Then, can we eat?" |
| 3.13 | Tom smirks | Close-up | 3s | I2V | "Just sit back and enjoy the show." |
| 3.14 | The car pulls up outside the nail spa storefront | Wide exterior | 4s | T2V | — |

**3.01 (Wan):** `A dark blue sedan pulls up in front of a rustic snowy cabin at dusk and stops, headlights on, light snow falling, exhaust in the cold air, static wide shot, cold blue winter light with warm cabin windows, [style]`

**3.02 (Wan):** `[DAN] steps out of a cabin door in heavy winter gear: charcoal parka, knit beanie with wild hair bursting out beneath it, long beard spilling over a scarf, thick gloves and boots, trudging through snow toward the camera with a grumpy deadpan face, full shot, snowy dusk, [style]`

**3.04 (Wan):** `Front view through a car windshield of [TOM] driving in a puffer jacket and beanie and [DAN] in the passenger seat in a parka with his beard over his scarf, Tom glancing over and talking, Dan staring ahead unimpressed, passing streetlights sweeping across their faces, winter evening, [style]`
LTX: `Through the windshield of a moving car at night, a young caveman driver chats while his bundled-up, bearded father stares straight ahead. Streetlights sweep across them rhythmically. Static windshield-mounted camera.`

**3.05 to 3.13 (Wan template):** `Close-up of [CHARACTER] in the car, [wardrobe], [action/expression], passing streetlight glow, shallow focus, [style]`
- 3.06: `slowly turns his head toward Tom, serious searching expression`
- 3.10: `eyebrows rising, curious`
- 3.12: `leans back into the seat, eyes half closed in contentment, then a small hopeful look`
- 3.13: `knowing smirk, eyes on the road`

**3.14 (Wan):** `A sedan pulls up to the curb outside a bright upscale nail spa storefront with a wide picture window, leather pedicure chairs visible inside, a neon "NAILS & SPA" sign, snowy city sidewalk with pedestrians, evening, static wide, [style]`

**Pacing:** This is a calm, intimate scene. Use slower cuts and let 3.06 sit; it's the one sincere beat before the chaos.

## 6. Scene Four: The Spa Transformation

**Set:** a bright nail spa. It has a front desk, a nail-tip color display, and a wall TV playing the government news. A wide picture window faces the street. Raised leather pedicure chairs (you step up into them) sit in front of the window with running-water foot basins, and a lower row of matching chairs sits behind them.

| # | Shot | Framing | Time | Mode | Dialogue |
|---|---|---|---|---|---|
| 4.01 | Spa interior establishing: window chairs, foot basins, nail display, TV news | Wide, slow pan | 5s | T2V | — |
| 4.02 | Dan and Tom at the desk in human-passing look, the two guests in line behind them | Medium wide | 4s | I2V | — |
| 4.03 | Desk worker greets them | Medium close-up | 4s | I2V | "Hello. Can I get the name for the appointment?" |
| 4.04 | Tom answers | Medium | 3s | I2V | "Tom, and Dan DaCaveman." |
| 4.05 | Worker gestures to the window chairs | Medium | 3s | I2V | "Have a seat right here." |
| 4.06 | They step up and sit, feet into the running water | Wide | 5s | I2V | — |
| 4.07 | Pedestrians start gathering outside the window | Exterior looking in | 4s | T2V/I2V | — |
| 4.08 | Dan sinks back, blissful | Close-up | 4s | I2V | "Wow, son! I feel good." |
| 4.09 | Tom, smug | Close-up | 5s | I2V | "Told you. This one of the best feelings in the world. To have women rub and pamper you." |
| 4.10 | Tom turns to his dad | Two-shot | 5s | I2V | "Be comfortable. We don't have to hide anymore. It's the law." |
| 4.11 | Dan | Close-up | 2s | I2V | "Everything?" |
| 4.12 | Tom | Close-up | 3s | I2V | "Everything, pop. Watch me!" |
| 4.13 | **Tom's transformation** | Medium, slow push | 5s | I2V (Wan) | — |
| 4.14 | Crowd outside gasps | Exterior wide | 3s | I2V | (gasp) |
| 4.15 | **Dan's transformation** | Medium, slow push | 5s | I2V (Wan) | — |
| 4.16 | The crowd rushes the window, shocked | Exterior wide | 4s | I2V | — |
| 4.17 | Insert: Tom's finger-length nails and thick toenails | Macro | 3s | I2V | — |
| 4.18 | Dan wiggles his toes happily | Close-up on feet | 4s | I2V | "Ah, it's good to finally give my feet some air!" |
| 4.19 | People outside filming on their phones | Exterior medium | 4s | I2V | — |
| 4.20 | Tom staring in amazement (beat 1) | Close-up | 2s | I2V | — |
| 4.21 | Tom staring in amazement (beat 2, tighter) | Extreme close-up | 2s | I2V | — |
| 4.22 | Dan, oblivious | Close-up | 2s | I2V | "What's wrong son?" |
| 4.23 | Tom | Close-up | 3s | I2V | "You could've left some clothing on." |
| 4.24 | Two guests bolt out the door | Wide | 3s | I2V | — |
| 4.25 | Dan pats his chest hair | Close-up | 3s | I2V | "My fur got me covered." |
| 4.26 | The customer beside them gags, hand over mouth | Medium | 3s | I2V | — |
| 4.27 | Employees One and Two walk out from the back, unaware | Medium tracking | 4s | I2V | — |
| 4.28 | More customers grab their things and leave | Wide | 3s | I2V | — |
| 4.29 | Employee One greets them, then jumps back | Medium | 4s | I2V | "How are you guys doing… ohh my God!" |
| 4.30 | Employee Two, frozen in fear and confusion | Close-up | 3s | I2V | "What the hell am I looking at?" |
| 4.31 | Employee One walks in circles, panicking | Medium wide | 4s | I2V | "We gotta close the shop! We gotta close the shop!" |
| 4.32 | The owner rushes out and nearly trips | Wide | 4s | I2V | — |
| 4.33 | Owner's rant | Medium close-up | 5s | I2V | "Are you freakin kidding me! The ban hasn't even been lifted for twenty-four hours yet. I thought you guys only come out at night!" |
| 4.34 | Dan, delighted | Close-up | 5s | I2V | "I know that song! The freaks come out at night! Nope, me and my son here for the free mani-pedi, it's my birthday." |
| 4.35 | Owner, disgusted, gulping | Close-up | 3s | I2V | "That's nasty." |
| 4.36 | Owner yells through the bullhorn toward the back | Medium | 5s | I2V | "Get me a chisel, a sander and a hazmat bucket. Better make it two hazmat buckets, a few face shields and some thick rubber gloves!" |
| 4.37 | Employee One protests | Medium close-up | 3s | I2V | "Naw man! One of y'all gonna have to pay!" |
| 4.38 | Owner | Close-up | 2s | I2V | "You can't say that!" |
| 4.39 | Employee One | Close-up | 4s | I2V | "What you mean? We can close the shop for the week on this ticket alone!" |
| 4.40 | Montage: employees in face shields and rubber gloves grinding claws with a sander | Medium | 5s | I2V | — |
| 4.41 | A new woman checks in at the desk with the owner | Medium | 4s | I2V | — |
| 4.42 | She sees the two cavemen and breathes deeply | Close-up | 3s | I2V | — |
| 4.43 | **Cavewoman transformation** | Medium, slow push | 5s | I2V (Wan) | — |
| 4.44 | Button: she throws her arms up | Medium wide | 3s | I2V | "It's my birthday!" |

### Key prompts

**4.01 (Wan):** `Interior of a bright modern nail spa: a row of raised black leather pedicure chairs with steps, in front of a wide street-facing picture window, running water filling the foot basins, a lower row of matching chairs behind, a wall display of colorful nail tips, a white front desk, a wall TV showing a news broadcast, slow lateral pan, clean soft daylight, [style]`

**4.02 (Wan):** `[TOM] in a hoodie, joggers, and gloves and [DAN] in a parka, beanie with hair poking out, and gloves stand at a white spa reception desk, two customers in shorts and t-shirts waiting behind them, nail-tip display on the wall, medium wide shot, bright spa light, [style]`

**4.03 (Wan):** `[DESK] smiles politely behind the reception counter and speaks, tablet in hand, medium close-up, bright clean spa lighting, [style]`

**4.06 (Wan):** `[DAN] and [TOM], still in human-passing clothes with shoes off and gloves on, step up into raised leather pedicure chairs in front of a large picture window and lower their feet into bubbling running-water basins, wide shot, [style]`

**4.07 (Wan):** `Exterior shot looking into a nail spa through a large picture window, curious pedestrians in winter coats gathering on the snowy sidewalk and peering in at two men in pedicure chairs, evening streetlight, static, [style]`

**4.13 Tom's transformation (Wan, I2V from a still of Tom seated):** `[TOM] seated in a raised leather pedicure chair inhales deeply with eyes closed, his hoodie and clothes ripple and fall away as his form subtly expands into a caveman: fuller hair, heavier brow, a brown sackcloth across his chest like a tank top and from his waist to upper thighs, fingernails growing as long as his fingers, toenails thickening, he exhales calmly and smiles, slow push-in, soft magical realism, PG-13, [style]`
LTX: `A young man in a spa chair takes a deep breath and transforms in one smooth motion. His clothes fall away into a brown sackcloth top and short wrap, his hair grows wild, and his nails lengthen into thick claws. Slow push-in, bright spa lighting, calm smile at the end.`
*Tip:* Make the before and after keyframes as separate stills and, if your workflow supports it, use first-frame/last-frame conditioning so the transformation lands on the canonical transformed reference.

**4.15 Dan's transformation (Wan):** same structure with `[DAN]`. End state: `a brown sackcloth covering only his waist to upper thighs, bare broad hairy chest, extremely long curved claws on hands and feet`. Add `beanie pops off, wild hair springs out`.

**4.14 / 4.16 (Wan):** `Exterior through the spa picture window: a crowd of pedestrians in winter coats gasping, hands over mouths, then rushing toward the glass with shocked faces, evening, handheld, [CROWD], [style]`

**4.17 (Wan):** `Macro close-up of [TOM]'s hand resting on a leather armrest, fingernails as long as his fingers, thick and ridged, then the camera tilts down to massive prehistoric toenails in bubbling water, [style]`

**4.18 (Wan):** `Close-up of [DAN]'s bare feet with enormous ancient claw-like toenails wiggling happily in the bubbling foot basin, steam rising, then tilt up to his blissful face, [style]`

**4.19 (Wan):** `Exterior medium shot of pedestrians pressed against the spa window holding up phones to film and photograph, phone flashes going off, excited shocked faces, [style]`

**4.24 (Wan):** `[GUESTS] in shorts and t-shirts leap up from the lower spa chairs and run out the front door in panic, bell on the door jangling, wide, [style]`

**4.26 (Wan):** `A woman in a spa chair next to the cavemen puts a hand to her mouth, cheeks puffing slightly as she gags, eyes watering, mild comedic, medium shot, [style]`

**4.29 (Wan):** `[EMP1] walks up smiling and starts a friendly greeting, then sees something off-camera and leaps backward in horror, arms flailing, medium shot, [style]`

**4.30 (Wan):** `[EMP2] freezes mid-step holding a nail file, slowly lowering her glasses, face fixed in fear and confusion, close-up, [style]`

**4.31 (Wan):** `[EMP1] pacing in a frantic small circle in the middle of a nail spa, hands on his head, shouting, medium wide, slight handheld, [style]`

**4.32 (Wan):** `[OWNER] bursts out of a back-room door, slips on the wet floor and nearly falls, catching himself on a manicure table, wide, comedic, [style]`

**4.33 / 4.35 (Wan):** `[OWNER] sweaty and outraged, waving his hands and ranting, face twisting in disgust and taking big gulps, medium close-up, [style]`

**4.34 (Wan):** `[DAN] in caveman form, reclining in a pedicure chair, lights up with delight and points as if recognizing a song, then shrugs happily, close-up, [style]`

**4.36 (Wan):** `[OWNER] raises a white bullhorn and yells toward the back of the nail spa, veins on his forehead, medium shot, [style]`

**4.40 (Wan):** `[EMP1] and [EMP2] in face shields and thick yellow rubber gloves, grimacing and leaning away as they grind enormous claw-like toenails with a power sander, sparks and dust, [DAN] relaxing blissfully, medium shot, comedic, [style]`

**4.41 / 4.42 (Wan):** `[CAVEWOMAN_HUMAN] at the spa front desk with [OWNER], she glances toward the window chairs, sees the two cavemen, her eyes widen and then she smiles and takes a deep breath, [style]`

**4.43 (Wan, I2V):** `[CAVEWOMAN_HUMAN] takes a deep breath and transforms smoothly into [CAVEWOMAN]: her coat falls away into a brown sackcloth wrapped across her chest and from waist to mid-thigh, her hair grows wild and voluminous, her nails grow into long thick claws matching the cavemen's, slow push-in, PG-13, [style]`

**4.44 (Wan):** `[CAVEWOMAN] throws both arms up joyfully and shouts, [OWNER] behind the desk drops his bullhorn in despair, the cavemen in the background cheering, medium wide, freeze-frame energy, [style]`

**Pacing:** Shots 4.01 to 4.12 should feel calm and almost sweet. After 4.13, speed up the cutting. Put a crowd reaction between each transformation and the next beat. The double "amazement" shots (4.20 and 4.21) are a deliberate stutter-hold. End on a hard cut to black after "It's my birthday!"

## 7. Recommended Generation Order

1. **Character reference sheets.** Generate Dan and Tom first, including every wardrobe state, then the Owner, Employee One, Employee Two, the desk worker, and the cavewoman in both forms. Lock seeds and choose the canonical images. Everything after this depends on them.
2. **Location plates.** Make empty-set stills of the treehouse exterior and interior, Dan's living room (fireplace, crock pot, rotisserie pig), Tom's apartment, the snowy cabin exterior, the car interior, the spa exterior, and the spa interior (window chairs, desk, nail display, TV). They keep backgrounds consistent between shots.
3. **News footage.** Generate 2.02 to 2.06 next. These are self-contained shots with no recurring faces, and they also serve as the TV-screen inserts in scene 4.
4. **Establishing shots.** Generate 1.01, 1.04, 2.01, 3.01, 3.14, and 4.01. They set the lighting and color grade that later shots should match.
5. **Character keyframes.** For each remaining shot, compose a still using the character references on the location plate, then animate it with image-to-video. This is where face consistency is won or lost.
6. **Dialogue and reaction shots.** Work scene by scene in story order so wardrobe states don't get mixed up.
7. **Transformation shots last.** Do 4.13, 4.15, and 4.43 with Wan 2.2 at the highest quality. They need both locked "before" and "after" keyframes and will take the most rerolls.
8. **Lip-sync and audio pass.** Record or synthesize each character's lines, run a lip-sync pass on the dialogue close-ups, then assemble, grade, and mix.

Draft everything in LTX-Video first for timing, then re-render the keepers in Wan 2.2.

## 8. Dialogue, Sound, and Edit Notes

- **Voices:** cast a distinct voice per character. Dan is a low, slow, gravelly deadpan. Tom is warm and quick. The Owner is loud and nasal. Employee One is high-energy. I haven't checked which open-source text-to-speech and lip-sync tools are best right now, so test a couple on one close-up before committing.
- **Music:** use a cozy acoustic bed for scenes 1 and 3, a serious news sting for scene 2, and spa lounge music in scene 4 that cuts out with a record-scratch at Tom's transformation. Add a brief sting of "The Freaks Come Out at Night" only if you license it; otherwise use a soundalike.
- **Edit rhythm:** hold one beat longer than feels natural on every deadpan line. The comedy lives in the pauses before the reaction cuts.

## 9. Script Issues to Fix Before Generating

1. Scene 4 opens with "Dan and **Dave** DaCaveman." This should probably be Tom.
2. Scene 2 has Tom sitting and blinking at the TV while Dan is "on the phone," then says Tom calls his father. I staged it as Tom at his apartment and Dan at home, intercut.
3. "Allusion of safety" should be "illusion." I kept it as written in case the wordplay is intentional.
4. "My **fir** got me covered" should be "fur." I used "fur" in the shot list.
5. "Twenty-**fours**" should be "twenty-four hours." I fixed it in 4.33.
6. **Content:** I kept the sackcloth coverage PG-13 so model safety filters don't block renders and the skit stays shareable. The celebration montage shows joyful, respectful crowds with no stereotyped costumes, and the gag beat is mild.

**Totals:** 81 shots (Scene 1: 8, Scene 2: 15, Scene 3: 14, Scene 4: 44). Raw clips run about 5:10, so expect a final cut of roughly 5 to 6 minutes with comedic holds, a bit longer than the estimate at the top of the packet.
