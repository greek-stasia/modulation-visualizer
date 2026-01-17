# Digital Modulation Learning Lab

An interactive web-based tool for learning and visualizing digital modulation schemes. Explore BPSK, QPSK, 16-QAM, and FSK through hands-on experimentation with constellation diagrams, time-domain signals, and frequency spectra.

![Modulation Visualizer](https://img.shields.io/badge/Status-Active-00ff88) ![License](https://img.shields.io/badge/License-MIT-blue)

## 🎯 Overview

This educational tool helps students, engineers, and hobbyists understand how digital data is encoded onto carrier signals using various modulation techniques. Instead of just reading about modulation—**interact with it**.

## ✨ Features

### Supported Modulation Schemes

| Scheme | Bits/Symbol | Description |
|--------|-------------|-------------|
| **BPSK** | 1 | Binary Phase Shift Keying - 2 phase states (0°, 180°) |
| **QPSK** | 2 | Quadrature PSK - 4 phase states (45°, 135°, 225°, 315°) |
| **16-QAM** | 4 | 16 Quadrature Amplitude Modulation - 16 amplitude/phase combinations |
| **FSK** | 1 | Frequency Shift Keying - 2 frequency states |

### Interactive Elements

- **🖱️ Clickable Constellation Diagram** — Click any point to add that symbol to your sequence
- **✏️ Bit Sequence Editor** — Toggle bits, add/remove, or generate random sequences
- **▶️ Playback Controls** — Step through symbols or auto-play at adjustable speeds
- **📊 Real-time Visualizations** — Constellation, time-domain waveform, and power spectral density all update together
- **📡 Noise Simulation** — Add AWGN (Additive White Gaussian Noise) to see how it affects signal quality

### Educational Content

Each modulation scheme includes:
- Detailed explanation of how it works
- Advantages and disadvantages
- Real-world applications (Wi-Fi, Bluetooth, satellite, etc.)

## 🚀 Quick Start

### Option 1: Use GitHub Pages (Recommended)

1. Fork or clone this repository
2. Go to **Settings** → **Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Your site will be live at `https://yourusername.github.io/repository-name/`

### Option 2: Run Locally

Simply open `index.html` in any modern web browser. No server required!

```bash
# Clone the repository
git clone https://github.com/yourusername/modulation-visualizer.git

# Open in browser
open index.html
# or on Windows
start index.html
# or on Linux
xdg-open index.html
```

## 📖 How to Use

### Building a Bit Sequence

1. **Click bits** in the editor to toggle between 0 and 1
2. **Click constellation points** to add complete symbols
3. Use **Add 0**, **Add 1**, or **Random** buttons for quick input
4. Watch the bit groupings change based on bits-per-symbol for each scheme

### Stepping Through Transmission

1. Click **▶ Play** to animate through your sequence
2. Use **◀ Prev** and **Next ▶** for manual stepping
3. Adjust **Speed** for slower/faster playback
4. Observe the current symbol highlighted in:
   - The bit sequence (colored group)
   - The constellation diagram (pulsing point)
   - The time-domain waveform (shaded region)

### Experimenting with Noise

1. Drag the **Channel Noise** slider to add interference
2. Watch the constellation points scatter
3. Notice how higher-order modulations (16-QAM) are more affected
4. Understand why robust schemes like BPSK are used in noisy environments

## 🧠 Learning Concepts

### Constellation Diagrams
The I-Q plane shows how symbols are mapped to amplitude and phase. Points further apart are easier to distinguish in noisy conditions.

### Spectral Efficiency
- BPSK: 1 bps/Hz
- QPSK: 2 bps/Hz (same bandwidth as BPSK, 2× data rate)
- 16-QAM: 4 bps/Hz (4× data rate, but needs better SNR)
- FSK: ~0.5 bps/Hz (robust but bandwidth-inefficient)

### Trade-offs
Higher-order modulations pack more bits per symbol but require:
- Higher signal-to-noise ratio (SNR)
- More precise hardware
- Better channel conditions

## 🛠️ Technical Details

- **Pure HTML/CSS/JS** — No build step required
- **React 18** — Loaded via CDN
- **Zero dependencies** — Everything in one file
- **Responsive design** — Works on desktop and tablet
- **~800 lines** — Lightweight and fast

## 📁 Project Structure

```
modulation-visualizer/
├── index.html      # Complete application (single file)
├── README.md       # This file
└── LICENSE         # MIT License
```

## 🎓 Ideal For

- **Students** studying telecommunications or signal processing
- **Engineers** needing a quick reference or teaching aid
- **Hobbyists** exploring software-defined radio (SDR)
- **Educators** demonstrating modulation concepts in class

## 🤝 Contributing

Contributions are welcome! Some ideas:

- [ ] Add more modulation schemes (8-PSK, 64-QAM, OFDM)
- [ ] BER (Bit Error Rate) calculation with noise
- [ ] Eye diagram visualization
- [ ] Audio output of modulated signal
- [ ] Mobile-optimized touch controls

## 📄 License

MIT License — feel free to use, modify, and distribute.

## 🙏 Acknowledgments

Built as an educational tool to make digital communications concepts more accessible and interactive.

---

**Happy Learning!** 📡✨
