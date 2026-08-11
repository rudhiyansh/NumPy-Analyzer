<div align="center">

# 🔢 NumPy Analyzer

### A menu-driven command-line toolkit for exploring NumPy arrays — create, slice, compute, and analyze, all from your terminal.

[![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Powered-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)
[![Build](https://img.shields.io/badge/Build-Passing-brightgreen?style=for-the-badge)](#)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-ff69b4?style=for-the-badge)](#-contributing)

</div>

---

## 📖 Table of Contents

- [Why This Project?](#-why-this-project)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Usage](#-usage)
- [Folder Structure](#-folder-structure)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [Author](#-author)
- [License](#-license)

---

## 💡 Why This Project?

Learning NumPy usually means jumping between a dozen scattered scripts and notebook cells just to test one operation at a time. **NumPy Analyzer** solves that by wrapping the most common NumPy workflows — array creation, indexing, math, reshaping, searching, sorting, filtering, and statistics — into a single interactive CLI.

No need to rewrite boilerplate every time you want to check how `np.where` or `np.std` behaves. Launch the tool, pick a menu option, and get instant, readable output. It's built to be a hands-on sandbox for anyone learning array-based computing in Python.

---

## ✨ Features

- 🧱 **Array Creation** — Build 1D, 2D, or 3D NumPy arrays interactively
- 🎯 **Indexing & Slicing** — Access single elements or ranges across any array dimension
- ➕ **Mathematical Operations** — Perform element-wise arithmetic on arrays
- 🔗 **Combine & Split** — Merge arrays together or break them into equal parts
- 🔍 **Search, Sort & Filter** — Locate values, sort in place, and apply conditional filters (greater than, less than, equal to, between)
- 📊 **Aggregate Statistics** — Compute sum, mean, median, standard deviation, and variance on demand

---

## 🛠 Tech Stack

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)](https://numpy.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)](https://jupyter.org/)

| Layer | Technology |
|---|---|
| Language | Python 3.9+ |
| Core Library | NumPy |
| Interface | Command-line (interactive menu) |
| Environment | Jupyter Notebook |

---

## 📦 Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/numpy-analyzer.git
cd numpy-analyzer

# 2. (Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install numpy jupyter
```

---

## 🚀 Usage

Run it directly as a Python script or inside Jupyter Notebook.

**Option A — Jupyter Notebook**

```bash
jupyter notebook Numpy_Analyzer.ipynb
```

Then run all cells and follow the on-screen menu.

**Option B — As a Python script**

```bash
python numpy_analyzer.py
```

**Example session:**

```text
Welcome to the NumPy analyst!
========================================

Choose an option:
1. Create a Numpy Array
2. Perform Mathematical Operations
3. Combine or Split Arrays
4. Search, Sort, or Filter Arrays
5. Compute Aggregates and Statistics
6. Exit

Enter your choice: 1
1. Create a new array
2. Indexing and Slicing
Enter your choice: 1

Select the type of array to create:
1. 1D Array
2. 2D Array
3. 3D Array

Enter your choice: 1
Enter elements separated by space: 4 8 15 16 23 42

Array created successfully:
[ 4  8 15 16 23 42]
```

---

## 📂 Folder Structure

```text
numpy-analyzer/
├── Numpy_Analyzer.ipynb     # Main notebook — DataAnalytics class + CLI
├── README.md                # Project documentation
├── LICENSE                  # License file
└── requirements.txt         # Project dependencies
```

---

## 🗺 Roadmap

- [ ] Export analysis results to CSV/JSON
- [ ] Add support for floating-point and complex-number arrays
- [ ] Visualize arrays with Matplotlib (histograms, heatmaps)
- [ ] Add unit tests with `pytest`
- [ ] Package as a pip-installable CLI tool
- [ ] Build a lightweight web UI (Streamlit) as an alternative frontend

---

## 🤝 Contributing

Contributions are welcome and appreciated! To contribute:

1. **Fork** the repository
2. **Create** your feature branch
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Commit** your changes
   ```bash
   git commit -m "Add: your feature description"
   ```
4. **Push** to your branch
   ```bash
   git push origin feature/your-feature-name
   ```
5. **Open a Pull Request** describing your changes

Bug reports and feature requests are just as valuable — feel free to open an [issue](https://github.com/your-username/numpy-analyzer/issues).

---

## 👤 Author

**Rudhiyansh Vijay Sandanshiv**

- GitHub: [@your-username](https://github.com/your-username)
- 💼 Open to Data Analyst opportunities

If this project helped you learn something, consider giving it a ⭐!

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

<div align="center">

Made with 🧠 and NumPy

</div>
