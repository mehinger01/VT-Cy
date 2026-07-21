# VT-Cy Operational Lesson Flow

## Current Student Flow

```text
Home / Quest Map
        ↓
Today's Mission
        ↓
Warm-Up
        ↓
Mini Lesson
        ↓
Guided Practice
        ↓
Geometry Design Lab
        ↓
Independent Mission
        ↓
Exit Ticket
        ↓
Geometry Reflection
        ↓
Return Home
```

## Purpose

This implementation provides a complete 60-minute tutoring lesson without requiring outside documents or a new application architecture. It intentionally reuses the existing homepage and Geometry Design Lab.

## Operational Lesson Structure

| Segment | Approximate Time | Purpose |
|---|---:|---|
| Warm-Up | 5–7 minutes | Retrieve prior geometry vocabulary and surface misconceptions |
| Agenda and Progress | 2–3 minutes | Make the learning path and current focus visible |
| Mini Lesson | 10 minutes | Review quadrilateral relationships, lines, angles, symmetry, perimeter, and area |
| Guided Practice | 15 minutes | Build and compare shapes with tutor support |
| Independent Mission | 14 minutes | Apply geometry concepts in a city-block blueprint |
| Exit Ticket | 6 minutes | Capture classification, angle, line, and explanation evidence |
| Reflection | 3 minutes | Record strategy, challenge, product, and confidence |

## Persistence

The implementation preserves existing Geometry Lab storage keys.

The new exit ticket is stored locally under:

```text
cyTodaysMissionExitTicket
```

No backend or Notion connection is required for this phase.

## Navigation

- The homepage primary action opens `todays-mission.html`.
- Today's Mission opens `geometry-design-lab.html` in a new tab so the lesson directions remain available.
- The Geometry Lab retains its existing Quest Map navigation.
- Today's Mission includes a clear Return Home action.

## Tutor Data to Record

After the session, record:

- warm-up accuracy
- independent mission completion
- exit-ticket accuracy
- confidence level
- prompting level
- skill requiring spaced review

## Future Expansion — Not Implemented in This Phase

The same instructional sequence can later be standardized for:

- Math Mountain
- Reading Forest
- Writer's Workshop
- Word Forge
- Mission Control
- STEM Lab

A later reusable lesson engine should represent lessons as data with the following shared stages:

```text
Lesson
├── Warm-Up
├── Agenda and Progress
├── Instruction
├── Guided Practice
├── Independent Work
├── Exit Ticket
└── Reflection and Mastery Update
```

That refactor should begin only after the current lesson is operational and tested.