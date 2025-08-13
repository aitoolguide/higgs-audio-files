# Higgs Audio – Config & RAM TPS Updated Files

This repository contains two files required for running Higgs Audio with the settings shown in my YouTube tutorial.

## 📂 Files in this Repository

1. **`config.json`**
   - **Path to place:**
     ```
     examples/voice-log-box/
     ```
   - **Purpose:**  
     This file contains the device configuration settings we used in the tutorial. It should replace or be added to the `examples/voice-log-box` folder inside your Higgs Audio installation.

2. **`ram-tps-updated`**
   - **Path to place:**
     ```
     [Main Higgs Audio Project Root Folder]/
     ```
   - **Purpose:**  
     Updated RAM TPS data for improved performance and stability. Place this file directly in the **main project folder** of your Higgs Audio installation.

---

## 📥 How to Use

1. **Download** both files from this repository.  
2. **Paste** them into their respective paths as described above.  
3. **Restart** your Higgs Audio project and test to ensure everything works as shown in the YouTube tutorial.

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
