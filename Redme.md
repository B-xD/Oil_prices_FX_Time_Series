---

## Key Findings

1. **Universal full-sample cointegration** - Long-run cointegrating relationships 
   confirmed for all four currency pairs when controlling for DXY and VIX

2. **Controls are methodologically essential** - Without DXY and VIX controls, 
   cointegration and asymmetry are substantially underdetected across all periods

3. **Crisis-driven asymmetry** - Both COVID-19 and Russia-Ukraine shocks activate 
   asymmetric oil-exchange rate transmission, with the supply shock generating the 
   most widespread asymmetry (3 of 4 pairs at 1% significance)

4. **Demand vs supply shock heterogeneity** - BRL asymmetry reverses direction 
   completely between COVID (negative shock dominance) and Russia-Ukraine 
   (positive shock dominance), reflecting Brazil's dual role as oil exporter 
   and emerging market

5. **Development level divide** - EUR maintains the strongest and most stable 
   cointegration throughout all periods while emerging economy pairs show more 
   episodic and crisis-dependent patterns

---

## Requirements

```python
# Core libraries
pandas
numpy
yfinance
statsmodels
scipy
matplotlib
seaborn

# Additional
ruptures          # Bai-Perron structural break detection
arch              # GARCH and additional econometric tests
```

Install all dependencies:

```bash
pip install pandas numpy yfinance statsmodels scipy matplotlib seaborn ruptures arch
```

---

## Data Sources

All data downloaded via `yfinance` Python library:

```
| Variable | Ticker | Source |
|---|---|---|
| Brent Crude Oil | BZ=F | Yahoo Finance |
| CAD/USD | CAD=X | Yahoo Finance |
| EUR/USD | EURUSD=X | Yahoo Finance |
| BRL/USD | BRL=X | Yahoo Finance |
| ZAR/USD | ZAR=X | Yahoo Finance |
| DXY | DX-Y.NYB | Yahoo Finance |
| VIX | ^VIX | Yahoo Finance |

*Note: EUR is inverted from USD/EUR to EUR/USD by taking the reciprocal.*

---

## How to Reproduce

1. Clone the repository:
```bash
git clone https://github.com/B-xD/Oil_prices_FX_Time_Series.git
cd Oil_prices_FX_Time_Series
```

2. Install dependencies:
```bash
pip install pandas numpy yfinance statsmodels scipy matplotlib seaborn ruptures arch
```

3. Open and run the notebook:
```bash
jupyter notebook Notebooks/Oil_prices_vs_FX.ipynb
```

4. Run all cells sequentially from top to bottom

*Note: Data is downloaded live from Yahoo Finance. Results may differ slightly 
from thesis figures if Yahoo Finance updates historical data.*

---

## Citation

If you use this code or methodology, please cite:

Manhica, B. A. J. (2026). Estimation of the Relationship between Oil prices and Exchange Rates 
Master's thesis, HSE Saint Petersburg.


## Contact

**Belton Armando Jeremias Manhica**
belton.xd3@gmail.com 
HSE Saint Petersburg
Master's in Data Analytics for Business and Economics

---

## License

This repository is for academic purposes only. 
All rights reserved © 2026 Belton Armando Jeremias Manhica.