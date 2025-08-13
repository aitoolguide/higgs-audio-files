# Higgs Audio – Updated TTS Script & Config File

This repository contains two files required for running Higgs Audio exactly as shown in my YouTube tutorial.

---

## 📂 Files in this Repository

1. **`config.json`**
   - **Path to place:**
     ```
     examples/voice-log-box/
     ```
   - **Purpose:**  
     This JSON file contains the audio reference configuration used by the **Voice Clone** section in the Gradio UI.  
     It simply maps your saved audio files from the folder to the interface so you can quickly select them.

2. **`run_tts_updated.py`**
   - **Path to place:**
     ```
     [Main Higgs Audio Project Root Folder]/
     ```
   - **Purpose:**  
     This is the updated **TTS run script** with changes as shown in the tutorial.  
     Add/Replace the original file in your main project folder with this updated version.

---

## 📥 How to Use

1. **Download** both files from this repository.  
2. **Paste** them into their respective paths as described above.  
3. **Restart** your Higgs Audio project.  
4. You will now see the updated Voice Clone audio list in the UI, and the improved TTS script will be used when running Higgs Audio.

---

## ⚙️ Important Setup Commands

To ensure GPU acceleration works and Gradio runs correctly with Higgs Audio, run the following commands in your project environment:

```bash
# Remove existing Torch, TorchVision, and TorchAudio
pip uninstall torch torchvision torchaudio

# Install specific versions with CUDA 12.4 support
pip install torch==2.4.1+cu124 torchaudio==2.4.1+cu124 --extra-index-url https://download.pytorch.org/whl/cu124

# Upgrade Gradio to the latest version
pip install --upgrade gradio
```

---

## 🎥 Watch the Tutorial

For step-by-step installation and setup, watch my YouTube video here:  
🔗 [Watch on YouTube](https://www.youtube.com/@aitoolmasteringtutorials)

---

## 👍 Support My Work

If this helped you, please consider **subscribing to my YouTube channel** and **liking the video**.  
Your support helps me create more free guides like this.
