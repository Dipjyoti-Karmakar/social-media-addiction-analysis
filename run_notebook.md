# Run Notebook (Windows)

## 1) Create and activate virtual environment

```powershell
python -m venv .venv
.\.venv\Scripts\activate
```

## 2) Install dependencies

```powershell
pip install -r requirements.txt
```

## 3) Start Jupyter

```powershell
jupyter notebook notebooks/social_media_addiction_analysis.ipynb
```

## 4) Path check

The notebook reads data from `../data/student_addiction_data.csv`.
Run Jupyter from the repository root so this relative path works without edits.
