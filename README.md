# 📊 Smart Portfolio Analytics

**Your EU bank has a shit UI but lets you download a CSV file of your portfolio?**

Drop the file here and enjoy a modern look and feel.

![Dashboard Preview](preview.png)

## 🚀 Try It Now

**[Launch the Dashboard →](https://yourusername.github.io/portfolio-analytics/)**

Just drag & drop your bank's CSV export and get instant insights.

---

## ✨ Features

### 📈 Portfolio Overview
- **Total portfolio value** with real-time prices
- **Asset allocation breakdown** — Cash, Bonds, Stocks, ETFs
- **Dividend yield analysis** with estimated annual income
- **Performance comparison** vs EU 60/40 benchmark (60% MSCI Europe / 40% Euro Bonds)

### 💱 Currency Risk Analysis
- **True USD exposure** — not just trading currency, but underlying assets too
  - Your Vanguard S&P 500 ETF trades in EUR but holds USD assets? We account for that.
- **Interactive FX simulator** — see how EUR/USD movements impact your portfolio
- Slide from EUR strengthening to weakening and watch your portfolio value change

### 📉 Risk Metrics
- **Maximum drawdown** with period identification
- **Annualized volatility**
- **Win rate** — percentage of positive months
- **Monthly returns distribution** chart

### 🎯 Scenario Analysis
- **What-if modeling** — "What happens if Alphabet drops 20%?"
- Pick any holding and simulate price changes
- See the impact on your total portfolio instantly

---

## 🔒 Privacy First

**Your data never leaves your browser. Ever.**

### 100% Client-Side
- **No server** = no database = no way to see other users' data
- Each user's CSV **stays in their browser only**
- No data is ever uploaded anywhere
- LocalStorage is sandboxed per user/browser
- When you close the tab, your portfolio data is gone

### 🔑 API Key Security
If you choose to use the Claude API, your key is stored in `localStorage` which is:
- Only accessible by the same origin (this website's URL)
- Never sent to any server except Anthropic's API
- Never visible to other users
- You can reset it anytime with the "Reset Key" button

### No Tracking
- No analytics
- No cookies (except localStorage for your API key preference)
- No third-party scripts that could leak data
- **Open source** — inspect the code yourself

---

## 📁 Supported CSV Formats

Works with Deutsche Bank exports (and similar EU bank formats):

| Format | Columns Used |
|--------|--------------|
| Raw Export | Pot, Assets, Instrument Name, ISIN, Mkt Val, Quantity, Pos Cur |
| Simplified | Category, Product Name, Value (EUR), Currency |

---

## 💡 Data Sources

The dashboard fetches live market data using:

1. **Free APIs (default, no setup needed)**
   - Yahoo Finance — stock & ETF prices
   - Frankfurter API — EUR/USD exchange rate

2. **Claude API (optional, higher quality)**
   - Enter your Anthropic API key for AI-powered data fetching
   - Get it at [console.anthropic.com](https://console.anthropic.com/)

---

## 🛠️ Local Development

No build process needed. Just:

```bash
# Clone the repo
git clone https://github.com/yourusername/portfolio-analytics.git

# Open in browser
open index.html
```

Or simply download `index.html` and double-click it.

---

## 📝 License

MIT — do whatever you want with it.

---

## 🙏 Credits

Built with:
- [React](https://react.dev/) — UI framework
- [Recharts](https://recharts.org/) — Charts
- [Frankfurter API](https://www.frankfurter.app/) — Free FX rates
- [Yahoo Finance](https://finance.yahoo.com/) — Market data

---

**Made with ☕ and frustration at legacy banking UIs**
