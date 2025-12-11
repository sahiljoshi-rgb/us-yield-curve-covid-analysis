# US Yield Curve Dynamics During COVID-19 (1975 - 2025)
*A Python-based empirical analysis of Treasury term structure behaviour, recession signals, and macro-financial dynamics.*

---

## Overview

This project explores the behaviour of the U.S. Treasury yield curve from 1975 to 2025, with a specific emphasis on the COVID-19 shock and the 2021 - 2023 monetary tightening cycle. Using data from the Federal Reserve’s FRED API, the analysis investigates:

- Long-term evolution of Treasury yields  
- Recession windows and crisis behaviour  
- Yield curve shapes (normal, flat, inverted)  
- Factor decomposition: level, slope, curvature  
- Bull/bear steepening and flattening  
- Yield curve inversion during tightening phases  
- Relationship between the 10Y - 2Y spread and the S&P 500

---

## Key Concepts

### Yield Curve Factors
- **Level** - parallel shifts across maturities  
- **Slope** - long/short yield differentials (e.g., 10Y - 2Y)  
- **Curvature** - mid-maturity deviations relative to short & long ends  

### Dynamics Observed
- **COVID-19 (2020):** sharp parallel decline, bull steepening  
- **Reopening (2021):** bear steepening driven by inflation expectations  
- **Tightening Cycle (2022 - 2023):** deep inversion, recession signals  

---

## Visuals

### US Treasury Yields (1975 - 2025)
<img width="1013" height="704" alt="image" src="https://github.com/user-attachments/assets/e9394b11-322f-4f22-92df-24755de0013d" />

### 10-Year Treasury Yield During COVID-19 Pandemic
<img width="1005" height="566" alt="image" src="https://github.com/user-attachments/assets/9f92c506-8227-4b07-ad92-fcce2a8dc33b" />

### 10-Year Treasury Yield During the Global Financial Crisis
<img width="1005" height="566" alt="image" src="https://github.com/user-attachments/assets/a4faecdd-6fb0-4019-87d8-478fb27485c1" />

### Pairwise Distribution and KDE of Daily Yield Data (1975-2025)
<img width="2698" height="2789" alt="image" src="https://github.com/user-attachments/assets/41b5c352-8bff-46cf-a671-201fa4593e50" />

### Late-cycle inversion
<img width="1005" height="704" alt="image" src="https://github.com/user-attachments/assets/cce0652b-0cd9-4172-a5f9-2a98606c2e7f" />

### Level, slope, and curvature over time (2018 - present)
<img width="1384" height="984" alt="image" src="https://github.com/user-attachments/assets/b5c8b4ec-f4e5-4a1d-a9b2-8bdb59089303" />

### 3-panel level dynamics
<img width="1584" height="1184" alt="image" src="https://github.com/user-attachments/assets/c3da1fbc-0fa2-44d8-a924-85bbef52369e" />

### Slope dynamics figure
<img width="1784" height="684" alt="image" src="https://github.com/user-attachments/assets/347c0f5f-d2e8-4f05-b529-b93057b38a27" />

### 10Y - 2Y Treasury Spread vs S&P 500 (1975-2025)
<img width="1384" height="684" alt="image" src="https://github.com/user-attachments/assets/cb765888-3e55-4c5c-b17f-55666a847018" />

---

## How to Run the Notebook

### 1. Clone the repository
```bash
git clone https://github.com/sahiljoshi-rgb/us-yield-curve-covid-analysis.git
cd us-yield-curve-covid-analysis
```
### 2. Install Dependencies
``` pip install -r requirements.txt ```

### 3. Launch Jupyter Notebook
``` jupyter notebook notebooks/us-yield-curve-covid-analysis.ipynb ```

### 4. Requirements
```
- pandas
- numpy
- matplotlib
- seaborn
- fredapi
- jupyterlab  (optional)
```

### 5. Data Source Attribution
``` All data is sourced from: FRED (Federal Reserve Economic Data) ```

### 6. Yield series used: 
``` DGS1MO, DGS3MO, DGS6MO, DGS1, DGS2, DGS3, DGS5, DGS7, DGS10, DGS20, DGS30 ```

### 7. Equity index series:
``` SP500 ```

### 8. Data is retrieved programmatically via the fredapi library.
``` Purpose of This Project
- A hands-on learning project in fixed-income analytics
- A replicable research notebook for term-structure studies
- A portfolio piece demonstrating Python, visualization, and macro-financial analysis
- A foundation for future models such as PCA, Nelson–Siegel, and affine term-structure models
```

### 9. License
```
This project is licensed under the MIT License.
```

### 10. Author
Sahil Joshi (LinkedIn: https://www.linkedin.com/in/sahil-joshi-90338a212/)
