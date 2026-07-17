# Guitar Jam Lab

An interactive, beginner-friendly guitar reference and practice lab for exploring scales, tunings, fretboard maps, CAGED shapes, harmonized lead lines, generated tab charts, and blues jamming.

Live site: https://dragonstorm97.github.io/guitar-jam-lab/

## What It Does

Guitar Jam Lab is a single-page static web app. It is meant for guitarists who can already noodle a bit and want a practical way to connect fretboard shapes, notes, intervals, harmony, and jam-friendly patterns.

The app is organized into four top-level sections:

- **Scales**: circle of fifths, scale generator, interval explanations, fretboard view, harmony builder, and generated tab charts.
- **CAGED**: movable C/A/G/E/D chord-shape exploration on a fretboard.
- **Practice**: guided scale paths, CAGED drills, fretboard note recall, tempo practice, and saved progress.
- **Blues Lab**: 12-bar blues form, A7/D7/E7 chord shapes, movable dominant 7 shapes, transpose map, blues boxes, and practice prompts.

## Features

### Circle Of Fifths And Scale Generator

- Choose a root note and scale/mode.
- See scale notes, interval numbers, formulas, and note functions.
- Explore common, rare, and exotic scales.
- View the selected scale on a horizontal fretboard.
- Use the circle of fifths to see major, minor, diminished, augmented, and selected-scale relationships.

### Tunings

The tuning selector updates the fretboards, notes, chords, and tab views across the app.

Included tunings:

- Standard
- Drop D
- Drop C
- Half-step down
- DADGAD
- Open G
- Open D

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

### CAGED Shape Lab

The CAGED tab shows movable chord shapes on a fretboard. Pick a root, shape, chord color, and scale overlay to see how chord tones connect to nearby scale tones.

### Beginner Practice Zone

The Practice tab turns the reference diagrams into short, repeatable exercises:

- Learn, play, and recall compact scale patterns.
- Practise scales up and down, in groups of three, in thirds, or by targeting roots.
- Use the global tempo with a four-count lead-in.
- Hunt CAGED roots, build chord tones, recall shapes, and connect adjacent shapes.
- Train note names and intervals with fretboard prompts.
- Focus on weak notes and keep accuracy and completion progress in local browser storage.
- Use full CAGED drills in Standard and half-step-down tunings, or upper-five-string drills in Drop D and Drop C.

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

1. Pick a tuning and tempo from the top bar.
2. Open the **Scales** tab and choose a root and scale.
3. Use the fretboard and tab chart to find playable positions.
4. Try the **Harmony Builder** to create a second-guitar part from the same scale.
5. Open **CAGED** to connect chord shapes to the same key.
6. Use **Practice** for guided scale, CAGED, and fretboard recall drills.
7. Open **Blues Lab** when you want a focused 12-bar jam practice setup.

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
