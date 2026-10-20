# DaCaveman finish checklist

**HANDOFF TO CHIEF OF STAFF. Analysis frozen 20 October 2026.**

No more picture analysis. Do not reopen the truck start frames. They are the wrong images and they are not assembly material.

Recover Alfred's five original Kling movies and start the edit. In the repo they are only short aliases: `clip1.mov` through `clip5.mov`. On the disks, search by the **original long Kling filenames** first. Do not stop when a folder has no `clip1.mov`. A file counts only when its size and sha256 match the table below. Then copy it to the alias and cut.

Read the approved screenplay for order. Read `script/dacaveman-skit.md` for the words. Do not regenerate the 81-shot plan. Do not rewrite the screenplay. Generate nothing until this cut shows a real hole.

**Screenplay:** [DaCaveman-Screenplay.pdf](../script/DaCaveman-Screenplay.pdf).  
**Lines:** [dacaveman-skit.md](../script/dacaveman-skit.md). His wording stays, including "allusion," "sittin," "fir," and "twenty-fours." Dave is Tom. Dan is the father. Tom is the son.

**Status rule:** nothing below is EXISTING until the hash matches on the machine that has the file.

## Verify first, then edit


On the M2 and on Ubuntu, search for the original long Kling download names, not only `clip1.mov`–`clip5.mov`. Those short names are the aliases in `gmenaldo/cloud-render-pipeline` `assets/MANIFEST.md`. The long names are not written in the repo. Claimed alias path after a match: `/workspace/alfred-clips/`. The binaries are not in git.

| File | Claimed size | Claimed sha256 | Claimed length | Manifest says it shows | Status |
|---|---|---|---|---|---|
| clip1.mov | 34,087,302 | `1aa9b1b3…7690c5` | 15.04 s | Treehouse, then scene 2 panels | UNKNOWN |
| clip2.mov | 10,092,682 | `ffc3e28b…bfa0e5` | 8.04 s | News and a celebration crowd | UNKNOWN |
| clip3.mov | 25,087,684 | `f0b34513…9ec2ea` | 10.04 s | Treehouse, truck cab, salon exterior | UNKNOWN |
| clip4.mov | 30,286,290 | `5afb2c8c…bba605` | 15.04 s | Salon, flannel two-shot, transformed pair | UNKNOWN |
| clip5.mov | 17,835,550 | `239248bd…7571f` | 7.04 s | Reception, nurse, transformed pair | UNKNOWN |
| voice/alfred-ref.wav | — | — | 18.5 s claimed | Voice reference only, not the performance | UNKNOWN |

If the hash matches, relabel that one file EXISTING and use it. If it fails, leave it UNKNOWN. Do not use `~/gal-studio/dacaveman/dacaveman-final.mp4` as the movie. Do not use the Vast look-check failures.

Locked stills named in the same manifest (`assets/refs/locked/dan.png`, `tom.png`, and the anchor frames) are also UNKNOWN until opened. If a still matches, it may hold a line. It is not new footage.

## Rules for every row

- Picture must match the Kling clip of that wardrobe once the clip is verified. Waist cloth on the cliff. Pajamas at home. Winter clothes outside and in the truck. Sackcloth only after each transformation. Private areas stay covered.
- Cavemen keep the prehistoric face from those clips: heavy brow, wide nose, deep-set eyes, dark weathered skin, thick beard, sharp teeth, ancient nails. No extra fingers, limbs, or a modern face. No Dave.
- Audio is Alfred's line, verbatim. Dan lower than Tom. No narrator. No music unless George approves it later.
- `(ON TV)`, the celebration montage, the nail insert, and `CONTINUOUS` into the salon are approved format. They are not an order to generate clips.

## Scene 1 — Mountain treehouse

| Beat | Passage | Who | Picture | Audio | Footage | If the five clips verify |
|---|---|---|---|---|---|---|
| 1.1 | Dan hangs on the treehouse. Rope dangles. His toenails hold him. Windows show the room. | Dan | Cliff, treehouse, unused rope, waist cloth, nails in bark | None | UNKNOWN | Likely covered by clip1. Do not regenerate. |
| 1.2 | Tom stands below, staring up. | Tom | Tom at the base, looking up | None | UNKNOWN | Manifest names a Tom still from clip1. Confirm before any new picture. |
| 1.3 | "Come on pop. At least hook the rope to your carabiner, for the allusion of safety." / "You being serious right now?" | Tom, then Dan | Same setup. Do not add a wave or a new joke. | Those two lines only | UNKNOWN | Use the verified picture. Voice is still UNKNOWN. |

Continuity: Dan is the one on the wall. Tom is the one on the ground.  
QC: rope is unused. Nails, not the rope, hold him. Cloth covers him.

## Scene 2 — News and the birthday call

| Beat | Passage | Who | Picture | Audio | Footage | If the five clips verify |
|---|---|---|---|---|---|---|
| 2.1 | Dan in pajamas. Fireplace, crock pot, pig on a spit, seen past his right shoulder. | Dan | His chair and that fireplace | None | UNKNOWN | Manifest points at clip1 panels and pajama stills. Confirm. |
| 2.2 | News report, then a pause, then "be you!" | News announcer (ON TV) | The television. Do not write a new graphic. | The line, with the pause | UNKNOWN | clip2 is the claimed news picture. Watch it before cutting. |
| 2.3 | Celebration | Immigrants named in the script | Montage of the dancing he wrote. Not a new caveman newsroom. | None, unless that clip already has sound | UNKNOWN | Use only the celebration already inside clip2. If clip2 is only a caveman anchor, hold a still. Do not invent a parade. |
| 2.4 | Tom blinks, surprised, at the same news. | Tom | Tom watching | None | UNKNOWN | Confirm a Tom-watching still before generating. |
| 2.5 | The phone call through "Get dressed. I'm on my way." | Tom and Dan | Dan at home. Tom not in Dan's room. | Five lines, verbatim | UNKNOWN | Intercut verified stills. No new scene. |

QC: the pause stays before "be you!" Do not "correct" the news line.

## Scene 3 — The ride

| Beat | Passage | Who | Picture | Audio | Footage | If the five clips verify |
|---|---|---|---|---|---|---|
| 3.1 | Tom honks. Dan comes out in coat, hat, boots, gloves, scarf. Hair out of the hat. Long beard. They drive. | Tom, Dan | Winter clothes. No snow unless the clip already has it. | Horn only if the clip has it | UNKNOWN | clip3 claims the pickup and the cab. |
| 3.2 | Car talk from "We ain't been out" through "Just sit back and enjoy the show." | Tom, Dan | The same cab | Those lines, in order | UNKNOWN | Hold the verified cab picture under the lines. Do not generate a new drive. |
| 3.3 | They arrive at the shop. | Both | Salon exterior | None | UNKNOWN | clip3 claims the exterior at 9.5 s. |

QC: this Dan is still in winter clothes. He has not transformed.

## Scene 4 — Nail salon

The interior is `CONTINUOUS` from the arrival. No time jump.

| Beat | Passage | Who | Picture | Audio | Footage | If the five clips verify |
|---|---|---|---|---|---|---|
| 4.1 | Desk. Claws covered. Two guests in shorts. Woman in a blue nurse outfit, short dark medium-long hair. Names, then "Have a seat right here." | Shop worker, Tom | Reception | Those three lines | UNKNOWN | clip5 claims reception and the nurse. |
| 4.2 | They sit at the window chairs. Water runs. People gather outside. | Dan, Tom | Raised leather chairs, foot baths | "Wow, son! I feel good." and Tom's pamper line | UNKNOWN | clip4 claims the salon interior. |
| 4.3 | "Be comfortable… It's the law." / "Everything?" / "Watch me!" | Tom, Dan | Same chairs, still in the pre-transformation clothes | Those lines | UNKNOWN | Do not cut to sackcloth yet. |
| 4.4 | Tom breathes and transforms. People gasp. | Tom | Sackcloth like a tank top and waist to upper thigh. Nails exposed. | Gasp only | UNKNOWN | clip4 and clip5 claim a transformed pair, not the change itself. If the change is not in the clip, this is the first real picture hole. |
| 4.5 | Dan breathes and transforms. People run to the glass. | Dan | Sackcloth from waist to upper thigh, chest hair, most of the body exposed, private areas covered | None | UNKNOWN | Same rule as 4.4. |
| 4.6 | Nail insert, then Dan's feet, then his line. | Tom, then Dan | Tom's fingernails as long as his fingers. Thick toenails. Then Dan's toenails in the water. | "Ah, it's good to finally give my feet some air!" | UNKNOWN | Generate this insert only if no verified frame shows the nails that close. One insert, not a new scene. |
| 4.7 | Amazement, "You could've left some clothing on," guests run, "My fir got me covered," the gag. | Tom, Dan, guests | The transformed pair. Guests leave. | Those lines | UNKNOWN | Use the transformed pair if verified. Guests may be a held still. |
| 4.8 | Employees enter, panic, owner almost falls, the night line, the birthday line, "That's nasty," the bullhorn list. | Employee One, Employee Two, Owner, Dan | Their reactions. No new joke. | Those lines, verbatim, including "twenty-fours" | UNKNOWN | No manifest file names the owner or the bullhorn. If the clips do not show them, use a still and the voice. Do not build a new cast. |
| 4.9 | Employees work the nails, uncomfortable. Owner checks in a woman. | Employees, Owner | The work, not a new montage | None | UNKNOWN | Still plus the existing salon, unless the clip already shows the work. |
| 4.10 | She breathes, transforms, "It's my birthday!" | Cavewoman | Sackcloth across the chest and to mid-thigh. Nails match Dan and Tom. | That one line | NEEDS APPROVAL | Her face was never approved. Do not generate her until George accepts one still. |

## What is actually missing

Picture files inspected here: none.  
Voice performances inspected here: none.  
Approved reference opened here: none.

After the hash check, generate only a hole a verified clip or still cannot cover.

| Hole | Clips | Seconds | Spend |
|---|---|---|---|
| Tom's nail close-up, only if no verified frame is close enough | 1 | about 3 | Do not buy yet |
| Tom's transformation, only if clip4 or clip5 does not already show the change | 1 | about 5 | Kling first, because the originals are Kling |
| Dan's transformation, same test | 1 | about 5 | Same test, not a second subscription |
| Cavewoman | 0 until approved | about 5 if approved | NEEDS APPROVAL |

Working maximum if every hole is real: 4 clips, about 18 seconds. If the five Kling files already show the transformations and the nails, the picture count is zero. Do not pad this into a new 81-shot render.

Voice is separate. There are 43 spoken cues. `alfred-ref.wav` is a reference, not those cues. If line recordings are not on the machine, make one voice pass from that reference, Dan pitched down. That is not a picture order.

Kling versus Dreamina or Seedance applies only to one missing shot, after this checklist's hash check. Do not buy both. Do not buy either until George sees the price. Do not spend Grok video credits.

## Order of work

1. Hash the five clips and the voice reference. Relabel only the files that match.
2. Cut those pictures in story order in Filmora. Hold a verified still under any line with no moving picture. No music.
3. Lay the 43 lines in order. Export the story cut. Do not wait for new renders.
4. Watch the cut once. Generate only a hole that is still empty, one Kling test at a time, matched to the verified face and clothes.
5. Leave the cavewoman out until her still is approved.
6. The movie is done when every line is heard in order and the picture never shows Dave, a wrong wardrobe, or an uncovered body.

Unresolved: the cavewoman's face, whether clip2's crowd is the celebration he wrote, and whether any line recordings already exist. Everything else can be edited now.
