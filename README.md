# Iron Bloom 176

### Analog time-domain artifacts for cymbals and transient-rich material

A cymbal hit explodes with thousands of simultaneous modes. Analog hardware — tubes, transformers, tape — didn't just record this. It reshaped it. Phase smear spread the transient across time. Variable-mu compression squeezed the peak while lifting the sustain. Transformer saturation filled the spectral gaps with harmonics. Magnetic hysteresis added density. Tape drift kept the sustain alive and breathing.

**Iron Bloom 176** recreates these artifacts as a plugin. Twelve controls shape how the signal interacts with a virtual analog chain: tube compression, transformer saturation, intermodulation distortion, magnetic hysteresis, pitch drift, and spectral stabilization. A real-time 3D spectrum analyzer shows you exactly what's changing — the peaks and valleys of your frequency content reshaping as the analog chain works.

---

## Downloads

### Windows (x64) — VST3
Copy the `windows/IronBloom176.vst3` folder to:
```
C:\Program Files\Common Files\VST3\
```
Works in Reaper, Ableton, Bitwig, Studio One, Cubase, FL Studio.

### macOS (ARM64 / Apple Silicon) — VST3
Copy `macos/IronBloom176.vst3` to:
```
~/Library/Audio/Plug-Ins/VST3/
```
Works in Reaper, Ableton, Bitwig, Studio One, Cubase, FL Studio.

### macOS (ARM64 / Apple Silicon) — Audio Units
Copy `macos/IronBloom176.component` to:
```
~/Library/Audio/Plug-Ins/Components/
```
Works in Logic Pro, GarageBand, Final Cut Pro.

### macOS note (unsigned)
These builds are not code-signed. On first use, macOS will block them. Fix with:
```bash
xattr -d com.apple.quarantine ~/Library/Audio/Plug-Ins/VST3/IronBloom176.vst3
xattr -d com.apple.quarantine ~/Library/Audio/Plug-Ins/Components/IronBloom176.component
```
Or right-click the plugin in Finder and choose Open.

---

## What the controls do to your sound

| Control | Effect |
|---------|--------|
| **Depth** | How far into the analog chain the signal travels |
| **HF Smear** | Spreads high-frequency transients across time (allpass phase dispersion) |
| **Transient Softening** | Rounds off the sharp leading edge of each hit |
| **Pitch Drift** | Micro-detuning instability in the sustain (tape wow) |
| **Tube Bend** | Variable-mu compression — squeezes peaks, lifts sustain |
| **Transformer Drive** | Pushes the signal into smooth tanh saturation |
| **Stereo** | Independent L/R processing vs mono sum |
| **Output Gain** | Level after processing |
| **Wet Mix** | Dry/wet blend |
| **Anti-Digital** | Intermodulation distortion + even harmonics (analog thickness) |
| **Bloom** | Transformer resonance — body and ring on each hit |
| **Transient Bend** | Time-domain reshaping of attack envelopes |

## The display

Click the waveform area to toggle views:

- **Waveform** — input (red) vs output (amber) overlay. See transients reshape in real-time.
- **3D Spectrum** — ridgeline waterfall from 500 Hz up. Red peaks (input) behind, amber peaks (output) in front. Watch saturation add harmonics, HF smear redistribute energy, and the spectral stabilizer hold the balance.

---

## Version
**v1.9.4** — Built by ChatGPT, Grok, and Pietro

Source code: private repository
