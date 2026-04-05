# Unglare

### Cymbals in the mix, not in your face

The problem was never frequency. It was *time*. EQ cuts brightness but kills presence. Unglare spreads high-frequency transient energy across time using phase dispersion — your brain hears the same brightness but interprets it as depth instead of aggression. Cymbals move from "at the speaker cone" to "in the room."

Twelve controls shape how your signal interacts with a chain of analog imperfections: asymmetric saturation, magnetic hysteresis, pitch drift, phase smear, transformer resonance. A 3D spectrum analyzer shows you the peaks and valleys reshaping in real-time.

---

## Downloads

### Windows (x64) — VST3
Copy the `windows/Unglare.vst3` folder to:
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
These builds are not code-signed. On first use:
```bash
xattr -d com.apple.quarantine ~/Library/Audio/Plug-Ins/VST3/Unglare.vst3
xattr -d com.apple.quarantine ~/Library/Audio/Plug-Ins/Components/Unglare.component
```
Or right-click the plugin in Finder and choose Open.

---

## Controls

| Control | What it does |
|---------|-------------|
| **Depth** | How far into the analog chain |
| **HF Smear** | Phase dispersion — pushes cymbals back in the mix |
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

**v2.1.2** — Built by ChatGPT, Grok, Claude, and Pietro
