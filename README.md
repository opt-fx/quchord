# QuChord

**A chord generator and arpeggiator for any MIDI keyboard.**

QuChord sits between a MIDI keyboard and your synths. Play one note and it sends a whole chord, a strum or an arpeggio. It started as a way to add chord memory to a QuNexus, but it works with any MIDI keyboard or controller.

The whole app is one HTML file and runs in the browser with no install. Made by OPT.

**Use it now: https://opt-fx.github.io/quchord/**

**Status: version 1.0.2.**

## What it does

- **Chord memory.** Eight slots. Press Learn, hold a chord and let go: every key then plays that chord shape built on itself. Number keys 1–8 switch slots.
- **Chord type.** Pick a chord (maj, min, 7, maj7, m7, m9, sus, dim, quartal and more) and every key plays it.
- **Scale chords.** Choose a key and scale, and each key plays the chord that belongs to it: triads, 7ths or 9ths. The seven chords of the key are shown with their roman numerals, and you can click them to hear them.
- **Single notes.** No chords: one note per key, for basslines and arpeggios.
- **Voicing.** Inversions, open and drop-2 spacing, octave shift, an added bass note, smooth voice leading, and a voice limit to fit a synth's polyphony (it drops the least important notes first).
- **Strum.** Spread a chord's notes in milliseconds or as a note length locked to the tempo, upwards, downwards or alternating.
- **Arpeggiator.** Up, Down, Up-Down, Down-Up, As played and Random, at 1/4 to 1/32 with triplets, over 1–4 octaves, with gate and swing. Latch keeps it running hands-free.
- **Tempo.** Follows MIDI clock from a port you choose (for example a sequencer), or a tempo you type or tap in. The arpeggiator restarts its pattern when the clock starts.
- **Velocity.** As played, with a curve and a minimum for keyboards that need hitting hard, or fixed.
- **Pass-through.** Pressure, pitch bend, CCs and program changes are forwarded, and polyphonic aftertouch is copied to every note of the chord.
- **Bypass.** Press B to send single notes straight through without changing your routing.
- **Preview sound.** Hear the output in the browser, with or without MIDI connected.

Settings are remembered in the browser.

## Quick start

1. Open the app's page, or download `index.html` and open it from disk, in Chrome or Edge. Allow MIDI access when asked.
2. Under **Routing**, set **MIDI in** to your keyboard and **MIDI out** to the port that reaches your synth or sequencer. Your choices are remembered.
3. Switch off any other route from the keyboard to the same destination, or you'll hear the single note as well as the chord.
4. Pick a chord source and play.

If your keyboard has an MPE mode, turn it off: QuChord sends each chord on one channel.

## Keys

| Key | Action |
|---|---|
| 1–8 | Select a chord memory slot |
| A | Arpeggiator on/off |
| B | Bypass on/off |
| Esc | Panic (all notes off), or cancel Learn |

## Notes

- Web MIDI works best in Chrome or Edge. Safari does not support it.
- The **Tips** button shows short explanations in each panel, including what the roman numerals mean.
- A mono synth plays one note at a time, so use Single notes or the arpeggiator with it, and keep the arpeggiator's Gate below 100%.

## Licence

GPL-3.0. See `LICENSE`.
