# Unglare

![Unglare](screenshot.png)

### Remove the glare. Keep the brightness.

Harsh cymbals. Brittle synths. Crispy drum machines. Sibilant vocals. Full mixes where the top end fatigues after 30 seconds. The problem isn't frequency — it's *time*. EQ removes energy. Unglare spreads it. Your brain hears the same brightness but interprets it as depth instead of aggression.

Twelve controls shape how your signal interacts with a chain of analog imperfections: phase dispersion, asymmetric saturation, magnetic hysteresis, pitch drift, transformer resonance. A 3D spectrum analyzer shows you the peaks and valleys reshaping in real-time.

---

## Downloads

### Windows (x64) — VST3
Copy `windows/Unglare.vst3` folder to:
```
C:\Program Files\Common Files\VST3\
```

### macOS (ARM64 / Apple Silicon) — VST3
Copy `macos/Unglare.vst3` to:
```
~/Library/Audio/Plug-Ins/VST3/
```

### macOS (ARM64 / Apple Silicon) — Audio Units
Copy `macos/Unglare.component` to:
```
~/Library/Audio/Plug-Ins/Components/
```

### macOS note (unsigned)
```bash
xattr -d com.apple.quarantine ~/Library/Audio/Plug-Ins/VST3/Unglare.vst3
xattr -d com.apple.quarantine ~/Library/Audio/Plug-Ins/Components/Unglare.component
```

---

## Controls

| Control | What it does |
|---------|-------------|
| **Depth** | How far into the analog chain |
| **HF Smear** | Phase dispersion — pushes harsh content back in the mix |
| **Transient Softening** | Envelope-dependent HF rolloff on loud transients |
| **Pitch Drift** | Micro-detuning instability in the sustain |
| **Tube Bend** | Envelope-dependent gain reduction |
| **Transformer Drive** | Asymmetric saturation depth |
| **Stereo** | Independent L/R processing vs mono sum |
| **Output Gain** | Level compensation |
| **Wet Mix** | Dry/wet blend |
| **Anti-Digital** | Intermodulation distortion + even harmonics |
| **Bloom** | Transformer resonance Q — body and ring on hits |
| **Transient Bend** | Time-domain reshaping of attack envelopes |

## Display

Click to toggle: **Waveform** (input red, output amber) or **3D Spectrum** (ridgeline waterfall from 500 Hz up).

---

Works in Reaper, Ableton, Logic, Bitwig, Studio One, Cubase, FL Studio, GarageBand.

**v2.1.2** — Built by ChatGPT, Grok, Claude, and Pietro
