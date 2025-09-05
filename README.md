
# Workflow Steps

## 1. Accessing the Notebook
- Access the notebook anytime via **Google Drive** or **Google Colab**.  
- Only **one person** should make major edits at a time to avoid conflicts.  
- Communicate changes on **Slack / Teams / GitHub** before editing.  

## 2. Dataset Setup & Usage

### a. Initial Download (One-time)
- One team member downloads and extracts the **Kaggle dataset** using their own API key in Colab.  
- Move the extracted CSV files (`Fake.csv`, `True.csv`, etc.) into the shared Drive folder.  

### b. Accessing the Dataset
- Everyone mounts Google Drive in their Colab notebook using:



```
python
from google.colab import drive
drive.mount('/content/drive')
```
Load dataset files from the shared folder, e.g.:

```
python
import pandas as pd
df = pd.read_csv('/content/drive/MyDrive/[shared-folder-name]/Fake.csv')
```

*(Replace `[shared-folder-name]` with the exact folder name.)*  

- No need for every member to set up Kaggle API keys after this step.  

### c. Updating Data
- If updated data is needed, one member repeats the **download + Drive update** process.  

## 3. GitHub Version Control

### a. Saving Notebooks to GitHub
- In Colab: **File > Save a copy to GitHub**  
- Commit to the correct repository and filename (e.g., `FakeNews_EDA.ipynb`)  
- Always add a **descriptive commit message**  

### b. Editing & Sync
- Always open the latest notebook version from GitHub before editing.  
- After making changes, save again with **“Save a copy to GitHub”**.  
- Only **one person edits at a time** to avoid overwriting.  
- Communicate with teammates before major changes.  
