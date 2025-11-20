# Python Data Science Handbook

A comprehensive online resource for learning Python for data science, built with Quarto. This handbook provides practical examples, step-by-step tutorials, and real-world applications for data analysis, visualization, and machine learning.

## 🌐 Live Website

Visit the handbook at: [https://jcfly3000.github.io/Into-Python/](https://jcfly3000.github.io/Into-Python/)

## 📚 Content Overview

This handbook covers everything you need to know for Python data science:

### Introduction (`intro/`)
- **Basic Python**: Installation, setup, and fundamental programming concepts
- **Python Books**: Essential reading resources and references
- **Data Books**: Specialized guides for data analysis
- **Statistics Books**: Statistical concepts and applications

### Data Manipulation (`data manipulation/`)
- **Input/Output**: Reading and writing various data formats (CSV, Excel, Parquet, etc.)
- **Data Structures**: Understanding Python's built-in data types and structures
- **Pandas**: Comprehensive data analysis and manipulation
- **Polar**: High-performance dataframes for Python
- **SQL Databases**: Working with structured data
- **Siuba**: Data manipulation with a grammar-based approach

### Data Visualization (`plot/`)
- **Seaborn**: Statistical data visualization
- **Plotnine**: Grammar of graphics implementation in Python
- **Plotly**: Interactive web-based visualizations

### Publishing & Sharing (`Publish/`)
- **Shiny**: Building interactive web applications
- **Quarto**: Creating reproducible documents and reports

### Advanced Topics (`other/`)
- **Web Scraping**: Extracting data from websites (comprehensive guide with real examples)
- **Web Scraping Projects**: Practical examples including whisky data scraping

## 🎯 Target Audience

This handbook is designed for:
- **Beginners** new to Python programming
- **Data analysts** transitioning to Python
- **Data scientists** looking for comprehensive reference material
- **Researchers** wanting to learn data analysis with Python
- **Students** seeking practical, hands-on learning materials

## 🚀 Getting Started

### Quick Start
1. **Visit the live website** for the best reading experience
2. **Clone this repository** if you want to run the code locally:
   ```bash
   git clone https://github.com/jcfly3000/Into-Python.git
   cd Into-Python
   ```
3. **Install Quarto** to render the documents locally:
   ```bash
   # macOS
   brew install quarto

   # Or download from https://quarto.org/
   ```
4. **Preview the site locally**:
   ```bash
   quarto preview index.qmd
   ```

### Prerequisites
- **Python 3.11+** with pip
- **Quarto** for document rendering
- **Essential Python packages**:
  ```bash
  pip install pandas numpy matplotlib seaborn plotly requests beautifulsoup4 selenium
  ```

## 🛠️ Technical Stack

- **Python 3.11+**: Core programming language
- **Quarto**: Publishing system for technical content
- **Pandas**: Data manipulation library
- **NumPy**: Numerical computing
- **Matplotlib/Seaborn**: Data visualization
- **Plotly**: Interactive visualizations
- **Requests/BeautifulSoup**: Web scraping libraries
- **Selenium**: Browser automation
- **Jupyter**: Interactive computing environment

## 📁 Project Structure

```
Into-Python/
├── intro/                  # Introduction and basics
├── data manipulation/      # Data analysis libraries
├── plot/                   # Visualization libraries
├── Publish/                # Publishing tools
├── other/                  # Advanced topics
├── docs/                   # Rendered HTML site
├── _quarto.yml            # Quarto configuration
├── styles.css             # Custom styling
├── foldableCodeBlock.lua  # Custom Quarto filter
└── CLAUDE.md              # Development guidelines
```

## 🔧 Development

### Building the Site
```bash
# Render entire site
quarto render

# Preview with live reload
quarto preview

# Render specific file
quarto render path/to/file.qmd
```


