# Python-advanced-methods and working with data structures and file handling
Includes advanced in-built functions for various datatypes in Python and more.
# Advanced Python Methods — advpy.ipynb

This Jupyter notebook (advpy.ipynb) is a hands-on collection of examples demonstrating intermediate-to-advanced Python features and standard library modules. It is intended as a learning / reference file covering string operations, collections, file and OS interaction, datetime, regular expressions, and other commonly used utilities.

Repository notebook permalink:
https://github.com/devcodes2108/Python-advanced-methods/blob/cd4e6116d003726f3132c50aaa79c41d91648855/advpy.ipynb

## Contents (high level)
- String properties and methods (immutability, slicing, case conversions, formatting)
- Number formatting and conversions (hex, binary, rounding, absolute)
- Collections: lists, sets, dictionaries — advanced operations and methods
- Advanced modules:
  - collections (Counter, defaultdict, namedtuple)
  - os and shutil (file operations, walking directories)
  - datetime (time, date, timedelta arithmetic)
  - re (regular expressions examples and searching)
- Examples that show typical usage patterns and small demonstrations (printing outputs)
- A few interactive cells that accept user input (via input())

## Notable examples / cells
- Demonstration of string immutability (attempt to assign to string index raises TypeError).
- Various string methods: .upper(), .lower(), .title(), .split(), .count(), .find(), .center()
- String formatting using `.format()` and f-strings; numeric formatting with precision specifiers.
- Converting integers to hex and binary using `hex()` / `bin()` (cells use input()).
- Rounding and absolute value demonstrations using `round()` and `abs()` (cells use input()).
- Set operations: add, discard, union, intersection, issubset, issuperset, isdisjoint, difference, symmetric_difference.
- Dictionary comprehensions and methods: `.items()`, `.keys()`, `.values()`.
- List methods: append, extend, insert, pop, remove, sort, reverse, sorted().
- collections module:
  - Counter for counting items and words (`Counter.most_common()`).
  - defaultdict usage for default values.
  - namedtuple usage.
- File and OS operations:
  - Basic file read/write using open().
  - `os.getcwd()`, `os.listdir()`, `os.walk()` examples.
  - Notes about safely deleting files (send2trash suggestion in the notebook).
- datetime:
  - `datetime.time`, `datetime.date`, `datetime.datetime`, timedelta arithmetic and `.total_seconds()`.
- Regular expressions:
  - re.search, re.findall, re.finditer, and examples for phone-number pattern matching.

## Requirements
- Python 3.x
- Jupyter Notebook (or JupyterLab)
- The notebook uses only Python standard library modules (collections, os, shutil, datetime, re). No external dependencies are required for the demonstrated examples.
- If you want to try the "move" or secure-delete suggestions, you may optionally install `send2trash` (not required): pip install send2trash

## How to run
1. Clone the repository:
   git clone https://github.com/devcodes2108/Python-advanced-methods.git
2. Change to the repository directory:
   cd Python-advanced-methods
3. Start Jupyter:
   jupyter notebook
4. Open advpy.ipynb in your browser and run the cells interactively.

Note: Some cells use input() and will prompt for user input. Running the entire notebook non-interactively may hang on those cells; either provide the expected input or skip those cells.

## Known issues / notes
- One cell intentionally demonstrates that strings are immutable by attempting item assignment which raises:
  TypeError: 'str' object does not support item assignment
  This is expected behavior and is shown for teaching purposes.
- The notebook was authored and executed on a specific machine (paths like `C:\Users\devan\Documents` appear in outputs). Outputs and file listings will differ per environment.
- A few cells are examples and may write files into the current working directory (e.g., `practice.txt`). Remove or move these files if not needed.

## Suggestions for improvement
- Convert interactive input() cells to parameterized examples or Notebook widgets for smoother automated runs.
- Add unit-test style example scripts for core demonstrations to make them runnable in CI.
- Split large topics into separate notebooks (strings.ipynb, collections.ipynb, datetime_re.ipynb) for modular learning.

## License & Author
- Author: devcodes2108
- Check the repository for the project license (if present). If none exists, assume all code is provided for educational purposes and confirm intended license before reusing.

If you'd like, I can:
- Create a cleaned, non-interactive version of this notebook (replace input() with example values).
- Split topics into separate notebooks or add a requirements.txt and execution script.
```
