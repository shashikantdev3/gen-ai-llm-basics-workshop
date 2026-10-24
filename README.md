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

## Step 1 — Download and Unzip the Files

Go to https://github.com/vinays75-coder/gen-ai-llm-basics-workshop, click the green **Code** button and choose **Download ZIP**. This gives you a file called `gen-ai-llm-basics-workshop-main.zip`.

- **Mac:** Double-click `gen-ai-llm-basics-workshop-main.zip` in Finder. A folder with the same name will appear in the same location. (If you downloaded it with Safari, it may already be unzipped for you.)
- **Windows:** Right-click `gen-ai-llm-basics-workshop-main.zip` → **Extract All…** → choose a destination folder → click **Extract**.
- **Linux:**
  ```
  unzip gen-ai-llm-basics-workshop-main.zip
  ```

If you already use Git, you can clone the repo instead of downloading the ZIP:

```
git clone https://github.com/vinays75-coder/gen-ai-llm-basics-workshop.git
```

> **Good to know:** All the pictures are saved inside the notebook file, so `genai_llm_workshop_final.ipynb` is the only file you need to open. You don't have to keep any image files next to it.

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
  cd ~/Downloads/gen-ai-llm-basics-workshop-main
  ```
- **Windows example:**
  ```
  cd C:\Users\YourName\Downloads\gen-ai-llm-basics-workshop-main
  ```

Replace the path with wherever you actually unzipped the files. If you cloned the repo, the folder is called `gen-ai-llm-basics-workshop`.

> **Windows tip:** **Extract All** sometimes puts the files one level deeper, inside a second folder with the same name. If you can't see `genai_llm_workshop_final.ipynb`, go into that inner folder.

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
| Typing `python` opens the Microsoft Store (Windows) | Python isn't installed yet, or it wasn't added to PATH. Install it from python.org, tick **Add Python to PATH**, then open a new Command Prompt |
| `jupyter` command not found | Make sure Python was added to PATH; try `python -m jupyter lab` instead |
| Images not showing | Make sure you opened the `.ipynb` file in JupyterLab or VS Code. If pictures are still missing, the download may not have finished, so download the ZIP again |
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
