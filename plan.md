# Project Plan: SignalSculptor

**Description:** A visual audio signal analyzer and modifier built using Rust, egui, and eframe. It allows users to load audio files, visualize their waveforms and frequency spectra, and apply basic effects like gain, equalization, and simple filtering.


## Development Goals

- [ ] Set up the basic eframe application boilerplate in src/main.rs and configure Cargo.toml.
- [ ] Create a struct to hold the application state, including the loaded audio data (waveform and frequency spectrum), effect parameters, and UI state variables.
- [ ] Implement the `eframe::App` trait for the struct.
- [ ] Implement audio loading functionality using the `hound` crate to read .wav files.
- [ ] Implement audio playback using the `rodio` and `cpal` crates.
- [ ] Implement FFT analysis of the audio data using the `rustfft` and `num-complex` crates.
- [ ] In the `update` method, create the main UI layout using `egui::CentralPanel`.
- [ ] Create a waveform visualization widget using `egui::Plot` to display the audio waveform data.
- [ ] Create a frequency spectrum visualization widget using `egui::Plot` to display the FFT output.
- [ ] Add UI elements (sliders, knobs, etc.) using `egui` widgets for controlling audio effects like gain, EQ (multiple band sliders), and basic filtering (low-pass, high-pass).
- [ ] Implement the effect processing logic to modify the audio data based on the UI controls.
- [ ] Add a menu bar with 'File' -> 'Open', 'Save', and 'Exit' options.
- [ ] Implement basic error handling and display error messages in the UI.
- [ ] (Optional) Add audio recording functionality.
