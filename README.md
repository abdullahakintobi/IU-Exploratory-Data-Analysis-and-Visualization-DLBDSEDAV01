## Course: Exploratory Data Analysis and Visualization (DLBDSEDAV01)

### Project Title

**A Visual Exploration of the Relationship Between Trade Tariffs and Germany's Economic Growth (1988-2021)**

### Project Description

This project conducts an exploratory data analysis (EDA) of Germany's trade and economic performance from 1988 to 2021. The primary goal is to determine the statistical correlation between changes in tariff rates, trade volumes, and economic growth. The analysis uses Python with key data science libraries to clean the data, calculate descriptive statistics, visualize trends, and provide insights into the complex relationship between trade policy and economic indicators.

### File Structure

The project is organized into a clean and logical file structure to facilitate navigation and reproducibility.

```
.
├── data
│   ├── meta
│   │   └── data_dictionary.csv
│   ├── processed
│   │   └── germany_trade_data.csv
│   └── raw
│       └── 34 years_world_export_import_dataset.csv
├── fig
│   └── (project's visualizations were saved here)
├── notebook
│   └── analysis.ipynb
├── .gitignore
├── python-version
├── LICENSE
├── pyproject.toml
├── README.md
└── uv.lock
```
### Features

* Data loading and cleaning using pandas

* Statistical analysis with NumPy and SciPy

* Interactive visualizations using Plotly

* Regression and statistical modeling via statsmodels

* Clear structure for reproducible analysis

### Technologies & Dependencies

The analysis was performed using Python 3.11+ and the following libraries. All dependencies are managed using `pyproject.toml`.

```toml
ipykernel>=6.30.1
nbformat>=5.10.4
numpy>=2.3.3
pandas>=2.3.2
plotly>=6.3.0
scipy>=1.16.2
statsmodels>=0.14.5
```

### Installation & Usage

To run this analysis locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/abdullahakintobi/IU-Exploratory-Data-Analysis-and-Visualization-DLBDSEDAV01.git
    cd IU-Exploratory-Data-Analysis-and-Visualization-DLBDSEDAV01
    ```
2.  **Set up a virtual environment and install dependencies:**
    ```bash
    python -m venv .venv
    .venv\Scripts\activate  # On Mac, use: .venv/bin/activate 
    pip install pip install -r requirements.txt
    ```
3.  **Launch the Jupyter Notebook:**
    ```bash
    jupyter notebook notebook/analysis.ipynb
    ```

### Key Findings

The analysis revealed several key insights into Germany's economic performance and trade policy.

  * **Trade Liberalization:** Germany consistently reduced its tariffs, with AHS tariffs falling from **20.64%** to **6.51%** and MFN tariffs from **24.70%** to **8.70%** between 1988 and 2021.
  * **Trade Volume Expansion:** This liberalization was strongly correlated with a significant expansion of trade volumes. The negative correlation between MFN tariffs and exports was **-0.693**, confirming that as tariffs fell, trade grew.
  * **Tariffs & Economic Growth:** The relationship between tariffs and economic growth was weak and positive, with a correlation of **0.330** (AHS vs. Growth) and **0.232** (MFN vs. Growth). This suggests that other factors beyond tariff policy were the primary drivers of GDP growth.

### License

This project is licensed under the MIT License. See the `LICENSE` file for details.

### Acknowledgements

This project was completed as part of my assignment for the **Exploratory Data Analysis and Visualization (DLBDSEDAV01)** course at **IU International University of Applied Sciences**.
