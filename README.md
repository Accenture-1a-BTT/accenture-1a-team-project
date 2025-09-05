# Accenture 1A Team Project

## Workflow Guidelines

### 1. Notebook Access
- Open the notebook via **Google Drive** or **Google Colab** at any time.  
- **Only one person** should make major edits at a time to avoid conflicts.  
- Communicate edits or changes on **Slack/Teams/GitHub** before making updates.  

---

### 2. Dataset Setup & Usage

#### a. Initial Download (One-time Setup)
1. One team member downloads and extracts the **Kaggle dataset** using their own API key in Colab.  
2. Move the extracted files (`Fake.csv`, `True.csv`, etc.) into the **shared Google Drive folder**.  

#### b. Accessing the Dataset
Everyone can access the dataset in Colab by mounting Google Drive:

```python
from google.colab import drive
drive.mount('/content/drive')
Then load the dataset:

python
Copy code
import pandas as pd
df = pd.read_csv('/content/drive/MyDrive/[shared-folder-name]/Fake.csv')
Replace [shared-folder-name] with the actual shared folder name.
After the initial setup, no one else needs a Kaggle API key.

c. Updating the Dataset
If updated data is required, one member should repeat the download and update the shared Drive folder.

3. GitHub Version Control
a. Saving Notebooks to GitHub
In Colab, go to File > Save a copy to GitHub.

Commit to the correct repository and filename (e.g., FakeNews_EDA.ipynb).

Add a clear, descriptive commit message.

b. Editing & Syncing
Always open the latest notebook version directly from GitHub before editing.

After making edits, save back to GitHub via Save a copy to GitHub.

To avoid overwriting, only one person should commit at a time.

Communicate with teammates before making major changes.
