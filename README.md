# GenAI / LLM Workshop Notebook — Setup Instructions

---

## Quick Start in Your Browser (No Install)

Don't want to install anything? You can run the whole workshop in Google Colab, which only needs a browser and a Google account.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vinays75-coder/gen-ai-llm-basics-workshop/blob/main/genai_llm_workshop_final.ipynb)

- Click the button above and sign in with your Google account if asked.
- Click **Runtime → Run all**, or click a code cell and press **Shift + Enter** to run cells one at a time.
- If Colab warns that the notebook was not authored by Google, click **Run anyway**. The notebook only uses Python's built-in libraries.
- Your changes are not saved automatically. To keep them, choose **File → Save a copy in Drive**.

Prefer to run it on your own computer? Follow the steps below.

---

## Prerequisites

**You need Python 3.8 or later installed.**

- **Check if you have it:** Open a terminal (Mac/Linux) or Command Prompt (Windows) and run:
  ```
  python --version
  ```
  or
  ```
  python3 --version
  ```
- **If not installed:** Download from https://www.python.org/downloads/ and install.
  On Windows, **check the box "Add Python to PATH"** during installation.

---

## Step 1 — Unzip the File

- **Mac:** Double-click `genai_llm_workshop_share.zip` in Finder. A folder or set of files will appear in the same location.
- **Windows:** Right-click `genai_llm_workshop_share.zip` → **Extract All…** → choose a destination folder → click **Extract**.
- **Linux:**
  ```
  unzip genai_llm_workshop_share.zip -d genai_llm_workshop
  ```

> **Important:** Keep all the files together in the same folder. The images must be in the same directory as the `.ipynb` file for them to display correctly.

---

## Step 2 — Install JupyterLab

Open a terminal / Command Prompt and run:

```
pip install jupyterlab
```

or if `pip` doesn't work, try:

```
pip3 install jupyterlab
```

Wait for the installation to complete (this only needs to be done once).

---

## Step 3 — Navigate to the Workshop Folder

In your terminal / Command Prompt, change directory to where you unzipped the files.

- **Mac/Linux example:**
  ```
  cd ~/Downloads
  ```
- **Windows example:**
  ```
  cd C:\Users\YourName\Downloads
  ```

Replace the path with wherever you actually unzipped the files.

---

## Step 4 — Launch JupyterLab

Run:

```
jupyter lab
```

This will automatically open a browser tab at `http://localhost:8888`. If it doesn't open automatically, copy the URL printed in the terminal (it looks like `http://localhost:8888/lab?token=...`) and paste it into your browser.

---

## Step 5 — Open the Notebook

In the JupyterLab file browser on the left, double-click:

```
genai_llm_workshop_final.ipynb
```

The notebook will open in a new tab with all the lesson content and images visible.

---

## Step 6 — Run the Notebook

You have two options:

**Option A — Run all cells at once:**
- Click the menu: **Run → Run All Cells**
- This runs every code cell from top to bottom automatically.

**Option B — Run cells one at a time (recommended for learning):**
- Click on a code cell (grey background, has `[ ]` to the left).
- Press **Shift + Enter** to run it and advance to the next cell.
- Repeat for each cell you want to execute.

> **Tip:** Markdown cells (white background with text/images) don't need to be "run" — they display automatically.

---

## Step 7 — Stopping JupyterLab When Done

- Close the browser tab.
- Go back to the terminal and press **Ctrl + C**, then confirm with `y` if prompted.

---

## Troubleshooting

| Problem | Fix |
|---|---|
| `jupyter` command not found | Make sure Python was added to PATH; try `python -m jupyter lab` instead |
| Images not showing | Confirm all `.png` files are in the **same folder** as the `.ipynb` file |
| `pip` not found on Mac | Use `pip3` instead of `pip` |
| Port 8888 already in use | Run `jupyter lab --port 8889` |
| Browser doesn't open | Copy the `http://localhost:8888/...` URL from the terminal into your browser manually |

---

## Alternative: Using VS Code (Optional)

If you prefer VS Code over JupyterLab:
1. Install VS Code from https://code.visualstudio.com/
2. Install the **Python** extension and **Jupyter** extension from the Extensions panel.
3. Open the folder containing the unzipped files: **File → Open Folder**.
4. Click on `genai_llm_workshop_final.ipynb` in the Explorer panel.
5. Select a Python kernel when prompted (choose the Python version you installed).
6. Use **Run All** at the top or **Shift + Enter** cell by cell.

---

**No internet connection is required to run this notebook on your own computer.**
All code uses only Python's built-in standard libraries — nothing extra to install beyond JupyterLab itself. Enjoy the workshop!
