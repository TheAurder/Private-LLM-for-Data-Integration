# 🔒 Private-LLM-for-Data-Integration

A **local private LLM chatbot** built for **data integration** and **data security**.  
It allows you to chat or upload PDFs to extract information — all without relying on the cloud or third-party services.

![./screenshot.png](https://github.com/TheAurder/Development-of-Private-LLM-for-Data-Integration/blob/main/UI.png)


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

## Contributors:

<br/>
<div align="center">
    <table style="border-collapse: collapse; border: none;">
        <tr>
            <td align="center" style="border: none; text-align: center; padding: 10px;">
                <a href="https://github.com/sandipanrakshit34" target="_blank">
                    <img src="Assets/Sandipan_Rakshit.png" 
                         alt="sandipanrakshit34" 
                         width="140" height="140" 
                         style="border-radius: 50%;" />
                </a>
                <br>
                <strong><a href="https://github.com/sandipanrakshit34" style="text-decoration: none; color: #61dafb;">sandipanrakshit34</a></strong>
            </td>
            <td align="center" style="border: none; text-align: center; padding: 10px;">
                <a href="https://github.com/Niloy-Aiml34" target="_blank">
                    <img src="Assets/niloy_das.png" 
                         alt="Niloy-Aiml34" 
                         width="140" height="140"
                         style="border-radius: 50%;" />
                </a>
                <br>
                <strong><a href="https://github.com/Niloy-Aiml34" style="text-decoration: none; color: #61dafb;">Niloy-Aiml34</a></strong>
            </td>
            <td align="center" style="border: none; text-align: center; padding: 10px;">
                <a href="https://github.com/Mrigangana-Sarkar" target="_blank">
                    <img src="Assets/mriganga_sarkar.png" 
                         alt="Mrigangana-Sarkar" 
                         width="140" height="140"
                         style="border-radius: 50%;" />
                </a>
                <br>
                <strong><a href="https://github.com/Mrigangana-Sarkar" style="text-decoration: none; color: #61dafb;">Mrigangana-Sarkar</a></strong>
            </td>
        </tr>
    </table>
</div>
