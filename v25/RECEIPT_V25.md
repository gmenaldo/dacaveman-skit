# RECEIPT_V25 — Nothing New, Foo! GOLDEN BUILD

- Bot: Grok Bot (executor)
- Task: t88u
- Started: 2026-11-09 06:56:57 EST (America/New_York)
- Finished: 2026-11-09 07:03:18 EST (America/New_York)
- What changed: Fresh V25 caption/lyrics blueprint; branch `v25` off nothing-new-foo-v24; stamped V25
- Paths: /workspace/three-minute-bounce/v25/* ; repo branch v25
- One-line result: Take2 kept after Dirty Souf fail on take1 (Dardisoff) and take2 (Dottysauce). Fayetteville clear both takes. Neither take passed Dirty South/Souf strictly.

## Caption (283 chars)
underground hip-hop, boom bap, deep raspy aggressive male rap vocals, hard-hitting 808 sub-bass you feel in the car, G-funk synth lead, turntable scratch transitions, mid-tempo groove, house party energy, no country, no clean pop vocals, no melodic singing, no twang, radio-ready mix

## Params
- AceStep_1_5_XL_Turbo_INT8; 180s; bpm 100; A major; 4/4; en; steps 8; guidance_scale 1; seed -1; mp3
- lyric guidance / LM temperature: UNSUPPORTED on deAPI (noted; not sent) — same finding as V24
- negative_prompt: NOT SENT (no-tags baked into caption)

## Takes
- take1: FAIL Dirty_South_or_Souf (heard "Dardisoff") → re-roll named that failure
- take2: also FAIL Dirty_South_or_Souf (heard "Dottysauce") but better verse2/chorus landing → MAIN
- Credits: 0.00239283 × 2 = 0.00478566
- No further re-roll (one-re-roll max already used)

## Audio
- Duration: 180.024000 s
- Bytes: 3308352
- Sample rate: 48000 Hz stereo
- Key: A major
- Requested BPM: 100; librosa tempo: 100.44642857142857
- SHA256: 5b989a4c20c99c209b7d3e9a57cbec4f6036461eb1d8dd263738054f9dc0f479
- mean/max dB: -15.1 / -0.0
- Silence (-50dB/2s): NO_LONG_SILENCE
- median F0: 83.73 Hz (male rap)

## Checks
- Fayetteville: YES
- Dirty_South_or_Souf: NO
- no_tag_words_sung: YES
- male_rap: YES
- no_we_dont_sleep: YES
- leaked tag words: none

## Vocal timestamps (for video cuts)
- 1.58-8.00s:  Big  ATL,  Fayetteville,  Dottysauce
- 10.86-28.80s:  Big  ATL,  Fayetteville,  Dottysauce  Big  ATL,  Fayetteville,  Dottysauce  Big  ATL,
- 40.16-59.62s:  Fayetteville,  Dottysauce  Big  ATL,  Fayetteville,  Dottysauce  Big  ATL,  Fayetteville,  Dottysauce  Alfred  on  the  doorknob  You  know  her  thorns  tonight  Melissa  runs  the  floor  Born  in  legends  We  always  grind  You  know  the  thing  we  do  We  do  it  well
- 68.92-98.30s:  Late  checkout,  no  born  voice  Expedia  wants  red  carpet  No  microwaves  The  ants  came  AC  quit  on  the  execs  Born  in  legends  We  always  grind  You  know  the  thing  we  do  We  do  it  well  Born  in  legends  We  always  grind  You  know  the  thing  we  do  We  do  it  well
- 102.42-107.80s:  One  identity  More  into  one
- 126.24-136.42s:  Born  in  legends  We  always  grind  You  know  the  thing  we  do  We  do  it  well
- 145.36-149.36s:  Born  in  legends  We  always  grind
- 158.54-166.00s:  You  know  the  thing  we  do  We  do  it  well  Nothing  new  for
- 168.02-174.74s:  Same  old  thing  Same  old  thing  We  be  about  it

## Line-by-line (29 sung lines; brief said 31 — exact lyrics yield 29 content lines)
Counts: landed 19 / garbled 8 / missing 2
- **LANDED** [raspy] `Big A-T-L` @ 1.58-3.90s | heard:  Big  ATL,
- **LANDED** [raspy] `Fay-et-ville` @ 3.94-6.24s | heard:  Fayetteville,
- **GARBLED** [raspy] `DIRTY SOUF` @ 6.54-8.00s | heard:  Dottysauce
- **MISSING** [verse1] `Da-Corrie with the plan` @ n/a | heard: —
- **GARBLED** [verse1] `Alfred on the door` @ 42.78-45.28s | heard:  Alfred  on  the  doorknob
- **GARBLED** [verse1] `George pulls the night` @ 45.28-46.92s | heard:  You  know  her  thorns  tonight
- **LANDED** [verse1] `Melissa runs the floor` @ 46.92-49.46s | heard:  Melissa  runs  the  floor
- **GARBLED** [chorus1] `Morning legends` @ 50.34-51.90s | heard:  Born  in  legends
- **LANDED** [chorus1] `We always grind` @ 52.92-54.94s | heard:  We  always  grind
- **LANDED** [chorus1] `You know the thing we do` @ 54.94-57.28s | heard:  You  know  the  thing  we  do
- **LANDED** [chorus1] `We do it well` @ 57.28-59.62s | heard:  We  do  it  well
- **LANDED** [verse2] `Late checkout, no Bonvoy` @ 68.92-73.04s | heard:  Late  checkout,  no  born  voice  Expedia  wants
- **LANDED** [verse2] `Expedia wants red carpet` @ 71.64-73.86s | heard:  Expedia  wants  red  carpet
- **LANDED** [verse2] `No microwaves, the ants came` @ 73.86-79.68s | heard:  No  microwaves  The  ants  came  AC  quit  on  the  execs  Born
- **LANDED** [verse2] `AC quit on the execs` @ 76.52-78.64s | heard:  AC  quit  on  the  execs
- **GARBLED** [chorus2] `Morning legends` @ 79.32-80.46s | heard:  Born  in  legends
- **LANDED** [chorus2] `We always grind` @ 81.40-83.46s | heard:  We  always  grind
- **LANDED** [chorus2] `You know the thing we do` @ 83.46-85.82s | heard:  You  know  the  thing  we  do
- **LANDED** [chorus2] `We do it well` @ 86.64-88.44s | heard:  We  do  it  well
- **MISSING** [bridge] `Different places` @ n/a | heard: —
- **LANDED** [bridge] `One identity` @ 102.42-103.74s | heard:  One  identity
- **GARBLED** [bridge] `Morph into one` @ 105.60-107.80s | heard:  More  into  one
- **GARBLED** [chorus3] `Morning legends` @ 126.24-128.54s | heard:  Born  in  legends
- **LANDED** [chorus3] `We always grind` @ 129.54-131.30s | heard:  We  always  grind
- **LANDED** [chorus3] `You know the thing we do` @ 131.30-134.30s | heard:  You  know  the  thing  we  do
- **LANDED** [chorus3] `We do it well` @ 134.30-136.42s | heard:  We  do  it  well
- **GARBLED** [outro] `Nothing new foo` @ 165.08-166.00s | heard:  Nothing  new  for
- **LANDED** [outro] `Same old thing` @ 168.02-170.14s | heard:  Same  old  thing
- **LANDED** [outro] `We be about it` @ 172.54-174.74s | heard:  We  be  about  it

## Leakage / invented fills
- No intro/verse/chorus/bridge/drop/break/raspy/vocal/outro tags sung.
- DIRTY SOUF never landed clean (take1 Dardisoff / take2 Dottysauce).
- Morning legends always ASR'd as "Born in legends".
- Alfred → "Alfred on the doorknob"; George → "You know her thorns tonight"; Morph → "More into one"; Nothing new foo → "Nothing new for".
- Da-Corrie with the plan and Different places missing from ASR.
- Intro raspy block loops Big ATL / Fayetteville / Dottysauce before verse1.
- Extra chorus fragments ~88–98s and ~145–166s (invented fills / repeats beyond written structure).

## GitHub
- Branch: v25 (created off nothing-new-foo-v24; no force-push)
- MP3 commit: 3b7d9fa1017f2ecf12de1902aae6478b630ba38b
- Tip may include receipt polish
- Commit-pinned raw: https://raw.githubusercontent.com/gmenaldo/dacaveman-skit/3b7d9fa1017f2ecf12de1902aae6478b630ba38b/Nothing_New_Foo_V25.mp3
- Curl verify: HTTP 200, bytes=3308352, sha256 MATCH
