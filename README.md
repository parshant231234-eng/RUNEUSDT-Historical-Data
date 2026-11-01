# RUNEUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **RUNEUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `RUNEUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `74` months
- **Total Candles:** `3,226,646` 1-minute candles
- **Historical Range:** `2020-09-04 06:50:00` to `2026-10-24 23:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
RUNEUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── RUNEUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/RUNEUSDT-Historical-Data/main/1m/2026/11/RUNEUSDT_1m_2026-11.csv"
df = pd.read_csv(url)
print(df.head())
```
