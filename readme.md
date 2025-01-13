# Twitch Games Data Analysis Project

## Overview

This project analyzes Twitch gaming data from 2016 to 2023, focusing on viewing patterns, game popularity trends, and viewer engagement metrics. The analysis includes basic statistical summaries, advanced visualizations, and complex analytical features such as clustering and growth trajectory analysis.

## Dataset

The dataset contains monthly statistics for the top 200 games on Twitch, including metrics such as:

- Hours watched
- Hours streamed
- Peak viewers
- Average viewers
- Channel statistics
- Viewer ratios

## Features

### Basic Analysis

- Data loading and preprocessing
- Summary statistics generation
- Unique game counting
- Date range analysis

### Trend Analysis

- Top games ranking by various metrics
- Monthly trend visualization
- Yearly pattern heatmaps
- Seasonal analysis

### Advanced Analytics

1. **Game Volatility Analysis**

   - Tracks ranking changes over time
   - Calculates volatility scores
   - Identifies most volatile games
2. **Cluster Analysis**

   - K-means clustering of games based on viewing patterns
   - PCA visualization of game clusters
   - Identification of similar games based on viewer behavior
3. **Growth Trajectory Analysis**

   - Linear regression analysis of viewership trends
   - Growth rate calculation and categorization
   - R-squared value assessment
   - Visual representation of growth patterns

### Visualization Features

- Time series plots
- Heatmaps
- Correlation matrices
- Scatter plots with annotations
- Bar charts and line graphs

## Requirements

The following Python packages are required:

- pandas
- numpy
- matplotlib
- seaborn
- scipy
- scikit-learn

## Installation

1. Clone this repository
2. Install required packages:

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn
```

## Usage

```python
# Initialize analyzer with data file
analyzer = TwitchAnalyzer('path_to_your_data.csv')

# Basic statistics
stats = analyzer.basic_statistics()

# Generate visualizations
analyzer.plot_monthly_trends('League of Legends')
analyzer.create_yearly_heatmap('Hours_watched')

# Advanced analysis
volatility_plot, volatility_data = analyzer.analyze_game_volatility()
cluster_plot, cluster_data = analyzer.perform_cluster_analysis()
growth_plot, growth_data = analyzer.analyze_growth_trajectory()
```

## Code Structure

- `TwitchAnalyzer`: Main class containing all analysis methods
- Each method is documented with docstrings explaining functionality
- Modular design allows for easy extension and modification

## Notes

- The code assumes the input data is in CSV format
- Some analyses require minimum data points (e.g., 6 months for growth analysis)
- Visualizations are automatically sized for readability
- All figures can be saved or displayed interactively

## Future Improvements

- Add more advanced statistical tests
- Implement predictive modeling
- Add export functionality for analysis results
- Include more interactive visualization options

## License

This project is licensed under the MIT License - see the LICENSE file for details.
