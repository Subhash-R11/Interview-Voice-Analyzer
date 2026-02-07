# Interview Voice Analyzer

A Python-based voice analysis tool that evaluates speech quality for interview readiness using audio signal processing.

This project records or uploads speech audio and analyzes key vocal traits such as confidence, calmness, clarity, and pacing, then provides a readiness score with visual feedback.
---

## 🚀 Features

- 🎙️ Record voice directly in Google Colab
- 📂 Upload pre-recorded audio files
- 📊 Analyze interview-relevant vocal traits:
  - Confidence (pitch stability & energy)
  - Calmness (pauses & jitter)
  - Clarity (spectral centroid)
  - Pacing (estimated words per minute)
- 📈 Visualizations:
  - Energy over time
  - Clarity indicator
  - Pitch distribution
- 🔊 Audio playback after recording
---

## 🧠 How It Works

The system uses audio signal processing techniques via **Librosa**:
- Pitch tracking (`piptrack`)
- RMS energy analysis
- Spectral centroid for clarity
- Silence detection for pause analysis
- Onset detection for speech rate estimation

Each metric is normalized and scored on a scale of **0–10**, then combined into an overall interview readiness percentage.
---

## 🛠️ Technologies Used

- Python
- Librosa
- NumPy
- SciPy
- Matplotlib
- IPython
- Google Colab
- JavaScript (for in-browser recording)
---

## ▶️ How to Run

### Option 1: Google Colab
1. Upload the notebook to Colab
2. Run all cells
3. Use the buttons to record or upload audio
4. Click **Analyze Recording**

### Option 2: Local (Audio Upload Only)
```bash
pip install -r requirements.txt
