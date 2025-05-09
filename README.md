📦 Project Setup Guide
This guide outlines the steps to set up and run the project, including environment setup, dependency installation, and model configuration.

1. Environment Setup
Create and activate a virtual environment:

bash
Copy
Edit
python -m venv venv_gpu
source venv_gpu/scripts/activate  # For Windows: venv_gpu\Scripts\activate
2. Install Dependencies
PyTorch (with CUDA)
Install PyTorch with CUDA support by following the official guide:

👉 https://pytorch.org/get-started/locally/

Or run the following command (for CUDA 12.1):

bash
Copy
Edit
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu128
Additional Packages
bash
Copy
Edit
pip install ctransformers[cuda]
pip install chromadb[client]
pip install -r requirements.txt
3. Model Setup
Download any model from the following link and place it in the appropriate folder:

👉 https://huggingface.co/TheBloke

Then update the model path in config.yml accordingly.

4. Run the App
Start the Streamlit application:

bash
Copy
Edit
streamlit run app.py
