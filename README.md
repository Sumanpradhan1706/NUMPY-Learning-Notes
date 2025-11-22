**Project Overview**

- **Name:** `NUMPY-Learning-Notes` — A concise, hands-on collection of Jupyter notebooks that introduce and demonstrate core NumPy concepts.
- **Purpose:** Provide an organized, example-driven walkthrough of NumPy basics (array creation, indexing, broadcasting, data types, and common mathematical functions) suitable for self-study, teaching, and quick reference.
- **Contents:** Six focused notebooks that progressively build NumPy skills with runnable examples.

**Repository Structure**

- **Notebooks:**
  - `01_Creating_numpy_arrays.ipynb` — Array creation, shapes, reshaping, dtypes.
  - `02_Indexing and Slicing.ipynb` — Flattening, slicing, views vs copies, element assignment.
  - `03_Multidimensional indexing and Axis.ipynb` — Multi-dimensional indexing, axis operations, 3D examples.
  - `04_Numpy_Data_Type.ipynb` — Data types, `.astype()`, complex/object/string arrays and notes on homogeneity.
  - `05_Broadcasting_in_Numpy.ipynb` — Vectorization and broadcasting examples (scalar, 1D↔2D, normalization example).
  - `06_mathematical_function_in_Numpy.ipynb` — Statistical and mathematical functions (mean, std, sum, median, log, exp, etc.).

**How To Use**

- **Quick start (recommended, conda):**

```powershell
conda create -n numpy-notes python=3.11 numpy jupyterlab -y
conda activate numpy-notes
jupyter lab
```

- **Open a notebook:**
  - In VS Code: open any `*.ipynb` file and run cells inline.
  - In JupyterLab: click the notebook name in the file browser and run cells.

- **Run a single notebook from the command line:**

```powershell
jupyter nbconvert --to notebook --execute "01_Creating_numpy_arrays.ipynb" --inplace
```

**Interactive / Online Options**

- **View (read-only) via NBViewer:**
  - `01_Creating_numpy_arrays.ipynb`: https://nbviewer.org/github/Sumanpradhan1706/NUMPY-Learning-Notes/blob/main/01_Creating_numpy_arrays.ipynb
  - `02_Indexing and Slicing.ipynb`: https://nbviewer.org/github/Sumanpradhan1706/NUMPY-Learning-Notes/blob/main/02_Indexing%20and%20Slicing.ipynb
  - `03_Multidimensional indexing and Axis.ipynb`: https://nbviewer.org/github/Sumanpradhan1706/NUMPY-Learning-Notes/blob/main/03_Multidimensional%20indexing%20and%20Axis.ipynb
  - `04_Numpy_Data_Type.ipynb`: https://nbviewer.org/github/Sumanpradhan1706/NUMPY-Learning-Notes/blob/main/04_Numpy_Data_Type.ipynb
  - `05_Broadcasting_in_Numpy.ipynb`: https://nbviewer.org/github/Sumanpradhan1706/NUMPY-Learning-Notes/blob/main/05_Broadcasting_in_Numpy.ipynb
  - `06_mathematical_function_in_Numpy.ipynb`: https://nbviewer.org/github/Sumanpradhan1706/NUMPY-Learning-Notes/blob/main/06_mathematical_function_in_Numpy.ipynb

- **Launch interactively (Binder):**
  - Launch Binder for the repository (may require an environment file to fully reproduce):

  https://mybinder.org/v2/gh/Sumanpradhan1706/NUMPY-Learning-Notes/main

- **Open in Colab (editable):**
  - Example: https://colab.research.google.com/github/Sumanpradhan1706/NUMPY-Learning-Notes/blob/main/01_Creating_numpy_arrays.ipynb

**Notebook Summaries**

- **`01_Creating_numpy_arrays.ipynb` — Core array creation and metadata**
  - **Focus:** `np.array`, `np.zeros`, `np.ones`, `np.full`, `np.eye`, `np.arange`, `np.linspace`, `reshape`, `dtype`, `astype`, and basic attributes (`shape`, `size`, `ndim`).
  - **Why it matters:** Building arrays and understanding shape/dtype is the foundation of all NumPy work.

- **`02_Indexing and Slicing.ipynb` — Views, slices, and flattening**
  - **Focus:** `flatten()`, slice notation, indexing single elements, and how slices can be views (assignment to a slice affects the original array).
  - **Why it matters:** Correct indexing avoids subtle bugs and enables efficient, memory-safe operations.

- **`03_Multidimensional indexing and Axis.ipynb` — Axis-aware operations**
  - **Focus:** Accessing rows/columns, `axis` parameter in reductions (e.g., `np.sum(..., axis=0|1)`), 3D-array indexing, and changing values along an axis.
  - **Why it matters:** Many scientific/data tasks require axis-aware reductions and careful multi-dimensional indexing.

- **`04_Numpy_Data_Type.ipynb` — Dtypes and conversions**
  - **Focus:** NumPy data types, `.astype()` conversions, unicode strings, complex and object arrays, and implications for performance.
  - **Why it matters:** Choosing the right dtype reduces memory use and avoids precision or performance issues.

- **`05_Broadcasting_in_Numpy.ipynb` — Vectorization and broadcasting**
  - **Focus:** Element-wise operations, scalar broadcasting, 1D↔2D broadcasting, and a real-world normalization example using broadcasting.
  - **Why it matters:** Broadcasting and vectorization replace slow Python loops with fast, idiomatic NumPy code.

- **`06_mathematical_function_in_Numpy.ipynb` — Common mathematical/statistical functions**
  - **Focus:** `np.mean`, `np.std`, `np.min`, `np.max`, `np.sum`, `np.prod`, `np.median`, `np.percentile`, `np.argmin`, `np.argmax`, `np.unique`, `np.diff`, `np.cumsum`, `np.log`, `np.exp`.
  - **Why it matters:** These functions are central to data analysis and exploratory workflows.

**Best Practices & Notes**

- **Prefer vectorized operations:** avoid Python loops for array math; use NumPy operations to leverage optimized C code.
- **Be mindful of views vs copies:** assignments to views modify the original array — use `.copy()` to get an independent array.
- **Pick appropriate dtypes:** smaller types save memory; complex/object dtypes should be used only when necessary.
- **Document experiments:** keep notebooks small, focused, and runnable to make them useful for learners.

**Contributing**

- **Improvements welcome.** If you'd like to add examples, exercises, or corrections, open a PR with a focused change and a brief description.

**License**

- No license file is present in the repository. Add a `LICENSE` if you want a specific license applied.

**Contact / Author**

- Repository owner: `Sumanpradhan1706` (GitHub). If this is your local copy, push to GitHub to enable Binder/Colab links.

---

If you'd like, I can:
- add a `requirements.txt` or `environment.yml` for reproducible Binder launches,
- add badges (Binder/Colab/nbviewer) directly into this README, or
- create short exercise notebooks or tests to accompany the examples.
