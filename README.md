# 5G Throughput Analysis - Downtown Minneapolis

Statistical analysis and visualization of commercial mmWave 5G throughput variability using real-world drive test data from downtown Minneapolis (April 2023).

## Project Overview

This project validates key findings from the [Lumos5G paper](https://dl.acm.org/doi/10.1145/3419394.3423629) (IMC 2020) through independent analysis of commercial 5G measurements. The study explores throughput distribution, geographic patterns, mobility impacts, and variability in NSA (Non-Standalone) and SA (Standalone) 5G deployments.

## Key Findings

- **High Variability**: 5G throughput shows coefficient of variation (CV) > 50% at most locations
- **Modest Real-World Performance**: Median throughput of 96 Mbps despite theoretical multi-Gbps capability
- **Extreme Fluctuations**: Throughput swings from near 0 to 700+ Mbps within seconds
- **Location Insufficient**: Geographic coordinates alone cannot reliably predict throughput
- **SA vs NSA Similar**: Both deployment types show comparable performance distributions

## Repository Contents
```
5G_Project/
├── 5G_Analysis.ipynb              # Main Jupyter notebook with all analysis
├── report.md                      # Full technical report
├── plot1_throughput_distribution.png
├── plot2_throughput_heatmap.png
├── plot3_speed_impact.png
├── plot4_variability.png
├── plot5_time_series.png
├── plot6_summary_statistics.png
├── README.md                      # This file
└── requirements.txt               # Python dependencies
```

## How to Run

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook

### Installation

1. Clone this repository:
```bash
git clone https://github.com/theonlydanmat7/5G-Throughput-Analysis.git
cd 5G-Project
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook
```

4. Open `5G_Analysis.ipynb` and run all cells

**Note**: The original dataset is not included in this repository due to size. To reproduce the analysis, you'll need to obtain the Lumos5G dataset from https://lumos5g.umn.edu or contact the authors.

## Visualizations

### Throughput Distribution
![Throughput Distribution](plot1_throughput_distribution.png)

### Geographic Heatmap
![Throughput Heatmap](plot2_throughput_heatmap.png)

### Time Series Fluctuation
![Time Series](plot5_time_series.png)

*See the full report for detailed analysis of all visualizations.*

## Full Report

For the complete technical analysis, methodology, and detailed findings, see [report.md](report.md).

## Dataset

- **Source**: Lumos5G Project, University of Minnesota
- **Location**: Downtown Minneapolis, Minnesota, USA
- **Time Period**: April 2023
- **Measurement Type**: Drive tests with NSA and SA 5G deployments
- **Sample Size**: 10,000+ measurements across 324 feature columns

## Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical visualizations
- **NumPy** - Numerical computing
- **Jupyter Notebook** - Interactive development environment

## References

Narayanan, A., Ramadan, E., Mehta, R., Hu, X., Liu, Q., Fezeu, R. A. K., Dayalan, U. K., Verma, S., Ji, P., Li, T., Qian, F., & Zhang, Z. L. (2020). **Lumos5G: Mapping and Predicting Commercial mmWave 5G Throughput**. *Proceedings of the ACM Internet Measurement Conference (IMC '20)*, 176-193. https://doi.org/10.1145/3419394.3423629

**Author: Daniel Mathew**
- Course: CSCI 4900 Internet of Things
- Date: 12/03/2025

## License

This project is for academic purposes. Dataset provided by the Lumos5G project team.

## Acknowledgments

- Lumos5G project team at the University of Minnesota for providing the dataset
- Original paper authors for their groundbreaking work on 5G throughput prediction
```
