# RECEIPT — Nothing New, Foo! V21

- Task: t85u
- Started: 2026-11-09 05:51:44 EST (America/New_York)
- Finished: 2026-11-09 05:57:16 EST (America/New_York)
- Model: AceStep_1_5_XL_Turbo_INT8
- Duration requested: 240 s / BPM 100 / Keyscale A major / timesignature 4 / en
- inference_steps 8 / guidance_scale 1 / seed -1 / format mp3

## Params accepted
- Accepted: model, caption, lyrics, duration, bpm, keyscale, timesignature, vocal_language, inference_steps, guidance_scale, seed, format
- NOT supported by deAPI v2: negative_prompt (documented Txt2MusicRequestBody has no such field; not sent)

## Caption
Dirty South hip-hop, boom bap, 90s, festival energy, heavy 808s, punchy snares, rolling hi-hats, rubbery bass, deep gritty male rap vocals, ad-libs, crowd noise, record scratches, polished mix

## Lyrics
Exact V21_LYRICS.txt

## Takes
- 3 total (any of checks 1–6 fail → re-roll; max 3)
- take1: Fay NO, intro spoken "Yeah…" — fail 1+6
- take2: Fay YES Dirty YES, intro ASR "THANK YOU FOR WATCHING!" — fail 6 only
- take3: Fay YES Dirty YES, intro ASR "Oh" — fail 6 only; KEPT (highest score)
- Credits: 0.00306835 × 3 = 0.00920505

## MAIN = take 3
- File: Nothing_New_Foo_V21.mp3
- Bytes: 4386672
- Duration (ffprobe): 240.024000 s
- Sample rate: 48000 Hz stereo
- SHA256: 5e023c1ff92be8e7b99e09fda7c7ac3f2c7d362a37ba915003c9174c08159c05
- Decode OK
- mean/max: @ / @ dB
- Silence (-50dB/2s): NO_LONG_SILENCE
- Tempo: 100.44642857142857 BPM
- Key: A major
- median F0 ≈ 82.76504502190036 Hz

## Checks
```
1_Fayetteville: YES
2_Dirty_South: YES
3_no_tag_style_sung: YES
4_male_rap_heuristic: YES
5_no_we_dont_sleep: YES
6_intro_no_spoken_first_8s: NO
```
Intro first-8s ASR: Oh

## Names caught (Alfred, George, Melissa, Jane, Tracy, Beth, Abby, Mike Johnson, Stacey, Trihana)
Alfred, George, Melissa, Jane, Tracy, Beth, Abby, Mike Johnson, Stacey, Trihana

## Lines landed vs garbled
- Landed (~>=60% token hit): 72
- Garbled:
- Trilith Guest House (ratio 0.0)

### ASR excerpt
```
Uh Big ATL Fayetteville, Georgia Decks on stacks, we always grind Five star pride, not Motel Six Stacks on stacks, burn mutations No hesitation, we on the clock Yes, that the desk wants a late checkout No vine boy car, but he still wants out We smile and say, of course, sir Then we call it a favor for sure Speed of your crew, want the red carpet We roll it out, and we do not start it We roll it out, and we do not start it We roll it out, and we do not start it We roll it out, and we do not start it Morning Legends, we always grind You know the thing we do, we do it well Cause you know the situation We all in this complication Dirty South Fayetteville Five star pride, not Motel Six One team, one shift This is it Legends don't quit No microwaves up in the rooms As found the crumbs, now the rule is true AC quit, under executives We bring the fans, and we fix what is Vegas milk In the freezer, please Special requests, we do what we ease Weddings on the lawn, the bride is glowing Champagne flowing, and the line keeps going Mud on the carpet, where you born in the barn Plates on the desk, your mama don't work here Weddings on the lawn, the bride is glowing Champagne flowing, and the line keeps going Mud on the carpet, where you born in the barn Plates on the desk, your mama don't work here Weddings on the lawn, the bride is glowing Champagne flowing, and the line keeps going Mud on the carpet, where you born in the barn Plates on the desk, your mama don't work here Weddings on the lawn, the bride is glowing Champagne flowing, and the line keeps going Mud on the carpet, where you born in the barn Plates on the desk, your mama don't work here Weddings on the lawn, the bride is glowing Champagne flowing, and the line keeps going Mud on the carpet, where you born in the barn Plat
```

## GitHub
- Branch: nothing-new-foo-v21
- Commit: 885f25967ffbca4f7bfa30bd6481e09682cc0c69
- Commit-pinned raw MP3: https://raw.githubusercontent.com/gmenaldo/dacaveman-skit/885f25967ffbca4f7bfa30bd6481e09682cc0c69/Nothing_New_Foo_V21.mp3
