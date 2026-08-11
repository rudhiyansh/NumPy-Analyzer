# 🧮 NumPy Analyzer

A menu-driven, command-line data analytics toolkit built entirely with **NumPy** and core **Python OOP concepts** (encapsulation, properties, static methods, and class methods). NumPy Analyzer lets you create, manipulate, and analyze 1D, 2D, and 3D arrays interactively — no need to write a single line of code to explore array operations.

## 📖 Project Description

NumPy Analyzer is an educational, interactive Python application that wraps common NumPy operations behind a simple text menu. It was built to demonstrate practical use of:

- **Object-Oriented Programming** — a `DataAnalytics` class encapsulating array state with private attributes, `@property`/setter, `@staticmethod`, and `@classmethod`
- **NumPy fundamentals** — array creation, reshaping, indexing, slicing, broadcasting, linear algebra, aggregation, and boolean filtering

Whether you're learning NumPy, teaching it, or just need a quick tool to poke at arrays without firing up a full notebook, this project provides a guided, menu-based interface to do it all.

## ✨ Features

### 🧱 Array Creation
- Create **1D, 2D, or 3D** NumPy arrays from custom user input
- Alternate constructor to create arrays directly from a numeric range (`create_from_range`)

### 🔍 Indexing & Slicing
- Access individual elements by index (1D, 2D, 3D supported)
- Slice arrays using flexible `start:end` range syntax

### ➕ Mathematical Operations
- Element-wise **addition, subtraction, multiplication, division**
- **Dot product** (2D arrays)
- **Matrix multiplication** with automatic shape validation

### 🔗 Combine & Split
- Concatenate 1D arrays or vertically stack 2D/3D arrays
- Split an array into *n* equal parts

### 🔎 Search, Sort & Filter
- Search for a value and get its index/indices
- Sort arrays (row-wise for multi-dimensional arrays)
- Filter elements by:
  - Greater than a value
  - Less than a value
  - Equal to a value
  - Between two values

### 📊 Aggregate & Statistical Analysis
- Sum, Mean, Median
- Standard Deviation
- Variance

## 🛠️ Tech Stack

- **Python 3**
- **NumPy**

## 📂 Project Structure

```
Numpy_Analyzer/
│
├── Numpy_Analyzer.ipynb   # Main notebook containing the DataAnalytics class & CLI
└── README.md              # Project documentation
```

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3 and NumPy installed:

```bash
pip install numpy
```

### Installation

1. Clone the repository:

```bash
git clone https://github.com/rudhiyansh/Numpy_Analyzer.git
cd Numpy_Analyzer
```

2. Launch the notebook:

```bash
jupyter notebook Numpy_Analyzer.ipynb
```

Or convert it to a script and run it directly from the terminal:

```bash
jupyter nbconvert --to script Numpy_Analyzer.ipynb
python Numpy_Analyzer.py
```

## ▶️ Usage

Once running, you'll be greeted with the main menu:

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

**Example — creating a 2D array:**

```
Enter your choice : 1
1. Create a new array
2. Indexing and Slicing
Enter your choice : 1

Select the type of array to create:
1. 1D Array
2. 2D Array
3. 3D Array
Enter your choice : 2
Enter the number of rows : 2
Enter the number of columns : 2
Enter 4 elements for the array separated by space : 1 2 3 4

Array created successfully:
[[1 2]
 [3 4]]
```

Simply follow the on-screen prompts to navigate between creating arrays, running math operations, filtering, sorting, and computing statistics.

## 🎯 Learning Highlights

This project is a great reference for:
- Using `@property` and setters to protect internal state
- The difference between `@staticmethod` and `@classmethod`
- Name mangling with double-underscore private attributes (`__array`)
- Practical NumPy operations: `reshape`, `np.dot`, `@` (matmul), `np.where`, `np.sort`, `np.array_split`, boolean masking

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/rudhiyansh/Numpy_Analyzer/issues) or open a pull request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Rudhiyansh**
GitHub: [@rudhiyansh](https://github.com/rudhiyansh)

---

⭐ If you found this project useful, consider giving it a star on GitHub!
