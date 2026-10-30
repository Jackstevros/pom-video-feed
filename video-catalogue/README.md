# POM video catalogue classification

Generated 2026-10-30T14:39:21.143Z from `resources/owner-bulk-video-approval-2026-10-30.json` (1737 owner-approved videos).
YouTube descriptions fetched: **yes**.

This public list tags each video with duration, instructor, equipment and a workout schedule
so it can be used on its own. Schedules come from the creator's own YouTube chapters or exercise
list (`scheduleSource`), not a POM review of the video. Not signed, not loaded by the app.

Files: `classified-videos.json`, `classified-videos.csv` (everything), `exceptions.csv`
(only videos needing owner review, with blank decision columns).
Equipment and level answers already requested in `../video-classification-exceptions.csv`
only need answering once, there; this list adds instructor, schedule and conflict checks.

## Status

| | Videos |
|---|---:|
| Fully classified | 165 |
| Needs owner review | 1572 |
| Schedule from YouTube chapters | 352 |
| Schedule from description list | 59 |
| No schedule | 1326 |

## Exceptions by reason

| Reason | Videos |
|---|---:|
| SCHEDULE_MISSING | 1326 |
| EQUIPMENT_UNKNOWN | 604 |
| INSTRUCTOR_UNKNOWN | 334 |
| EQUIPMENT_CONFLICT | 20 |
| DURATION_MISMATCH | 16 |
| IDENTITY_HOLD | 1 |

## Instructor

| Instructor | Videos |
|---|---:|
| FEMALE | 850 |
| UNKNOWN | 334 |
| MALE | 304 |
| MIXED | 249 |

## Equipment (a video can use several)

| Equipment | Videos |
|---|---:|
| DUMBBELLS | 576 |
| NONE | 521 |
| BANDS | 51 |
| KETTLEBELLS | 34 |

## Channels needing an instructor decision

- Nobadaddiction (78 videos): female, male or mixed?
- EDR Fitness (69 videos): female, male or mixed?
- Midas Movement (43 videos): female, male or mixed?
- fitbymik (34 videos): female, male or mixed?
- Pilates by Zola (23 videos): female, male or mixed?
- Tone and Tighten (21 videos): female, male or mixed?
- PS Fit (13 videos): female, male or mixed?
- Headspace (13 videos): female, male or mixed?
- Rehab Science (13 videos): female, male or mixed?
- fitness__kaykay (13 videos): female, male or mixed?
- Treat My Achilles (6 videos): female, male or mixed?
- Breathe and Flow (2 videos): female, male or mixed?
- Dansique Fitness (2 videos): female, male or mixed?
- Spark Healthy Runner (2 videos): female, male or mixed?
- Global Triathlon Network (1 videos): female, male or mixed?
- Juice & Toya (1 videos): female, male or mixed?
