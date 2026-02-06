## 🚀 Setup Instructions

Follow these steps to get the environment ready on your Mac.

### 1. Download the Model
Open your **Terminal** and run the following command to download the specific 32B model used in the script:
```bash
ollama pull deepseek-r1:32b
```
### 2. Python Environment Setup
Ensure you have the required Python libraries installed:
```bash
pip install -r requirements.txt
```
Install the Jupyter Extension in VS Code (if not already installed) via the Extensions marketplace.

## 🛠️ How to Run
- **Open the Notebook**: Click on `pipeline.ipynb` in the VS Code file explorer.
- **Select Kernel**: In the top-right corner of the editor, click "Select Kernel" and choose your Python environment.
- **Data Check**: Ensure `filtered_claims.json` is in the root directory.
- **Run All**: Click "Run All" or execute cells individually. (The tqdm progress bar will appear below the cell to show processing status.)
- **Output**: Once finished, a new file `questions_decomposed_my_prompt.json` and `questions_decomposed_LIS_prompt.json` will be generated.

## 📁 Repository Structure
- `pipeline.ipynb`: Main Jupyter Notebook.
- `requirements.txt`: List of Python dependencies (Ollama, tqdm, etc.).
- `filtered_claims.json`: The input data file.
- `.gitignore`: Prevents large JSON outputs from being pushed to Git.

## ⚠️ Troubleshooting
- **Ollama Connection**: Ensure the Ollama app is active in your menu bar.
- **File Permissions**: If you get a "File Not Found" error, ensure you opened the root folder of the project in VS Code, not just the single file.
