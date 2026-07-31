# 🔢 NumPy Analyzer

A menu-driven Python toolkit that combines **NumPy** array operations with **Object-Oriented Programming (OOP)** principles — encapsulation, static methods, and class methods — to let you create, manipulate, and analyze numerical data from the command line.

---

## 🎥 Project Walkthrough

📺 **[Watch me build this project — screen recording](#)**
*(Replace the `#` above with your actual video link)*

---

## 📝 Description

NumPy Analyzer is a single-class (`DataAnalytics`) command-line toolkit built around NumPy. It lets you create 1D, 2D, or 3D arrays, index and slice them, run element-wise math (plus dot product and matrix multiplication) against a second array, combine or split arrays, search/sort/filter values, and compute aggregate statistics — all through a simple numbered menu. The underlying array is kept private and only touched through the class's own methods, so all the array logic stays encapsulated inside `DataAnalytics`.

---

## ✨ Features

- **Array Creation** — Build 1D, 2D, or 3D NumPy arrays from user input (2D/3D reshaped automatically from a flat list of values)
- **Indexing & Slicing** — Access single elements or ranges, with dedicated handling for 1D vs. 2D/3D arrays
- **Mathematical Operations** — Element-wise addition, subtraction, multiplication, and division against a second array of matching shape, plus **dot product** and **matrix multiplication** for 2D arrays
- **Combine & Split** — Concatenate (1D) or vertically stack (2D/3D) two arrays, or split an array into N equal parts
- **Search, Sort & Filter** — Locate a value's index/indices, sort the array, or filter elements by greater-than, less-than, equal-to, or a between-two-values range
- **Aggregates & Statistics** — Sum, mean, median, standard deviation, and variance
- **Encapsulation** — The underlying array is stored as a private attribute (`__array`), accessed only via a `@property` getter/setter or the class's own methods
- **`@staticmethod`** — A `display()` method that doesn't need an instance to run
- **`@classmethod`** — `create_from_range()`, an alternate constructor that builds a `DataAnalytics` object directly from a NumPy range
- **Menu-Driven UI** — Full numbered menu with a working exit option

---

## ✅ Requirement Coverage

| Requirement (from project brief) | Status | Notes |
|---|---|---|
| `DataAnalytics` class encapsulating all functionality | ✅ | Single class wraps every operation |
| Array creation (1D/2D/3D) | ✅ | `create_array()` |
| Indexing & slicing | ✅ | `sli()` |
| Combining arrays | ✅ | `com_slp()` — concatenate/vstack |
| Splitting arrays | ✅ | `com_slp()` — `np.array_split` |
| Element-wise +, −, ×, ÷ | ✅ | `math()` |
| Dot product / matrix multiplication (2D) | ✅ | `math()` — options 5 & 6, verified working |
| Search for a value | ✅ | `sea_sort()` — `np.where` |
| Sort ascending/descending | ⚠️ Partial | Only ascending sort (`np.sort`) is available; still no descending option |
| Filter by condition | ✅ | `sea_sort()` — greater/less/equal/between |
| Sum, mean, median, std dev, variance | ✅ | `ag_stat()` |
| Min/max values | ❌ Missing | Still not in `ag_stat()`'s menu |
| Percentiles | ❌ Missing | Still not implemented |
| Correlation coefficients between arrays | ❌ Missing | Still not implemented |
| Constructors for initializing arrays | ✅ | `__init__` + `array` setter |
| Encapsulation, private internal methods | ✅ | `__array`, `__check()` |
| `@classmethod` for additional utility | ✅ | `create_from_range()` |
| `@staticmethod` for additional utility | ⚠️ Partial | `display()` is defined but still never called in `main()` |
| Menu-driven UI with exit | ✅ | `main()` loop |

**Improved from the previous version** — dot product and matrix multiplication are now implemented and tested working. Still outstanding: descending sort, min/max, percentiles, and correlation coefficients.

---

## 🐞 A Few Things Worth Knowing

Not blockers, just flagging in case you want to tidy them up:

- **`create_from_range()` and `display()` still aren't wired into the menu.** Both exist on the class but there's no menu option that calls them, so a reviewer won't see them run.
- **Combine only supports two arrays at a time** (the original plus one you enter), not an arbitrary number, even though the brief says "concatenate multiple arrays."
- Minor typos in prompts: `"elemnts"` instead of "elements", `"Invaild choice."` instead of "Invalid choice."

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Dependencies:** [NumPy](https://numpy.org/)

---

## 📂 Project Structure

```
├── Numpy_Analyzer.ipynb   # Main application (Jupyter Notebook)
└── README.md              # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- NumPy (`pip install numpy`)
- Jupyter Notebook / JupyterLab (or convert the notebook to a `.py` file to run from a terminal)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/rudhiyansh/numpy-analyzer.git
   cd numpy-analyzer
   ```

2. Install dependencies:
   ```bash
   pip install numpy
   ```

3. Open and run the notebook:
   ```bash
   jupyter notebook Numpy_Analyzer.ipynb
   ```

---

## 💻 Usage

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
```

- **1. Create a Numpy Array** — Choose to create a new 1D/2D/3D array, or index/slice an existing one.
- **2. Perform Mathematical Operations** — Element-wise +, −, ×, ÷, or dot product / matrix multiplication (2D arrays) with a second array.
- **3. Combine or Split Arrays** — Merge with another array, or split the current array into N parts.
- **4. Search, Sort, or Filter Arrays** — Look up a value, sort the array, or filter by a condition.
- **5. Compute Aggregates and Statistics** — Sum, mean, median, standard deviation, or variance.
- **6. Exit** — Closes the program.

### Example

```
Enter your choice: 2

Choose a mathematical operation:
1. Addition
2. Subtraction
3. Multiplication
4. Division
5. Dot Product (2D only)
6. Matrix Multiplication (2D only)
Enter your choice: 6

Enter rows for second matrix (should be 3): 3
Enter columns for second matrix: 2
Enter 6 elements for second matrix: 1 2 3 4 5 6

Original Array:
[[10 20 30]
 [40 50 60]]

Second Array:
[[1 2]
 [3 4]
 [5 6]]

Matrix Multiplication Result:
[[220 280]
 [490 640]]
```

## 👤 Author

**GitHub:** [@rudhiyansh](https://github.com/rudhiyansh)

---

## 📄 License

This project is submitted for academic purposes as part of a Python OOP / Data Analysis assignment.

---

*"Quality is our Motto."*
