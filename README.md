# Guitar Jam Lab

An interactive, beginner-friendly guitar reference and practice lab for exploring scales, tunings, fretboard maps, CAGED shapes, harmonized lead lines, generated tab charts, and blues jamming.

Live site: https://dragonstorm97.github.io/guitar-jam-lab/

## What It Does

Guitar Jam Lab is a single-page static web app. It is meant for guitarists who can already noodle a bit and want a practical way to connect fretboard shapes, notes, intervals, harmony, and jam-friendly patterns.

The app is organized into five top-level sections:

- **Scales**: circle of fifths, scale generator, interval explanations, fretboard view, harmony builder, and generated tab charts.
- **CAGED**: movable C/A/G/E/D chord-shape exploration on a fretboard.
- **Practice**: guided scale paths, CAGED drills, fretboard note recall, tempo practice, and saved progress.
- **Blues Lab**: 12-bar blues form, A7/D7/E7 chord shapes, movable dominant 7 shapes, transpose map, blues boxes, and practice prompts.
- **Tunings**: side-by-side tuning comparison across six-, seven-, eight-, and nine-string guitars.

## Features

### Circle Of Fifths And Scale Generator

- Choose a root note and scale/mode.
- See scale notes, interval numbers, formulas, and note functions.
- Build the selected seven-note scale into diatonic triads or seventh chords.
- Learn major, minor, perfect, diminished, and augmented intervals plus common chord symbols.
- Explore common, rare, and exotic scales.
- View the selected scale on a horizontal fretboard.
- Use the circle of fifths to see major, minor, diminished, augmented, and selected-scale relationships.

### Tunings

The string-count and tuning selectors update the fretboards, notes, chords, tabs, harmony parts, and practice drills across the app. Choose a six-, seven-, eight-, or nine-string instrument, then pick one of its common tunings.

Included six-string tunings:

- Standard
- Half-step down, full-step down, and two steps down
- Drop D
- Drop C
- Drop B, Drop Bb, and Drop A
- DADGAD
- Open G
- Open D

Extended-range options include:

- Seven-string Standard, Drop A, half-step down, full-step down, and two steps down
- Eight-string Standard, Drop E, half-step down, full-step down, and two steps down
- Nine-string Standard, Drop B, half-step down, full-step down, and two steps down
- Six-string B standard and F# standard baritone references

The **Tunings** tab aligns two instruments by pitch and highlights exact shared strings, matching low strings, pitch range, and whether familiar shapes transfer directly. Its worked examples include the exact upper-string relationship between six-string Standard and eight-string Standard, plus the relationship between baritone and extended-range layouts.

### Harmony Builder

The Harmony Builder demonstrates harmonized lead guitar, the kind of twin-guitar sound often used in melodic metal, hard rock, and metalcore.

You can choose:

- Diatonic 3rds, 4ths, 5ths, 6ths, or octaves
- Fixed minor 3rd, major 3rd, or perfect 5th
- Harmony above or below the lead line
- Lower, middle, or upper neck register

It shows:

- Lead note to harmony note pairings
- A fretboard with both guitar parts marked
- A generated two-guitar tab chart

### HTML Tab Charts

The tab chart section generates visual and text tabs from the selected root, scale, shape, and tuning. This is useful for quickly turning a scale view into something closer to a playable practice line.

### Fretboard Math

The Fretboard Math panel visualizes pitch-class arithmetic: each fret adds one semitone, and the values wrap from 12 back to 1. It uses the A-based numbering system `A = 1` through `G#/Ab = 12`.

- Pick any open string from the current tuning and move up to 24 frets.
- Follow the calculation on a 12-note wheel and one-string fret strip.
- See enharmonic names such as `A#/Bb` and `C#/Db` together.
- Practise the same calculation as a scored **Fret math** drill in Fretboard Recall.

### CAGED Shape Lab

The CAGED tab shows movable chord shapes on a fretboard. Pick a root, shape, chord color, and scale overlay to see how chord tones connect to nearby scale tones.

### Beginner Practice Zone

The Practice tab turns the reference diagrams into short, repeatable exercises:

- Learn, play, and recall compact scale patterns.
- Practise scales up and down, in groups of three, in thirds, or by targeting roots.
- Follow the exercise in a scrolling tab with a fixed playhead and the active number of strings.
- Use the global tempo with a four-count lead-in.
- Hunt CAGED roots, build chord tones, recall shapes, and connect adjacent shapes.
- Train note names and intervals with fretboard prompts.
- Calculate fretboard notes with pitch-class arithmetic across fret ranges 0-5, 0-12, and 0-24.
- Focus on weak notes and keep accuracy and completion progress in local browser storage.
- Use CAGED on its familiar upper six strings; added extended-range strings are shown muted so the original shapes stay legible.

### Blues Lab

The Blues Lab focuses on practical jamming:

- 12-bar blues form
- Jam console with tempo and bar tracking
- Open A7, D7, and E7 chord diagrams
- Movable dominant 7 shapes
- Blues transpose map
- Blues box fretboard reference
- Practice prompts for rhythm, lead, and trading phrases

## How To Use It

1. Pick a string count, tuning, and tempo from the top bar.
2. Open the **Scales** tab and choose a root and scale.
3. Use the fretboard and tab chart to find playable positions.
4. Try the **Harmony Builder** to create a second-guitar part from the same scale.
5. Open **CAGED** to connect chord shapes to the same key.
6. Use **Practice** for guided scale, CAGED, and fretboard recall drills.
7. Open **Tunings** to compare instrument ranges and find reusable string layouts.
8. Open **Blues Lab** when you want a focused 12-bar jam practice setup.

## Technical Notes

This is a static HTML/CSS/JavaScript app.

- No build step required.
- No framework required.
- No backend required.
- GitHub Pages can serve it directly from `index.html`.

## Running Locally

You can open `index.html` directly in a browser, or serve the folder with any static file server.

For example:

```powershell
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Deployment

This repo is set up for GitHub Pages.

Recommended Pages settings:

- Source: **Deploy from a branch**
- Branch: **main**
- Folder: **/**

The site entry point is `index.html`.
