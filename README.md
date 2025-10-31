# TU Wien Machine Learning Exercise 1 (2025W)

This repository contains our code and notebooks for **Exercise 1: Classification** in the Machine Learning (2025W) course at TU Wien.

---

## ⚙️ Setup Instructions (for all team members)

### 1️⃣ Clone the repository
```bash
git clone <repo-url>
cd TUWIEN-MLExercise
```

---

### 2️⃣ Create a virtual environment
```bash
python -m venv .venv
```

Activate it:

**macOS/Linux**
```bash
source .venv/bin/activate
```

**Windows (PowerShell)**
```bash
.venv\Scripts\activate
```

---

### 3️⃣ Install dependencies
This installs all required libraries, including **Jupyter**, **Jupytext**, and **Nbdime**.
```bash
pip install -r requirements.txt
```

---

### 4️⃣ Enable nbdime Git integration
Run this **inside your activated virtual environment** once per machine:
```bash
nbdime config-git --enable
```
This configures Git to use nbdime’s smarter diff and merge tools for `.ipynb` files.

---

### 5️⃣ Working in VS Code

1. **Open the folder in VS Code**
   - File → Open Folder → select your project folder.

2. **Select the correct Python environment**
   - Click the **kernel picker** (top-right of notebook) and choose your `.venv` environment.  
   - It should appear as “Python (venv)” or similar.

3. **Open and run notebooks**
   - Open any `.ipynb` file and use the “Run Cell” ▶ buttons to execute cells.  
   - You can also use the “Run All” command from the top toolbar.

4. **Clear notebook outputs before committing**
   - Press `Ctrl+Shift+P` (Command Palette) → search for “Notebook: Clear All Outputs”.  
   - Save the notebook after clearing outputs.

5. **Pair notebooks with Jupytext (optional but recommended)**
   - Use the VS Code Command Palette → search “Jupytext: Pair Notebook with Percent Script”.  
   - This will create a `.py` version of your notebook for easier Git diffing.
---

## 🧾 Useful Commands Summary

| Purpose | Command |
|----------|----------|
| Activate environment (Linux/macOS) | `source .venv/bin/activate` |
| Activate environment (Windows) | `.venv\Scripts\activate` |
| Install dependencies | `pip install -r requirements.txt` |
| Enable nbdime Git integration | `nbdime config-git --enable` |
| Clear notebook outputs in VS Code | Command Palette → “Notebook: Clear All Outputs” |
| Run notebooks | Open `.ipynb` in VS Code → “Run Cell” ▶ |

---

## 💡 Notes
- Everyone uses their own `.venv`; it is **not** committed to Git.
- Only `.ipynb` and `.py` notebook files are tracked — no large datasets or output files.
- If a merge conflict happens on a notebook, nbdime provides a helpful diff view to resolve it.
- All development and testing can be done directly inside VS Code — no separate Jupyter server needed.