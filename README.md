# neoaudioscope

**Version 1.0.1** &nbsp;·&nbsp; One HTML file &nbsp;·&nbsp; Works offline &nbsp;·&nbsp; No installation

neoaudioscope shows you what is inside a sound. Load a music file, a voice recording or a
video, and the page draws the sound in real time: the frequencies, the levels, the stereo
image and the loudness.

It is a measurement tool, not an art toy. Every display gives you information you can read
and trust.

---

## Start in 30 seconds

1. Download `neoaudioscope-v1.0.1.html`.
2. Double-click it. Your web browser opens it.
3. Push **Open file** and select an audio or a video file.

That is all. There is nothing to install and nothing to sign in to.

> **Your files stay with you.** The page does not send anything anywhere. It has no
> internet connection, no accounts and no tracking. You can disconnect from the network
> and it works the same.

---

## What you can load

| Type | What happens |
|---|---|
| Audio file (MP3, WAV, FLAC, M4A, OGG…) | Plays and analyses the sound |
| Video file (MP4, MOV, WebM…) | Uses the sound track only. No picture is shown |
| Microphone or line input | Analyses live sound. Push the **● in** button |

You can also drag a file from your desktop and drop it on the window.

For live input, the output stays silent. This prevents the howling sound that happens when
a microphone hears its own loudspeaker.

---

## The displays

You can show any of these, one at a time or many together.

### Spectrum
The classic curve. It shows how loud each frequency is, from deep bass on the left to high
treble on the right. A small circle marks the strongest frequency and names the musical
note. Move your pointer over the graph to read any point.

**Use it to:** find a boomy bass note, see if a mix is too bright or too dull, identify a
hum.

### Spectrogram
The same information, but drawn against time. The picture scrolls from left to right, and
colour shows the level. Bass is at the bottom, treble at the top.

**Use it to:** see the shape of a song, find clicks and noises, watch a drum pattern.

### Third octave
31 bars, the same standard bands used on hardware analysers. You can switch to 10 wider
bars, and you can apply A or C weighting, which makes the display follow how human ears
hear.

**Use it to:** compare rooms and speakers, do simple acoustic checks.

### Oscilloscope
The raw shape of the wave. A trigger holds the picture still so it does not shake.

**Use it to:** see distortion and clipping, check the attack of a drum, look at the
difference between the two channels.

### Stereo field
A goniometer: the two channels drawn against each other.

- A tall vertical line means mono.
- A wide cloud means a broad stereo image.
- A flat horizontal line is a warning. The channels fight each other, and the sound can
  disappear on a mono speaker.

### Phase & balance
Three bars and a history line:

- **Correlation** — how well the two channels agree. Green is safe, red needs attention.
- **Balance** — is the sound louder on the left or on the right?
- **Width** — how wide the stereo image is.

### Levels
The meters an engineer watches. Each channel shows the peak level and the average (RMS)
level, with a hold line for the highest value and a red indicator if the sound clips.

**Use it to:** set a safe recording level, find where a track is too hot.

### Loudness
How loud the material feels to a person, not to a meter. It shows the momentary value, the
short-term value, the integrated (whole programme) value and the loudness range. You can
set a target, for example −14 LUFS for streaming services or −23 LUFS for broadcast.

**Use it to:** check that a podcast, a video or a master is at the correct loudness.

### Readout
All the numbers in one list: peak and average levels, the strongest frequency with its
musical note, the tone colour (centroid and flatness), the crest factor, the loudness, an
estimate of the tempo in beats per minute, and the settings in use.

---

## Arrange the workspace

neoaudioscope is modular. Build the view you want.

- **Change a display** — use the menu at the top left of each panel.
- **Split a panel** — the second button divides it left and right, the third button divides
  it top and bottom.
- **Make one panel large** — push the fourth button. Push it again to return.
- **Close a panel** — push the × button.
- **Change the sizes** — drag the line between two panels. Double-click that line to make
  the two panels equal.
- **Panel options** — push the gear button to show the settings for that display only.

### Layout presets

| Preset | For this work |
|---|---|
| Full suite | A view of everything |
| Spectrum work | Frequency analysis in detail |
| Stereo check | Stereo image and phase |
| Loudness | Levels and loudness for delivery |
| Waveform | The wave shape and the stereo field |
| Single panel | One large display |

### Themes

Six skins: Graphite, Deep blue, Blueprint (light), Phosphor (green screen), Ember (warm)
and High contrast. Press the number keys 1 to 6 to change between them.

---

## Controls

| Control | Function |
|---|---|
| Play / Pause / Stop | Transport for the loaded file |
| ↻ | Play the file again and again |
| Position bar | Move to any point in the file |
| Speaker button | Silence the output. The analysis continues |
| Gear button | Analyser settings |
| ? button | Help |

### Keys

| Key | Function |
|---|---|
| Space | Play or pause |
| ← → | Move 5 seconds |
| M | Silence the output |
| R | Clear all hold values and loudness |
| 1 – 6 | Select a theme |
| Esc | Close a window |

---

## Analyser settings

The gear button opens the settings that apply to all panels.

- **FFT size** — small values react fast, large values show fine detail. 4096 is a good
  start.
- **Smoothing** — how much the display calms down movement.
- **Top and bottom of scale** — the level range of the graphs.
- **Highest frequency** — how far to the right the graphs go.
- **Loudness target** — the reference line in the Loudness panel.
- **Render quality** — decrease it if an old computer becomes slow.

---

## Speed

neoaudioscope calculates the sound one time for each frame and shares the result with all
panels. A panel that you cannot see does no work. On a normal laptop, six panels draw in
2 to 4 milliseconds, which leaves the computer free for the rest of its work.

---

## Two honest limits

- The loudness values use a K-weighting filter to the ITU-R BS.1770 method, but the
  calculation is an approximation. Use the values to compare material, not for a legal
  compliance report.
- The peak value is a sample peak. A true peak can be a little higher.

---

## What you need

Any recent browser: Chrome, Edge, Safari or Firefox, on a computer, a tablet or a phone.
The file format support comes from the browser. If a file does not play, the status bar
tells you.

---

## Version history

### 1.0.1
- New name: neoaudioscope. The browser tab shows the name only.

### 1.0.0 — first release
- Nine displays: spectrum, spectrogram, third octave, oscilloscope, stereo field,
  phase & balance, levels, loudness and readout.
- Modular workspace: split, resize, maximise and close any panel.
- Six layout presets and six themes.
- Audio files, video files (sound only) and live input.
- Loudness to the ITU-R BS.1770 method, with momentary, short term, integrated and range
  values.
- Peak and RMS meters with hold and clip indication.
- Tempo estimate, musical note detection and spectral descriptors.
- One file, offline, no libraries.
