# Nothing New, Foo! V22 — cartoon music-video shot list

- Task: nnf-v22-video (DaCaveman Video Producer). Audio: Nothing_New_Foo_V22.mp3, 240.024 s, 48 kHz, sha256 7475748785b51ed871d9a789fc5ddcc983afa66feaef00e53c401166d2a61e44 (verified).
- Measured: 100.00 BPM, beat 0.600 s, first strong beat 0.58 s; music drop ~18.6 s; low-energy breakdown ~174-180 s; fade ~236-240 s. Every cut below is snapped to that beat grid.
- What ASR heard sung (faster-whisper small, word timestamps): intro 'Big A-T-L / Fayetteville / Dirty South / Morning legends / We always grind / We do it well' 0.5-19 s; chorus 60-76 s; VERSE names ARE sung ~76.5-86.3 s ('Da-Corrie with the plan, Alfred on the door, George pulls the night, Melissa runs the floor'); 'We be about it' ~112.5-115.5 s; outro 'Nothing new foo, same old thing, we be about it' ~222-228 s. Bridge words were not detected → bridge scenes are beat-timed only.
- Global style for all Grok Image stills: 2D cartoon TV-series style, clean bold outlines, vibrant cel-shaded colors (style ref: nnf_00_george_alfred_desk). All crew are stylized cartoon characters (no reference photos; no likeness claimed).
- Wan I2V settings (all clips): Wan2.2 TI2V 5B fp16, euler / simple, shift 8, 20 steps, cfg 4, 640x480, 73 frames (4n+1, ~3.0 s @24 fps), sequential on Mac Studio ComfyUI. Prompt suffix on every clip: "Single continuous shot, slow steady camera, 2D cartoon animation style with clean bold outlines and vibrant flat colors, consistent character design, smooth lively motion until the last frame."
- Wan negative prompt (all clips): "static, still image, frozen pose, slideshow, rapid camera movement, whip pan, flicker, scene cut, magenta, purple tint, overexposed, underexposed, blurry, photorealistic, 3d render, text distortion, watermark, extra fingers, extra limbs, face distortion, identity change, melting"
- Assembly: clean-window Wan clip ping-pong (fwd+rev) per shot, punch-in crop on re-use, 4:3 picture on blurred 16:9 bed at 1280x720, saturation +12 %, white flash on titled shots, name cards / gag captions as lower thirds (visual only).

## A. Assets (Grok Image still → Wan I2V motion prompt)

| asset id | status | Grok Image still prompt (summary) | Wan I2V motion prompt |
|---|---|---|---|
| nnf_00_george_alfred_desk | V21 set | George (stocky, curly dark hair, thick mustache, black glasses, white shirt, navy vest, patterned tie, gold badge, NIGHT AUDIT clipboard) and Alfred (tall, short braids, trimmed beard, dark three-piece suit, thumbs up) behind the wooden front desk; gold 'Trilith Guest House' sign; amber lamps, teal night windows. Refs: igo_01_lobby_welcome.jpg + igo_george_cu.jpg (existing Alfred Studio stills). | The mustached clerk waves the night audit clipboard and grins while the man in the dark suit gives a thumbs up and nods, both bobbing to the music. |
| nnf_01_exterior_night | V21 set | Exterior of the boutique hotel at night, glowing gold 'Trilith Guest House' sign, warm windows, string lights, Georgia trees, purple-teal starry sky, smiling moon; no people. | Slow gentle push-in toward the glowing hotel entrance, string lights twinkling, trees swaying softly, stars sparkling, the little moon smiling. |
| nnf_02_title_fayetteville | V21 set | Title card: chunky 3D lettering 'FAYETTEVILLE, GEORGIA' over graffiti 'DIRTY SOUTH!', stylized sunset skyline, Georgia pines, peaches, road sign; 90s hip-hop poster, orange/magenta/teal. (Animated in ffmpeg, not Wan, so text never warps.) | — (ffmpeg-animated still: slow push + beat pulse; not sent to Wan) |
| nnf_03_late_checkout | V21 set | George at the desk holding an alarm clock and a 'LATE CHECKOUT = MEMBERS' sign; a pleading guest in bathrobe and sunglasses shows an empty wallet, a moth flies out. | The guest in the bathrobe pleads dramatically, shaking his empty wallet as a moth flutters out, while the mustached clerk holds up the alarm clock and sign and shakes his head with a polite grin. |
| nnf_04_red_carpet | V21 set | Online-booking crew of travelers waving phones ('$1 BOOKING!', 'VIP UPGRADE!'), diva poses; Alfred deadpan unrolls a red carpet. No brand logos. | The travelers wave their phones and strike diva poses while the man in the dark suit slowly unrolls the red carpet along the floor with a deadpan face. |
| nnf_05_ants_hallway | V21 set | Hotel hallway with sign 'NO MICROWAVES IN ROOMS'; conga line of cute big-eyed ants carrying pizza, popcorn, noodles; one in a chef hat. | The cute cartoon ants march happily in a conga line along the hallway carpet, carrying the pizza slice, popcorn and noodles, bobbing their heads to the beat. |
| nnf_06_ac_war | V21 set | Meeting room: three red-faced executives sweating, fanning with papers, fiery thermostat; staff rush in with box fans; wind lines, flying papers. | The sweating executives fan themselves frantically as the staff rush in carrying box fans, wind blowing papers and ties, sweat drops flying. |
| nnf_07_baby_milk_freezer | V21 set | George opens a glowing staff freezer with sparkling snowflakes; dad in striped pajamas holds a giggling baby with a milk bottle. | The mustached clerk proudly opens the glowing freezer as sparkling snowflakes float out, the dad smiles and the baby giggles and waves the milk bottle. |
| nnf_08_wedding_lawn | V21 set | Golden-hour wedding on the lawn of the Trilith Guest House: couple under floral arch, cheering guests, petals, tiered cake, staff with champagne trays. | The bride and groom smile under the floral arch as guests cheer and toss flower petals, waiters raise champagne trays, petals and butterflies drifting. |
| nnf_09_fivestar_vs_motel | V21 set | Lightning split screen: left a five-star lobby with chandeliers, five gold stars and a bowing doorman; right a shabby roadside motel with buzzing neon 'MOTEL 6', raccoon on ice machine, tumbleweed. | On the left the doorman bows grandly under sparkling gold stars and chandeliers; on the right the neon motel sign flickers and the raccoon scratches its head while the tumbleweed rolls. |
| nnf_10_morph_team_pose | V21 set | Original Saturday-morning hero-team homage (no franchise logos/costumes): crew in color-coded suits (red, yellow, green, blue, pink, purple, gold, silver) with key/bell/star/coffee emblems, fist-pump poses, energy beams and sparkles. | The colorful superhero team pump their fists and strike dynamic poses in sync as colored energy beams and sparkles burst behind them. |
| nnf_11_morph_into_one | V21 set | Rainbow energy streams rise from the hero team and merge into one giant glowing hero holding a golden key over the Trilith Guest House at dawn. | The rainbow energy streams swirl upward from the heroes and the giant glowing hero raises the golden key high, light rays pulsing, sparkles swirling. |
| nnf_12_lobby_dance | V21 set | Whole crew (~12) dancing hip-hop moves in the lobby around George and Alfred, confetti, purple/gold party light, Trilith sign. | The whole hotel crew dances hip-hop moves together in the lobby, arms pumping and heads bobbing to the beat, confetti falling. |
| nnf_13_barn_mud | V21 set | Mud-covered guest in cowboy hat tracks muddy footprints across the lobby; George gasps holding a mop; cow and chicken peek in the door. | The muddy guest in the cowboy hat stomps across the lobby leaving muddy footprints while the mustached clerk gasps and clutches his mop, the cow and chicken peeking in. |
| nnf_14_mama_plates | V21 set | Alfred, arms crossed and eyebrow raised, at a desk piled with dirty plates and a half-eaten burger; guest walks off whistling; thought bubble of a scolding grandma. | The man in the dark suit stands with crossed arms and raises one eyebrow at the pile of dirty plates, slowly shaking his head, while the guest walks away whistling. |
| nnf_15_sunrise_legends | V21 set | Whole crew on the porch steps of the Trilith Guest House at sunrise, coffee mugs raised, George and Alfred center, birds, golden rays. | The hotel crew on the porch raise their coffee mugs in a toast and cheer, swaying together as the sun rises and birds fly across the sky. |
| nnf_16_atl_skyline | NEW for V22 | Stylized Atlanta-style skyline at night turning to dawn, needle-topped tower, highway light trails, purple-to-peach sky, smiling stars, pine silhouettes. No text/logos. | Slow gentle push-in toward the glowing city skyline, highway light trails streaming forward, smiling stars twinkling, the sky brightening from purple to peach. |
| nnf_17_fayetteville_street | NEW for V22 | Small-town Southern main street at dawn leading to the white columned guest house, brick storefronts, string lights, green road sign 'FAYETTEVILLE', birds. | Slow forward dolly down the tree-lined main street toward the white guest house, string lights twinkling, birds flying across the pink dawn sky, leaves swaying. |
| nnf_18_dawn_desk_crew | NEW for V22 | 'Morning legends' at dawn: George, Alfred and three crew behind the front desk with steaming coffee mugs, sunrise through tall windows, Trilith sign. | The crew behind the front desk sip their steaming coffee, smile at each other and raise their mugs in a toast as golden sunrise light glows through the windows. |
| nnf_19_melissa_floor | NEW for V22 | Melissa (wavy blonde bob, headset, navy blazer) strides through the busy lobby with walkie and tablet, pointing; bellhop, housekeeper, server hustle past. | The blonde manager with the headset strides forward through the lobby talking into her walkie-talkie and pointing, while the bellhop, housekeeper and server hustle past behind her. |
| nnf_20_outro_shrug | NEW for V22 | Outro 'nothing new, foo — same old thing': George and Alfred lean on the desk doing a big shrug, clock spinning back, a new guest staggers in under a mountain of luggage. | The two men at the desk do a big slow exaggerated shrug and smirk at each other, the clock hands spin, the tired guest staggers in under the giant pile of luggage. |
| nnf_21_george_morph | NEW for V22 | George mid-transformation in the lobby raising a glowing golden key, red energy ribbons swirling as his vest becomes an original red hero suit with key emblem. | Red energy ribbons and sparkles swirl faster around the mustached hero as he thrusts the glowing golden key upward, his curly hair blowing, light rays pulsing. |
| nnf_rc01_dacorrie | V21 set | Da-Corrie: confident GM, neat fade + goatee, burgundy blazer, rolled blueprint, pointing at a whiteboard of arrows/stars/checkmark. | The man in the burgundy blazer taps the whiteboard plan confidently, nods and grins knowingly at the camera, holding the blueprint. |
| nnf_rc02_alfred | V21 set | Alfred swings the hotel front door open with a welcoming bow, golden light spilling onto the night porch. | The man in the dark suit swings the door open wider and bows graciously with a welcoming sweep of his arm, smiling. |
| nnf_rc03_george | V21 set | George on night audit: wink + thumbs up, glowing spreadsheet monitor, giant coffee, 3:00 clock, moon in window. | The mustached clerk winks, gives a big thumbs up and chuckles, steam rising from his coffee mug, the monitor glowing. |
| nnf_rc04_melissa | V21 set | Melissa at the front desk: wavy blonde bob, headset, navy blazer, slides a key card across the counter. | The blonde woman with the headset slides the key card across the counter and smiles warmly, nodding. |
| nnf_rc05_maggie | V21 set | Maggie keeps it fresh: red curly ponytail, mint housekeeping uniform, snapping a white sheet over a bed, petals, air-freshener puff. | The red-haired housekeeper snaps the white sheet up into the air and lets it float down over the bed, petals and sparkles swirling. |
| nnf_rc06_nia | V21 set | Nia brings the smile: curly puff, gold hoops, navy vest, tray of cookies, radiant smile with tooth sparkle. | The woman with the cookie tray beams a huge radiant smile and tilts her head, a sparkle glinting on her teeth. |
| nnf_rc07_jane | V21 set | Jane goes the extra mile: brown high ponytail, sneakers, sprinting a loaded luggage cart down the hallway toward a finish ribbon. | The woman sprints forward pushing the luggage cart, ponytail bouncing, speed lines and dust puffs behind her. |
| nnf_rc08_tracy | V21 set | Tracy on the phone: sleek black bob, cat-eye glasses, juggling three ringing phones, sticky notes everywhere. | The woman with glasses juggles the ringing phones, answering one after another, smiling and giving an OK sign. |
| nnf_rc09_beth_stacey | V21 set | Beth (silver-streaked hair, navy cardigan) and Stacey (long box braids, teal blazer) swing open the grand lobby doors, golden light. | The two women dance through the open doorway, pumping their fists and laughing, golden light glowing behind them. |
| nnf_rc10_trihana | V21 set | Trihana checks every floor: high bun, lavender supervisor suit, clipboard, magnifying glass, peeking from the elevator into a spotless room. | The woman in lavender peers through the magnifying glass, then gives a satisfied nod and checks her clipboard. |
| nnf_rc11_pete | V21 set | Pete at Prolog / Oliver's Twist: red beard, flat cap, apron, pouring latte art while holding a twisted pretzel in a cozy coffee bar. | The bearded barista pours latte art into the cup with a flourish while smiling, steam swirling up. |
| nnf_rc12_abby | V21 set | Abby at the bar: pixie cut, black vest + bow tie, shaking a cocktail, cherry lands in the glass, 'never miss' bullseye sparkle. | The bartender shakes the cocktail shaker energetically with a confident smile, glowing bottles behind her. |
| nnf_rc13_mike_lena | V21 set | Mike Johnson (shaved head, charcoal suit) and Lena (auburn waves, red dress) back to back with fire extinguishers putting out a tiny cake flame at an event venue (AYS). | The man and woman stand back to back spraying their fire extinguishers, foam puffs flying, both winking and smiling. |

## B. V22 edit decision list (beat-snapped)

| # | section | start–end (s) | dur (s) | asset (reuse/NEW) | on-screen card |
|---|---|---|---|---|---|
| 00 | INTRO (sung) | 0.00–3.58 | 3.58 | nnf_16_atl_skyline (NEW) | BIG A-T-L |
| 01 | INTRO (sung) | 3.58–7.78 | 4.20 | nnf_17_fayetteville_street (NEW) |  |
| 02 | INTRO (sung) | 7.78–9.58 | 1.80 | nnf_02_title_fayetteville (reuse, animated still) |  |
| 03 | INTRO (sung) | 9.58–12.58 | 3.00 | nnf_01_exterior_night (reuse) | NOTHING NEW, FOO! / Trilith Guest House |
| 04 | INTRO (sung) | 12.58–18.58 | 6.00 | nnf_18_dawn_desk_crew (NEW) | MORNING LEGENDS |
| 05 | MONTAGE A (instrumental) | 18.58–22.18 | 3.60 | nnf_12_lobby_dance (reuse) |  |
| 06 | MONTAGE A (instrumental) | 22.18–29.38 | 7.20 | nnf_03_late_checkout (reuse) | NO BONVOY CARD? / ...still wants late checkout |
| 07 | MONTAGE A (instrumental) | 29.38–34.18 | 4.80 | nnf_04_red_carpet (reuse) | THE EXPEDIA CREW / wants the red carpet |
| 08 | MONTAGE A (instrumental) | 34.18–38.98 | 4.80 | nnf_05_ants_hallway (reuse) | NO MICROWAVES / the ants found the crumbs |
| 09 | MONTAGE A (instrumental) | 38.98–43.78 | 4.80 | nnf_06_ac_war (reuse) | THE AC WAR |
| 10 | MONTAGE A (instrumental) | 43.78–48.58 | 4.80 | nnf_07_baby_milk_freezer (reuse) | SPECIAL REQUEST / baby's milk in the freezer |
| 11 | MONTAGE A (instrumental) | 48.58–53.38 | 4.80 | nnf_08_wedding_lawn (reuse) | WEDDING ON THE LAWN |
| 12 | MONTAGE A (instrumental) | 53.38–57.58 | 4.20 | nnf_09_fivestar_vs_motel (reuse) | FIVE-STAR PRIDE / not Motel 6 |
| 13 | MONTAGE A (instrumental) | 57.58–59.98 | 2.40 | nnf_00_george_alfred_desk (reuse) |  |
| 14 | CHORUS (sung) | 59.98–62.98 | 3.00 | nnf_18_dawn_desk_crew (NEW) |  |
| 15 | CHORUS (sung) | 62.98–64.78 | 1.80 | nnf_02_title_fayetteville (reuse, animated still) |  |
| 16 | CHORUS (sung) | 64.78–67.78 | 3.00 | nnf_18_dawn_desk_crew (NEW) | MORNING LEGENDS |
| 17 | CHORUS (sung) | 67.78–70.18 | 2.40 | nnf_12_lobby_dance (reuse) |  |
| 18 | CHORUS (sung) | 70.18–72.58 | 2.40 | nnf_18_dawn_desk_crew (NEW) |  |
| 19 | CHORUS (sung) | 72.58–74.98 | 2.40 | nnf_15_sunrise_legends (reuse) |  |
| 20 | CHORUS (sung) | 74.98–76.18 | 1.20 | nnf_00_george_alfred_desk (reuse) |  |
| 21 | VERSE (sung, ~76.5-86.3 s) | 76.18–79.78 | 3.60 | nnf_rc01_dacorrie (reuse) | DA-CORRIE / with the plan |
| 22 | VERSE (sung, ~76.5-86.3 s) | 79.78–81.58 | 1.80 | nnf_rc02_alfred (reuse) | ALFRED / on the door |
| 23 | VERSE (sung, ~76.5-86.3 s) | 81.58–84.58 | 3.00 | nnf_rc03_george (reuse) | GEORGE / pulls the night |
| 24 | VERSE (sung, ~76.5-86.3 s) | 84.58–86.98 | 2.40 | nnf_19_melissa_floor (NEW) | MELISSA / runs the floor |
| 25 | MONTAGE B / crew (instrumental) | 86.98–89.38 | 2.40 | nnf_rc05_maggie (reuse) | MAGGIE / keeps it fresh |
| 26 | MONTAGE B / crew (instrumental) | 89.38–91.78 | 2.40 | nnf_rc06_nia (reuse) | NIA / brings the smile |
| 27 | MONTAGE B / crew (instrumental) | 91.78–94.18 | 2.40 | nnf_rc07_jane (reuse) | JANE / goes the extra mile |
| 28 | MONTAGE B / crew (instrumental) | 94.18–96.58 | 2.40 | nnf_rc08_tracy (reuse) | TRACY / on the phones |
| 29 | MONTAGE B / crew (instrumental) | 96.58–98.98 | 2.40 | nnf_rc09_beth_stacey (reuse) | BETH & STACEY / open every door |
| 30 | MONTAGE B / crew (instrumental) | 98.98–101.38 | 2.40 | nnf_rc10_trihana (reuse) | TRIHANA / checks every floor |
| 31 | MONTAGE B / crew (instrumental) | 101.38–103.78 | 2.40 | nnf_rc11_pete (reuse) | PETE / Prolog / Oliver's Twist |
| 32 | MONTAGE B / crew (instrumental) | 103.78–106.18 | 2.40 | nnf_rc12_abby (reuse) | ABBY / at the bar |
| 33 | MONTAGE B / crew (instrumental) | 106.18–108.58 | 2.40 | nnf_rc13_mike_lena (reuse) | MIKE JOHNSON & LENA / at AYS |
| 34 | MONTAGE B / crew (instrumental) | 108.58–112.18 | 3.60 | nnf_12_lobby_dance (reuse) |  |
| 35 | 'We be about it' hit | 112.18–115.78 | 3.60 | nnf_00_george_alfred_desk (reuse) | WE BE ABOUT IT |
| 36 | MONTAGE C (instrumental) | 115.78–118.18 | 2.40 | nnf_05_ants_hallway (reuse) |  |
| 37 | MONTAGE C (instrumental) | 118.18–120.58 | 2.40 | nnf_06_ac_war (reuse) |  |
| 38 | MONTAGE C (instrumental) | 120.58–122.98 | 2.40 | nnf_07_baby_milk_freezer (reuse) |  |
| 39 | MONTAGE C (instrumental) | 122.98–125.38 | 2.40 | nnf_08_wedding_lawn (reuse) |  |
| 40 | MONTAGE C (instrumental) | 125.38–127.78 | 2.40 | nnf_03_late_checkout (reuse) |  |
| 41 | MONTAGE C (instrumental) | 127.78–130.18 | 2.40 | nnf_09_fivestar_vs_motel (reuse) |  |
| 42 | MONTAGE C (instrumental) | 130.18–132.58 | 2.40 | nnf_13_barn_mud (reuse) | BORN IN A BARN? |
| 43 | MONTAGE C (instrumental) | 132.58–134.98 | 2.40 | nnf_04_red_carpet (reuse) |  |
| 44 | MONTAGE C (instrumental) | 134.98–137.38 | 2.40 | nnf_14_mama_plates (reuse) | YOUR MAMA DON'T WORK HERE |
| 45 | MONTAGE C (instrumental) | 137.38–139.78 | 2.40 | nnf_08_wedding_lawn (reuse) |  |
| 46 | MONTAGE C (instrumental) | 139.78–142.18 | 2.40 | nnf_15_sunrise_legends (reuse) |  |
| 47 | chorus bit ~143 s | 142.18–145.78 | 3.60 | nnf_18_dawn_desk_crew (NEW) |  |
| 48 | MONTAGE D / crew (instrumental) | 145.78–148.18 | 2.40 | nnf_19_melissa_floor (NEW) |  |
| 49 | MONTAGE D / crew (instrumental) | 148.18–150.58 | 2.40 | nnf_rc04_melissa (reuse) |  |
| 50 | MONTAGE D / crew (instrumental) | 150.58–152.98 | 2.40 | nnf_rc05_maggie (reuse) |  |
| 51 | MONTAGE D / crew (instrumental) | 152.98–155.38 | 2.40 | nnf_rc08_tracy (reuse) |  |
| 52 | MONTAGE D / crew (instrumental) | 155.38–157.78 | 2.40 | nnf_rc07_jane (reuse) |  |
| 53 | MONTAGE D / crew (instrumental) | 157.78–160.18 | 2.40 | nnf_rc12_abby (reuse) |  |
| 54 | MONTAGE D / crew (instrumental) | 160.18–162.58 | 2.40 | nnf_rc11_pete (reuse) |  |
| 55 | MONTAGE D / crew (instrumental) | 162.58–164.98 | 2.40 | nnf_rc06_nia (reuse) |  |
| 56 | MONTAGE D / crew (instrumental) | 164.98–167.38 | 2.40 | nnf_rc10_trihana (reuse) |  |
| 57 | MONTAGE D / crew (instrumental) | 167.38–169.78 | 2.40 | nnf_rc09_beth_stacey (reuse) |  |
| 58 | MONTAGE D / crew (instrumental) | 169.78–172.18 | 2.40 | nnf_rc13_mike_lena (reuse) |  |
| 59 | BRIDGE build (breakdown, beat-timed) | 172.18–173.38 | 1.20 | nnf_rc01_dacorrie (reuse) | DIFFERENT PLACES |
| 60 | BRIDGE build (breakdown, beat-timed) | 173.38–174.58 | 1.20 | nnf_rc02_alfred (reuse) |  |
| 61 | BRIDGE build (breakdown, beat-timed) | 174.58–175.78 | 1.20 | nnf_rc03_george (reuse) | ONE IDENTITY |
| 62 | BRIDGE build (breakdown, beat-timed) | 175.78–176.98 | 1.20 | nnf_rc04_melissa (reuse) |  |
| 63 | BRIDGE build (breakdown, beat-timed) | 176.98–178.18 | 1.20 | nnf_rc05_maggie (reuse) |  |
| 64 | BRIDGE build (breakdown, beat-timed) | 178.18–179.38 | 1.20 | nnf_rc06_nia (reuse) |  |
| 65 | BRIDGE build (breakdown, beat-timed) | 179.38–179.98 | 0.60 | nnf_rc12_abby (reuse) |  |
| 66 | BRIDGE drop / MORPH (beat-timed) | 179.98–183.58 | 3.60 | nnf_21_george_morph (NEW) | MORPH INTO ONE! |
| 67 | BRIDGE drop / MORPH (beat-timed) | 183.58–188.38 | 4.80 | nnf_10_morph_team_pose (reuse) |  |
| 68 | BRIDGE drop / MORPH (beat-timed) | 188.38–194.38 | 6.00 | nnf_11_morph_into_one (reuse) | ONE TEAM. ONE SHIFT. |
| 69 | BRIDGE drop / MORPH (beat-timed) | 194.38–198.58 | 4.20 | nnf_10_morph_team_pose (reuse) |  |
| 70 | chorus bit ~203 s | 198.58–203.38 | 4.80 | nnf_18_dawn_desk_crew (NEW) |  |
| 71 | chorus bit ~203 s | 203.38–205.78 | 2.40 | nnf_15_sunrise_legends (reuse) |  |
| 72 | MONTAGE E (instrumental) | 205.78–208.18 | 2.40 | nnf_09_fivestar_vs_motel (reuse) |  |
| 73 | MONTAGE E (instrumental) | 208.18–210.58 | 2.40 | nnf_03_late_checkout (reuse) |  |
| 74 | MONTAGE E (instrumental) | 210.58–212.98 | 2.40 | nnf_05_ants_hallway (reuse) |  |
| 75 | MONTAGE E (instrumental) | 212.98–215.38 | 2.40 | nnf_06_ac_war (reuse) |  |
| 76 | MONTAGE E (instrumental) | 215.38–217.78 | 2.40 | nnf_07_baby_milk_freezer (reuse) |  |
| 77 | MONTAGE E (instrumental) | 217.78–220.18 | 2.40 | nnf_08_wedding_lawn (reuse) |  |
| 78 | MONTAGE E (instrumental) | 220.18–222.58 | 2.40 | nnf_12_lobby_dance (reuse) |  |
| 79 | OUTRO + final chorus (sung ~222-240 s) | 222.58–228.58 | 6.00 | nnf_20_outro_shrug (NEW) | NOTHING NEW, FOO! / same old thing |
| 80 | OUTRO + final chorus (sung ~222-240 s) | 228.58–231.58 | 3.00 | nnf_18_dawn_desk_crew (NEW) | WE BE ABOUT IT |
| 81 | OUTRO + final chorus (sung ~222-240 s) | 231.58–235.18 | 3.60 | nnf_15_sunrise_legends (reuse) |  |
| 82 | OUTRO + final chorus (sung ~222-240 s) | 235.18–240.04 | 4.86 | nnf_01_exterior_night (reuse) | NOTHING NEW, FOO! / Trilith Guest House • Fayetteville, GA |
