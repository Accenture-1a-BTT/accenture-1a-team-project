
Workflow Steps: 

Access the notebook via Google Drive or Colab at any time.

Only one person should make major edits at a time to avoid conflicts—communicate changes on Slack/Teams/GitHub.

2. Dataset Setup & Usage
a. Initial Download (One-time)
Only one member downloads/extracts the Kaggle dataset using their own API key in Colab.

Move the extracted CSV files (Fake.csv, True.csv, etc.) into our shared Drive folder.

b. Accessing the Dataset
Everyone mounts Google Drive in their Colab notebook using:

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
(Replace [shared-folder-name] with the exact folder name.)
```
No need for everyone to set up Kaggle API keys after this point.

c. (If Data Is Updated)
If we need updated data, one person repeats the download step and updates the Drive folder.

3. GitHub Version Control
a. Saving Notebooks to GitHub
To save the latest changes: In Colab, click File > Save a copy to GitHub

Commit to the correct repository and filename (e.g., FakeNews_EDA.ipynb)

Add a descriptive commit message

b. Editing & Sync
Always open the latest notebook version from GitHub before making changes.

After making edits, repeat “Save a copy to GitHub”—only one person at a time to avoid overwriting.

Communicate with teammates before major changes to coordinate editing.
