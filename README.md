# Web Synthesizer

A feature-rich, browser-based synthesizer built with vanilla JavaScript and the Web Audio API. Create music directly in your browser with no plugins or downloads required.

![image](https://github.com/user-attachments/assets/f4d286df-d652-4542-b8b9-6e86aeb3e32d)

## Features

### 🎹 **Interactive Keyboard**
- 2-octave virtual keyboard with both white and black keys
- Computer keyboard support (QWERTY layout)
- Visual feedback for active notes

### 🎛️ **Sound Synthesis**
- **Oscillator**: 4 waveform types (Sawtooth, Square, Triangle, Sine)
- **Detune**: Fine-tune oscillator pitch (-50 to +50 cents)
- **Low-pass Filter**: Adjustable cutoff frequency and resonance
- **ADSR Envelope**: Full Attack, Decay, Sustain, Release control

### 🎚️ **Built-in Effects**
- **Delay**: Adjustable delay time with feedback
- **Reverb**: Convolution reverb for spatial depth
- **Master Volume**: Global output level control

### 🎵 **Preset System**
- **Lead**: Bright, cutting lead synthesizer sound
- **Bass**: Deep, punchy bass tones
- **Pad**: Lush, atmospheric pad sounds
- **Pluck**: Short, percussive plucked sounds

### 🎨 **Professional Interface**
- Retro-futuristic design inspired by classic synthesizers
- Real-time visual feedback with animated value bars
- Responsive layout that works on desktop and mobile

## Getting Started

### Quick Start
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/web-synthesizer.git
   ```

2. Open `web_synth.html` in your web browser

3. Start playing! Use your mouse to click keys or use your computer keyboard

### Computer Keyboard Mapping
```
|   |   |   |   |   |   |   |   |   |   |   |   |
|   | W |   | E |   |   | T |   | Y |   | U |   |
|   |   |   |   |   |   |   |   |   |   |   |   |
| A | S | D | F | G | H | J | K | L | ; | ' |   |
|   |   |   |   |   |   |   |   |   |   |   |   |
```

- **A S D F G H J**: White keys (C D E F G A B)
- **W E T Y U**: Black keys (C# D# F# G# A#)

## Technical Details

### Built With
- **HTML5**: Structure and layout
- **CSS3**: Styling with gradients, animations, and responsive design
- **JavaScript ES6+**: Core functionality and audio processing
- **Web Audio API**: Real-time audio synthesis and effects

*Note: Requires a modern browser with Web Audio API support*

### Architecture
```
AudioContext
    ↓
Oscillator → Filter → Effects Chain → Master Gain → Output
                  ↓
              Delay + Reverb
```

## Usage Examples

### Basic Playing
1. Click on the keyboard keys or use your computer keyboard
2. Adjust the filter cutoff for different tonal colors
3. Modify the envelope settings to change how notes start and end

### Sound Design
1. **Creating a Lead Sound**:
   - Set waveform to Sawtooth
   - Increase filter cutoff (3000+)
   - Add some resonance (10-15)
   - Quick attack, medium release

2. **Creating a Bass Sound**:
   - Set waveform to Square
   - Lower filter cutoff (800-1200)
   - Increase resonance (15-20)
   - Very quick attack, short release

3. **Creating a Pad Sound**:
   - Set waveform to Triangle
   - Moderate filter cutoff (1500-2000)
   - Long attack and release times
   - Add reverb for space

### Key Classes
- `MicroKorgSynth`: Main synthesizer class handling audio generation
- Audio nodes: Oscillator, Filter, Delay, Reverb, Master Gain

### Adding New Features
The synthesizer is designed to be extensible. You can easily add:
- New waveforms
- Additional effects
- More presets
- Extended keyboard range
- MIDI support

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Inspired by classic hardware synthesizers like the MicroKorg
- Built using the powerful Web Audio API

---

**🎵 Happy Music Making! 🎵**
