# ☁️ Cloud Cost Calculator 

An enterprise-grade cloud infrastructure cost analysis tool — compare AWS, Azure, and GCP pricing in real time with USD ↔ INR conversion.

---

## 🚀 Features

- **Multi-cloud comparison** — AWS, Azure, and GCP side by side
- **Live cost breakdown** — Storage, Compute, and Data Transfer
- **USD ↔ INR conversion** — Live exchange rate via ExchangeRate API (fallback: ₹83)
- **Interactive charts** — Bar chart for storage tier comparison, line chart for real-time analysis
- **Storage tiers** — HOT, COOL, and ARCHIVE pricing for all three providers
- **Time-range analysis** — Weekly, Monthly, and Yearly cost projections
- **Cloud architecture diagram** — Visual overview of Networking → Compute → Storage layers
- **Reset functionality** — One-click restore to default values
- **Glassmorphism UI** — Dark-themed, responsive design with animated particles background

---

## 🧠 How It Works

```
User Input (Storage GB, Compute Hours, Rate, Data Out)
        ↓
Platform Selection (AWS / Azure / GCP)
        ↓
Cost Calculation (Storage + Compute + Data Transfer)
        ↓
Live Exchange Rate Fetch (USD → INR)
        ↓
Chart & Table Update (Chart.js)
        ↓
Displayed Results ($USD / ₹INR)
```

---

## 📁 Project Structure

```
.
├── index.html       # Main UI — layout, sections, chart canvases
├── style.css        # Glassmorphism dark theme, animations, responsive styles
└── script.js        # Pricing logic, chart rendering, currency conversion
```

---

## 💰 Pricing Reference (per GB/month)

| Tier    | AWS      | Azure    | GCP      |
|---------|----------|----------|----------|
| HOT     | $0.023   | $0.0208  | $0.020   |
| COOL    | $0.0125  | $0.0100  | $0.010   |
| ARCHIVE | $0.0024  | $0.0018  | $0.0015  |

| Provider | Data Out (per GB) |
|----------|-------------------|
| AWS      | $0.09             |
| Azure    | $0.087            |
| GCP      | $0.12             |

---

## ⚙️ Setup

No build step required. Just open `index.html` in a browser.

**External dependencies (loaded via CDN):**

- [Chart.js](https://cdn.jsdelivr.net/npm/chart.js) — Charts & visualizations
- [Font Awesome 6.5](https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css) — Icons
- [Google Fonts – Inter](https://fonts.googleapis.com) — Typography
- [ExchangeRate API](https://api.exchangerate-api.com/v4/latest/USD) — Live USD → INR rate

---

## 🖥️ Usage

1. Open `index.html` in any modern browser
2. Select your cloud platform: **AWS**, **Azure**, or **GCP**
3. Enter your configuration:
   - Storage (GB)
   - Compute Hours/Month
   - Compute Cost per Hour ($)
   - Data Out (GB/month)
4. Costs update instantly in both **$USD** and **₹INR**
5. Scroll down to explore:
   - Storage tier comparison table & bar chart
   - Real-time cost analysis with Weekly / Monthly / Yearly toggle

---

## 📊 Sections

| Section | Description |
|---|---|
| Configuration | Input panel + per-platform cost breakdown |
| Architecture Diagram | Visual: Networking → Compute → Storage |
| Storage Cost Comparison | Table + grouped bar chart across all providers |
| Real-Time Storage Analysis | Line chart with duration toggle |

---

## 🔥 Potential Improvements

- Add Reserved / Spot instance pricing tiers
- Export cost report as PDF or CSV
- Support more currencies beyond INR
- Add network ingress cost calculation
- Multi-region pricing support

---

## 🧑‍💻 Author

Built as a frontend cloud cost analysis tool for comparing major cloud providers.

---

## ⭐ Support

If you found this useful:
- Star the repo
- Fork it
- Share it with your team
