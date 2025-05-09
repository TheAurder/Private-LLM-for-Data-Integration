# 🔒 Private-LLM-for-Data-Integration

A **local private LLM chatbot** built for **data integration** and **data security**.  
It allows you to chat or upload PDFs to extract information — all without relying on the cloud or third-party services.

![./screenshot.png](https://github.com/TheAurder/Development-of-Private-LLM-for-Data-Integration/blob/main/UI.png))  
*Replace with your actual UI screenshot.*

---

## 🚀 Features

- 🔐 100% local — no internet connection required
- 📄 PDF integration — ask questions directly from uploaded documents
- 🧠 Powered by open-source LLMs (downloadable from Hugging Face)
- ⚡ GPU acceleration using PyTorch + CUDA
- 🎛️ Configurable via `config.yml`

---

## 🛠️ Setup Instructions

### 1. Create a Virtual Environment

```bash
python -m venv venv_gpu
source venv_gpu/scripts/activate  # On Windows: venv_gpu\Scripts\activate
```

### 2. Install Dependencies

#### PyTorch with CUDA

Visit the official PyTorch site to choose your configuration:  
👉 https://pytorch.org/get-started/locally/

Or install directly (for CUDA 12.1):

```bash
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu128
```

#### Additional Packages

```bash
pip install ctransformers[cuda]
pip install chromadb[client]
pip install -r requirements.txt
```

---

## 📥 Model Setup

Download any model from TheBloke’s Hugging Face repository:  
👉 https://huggingface.co/TheBloke

Place the downloaded model in the designated folder, then update the model path in `config.yml`.

---

## ▶️ Run the App

```bash
streamlit run app.py
```

---

## 📄 License

This project is intended for private and educational use. Review licenses of third-party models for respective terms.
