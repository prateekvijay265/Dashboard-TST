<div align="center">
  <img src="assets/banner.svg" alt="InsightPulse Dashboard Banner" width="100%" />

  <h1>InsightPulse Executive Dashboard</h1>
  <p><strong>A Modern, Interactive, Data-Driven Analytics Dashboard</strong></p>

  [![Live Demo](https://img.shields.io/badge/Live_Demo-View_Website-6366f1?style=for-the-badge&logo=vercel)](https://dashboard-ten-virid-64.vercel.app/)
  [![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-161d2e?style=for-the-badge&logo=github)](https://github.com/prateekvijay265/Dashboard-TST)

</div>

<br>

## 🌟 Overview

**InsightPulse** is a beautiful, fully responsive executive dashboard designed for modern business analytics. Built with performance and usability in mind, it visualizes complex metrics through an intuitive interface, leveraging glass-morphism aesthetics, fluid animations, and real-time interactive charts.

---

## 📸 Platform Screenshots

<div align="center">
  <h3>📊 Overview Page</h3>
  <img src="assets/overview.png" alt="Overview Analytics" width="90%" style="border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.2);" />
  <br><br>
  
  <h3>👥 Customers Intelligence</h3>
  <img src="assets/customers.png" alt="Customers Page" width="90%" style="border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.2);" />
  <br><br>
  
  <h3>📈 Advanced Analytics</h3>
  <img src="assets/analytics.png" alt="Analytics Page" width="90%" style="border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.2);" />
</div>

---

## 🛠️ How It Works (Architecture & Data Flow)

The dashboard uses a monolithic frontend approach powered by vanilla HTML/CSS/JS and `Chart.js` for data visualization. Here is how the user interacts with the app:

```mermaid
graph TD
    A[User Visits Dashboard] --> B[HTML Skeleton Loads]
    B --> C[CSS Design System Applied]
    C --> D[app.js Initializes]
    
    subscript_1[Navigation Engine]
    subscript_2[Chart.js Render Engine]
    subscript_3[Interactive Elements]
    
    D --> subscript_1
    D --> subscript_2
    D --> subscript_3
    
    subscript_1 --> E{User Clicks Menu}
    E --> |Overview| F[Render KPI & Revenue Charts]
    E --> |Customers| G[Render Geo & Retention Data]
    E --> |Analytics| H[Render Funnel & Forecasts]
    
    subscript_3 --> I[Date Filter & Export Buttons]
    I --> J[Toast Notifications Trigger]
```

### 🧩 Core Components
1. **Navigation Engine (`app.js`)**: A custom-built Vanilla JS router handles page transitions smoothly without reloading the browser. It implements lazy-loading for charts (charts are only instantiated when a user visits that specific page).
2. **Design Tokens (`styles.css`)**: Built entirely on custom CSS properties (`:root`), it maintains a scalable glass-morphic dark theme (`--bg-card`, `--accent`, `--border`).
3. **Data Visualization (`Chart.js`)**: Customized chart instances with complex gradient fills, custom tooltips, and interactive legends.

---

## 🚀 Features by Page

| Page | Key Features | Visualizations |
|------|-------------|----------------|
| **Overview** | High-level metrics, activity heatmap, top transactions. | Animated KPIs, Revenue/Orders Line Chart, Heatmap Grid. |
| **Revenue** | Deep dive into revenue streams. | Channel Bar Chart, Doughnut Split, YoY Quarterly Growth. |
| **Customers** | Demographic & Retention insights. | Cohort Retention Line Chart, Geo Distribution Bars. |
| **Products** | Inventory tracking & product rankings. | Category Bar Chart, Top 10 Dynamic Table. |
| **Analytics** | Forecasts and behavioral patterns. | Conversion Funnel, AI Forecast Chart, Scatter Plot. |

---

## ⚙️ Local Development

Want to run this locally? It's as simple as:

1. **Clone the repo:**
   ```bash
   git clone https://github.com/prateekvijay265/Dashboard-TST.git
   ```
2. **Navigate into the directory:**
   ```bash
   cd Dashboard-TST
   ```
3. **Run a local server** (e.g., using Python, VS Code Live Server, or Node):
   ```bash
   npx serve .
   # OR
   python -m http.server 8000
   ```
4. **Open in browser:** Visit `http://localhost:8000`

---

<div align="center">
  <p>Built with ❤️ for elegant data visualization.</p>
</div>
