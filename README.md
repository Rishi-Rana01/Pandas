# Pandas Learning Examples

A small, friendly collection of Pandas examples and notebooks to help you learn data loading, cleaning, and plotting with step-by-step instructions.

## Repository structure

- `01.Basics/` — Starter examples and notebooks
  - `01.py` — a short Python script with basic Pandas operations
  - `02pandaSeries.ipynb` — Pandas Series examples
  - `03Read_csv.ipynb` — how to read CSV files with Pandas
  - `04Json.ipynb` — working with JSON data
  - `05.ipynb` — extra examples
  - `data.csv`, `data.json` — example data used by the notebooks

- `02.Cleaning Data/` — notebooks focused on cleaning and preprocessing
  - `01/` and `02/` — each contains notebooks (`.ipynb`) and a `data.csv` file with examples

- `03/` — additional examples
  - `data.csv`, `Removing.ipynb` — demonstrates row/column removal and other cleaning

- `04.Correlations/` — correlation and plotting examples
  - `01correlations.ipynb`, `02plotting.ipynb`, `data.csv`

## Who is this for?

Anyone who wants to learn Pandas with hands-on examples. No prior Pandas experience required — basic Python knowledge is helpful.

## Prerequisites

- Python 3.8+ installed
- A terminal (PowerShell on Windows is used in these steps)

Optional but recommended tools:
- Jupyter Notebook or JupyterLab to open and run the `.ipynb` files
- A code editor such as VS Code

## Quick setup (Windows / PowerShell)

1. Open a PowerShell window and change into the project folder:

```powershell
cd "c:\Users\rishi\Downloads\Python\Pandas"
```

2. Create and activate a virtual environment (recommended):

```powershell
python -m venv .venv
# Activate in PowerShell
.\.venv\Scripts\Activate.ps1
```

3. Install the minimal packages you'll need:

```powershell
pip install --upgrade pip
pip install pandas jupyter matplotlib seaborn
```

Tip: If you prefer, create a `requirements.txt` and run `pip install -r requirements.txt`.

## How to run the examples

A. Run the simple script in `01.Basics`:

```powershell
# From the project root
python .\01.Basics\01.py
```

B. Open the notebooks with Jupyter Notebook / Lab:

```powershell
# Start Jupyter Notebook (or jupyter lab if you installed it)
jupyter notebook
# Then use your browser to open any of the .ipynb files in the folder structure
```

C. Notes for notebooks

- Many notebooks read `data.csv` or `data.json` files that are placed alongside the notebooks. If you move files, update the path in the notebook before running the cells.
- Run cells from top to bottom. If a cell depends on earlier cells (imports, variables), they must be run first.

## Step-by-step learning path (suggested)

1. `01.Basics/02pandaSeries.ipynb` — learn what a Pandas Series is and how it's different from a list
2. `01.Basics/03Read_csv.ipynb` — practice loading CSV files and inspecting data
3. `01.Basics/04Json.ipynb` — try loading and converting JSON data
4. `02.Cleaning Data/01/01.ipynb` and `02.Cleaning Data/02/2.ipynb` — follow cleaning examples (missing values, duplicates, type conversions)
5. `04.Correlations/01correlations.ipynb` and `02plotting.ipynb` — explore correlations and plotting with Matplotlib/Seaborn

## Common troubleshooting

- "ModuleNotFoundError: No module named 'pandas'" — activate your venv and `pip install pandas` in that environment.
- Jupyter opens but notebook kernel is not found — make sure the notebook kernel matches the Python environment (you can add your venv as a kernel using `ipykernel` if needed).

## Small tips

- Use `df.head()` to preview the first rows of a DataFrame.
- Use `df.info()` to see columns, data types, and non-null counts.
- Save modified data with `df.to_csv('out.csv', index=False)`.

## Want to contribute or extend?

- Add new notebooks or scripts in a new folder.
- Keep example datasets small so the notebooks stay fast.

## Files changed / created

- `README.md` — This file: a simple step-by-step guide for setup + how to run the notebooks and script.

---

If you'd like, I can also:
- add a `requirements.txt` with the exact packages used,
- add a tiny `run_all.sh`/PowerShell script that opens Jupyter or runs the `01.py` script,
- or open one of the notebooks and extract a short summary of what it contains.

Tell me which of those you'd like next.