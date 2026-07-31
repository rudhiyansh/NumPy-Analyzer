# 🔢 NumPy Analyzer

A menu-driven, terminal-based data analysis toolkit built entirely with **NumPy** and core **Python OOP concepts** (encapsulation, properties, class methods, static methods). Create arrays of any dimension and perform math operations, indexing/slicing, combining/splitting, searching/sorting/filtering, and statistical analysis — all through a simple interactive CLI.

<p align="center">
  <a href="#-video-walkthrough">
    <img src="https://img.shields.io/badge/▶-Watch%20the%20Build%20Video-red?style=for-the-badge&logo=youtube" alt="Watch the video">
  </a>
</p>

---

## 📖 Project Description

**NumPy Analyzer** is a Python console application that wraps common NumPy operations inside a clean, guided menu system. Instead of writing NumPy code from scratch every time, you launch the tool and simply pick what you want to do — create a 1D/2D/3D array, run math on it, slice it, sort it, filter it, or compute statistics — and the tool handles the NumPy calls for you.

It was built as a hands-on project to practice:
- NumPy array creation, reshaping, and manipulation
- Python OOP (private attributes, `@property`, `@staticmethod`, `@classmethod`)
- Writing clean, exception-safe, user-driven CLI programs

---

## ✨ Features

| Menu Option | What it does |
|---|---|
| **1. Create a NumPy Array** | Build a 1D, 2D, or 3D array from your own input values |
| &nbsp;&nbsp;↳ Indexing & Slicing | Access single elements or slice sub-arrays for any dimension |
| **2. Mathematical Operations** | Element-wise Addition, Subtraction, Multiplication, Division, plus Dot Product and Matrix Multiplication (2D) |
| **3. Combine or Split Arrays** | Concatenate/vertically stack two arrays, or split an array into N equal parts |
| **4. Search, Sort & Filter** | Find a value's index with `np.where`, sort arrays, or filter with conditions (`>`, `<`, `==`, or a value range) |
| **5. Aggregates & Statistics** | Compute Sum, Mean, Median, Standard Deviation, and Variance |
| **6. Exit** | Cleanly exits the program |

Additional highlights:
- ✅ Supports **1D, 2D, and 3D arrays**
- ✅ Input validation with graceful error handling (`try/except` everywhere)
- ✅ Clean OOP design — array state is encapsulated in a private attribute with getter/setter properties
- ✅ Alternate constructor via `create_from_range()` classmethod (build an array with `np.arange`)

---

## 🛠️ Tech Stack

- **Python 3**
- **NumPy**
- Jupyter Notebook (`.ipynb`) — original development environment

---

## 📂 Project Structure

```
Numpy-Analyzer/
├── Numpy_Analyzer.ipynb   # Main notebook containing the DataAnalytics class + CLI
└── README.md              # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- NumPy
- Jupyter Notebook / JupyterLab (or run as a `.py` script)

### Installation

```bash
# Clone the repository
git clone https://github.com/rudhiyansh/Numpy-Analyzer.git
cd Numpy-Analyzer

# Install dependencies
pip install numpy notebook
```

### Usage

**Option 1 — Run in Jupyter Notebook**
```bash
jupyter notebook Numpy_Analyzer.ipynb
```
Run the cell and follow the on-screen menu prompts.

**Option 2 — Run as a Python script**
```bash
jupyter nbconvert --to script Numpy_Analyzer.ipynb
python Numpy_Analyzer.py
```

### Example Session

```
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
Enter your choice: 2
Enter the number of rows: 2
Enter the number of columns: 3
Enter 6 elements for the array separated by space: 20 30 40 50 60 70

Array created successfully:
[[20 30 40]
 [50 60 70]]
```

---

## 🎥 Video Walkthrough

I recorded a full screen-recording documentary-style video while building this project, walking through the thought process and code line by line.

<p align="center">
  <a href="PASTE_YOUR_VIDEO_LINK_HERE">
    <img src="https://img.shields.io/badge/▶️_Open_My_Video-Watch_Now-red?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch the video walkthrough">
  </a>
</p>

> Replace `PASTE_YOUR_VIDEO_LINK_HERE` above with your actual video URL (YouTube, Google Drive, etc.) so the button links correctly.

---

## 🔮 Future Improvements

- [ ] Add unit tests for each operation
- [ ] Support loading array data from CSV files
- [ ] Add a simple GUI (Tkinter / Streamlit) version
- [ ] Export results to file

---

## 👤 Author

**Rudhiyansh**
GitHub: [@rudhiyansh](https://github.com/rudhiyansh)

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

---

<p align="center">If you found this project useful, consider giving it a ⭐!</p>
