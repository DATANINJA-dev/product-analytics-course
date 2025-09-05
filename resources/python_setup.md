# Python Environment Setup Guide

## Prerequisites

- Python 3.8 or higher
- Git installed on your machine
- A code editor (VS Code recommended) or Jupyter Notebook

## Installation Steps

### 1. Clone the Repository

```bash
git clone <repository-url>
cd product-analytics-course
```

### 2. Create Virtual Environment

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

## Verifying Installation

Run this code in a Jupyter cell to verify everything is working:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
from scipy import stats
import sklearn

print("✅ All libraries imported successfully!")
print(f"Pandas version: {pd.__version__}")
print(f"NumPy version: {np.__version__}")
print(f"Scikit-learn version: {sklearn.__version__}")
```

## Troubleshooting

### Common Issues

**Issue**: Module not found error
**Solution**: Make sure your virtual environment is activated and all packages are installed

**Issue**: Jupyter kernel not found
**Solution**: 
```bash
python -m ipykernel install --user --name=venv
```

**Issue**: Plotting not working
**Solution**: 
```bash
pip install --upgrade matplotlib plotly
```

## Additional Tools (Optional)

### VS Code Extensions
- Python
- Jupyter
- Python Docstring Generator

### Browser Requirements
- Modern browser (Chrome, Firefox, Safari, Edge) for Plotly interactive plots

## Getting Help

If you encounter issues:
1. Check that your Python version is 3.8+: `python --version`
2. Verify virtual environment is active (you should see `(venv)` in terminal)
3. Try reinstalling requirements: `pip install -r requirements.txt --upgrade`