## KEPT — Take 2 (seed 1803955082) — line-by-line (faster-whisper small.en, word timestamps, no prompt bias; cross-checked with prompted pass)
| # | Section | Lyric line | Heard | Time | Verdict |
|---|---|---|---|---|---|
| 1 | Intro | Morning legends | "Morning legends" | 8.6-10.7s | PASS |
| 2 | Intro | We always grind | "we always cry" | 13.1-15.3s | GARBLED |
| 3 | Chorus 1 | Morning legends, we always grind | "morning legends, we always grind" | 38.6-44.0s | PASS |
| 4 | Chorus 1 | You know the thing we do, we do it well | "You know the thing we do, we do it / well" | 44.0-50.9s | PASS |
| 5 | Chorus 1 | Cause you know the situation | "cause you know the situation" | 51.5-53.5s | PASS |
| 6 | Chorus 1 | We all in this complication | "We all in this complication" | 53.5-55.9s | PASS |
| 7 | Chorus 1 | Stacks on stacks, permutations | "some stacks, some stacks, permutations" | 56.2-58.6s | GARBLED |
| 8 | Verse 1 | Late checkout free, no Bonvoy in sight | "Late check out free, uh / No born boy in sight" | 61.7-66.6s | GARBLED (Bonvoy) |
| 9 | Verse 1 | Expedia red carpet, that's not the flight | "A speedy or a red carpet, that's not the flight" | 66.6-71.3s | GARBLED (Expedia) |
| 10 | Verse 1 | No microwaves cause the ants came to play | "No microwaves cause the ants came to play" | 71.3-73.7s | PASS |
| 11 | Verse 1 | AC quit on the execs, what a day | "AC quit on the execs, but according to legends" | 73.7-78.0s | GARBLED (end) |
| 12 | Chorus 2 | Morning legends, we always grind | "(morning) legends / We always grind" | 76.3-82.4s | PASS |
| 13 | Chorus 2 | You know the thing we do, we do it well | "You know the thing we do, we do it / well" | 83.9-89.3s | PASS |
| 14 | Chorus 2 | Cause you know the situation | "cause you know the situation" | 89.4-91.9s | PASS |
| 15 | Chorus 2 | We all in this complication | "We all in this complication" | 91.9-94.3s | PASS |
| 16 | Chorus 2 | Stacks on stacks, permutations | "Stacks from stacks, permutations" | 94.3-97.0s | GARBLED (minor) |
| 17 | Verse 2 | Baby milk in the freezer, special request | "Baby milk in the freezer / Special requests" | 99.6-103.8s | PASS |
| 18 | Verse 2 | Weddings on the lawn while the kitchen's blessed | "weddings on the lawn while the kitchen is blessed" | 103.8-108.6s | PASS |
| 19 | Verse 2 | Five-star not Motel 6, that's the name | "Five star nine motel six, that's the name" | 108.6-113.6s | GARBLED (not→nine) |
| 20 | Verse 2 | Movie stars in the lobby, not the same game | "movie stars in the lobby, not the same game" | 113.8-118.5s | PASS |
| — | (extra) | — | Verse 2 sung a 2nd time, unprompted by lyrics ("they be milk in the freezer…") | 118.5-137.7s | EXTRA REPEAT |
| 21 | Bridge | Different places, one identity | "different places, one identity" | 138.3-141.8s | PASS |
| 22 | Bridge | Morph into one, like Power Rangers be | "morph into one more, like Power Rangers" | 142.1-146.3s | PASS (minor) |
| 23 | Bridge | Without one we can't do it | "we did without one, we can't do it" | 146.4-150.3s | PASS |
| 24 | Bridge | Without the other, we don't move it | "without the other, we don't move it" | 151.3-155.1s | PASS |
| 25 | Outro | Fay-et-ville, Dirty South | "Fade and fail/build … dirty style" (x2) | 158.2-161.1s, 167.1-170s | GARBLED |
| 26 | Outro | We always grind, that's what we're about | "yeah, that's what we're about" ("we always grind" not heard) | 161.3-163.6s | GARBLED |
Tally take 2: PASS 18 · GARBLED 8 · MISSING 0 (+1 unrequested Verse 2 repeat). Fay-et-ville GARBLED ("Fade and build"), Dirty South GARBLED ("dirty style").

## Take 1 (seed -1/random) — tally and key lines (full ASR in takes/take1_words*.json)
Line order drifted: lines 4-5 of chorus sung inside the intro (24-31s). 
PASS 16 · GARBLED 9 · MISSING 1.
GARBLED: 1 "Born in a legend" 0.0s; 3 "Born in legend, we always cry" 39.1s; 6 "we all end this complication" 47.9s; 8 "no bond for insight" 57.4s; 9 "It's PDF, red carpet" 60.3s; 16 "stack, don't stack / this permutation" 91-98s; 19 "five star, nine motel, six" 122.3s; 22 "like Power Rangers' beam" 130.9s; 24 "we don't move in" 134.1s.
MISSING: 25 "Fay-et-ville, Dirty South" (never sung; outro 151-174s only "We always grind, that's what we're about" repeated).
Re-roll trigger: take1 line 25 MISSING → one whole-song re-roll (deAPI has no section re-roll) → take2.
Keep decision: take2 (more PASS lines, every section present in order, outro attempted); both takes fail Fayetteville/Dirty South; re-roll budget (1) spent.
