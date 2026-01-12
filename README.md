# ML_Lab

A small hands-on repository with practical Jupyter notebooks and data files for learning machine-learning basics.

## 📁 What’s in this repo

- `01_practical.ipynb` … `06_practical.ipynb` — Jupyter notebooks with step-by-step practical exercises.
- `test.py` — a simple script demonstrating how to run code outside notebooks.
- `requirements.txt` — Python packages required to run the notebooks and scripts.
- `ML_Env/` — an included virtual environment (you can use this or create your own).
- `src/` — sample datasets (e.g. `Diwali_sales.csv`, `NaiveText.csv`).

---

## ✅ Quick start (for absolute beginners)

### 1) Install Python

- Install **Python 3.10+** from https://www.python.org/downloads/ and make sure to check **"Add Python to PATH"** during installation.

### 2) Open a terminal in this folder

- In File Explorer: Shift + Right-click → **Open PowerShell window here**
- Or open VS Code and `File -> Open Folder` then open an integrated terminal (Ctrl+`).

### 3) Create a virtual environment (recommended)

Option A — Create a fresh venv (recommended):

```powershell
# Create venv named 'venv'
python -m venv venv

# Activate (PowerShell)
.\venv\Scripts\Activate.ps1

# Or activate in Command Prompt
.\venv\Scripts\activate.bat
```

Option B — Use the provided `ML_Env` folder (already contains a venv):

```powershell
# Activate the provided environment (PowerShell)
.\ML_Env\Scripts\Activate.ps1
```

Note: If PowerShell prevents activation, run (in an elevated or current-user context):

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

(Only do that if you understand why — it allows local scripts to run.)

### 4) Install requirements

With the venv **activated**, run:

```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If you used `ML_Env` and packages are already installed, this step may finish quickly.

### 5) Run Jupyter notebooks

Option A — Browser (classic Jupyter):

```powershell
jupyter notebook
# Browse to http://localhost:8888 and open the notebook files
```

Option B — JupyterLab (if installed):

```powershell
jupyter lab
```

Option C — VS Code: Open the folder, select the Python interpreter from your venv (bottom-right corner), then open any `.ipynb` file and run the cells.

### 6) Run the simple script

```powershell
# With venv active
python test.py
```

### 7) Add or update dependencies

If you install new packages while developing, update `requirements.txt` with:

```powershell
pip freeze > requirements.txt
```

---

## ⚠️ Troubleshooting tips

- If `python` command is not found: ensure Python is installed and added to PATH.
- If `pip` or `jupyter` is missing: make sure the virtual environment is activated; try `python -m pip install jupyter`.
- Activation errors in PowerShell: see the `Set-ExecutionPolicy` note above.

---

## 🧾 Short file descriptions

- **Notebooks**: Step-by-step practical exercises — open them in Jupyter or VS Code.
- **`test.py`**: Example script to run from the terminal.
- **`requirements.txt`**: Install with `pip install -r requirements.txt`.
- **`ML_Env/`**: Included virtual environment (optional to use).
- **`src/`**: Dataset files used in the notebooks (CSV files).

---

## 💡 Final tips

- Prefer creating your own `venv` for reproducibility.
- Use VS Code for an easy notebook experience and quick interpreter switching.
- If you want, create an issue in the repo or ask your instructor if something is unclear.

---

Happy learning! 🎓
