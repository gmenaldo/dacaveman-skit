# RECEIPT — Nothing New, Foo! V24

- Bot: Grok Bot (executor)
- Task: t87u
- Started: 2026-11-09 06:29:06 EST (America/New_York)
- Finished: 2026-11-09 06:32:26 EST (America/New_York)
- What changed: New V24 caption/lyrics (180s); bare [Instrumental break]; branch nothing-new-foo-v24 off nothing-new-foo-v22
- Paths touched: /workspace/three-minute-bounce/v24/* ; repo nothing-new-foo-v24
- One-line result: Take1 kept (Fayetteville+Dirty South clear; no re-roll). Lyric guidance 0.5 and LM temperature 1.0 unsupported by deAPI v2 — used guidance_scale=1. Caption trimmed 378→300 chars for API limit.

## Params
- model AceStep_1_5_XL_Turbo_INT8; duration 180; bpm 100; A major; timesignature 4; en; inference_steps 8; guidance_scale 1; seed -1; mp3
- lyric_guidance_scale 0.5: NOT SUPPORTED (no field in deAPI v2 music schema)
- lm_temperature 1.0: NOT SUPPORTED (no field)
- negative_prompt: NOT SENT

## Caption
Requested was 378 chars (API max 300). Used trimmed:
90s golden era boom bap, West Coast G-funk synths, hard 808 sub-bass rattling car speakers, rapid-fire triplet rap with melodic hooks, aggressive baritone male, multiple rappers trading verses, raspy ad-libs, crowd noise, turntable scratches, festival house party, 100 BPM, punchy dry radio-ready mix

## Takes
- take1 only (Fay YES, Dirty YES → no re-roll)
- Credits: 0.00239283

## Audio
- Duration: 180.024000 s
- Bytes: 3299328
- Sample rate: 48000 Hz stereo
- SHA256: 2425cfea411b0bbc8cfdd7239d92471c13553c3a66fde76abb25df77e6d9237b
- mean/max dB: -13.7 / 0.0
- Silence (-50dB/2s): [silencedetect @ 0x7f7fa40030c0] silence_start: 177.15775
[silencedetect @ 0x7f7fa40030c0] silence_end: 180 | silence_duration: 2.84225
- Tempo: 100.44642857142857 BPM
- median F0: 83.24 Hz (voiced_frac=0.752)

## Checks
- Fayetteville: YES
- Dirty_South: YES
- no_stage_tag_or_negative_words: YES
- male_rap_heuristic: YES
- no_we_dont_sleep: YES
- leaked tag/negative words: none
- Distinct voices: Cannot reliably count distinct traded rap voices from this mono mix without speaker diarization; no diarization model run.

## Line-by-line (29 sung occurrences; 3 chorus repeats listed separately)
Counts: landed 18 / garbled 8 / missing 3
- **LANDED** [Intro] `Big A-T-L` @ 0.00-1.36s | heard:  Big  ATL
- **LANDED** [Intro] `Fay-et-ville` @ 3.54-4.94s | heard:  Fayetteville
- **LANDED** [Intro] `Dirty South` @ 8.44-9.64s | heard:  Dirty  South
- **LANDED** [Verse1] `Da-Corrie with the plan` @ 39.02-41.10s | heard:  Corrie  with  the  plan
- **LANDED** [Verse1] `Alfred on the door` @ 41.79-43.46s | heard:  Alfred  on  the  door
- **LANDED** [Verse1] `George pulls the night` @ 51.51-53.12s | heard:  George  pulls  the  night
- **LANDED** [Verse1] `Melissa runs the floor` @ 53.61-55.64s | heard:  Melissa  runs  the  floor
- **LANDED** [Chorus1] `Morning legends` @ 59.30-60.32s | heard:  Morning  Legends
- **GARBLED** [Chorus1] `We always grind` @ 60.32-61.82s | heard:  we always cry
- **MISSING** [Chorus1] `You know the thing we do` @ n/a | heard: —
- **GARBLED** [Chorus1] `We do it well` @ 64.40-66.72s | heard:  We do it wild
- **GARBLED** [Verse2] `Pete checks upstairs` @ 88.18-89.42s | heard:  check  some  stairs,
- **GARBLED** [Verse2] `Beth sees everything` @ 90.32-91.40s | heard:  sees  everything
- **LANDED** [Verse2] `Jane holds the desk` @ 91.40-94.14s | heard:  Jane  holds  the  desk,
- **GARBLED** [Verse2] `Abby pours the shine` @ 94.84-96.48s | heard:  happy  force  to  shine
- **LANDED** [Chorus2] `Morning legends` @ 96.48-97.78s | heard:  Morning  legends,
- **GARBLED** [Chorus2] `We always grind` @ 98.40-100.28s | heard:  we always cry
- **MISSING** [Chorus2] `You know the thing we do` @ n/a | heard: —
- **LANDED** [Chorus2] `We do it well` @ 100.28-115.40s | heard:  We do it well
- **LANDED** [Bridge] `Different places` @ 126.12-127.84s | heard:  Different  places,
- **LANDED** [Bridge] `One identity` @ 128.34-130.16s | heard:  one  identity
- **GARBLED** [Bridge] `Morph into one` @ 139.90-142.20s | heard:  Morphin'  to  one
- **LANDED** [Chorus3] `Morning legends` @ 142.20-146.98s | heard:  Morning  legends,
- **GARBLED** [Chorus3] `We always grind` @ 146.98-148.52s | heard:  we always cry
- **MISSING** [Chorus3] `You know the thing we do` @ n/a | heard: —
- **LANDED** [Chorus3] `We do it well` @ 150.98-154.12s | heard:  We do it well
- **LANDED** [Outro] `Nothing new foo` @ 164.78-166.58s | heard:  Nothing  new  fool,
- **LANDED** [Outro] `Same old thing` @ 166.76-168.80s | heard:  same  old  thing
- **LANDED** [Outro] `We be about it` @ 168.80-172.32s | heard:  We  be  about  it

## Leakage / invented
- No intro/chorus/verse/bridge/outro/instrumental/scratch/DJ or negative-list words sung as tags.
- Chorus often became "we always cry" / "we do it wild"; verse2 Pete/Beth/Abby near-misses; Morphin' to one; Nothing new fool.
- Melodic oh-oh fills in gaps (not lyric text).
