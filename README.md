# 📊 Personal Life Dashboard

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20Seaborn%20%7C%20Scikit--learn-blueviolet.svg)](#dependencies)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A comprehensive data science project for exploring and quantifying relationships between daily life metrics including sleep, mood, productivity, and weather patterns.

## 🎯 Project Overview

This project serves as a personal "life dashboard" designed for anyone interested in the **quantified self** movement. It provides a complete framework for analyzing how various daily factors influence each other, helping you understand patterns in your personal data.

### What Makes This Special?

- **Realistic Synthetic Data**: Generates 180 days of life data with built-in correlations that mirror real-world relationships
- **Complete Analysis Pipeline**: From data generation to predictive modeling
- **Easy Customization**: Designed as a template for your own personal data
- **Professional Visualizations**: Publication-ready charts and insights

## ✨ Features

### 🔄 Synthetic Data Generation
- Creates realistic daily entries for sleep, mood, productivity, and weather
- Built-in logical correlations (e.g., better sleep → improved mood)
- 180-day dataset perfect for trend analysis

### 📈 Comprehensive Exploratory Data Analysis
- **Time Series Analysis**: Track metrics over time to identify trends and patterns
- **Distribution Analysis**: Understand the spread and shape of your data
- **Categorical Analysis**: Visualize weather patterns and their frequency

### 🔍 Advanced Correlation Analysis
- **Correlation Heatmap**: Color-coded matrix showing relationships between variables
- **Pair Plot Analysis**: Deep-dive visualizations revealing complex interactions
- **Weather Impact Assessment**: How external factors affect your daily metrics

### 🤖 Predictive Modeling
- **Linear Regression Model**: Predict daily productivity based on multiple factors
- **Feature Engineering**: Smart encoding of categorical variables
- **Model Evaluation**: R-squared metrics and coefficient interpretation

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/personal-life-dashboard.git
   cd personal-life-dashboard
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
   Or install manually:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook code.ipynb
   ```

4. **Run the analysis**
   Execute all cells to generate synthetic data and run the complete analysis pipeline.


## 🔧 Using Your Own Data

Transform this project into your personal analytics tool:

### 1. Data Collection Methods

| Metric | Collection Method | Tools |
|--------|------------------|-------|
| **Sleep** | Fitness trackers, sleep apps | Oura, Whoop, Fitbit, Sleep Cycle |
| **Mood** | Daily rating (1-10 scale) | Daylio, Mood Meter, spreadsheet |
| **Productivity** | Self-assessment (1-10 scale) | RescueTime, Toggl, manual tracking |
| **Weather** | API or manual entry | OpenWeatherMap API, Weather Underground |

### 2. Data Format

Your CSV should include these columns:
```csv
Date,Sleep_Hours,Sleep_Quality,Mood,Productivity,Weather
2024-01-01,7.5,4,8,7,Sunny
2024-01-02,6.2,3,6,5,Rainy
...
```

### 3. Integration Steps

Replace the synthetic data generation with your own:

```python
# Comment out synthetic data generation
# df = generate_life_data(days=180)

# Load your personal data
df = pd.read_csv('data/my_life_data.csv', parse_dates=['Date'], index_col='Date')
```

## 📊 Sample Insights

The analysis reveals fascinating patterns in daily life data:

- **Sleep Quality Impact**: Each point improvement in sleep quality correlates with a 0.8 point increase in next-day productivity
- **Weather Effects**: Sunny days show 15% higher average mood scores compared to rainy days
- **Productivity Patterns**: Strong positive correlation (r=0.72) between sleep hours and productivity

## 🛠 Dependencies

- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **matplotlib**: Basic plotting
- **seaborn**: Statistical visualizations
- **scikit-learn**: Machine learning models
- **jupyter**: Interactive notebook environment

## 🤝 Contributing

Contributions are welcome! Here are some ways you can help:

- Add new visualization types
- Implement additional ML models
- Create data import utilities for popular tracking apps
- Improve documentation

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🎉 Acknowledgments

- Inspired by the quantified self movement
- Built with love for data-driven personal insights
- Thanks to the open-source Python community

---

**Ready to discover patterns in your life?** Start by running the notebook with synthetic data, then plug in your own metrics to uncover personal insights that can help optimize your daily routine.

⭐ **Star this repo** if you find it useful for your personal analytics journey!
