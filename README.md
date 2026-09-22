# Groww Web Clone — Stocks Explore

A pixel-accurate, frontend-only desktop clone of the **Groww Stocks → Explore** dashboard. Built with semantic HTML5 and a modular Vanilla CSS architecture, recreating the full design hierarchy, typography, data visualizations, and layout.

---

## 📸 Overview

This project reproduces the Groww Stocks Explore desktop interface (~1366px reference width), featuring a continuous vertical dashboard feed alongside an investments summary and trading tools sidebar.

### Key Sections Recreated

* **Top Header & Navigation**:
  * Primary navigation with Groww branding, search bar with `Ctrl+K` badge, notification bell with unread badge, and user avatar.
  * Secondary navigation bar with active tab indicator (`Explore`) and Terminal button.
  * Live-style indices ticker strip (*NIFTY 50, SENSEX, BANKNIFTY, MIDCPNIFTY, FINNIFTY*) with color-coded positive/negative movements.
* **Primary Dashboard Feed (Left Column)**:
  * **Most Bought Stocks**: 4-column card grid with company branding, market prices, and 1D percentage changes.
  * **Top Movers Today**: Tabbed filter bar (*Gainers, Losers, Volume Shockers*) and index selector (*NIFTY 100*) with tabular data, inline SVG sparklines, and volume figures.
  * **MTF & Intraday Stocks**: Dedicated 4-column card grids for margin trading and intraday opportunities.
  * **Trending Sectors**: Advance/decline market breadth visualization featuring split green/red ratio bars and percentage performance.
  * **ETFs & Bonds**: Categorized ETF cards (*Gold, Silver, International, Nifty 50*), Groww mutual/index ETFs, and Popular Bonds with yield, tenure, and credit ratings.
  * **Market News**: 2×2 card grid with company emblems, price impact tags, headlines, and relative timestamps.
* **Right Sidebar**:
  * **Your Investments**: Portfolio snapshot showing current valuation, 1D returns, total returns, and invested capital.
  * **Products & Tools**: Quick access list (*IPO with open badges, Bonds, ETFs, Intraday Screener, Stocks SIP, MTF, Events Calendar, All Stocks Screener*).
  * **Trading Screens**: Technical strategy cards (*Resistance breakouts, MACD, RSI overbought/oversold*) with custom SVG indicator graphics and sticky positioning.
* **Comprehensive 4-Tier Footer**:
  * Corporate information, Bengaluru headquarters address, Contact Us, social handles, and app download badges.
  * Groww corporate and multi-column Products directory.
  * Directory section with category tabs (*Share Market, Indices, F&O, etc.*) and a 5-column stock index.
  * Regulatory, compliance, and A–Z alphabetical navigation directories.

---

## 🎨 Design System & Tokens

All core styles are centralized in `css/variables.css`:

| Token | Value | Description |
| :--- | :--- | :--- |
| `--color-primary` | `#00d09c` | Groww signature teal/green |
| `--color-primary-dark` | `#00b386` | Primary hover state |
| `--color-primary-subtle` | `#e6f9f5` | Bullish badge background |
| `--color-danger` | `#eb5b3c` | Negative return / Bearish red |
| `--color-danger-subtle` | `#fdeee9` | Bearish badge background |
| `--color-text-title` | `#222222` | Headings and primary titles |
| `--color-text-main` | `#44475b` | Body and table content |
| `--color-text-muted` | `#7c7e8c` | Subtitles, labels, and timestamps |
| `--color-border` | `#eef0f2` | Card borders and divider lines |
| `--font-family` | `'Inter', sans-serif` | Clean geometric grotesque typography |

---

## 📂 Project Structure

```
groww-web-clone/
├── .gitignore            # Git exclusion rules
├── README.md             # Project documentation
├── index.html            # Master semantic HTML structure & SVG graphics
└── css/
    ├── variables.css     # Design tokens (colors, typography, radii, shadows)
    ├── main.css          # Base resets, container, typography, and section headers
    ├── header.css        # Primary navbar, secondary tabs, search bar, and ticker
    ├── cards.css         # Stock cards, ETF cards, bond cards, and news grid
    ├── tables.css        # Top movers table, sparklines, and sector ratio bars
    ├── sidebar.css       # Investments widget, products & tools, and trading screens
    └── footer.css        # 4-tier footer, directory tabs, legal links, and A-Z index
```

---

## 🚀 Getting Started

This is a zero-dependency, static frontend project. No build tools, package managers, or local runtimes are required.

### Option 1: Direct Browser Launch
Simply double-click `index.html` or open it in any modern browser:
```bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
```

### Option 2: Local HTTP Server (Optional)
If you prefer running via a local web server:

```bash
# Using Python 3
python -m http.server 3000

# Using Node (npx)
npx serve .

# Using PHP
php -S localhost:3000
```
Then visit `http://localhost:3000` in your browser.

---

## 🔒 Security & Privacy

* **Zero External Data Transmission**: No client-side telemetry, forms, or network tracking.
* **No Authentication / PII**: No hardcoded API keys, user identifiers, passwords, or personal credentials.
* **Safe External Asset Loading**: Uses standard Google Fonts over HTTPS. All icons and graphical charts are implemented inline using secure, self-contained SVG elements.

---

## 📄 License

This project is created for educational and personal portfolio demonstration purposes. All brand names, logos, and trademarks belong to their respective owners.
