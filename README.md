# Guitar & Drums

Tracks your progress on guitar and drums: what you can play, what to learn next, and how much you practise.

Live page: https://claude.ai/artifact/6QTa6aYS9D1NUdgvu4Dewf

## Tabs

- **Progress**: one card per instrument with overall progress, lesson progress, minutes this week against your weekly goal, practice streak and what to learn next. Below: minutes per week for the last 8 weeks, skills due for review, and your weekly goals.
- **Lessons**: step-by-step lessons with a built-in metronome (4/4, accent on beat 1).
  - Guitar: first chords, strumming patterns, more open chords, barre and power chords, picking and scales.
  - Drums: strokes, essential rudiments, first beats, fills and feel, plus four **practice pad** lessons for home: a daily 15-minute pad routine, feet without a kit, beats on the pad (pad + knee + floor taps) and fills on the pad. **Show: Practice pad / Drum kit** filters the list; strokes and rudiments count for both.
  - Deep links: `#guitar`, `#drums` and `#pad` open the Lessons tab for that instrument (Life OS habits use them).
  - **Chords** have a diagram and a mastery level from "Can form the shape" to "Switch on every beat".
  - **One-minute changes**: count how many clean changes between two chords you make in 60 seconds. 30 is good, 60 is automatic.
  - **Drills** (strokes, rudiments, grooves, strumming and picking) have a tempo ladder. Tap a tempo once you play it cleanly 3 times in a row. A drill's level is the share of its tempo steps you've reached. **▶ Click at … BPM** starts the metronome at your next step.
  - Every chord and drill has a link to a YouTube search for a video lesson.
- **Log**: record a practice session (instrument, minutes, date, what you worked on, a note).
- **Skills**: the long-term roadmap, 14 skills per instrument with stages 0–5. A skill comes back for review after 1, 3, 7, 14 or 30 days, depending on its stage. You can add your own skills.
- **Tips & tricks**: practice habits, guitar chord, strumming and picking tips, drum technique and beat tips, a tempo guide and links to free resources.
- **Backup**: copy all your data as text and restore it.

## Your data

Progress is not stored in this repository. It lives in the artifact's database on claude.ai (`data/users/<id>/music`, with a `logs` collection), private to your account. Opened outside claude.ai, the page falls back to the browser's localStorage.

## Files

- `index.html`: the whole app (HTML, CSS, JavaScript), no build step. Lessons, chord shapes and tips are the `LESSONS`, `CHORDS` and `TIPS` constants near the top of the script.

## Updating the live page

Edit `index.html`, then republish it to the same artifact URL. Commit the same change here, so git matches the live page.
