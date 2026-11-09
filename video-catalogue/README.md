# POM video catalogue classification

Generated 2026-11-09T20:51:28.314Z from `resources/owner-bulk-video-approval-2026-10-30.json` (1737 owner-approved videos).
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
| Fully classified | 264 |
| Needs owner review | 1473 |
| Schedule from YouTube chapters | 352 |
| Schedule from description list | 59 |
| No schedule | 1326 |

## Exceptions by reason

| Reason | Videos |
|---|---:|
| SCHEDULE_MISSING | 1326 |
| EQUIPMENT_UNKNOWN | 604 |
| EQUIPMENT_CONFLICT | 20 |
| DURATION_MISMATCH | 16 |
| OWNER_DURATION_CONFLICT | 5 |
| INSTRUCTOR_UNKNOWN | 1 |
| IDENTITY_HOLD | 1 |

## Instructor

| Instructor | Videos |
|---|---:|
| FEMALE | 914 |
| MALE | 458 |
| MIXED | 364 |
| UNKNOWN | 1 |

## Equipment (a video can use several)

| Equipment | Videos |
|---|---:|
| DUMBBELLS | 576 |
| NONE | 521 |
| BANDS | 51 |
| KETTLEBELLS | 34 |

## Channels needing an instructor decision

- Juice & Toya (1 videos): female, male or mixed?
