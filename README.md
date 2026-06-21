How to Setup and Run SalusOffline Locally:

1. Download and Unzip the Code:
   Download the 'salus-offline-code.zip' file from the repository and extract it into a folder on your desktop.

2. Prepare the Python Virtual Environment:
   Open your terminal inside the extracted project folder and set up your dependencies:
   $ python3 -m venv venv
   $ source venv/bin/activate
   $ pip install -r requirements.txt

3. Download the Model Binary File:
   Because Large Language Model binaries are too heavy for GitHub, download the authentic 2.4 GB 4-bit quantized Phi-3 model directly from Hugging Face:
   Link: https://huggingface.co/microsoft/Phi-3-mini-4k-instruct-gguf/resolve/main/Phi-3-mini-4K-instruct-q4.gguf
   
   Place the downloaded file inside a folder named 'models' in the root directory and ensure it is named exactly: 'Phi-3-mini-4k-instruct-q4.gguf'

4. Launch the Application:
   With your virtual environment active, run the main file to boot up the CustomTkinter Dark-Mode interface:
   $ python3 app.py

5. How to Test the Triage System:
   - Select your preferred language from the dropdown menu (English, Hausa, Yoruba, Igbo).
   - Enter the patient's vitals on the left sidebar panel (Age, Temperature, BP, Heart Rate).
   - Type or paste the patient's complaints into the symptoms box.
   - Press 'Ctrl + Enter' inside the symptoms box to execute the RAG pipeline. The application will process the data locally on your CPU and render the safety assessment instructions inside the bottom console frame.
