# Student Marks Analysis with NumPy

A practical demonstration of NumPy array operations for educational data analysis. This project analyzes student marks across multiple subjects using NumPy's powerful vectorized operations.

## Overview

This Jupyter notebook showcases essential NumPy operations through a real-world use case: analyzing student performance data across subjects. It demonstrates practical data manipulation techniques commonly used in data science and analysis workflows.

## Features

- **Array Creation & Manipulation**: Working with 2D NumPy arrays for structured data
- **Aggregation Operations**: Computing totals and averages across different axes
- **Statistical Analysis**: Finding maximum/minimum values and percentages
- **Boolean Indexing**: Filtering data based on conditions
- **Data Formatting**: Clean, readable output presentation

## What You'll Learn

- Creating and structuring NumPy arrays
- Using `np.sum()` and `np.mean()` with axis parameters
- Finding extremes with `np.argmax()` and `np.argmin()`
- Boolean masking and conditional filtering
- Practical applications of NumPy in education/data analysis

## Prerequisites

- Python 3.7+
- NumPy
- Jupyter Notebook

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/numpy-marks-analysis.git
cd numpy-marks-analysis

# Install dependencies
pip install numpy jupyter

# Or using conda
conda install numpy jupyter
```

## Usage

1. **Open the notebook:**
```bash
jupyter notebook NumPY.ipynb
```

2. **Run all cells** to see the analysis output

3. **Modify data** in the first cell to analyze your own marks:
```python
marks = np.array([
    [85, 92, 78, 88],   # Student 1
    [76, 65, 90, 72],   # Student 2
    # Add more rows for more students
])

names = np.array(["Name1", "Name2", ...])
subjects = ["Math", "Science", "English", "SST"]
```

## Output Example

```
📋 Marks Data:
[[85 92 78 88]
 [76 65 90 72]
 ...
]

📊 STUDENT MARKS ANALYSIS
==================================================

Total marks per student:
  Arjun    : 343/400  (85.8%)
  Priya    : 303/400  (75.8%)
  ...

Class average per subject:
  Math     : 80.8
  Science  : 82.4
  English  : 82.6
  SST      : 82.6

🏆 TOP STUDENT: Vikram with 362 marks
😓 HARDEST SUBJECT: Math (avg 80.8)
⭐ Above 80% : ['Arjun', 'Ravi', 'Vikram']
```

## Key NumPy Operations Used

| Operation | Code | Purpose |
|-----------|------|---------|
| Sum | `np.sum(marks, axis=1)` | Total marks per student |
| Mean | `np.mean(marks, axis=0)` | Average marks per subject |
| Max Index | `np.argmax(totals)` | Find top performer |
| Min Index | `np.argmin(subject_avg)` | Find hardest subject |
| Boolean Filter | `names[percentages > 80]` | Filter students by criteria |

## Project Structure

```
numpy-marks-analysis/
├── NumPY.ipynb          # Main Jupyter notebook
├── README.md            # This file
└── data/                # (Optional) Store sample datasets
    └── marks_data.csv   # (Optional) CSV format data
```

## Practice Exercises

Try implementing these to deepen your NumPy skills:

1. Find the subject with highest marks (not just average)
2. Calculate standard deviation of marks per subject
3. Identify students scoring below class average in each subject
4. Rank students by percentage
5. Create a correlation matrix between subjects

## Resources

- [NumPy Documentation](https://numpy.org/doc/)
- [NumPy Beginner's Guide](https://numpy.org/doc/stable/user/absolute_beginners.html)
- [DataCamp NumPy Cheat Sheet](https://www.datacamp.com/cheat-sheet/numpy-cheat-sheet-data-analysis-in-python)

## License

This project is open source and available under the MIT License - see LICENSE file for details.

## Author

**Yadala Avinash**
- B.Tech ECE Student at MITS (Class of 2027)
- SDE Aspirant | AI Enthusiast
- Building [HireReady](https://github.com/yourusername/hireready) - AI-powered interview coaching platform

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/yourusername/numpy-marks-analysis/issues).

## Feedback

Have suggestions? Open an issue or reach out!

---

**Last Updated**: September 2026
