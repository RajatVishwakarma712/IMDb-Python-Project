# IMDb Data Analysis & Visualization Project

Dive into the world of IMDb data with powerful analysis and stunning visualizations. Discover movie trends, ratings, genres, and hidden insights through data-driven storytelling and interactive charts.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Data Analysis](#data-analysis)
- [Visualizations](#visualizations)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This project leverages IMDb dataset to perform comprehensive data analysis and create insightful visualizations. It explores movie trends, ratings distribution, genre patterns, and reveals hidden insights about the film industry through interactive charts and statistical analysis.

## ✨ Features

- **Data Cleaning & Preprocessing**: Handle missing values and prepare data for analysis
- **Statistical Analysis**: Comprehensive statistical insights into IMDb data
- **Movie Trends**: Analyze release patterns and trends over time
- **Rating Analysis**: Explore rating distributions and correlations
- **Genre Insights**: Discover patterns within different movie genres
- **Interactive Visualizations**: Beautiful, informative charts and plots
- **Performance Metrics**: Movie performance analysis by various parameters

## 📁 Project Structure

```
IMDb-Python-Project/
├── README.md                    # Project documentation
├── data/                        # Data files (if applicable)
│   └── imdb_data.csv           # Raw IMDb dataset
├── notebooks/                   # Jupyter notebooks
│   ├── 01_data_exploration.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_analysis.ipynb
│   └── 04_visualizations.ipynb
├── src/                        # Source code
│   ├── data_loader.py
│   ├── preprocessing.py
│   ├── analysis.py
│   └── visualization.py
└── requirements.txt            # Project dependencies
```

## 🚀 Installation

### Prerequisites

- Python 3.7 or higher
- pip package manager

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/RajatVishwakarma712/IMDb-Python-Project.git
   cd IMDb-Python-Project
   ```

2. **Create a virtual environment** (optional but recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 💻 Usage

### Running Jupyter Notebooks

```bash
jupyter notebook
```

Navigate to the `notebooks/` directory and open the notebooks in order:
1. `01_data_exploration.ipynb` - Initial data exploration
2. `02_data_cleaning.ipynb` - Data preprocessing and cleaning
3. `03_analysis.ipynb` - Statistical analysis
4. `04_visualizations.ipynb` - Generate visualizations

### Using the Python Modules

```python
from src.data_loader import load_imdb_data
from src.preprocessing import clean_data
from src.analysis import analyze_ratings, analyze_genres
from src.visualization import plot_trends, plot_ratings

# Load and process data
data = load_imdb_data('data/imdb_data.csv')
clean_data = clean_data(data)

# Perform analysis
analyze_ratings(clean_data)
analyze_genres(clean_data)
```

## 📊 Data Analysis

The project analyzes the following aspects:

- **Movie Release Patterns**: Trends in movie releases over decades
- **Rating Distribution**: Analysis of IMDb rating patterns and outliers
- **Genre Performance**: How different genres perform in terms of ratings and popularity
- **Temporal Trends**: Changes in movie characteristics over time
- **Correlations**: Relationships between various movie attributes

## 🎨 Visualizations

Included visualizations:

- Line charts showing movie release trends
- Histograms of rating distributions
- Box plots for genre comparisons
- Scatter plots for correlation analysis
- Bar charts for top-rated movies and genres
- Heatmaps for correlation matrices

## 🛠️ Technologies Used

- **Python 3.x** - Programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive computing environment
- **Scikit-learn** - Machine learning and data analysis (if applicable)

## 📌 Getting Started

### Quick Start Example

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load the data
df = pd.read_csv('data/imdb_data.csv')

# Display basic info
print(df.head())
print(df.info())

# Create a simple visualization
plt.figure(figsize=(12, 6))
sns.histplot(data=df, x='rating', bins=30)
plt.title('IMDb Rating Distribution')
plt.xlabel('Rating')
plt.ylabel('Frequency')
plt.show()
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

## 📝 License

This project is open source and available under the MIT License - see the LICENSE file for details.

## 📧 Contact

For questions or suggestions, feel free to reach out:
- **GitHub**: [@RajatVishwakarma712](https://github.com/RajatVishwakarma712)

## 📚 Resources

- [IMDb Dataset Documentation](https://www.imdb.com/interfaces/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Matplotlib Documentation](https://matplotlib.org/contents.html)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [Jupyter Notebook Guide](https://jupyter.org/documentation)

---

**Happy analyzing! 🎬📊**