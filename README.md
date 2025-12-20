# 🍔 Food Delivery Performance Analytics BI Dashboard

---

## 📑 Table of Contents

- <a href="#project-overview">📌 Project Overview</a>
- <a href="#project-context">🏢 Project Context</a>
- <a href="#project-objectives">🎯 Project Objectives</a>
- <a href="#target-audience">🔍 Target Audience</a>
- <a href="#business-problems-addressed">🛑 Business Problems Addressed</a>
- <a href="#key-features-\&-visual-insights">💡 Key Features & Visual Insights</a>
- <a href="#data-sources-\&-description">📊 Data Sources & Description</a>
- <a href="#project-lifecycle-\&-technical-workflow">🔄 Project Lifecycle & Technical Workflow</a>
- <a href="#data-modeling-approach">⚙️ Data Modeling Approach</a>
- <a href="#dax-measures-implemented">🧮 DAX Measures Implemented</a>
- <a href="#insight-generation-\&-analysis">🔎 Insight Generation & Analysis</a>
- <a href="#performance-dashboard-metrics">📊 Performance Dashboard Metrics</a>
- <a href="#key-business-takeaways">📈 Key Business Takeaways</a>
- <a href="#tools-\&-technologies">📚 Tools & Technologies Used</a>
- <a href="#conclusion">🔚 Conclusion</a>
- <a href="#future-scope">🚀 Future Scope</a>
- <a href="#best-practices-\&-recommendations">💡 Best Practices & Recommendations</a>
- <a href="#how-to-use-this-project">📦 How to Use This Project</a>
- <a href="#contact">📬 Connect with Me</a>
- <a href="#dashboard-snapshot">🖼️ Dashboard Snapshot</a>

---

## <span id="project-overview">🧩 Project Overview</span>

The Food Delivery Performance Analytics Dashboard is a comprehensive Power BI solution designed to analyze end-to-end food delivery operations. It provides insights into customer behavior, order trends, revenue performance, delivery efficiency, meal periods, and partner contributions. The dashboard enables businesses to track KPIs such as total customers, orders, revenue, average delivery time, and order status distribution, transforming raw operational data into actionable insights for strategic decision-making.

---

## <span id="project-context">🏢 Project Context</span>

The food delivery industry is fast-paced and highly competitive, where operational efficiency, customer satisfaction, and timely deliveries directly impact business success. Companies often struggle with fragmented data across delivery partners, payment modes, and time periods. This project consolidates all critical delivery metrics into a single interactive Power BI dashboard, allowing stakeholders to monitor performance, identify bottlenecks, and optimize delivery operations effectively.

---

## <span id="project-objectives">🎯 Project Objectives</span>

The primary objective of this project is to build a centralized BI dashboard that helps stakeholders:

- Monitor total customers, orders, revenue, and menus.
- Analyze order status distribution (Delivered, Cancelled, Pending, Returned).
- Track revenue trends across months.
- Evaluate delivery time performance.
- Understand customer ordering behavior by meal period and day.
- Compare performance across delivery partners and payment modes.
- Improve operational efficiency and customer satisfaction.

---

## <span id="target-audience">🔍 Target Audience</span>

- **Operations Managers** – To track delivery efficiency and order fulfillment.
- **Business Analysts** – To analyze trends and identify growth opportunities.
- **Marketing Teams** – To plan campaigns based on peak meal periods and days.
- **Product Managers** – To optimize menus and pricing strategies.
- **Leadership Teams** – For high-level performance monitoring and decisions.

---

## <span id="business-problems-addressed">🛑 Business Problems Addressed</span>

- ❌ No unified view of food delivery KPIs.
- ❌ Limited visibility into order cancellations and delays.
- ❌ Difficulty tracking delivery partner performance.
- ❌ Lack of insights into peak ordering times and days.
- ❌ Inability to measure average delivery time effectively.
- ❌ No revenue trend analysis across months.

---

## <span id="key-features-\&-visual-insights">💡 Key Features & Visual Insights</span>

### 1. KPI Cards

- 🟢 **Total Customers** – Unique customers using the platform.
- 🔵 **Total Orders** – Number of orders placed.
- 🟣 **Total Revenue** – Overall earnings from food deliveries.
- 🟠 **Total Menus** – Total menu items available.
- ⏱️ **Average Delivery Time** – Average time taken to deliver orders.

### 2. Order Summary

Doughnut charts showing order distribution:

- ✅ Delivered – Successfully completed orders.
- ❌ Cancelled – Orders cancelled by users or partners.
- ⏳ Pending – Orders yet to be delivered.
- 🔄 Returned – Orders returned due to issues.

### 3. Orders by Meal Period

Doughnut chart highlighting customer ordering patterns:

- 🌅 Morning
- 🌤️ Afternoon
- 🌆 Evening
- 🌙 Night

This helps identify peak demand windows.

### 4. Delivery Partner Performance

Treemap visualization comparing order volumes across:

- Uber Eats
- Swiggy
- Zomato
- Dunzo
- In-house Delivery

### 5. Total Revenue by Month

Line/area chart tracking monthly revenue trends to identify growth and seasonal patterns.

### 6. Orders by Delivery Time

Tabular breakdown of orders based on delivery duration:

| Delivery Time | Quantity | Orders |
|---------------|---------|--------|
| 11–20 Min     | Fast    | Low    |
| 21–30 Min     | Moderate| High   |
| 31–40 Min     | Average | High   |
| 41–50 Min     | Slow    | Medium |
| 50+ Min       | Delayed | High   |

### 7. Orders by Day Name

Horizontal bar chart showing order volume by weekday, identifying peak ordering days.

### 8. Filters & Slicers

- 📅 Month Selector
- 💳 Payment Mode – COD, Online, Wallet

---

## <span id="data-sources-\&-description">📊 Data Sources & Description</span>

- **Orders Dataset** – Order ID, customer, status, delivery time, revenue.
- **Customer Dataset** – Customer details and ordering behavior.
- **Delivery Partner Dataset** – Partner-wise order fulfillment.
- **Payment Dataset** – Payment modes used.
- **Date Dataset** – Month and day analysis.
- **File Format** – CSV / Excel.
- **Data Cleaning** – Handled using Power Query.

---

## <span id="project-lifecycle-\&-technical-workflow">🔄 Project Lifecycle & Technical Workflow</span>

- Requirement Gathering
- Data Collection & Understanding
- Data Cleaning & Transformation (Power Query)
- Data Modeling & Relationships
- DAX Measure Creation
- Dashboard UI Design
- Visual Development
- Insight Generation & Optimization

---

## <span id="data-modeling-approach">⚙️ Data Modeling Approach</span>

- **Schema Type** – Star Schema
- **Fact Table** – Orders
- **Dimension Tables** – Customers, Delivery Partners, Date, Payment Mode
- **Relationships** – One-to-many for optimal performance

---

## <span id="dax-measures-implemented">🧮 DAX Measures Implemented</span>

- **Total Customers** = `DISTINCTCOUNT(Customer\_ID)`
- **Total Orders** = `COUNT(Order\_ID)`
- **Total Revenue** = `SUM(Revenue)`
- **Average Delivery Time** = `AVERAGE(Delivery\_Time)`
- **Delivered Orders %** = `DIVIDE(\[Delivered Orders], \[Total Orders])`

---

## <span id="insight-generation-\&-analysis">🔎 Insight Generation & Analysis</span>

- Analyzed peak ordering times and days to optimize staffing.
- Correlated delivery time with cancellation rates.
- Evaluated delivery partner performance for strategic partnerships.
- Identified high-demand menu items by meal period.

---

## <span id="performance-dashboard-metrics">📊 Performance Dashboard Metrics</span>

| Metric | Value | Insight |
|--------|-------|---------|
| Total Orders | 12,450 | High activity during weekends |
| Total Customers | 5,620 | Repeat orders indicate loyalty |
| Average Delivery Time | 28 mins | On-time delivery 85% |
| Delivered Orders % | 92% | Strong operational efficiency |
| Revenue | $245,000 | Monthly growth of 15% |

---

## <span id="key-business-takeaways">📈 Key Business Takeaways</span>

- ✅ Majority of orders are successfully delivered.
- ✅ Morning and afternoon periods generate the highest demand.
- ✅ Certain weekdays outperform others in order volume.
- ✅ Longer delivery times lead to higher cancellation risk.
- ✅ Online payments dominate over COD.
- ✅ Top delivery partners contribute the majority of orders.

---

## <span id="tools-\&-technologies">📚 Tools & Technologies Used</span>

- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- CSV / Excel Files
- Star Schema Data Modeling

---

## <span id="best-practices-\&-recommendations">💡 Best Practices & Recommendations</span>

- Maintain centralized data for real-time updates.
- Optimize delivery routes using peak-time insights.
- Track high-demand items for inventory planning.
- Monitor partner performance monthly.
- Use dashboard insights for marketing campaigns.

---

## <span id="conclusion">🔚 Conclusion</span>

The Food Delivery Performance Analytics Dashboard provides a holistic view of delivery operations, enabling stakeholders to:

- Improve delivery efficiency
- Reduce cancellations and delays
- Optimize partner performance
- Enhance customer satisfaction
- Drive data-driven business decisions

---

## <span id="future-scope">🚀 Future Scope</span>

- 🔮 Delivery time prediction using ML
- 📍 Geo-mapping of delivery locations
- 👥 Customer segmentation & loyalty analysis
- 📊 Real-time dashboard integration
- 📦 Rider performance and SLA tracking

---

## <span id="how-to-use-this-project">📦 How to Use This Project</span>

1. Clone or download the repository
2. Open the `.pbix` file in Power BI Desktop
3. Load your dataset or use sample data
4. Interact with filters and visuals

---

## <span id="contact">📬 Connect with Me</span>

<!-- Typing Animation / 🤝 Connect with me -->
[![Typing SVG](https://readme-typing-svg.herokuapp.com?color=0DAD8D&lines=Let’s+connect+and+collaborate+on+meaningful+projects!;Reach+me+via+X,+LinkedIn,+GitHub,+Email+or+my+Website+🌐;Click+the+buttons+below+to+connect+with+me+directly!)](https://git.io/typing-svg)

<div align="center">
<!-- ✖️ X -->
<a href="https://x.com/rajeevtiwariRT" target="_blank">
  <img src="https://cdn-icons-png.flaticon.com/512/5969/5969020.png" alt="X" width="30" height="30">
</a>
<!-- 💼 LinkedIn -->
<a href="https://www.linkedin.com/in/rajeev-tiwari123"><img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" width="25" height="25"/></a>
<!-- 🆔 GitHub -->
<a href="https://github.com/rajeevgit8055hub" target="_blank">
  <img src="https://cdn-icons-png.flaticon.com/512/733/733553.png" alt="GitHub" width="30" height="30">
</a>
<!-- 📮 Gmail -->
<a href="mailto:rajeevtiwari8055@gmail.com" target="_blank">
<img src="https://cdn-icons-png.flaticon.com/512/732/732200.png" alt="Email" width="30" height="30">
</a>
<!-- 🌐 Website -->
<a href="https://rajeevgit8055hub.github.io/rajeevtiwari.github.io/" target="_blank">
  <img src="https://cdn-icons-png.flaticon.com/512/841/841364.png" alt="Website" width="30" height="30">
</a>
</div>

<!-- ⭐💫 Shower stars if you like my repos -->
<div align="center">
<img src="https://media.giphy.com/media/ObNTw8Uzwy6KQ/giphy.gif" width="30">
<a href="https://github.com/rajeevgit8055hub/rajeevgit8055hub" alt="GitHub Stars" title="Star my repositories">
<img src="https://img.shields.io/badge/Shower_stars_if_you_like_my_repositories-15k?style=for-the-badge&color=f9c513&logo=github&logoColor=black"/>
</a>
</div>

🤝 *Thanks for visiting my profile!*  

If you find this repository valuable, consider giving it a **Star** ⭐ on GitHub to support my work.  

<img src="https://img.shields.io/badge/Thanks_for_visiting_my_profile!-Welcome 🤝-style=for-the-badge&color=0d1117&logo=github&logoColor=white"/>

<img src="https://img.shields.io/badge/If_you_like_this_repo-Give_it_a_Star ⭐-style=for-the-badge&color=f9c513&logo=github&logoColor=black"/>

<img src="https://img.shields.io/badge/Thanks_for_visiting-My_GitHub_Profile 🤝-style=for-the-badge&color=24292e&logo=github"/>

<img src="https://img.shields.io/badge/Support_my_work-Star_the_repo ⭐-style=for-the-badge&color=f9c513&logo=github&logoColor=black"/>

<img src="https://img.shields.io/badge/If_you_find_this_repository_valuable-Consider_giving_it_a_Star ⭐_to_support_my_work-style=for-the-badge&color=f9c513&logo=github&logoColor=black"/>

<img src="https://img.shields.io/badge/If_you_find_this_repository_valuable-Consider_giving_it_a_Star ⭐_to_support_my_work-style=for-the-badge&color=f9c513&logo=github&logoColor=black"/>

<img src="https://img.shields.io/badge/Thanks_for_visiting_my_profile!-🤝-style=for-the-badge&color=0DAD8D"/>

<img src="https://img.shields.io/badge/Thanks_for_visiting_my_profile!-🤝-style=for-the-badge&color=0DAD8D&logo=github&logoColor=white"/>

<img src="https://img.shields.io/badge/If_you_find_my_work_valuable-Please_consider_giving_a_Star ⭐-style=for-the-badge&color=f9c513&logo=github&logoColor=black"/>

<img src="https://img.shields.io/badge/If_you_find_my_work_valuable-Please_consider_giving_a_Star ⭐-style=for-the-badge&color=f9c513&logo=github&logoColor=black"/>

<img src="https://img.shields.io/badge/Support_my_work-Give_it_a_Star ⭐-style=for-the-badge&color=f9c513&logo=github&logoColor=black"/>

<img src="https://img.shields.io/badge/Support_my_work-⭐_Star_on_GitHub-style=for-the-badge&color=0DAD8D&logo=github&logoColor=white"/>

---

## <span id="dashboard-snapshot">🖼️ Dashboard Snapshot</span>

_Above: A snapshot of the Food Delivery Performance Analytics dashboard showcasing KPIs, order insights, delivery efficiency, and revenue trends._

🗂️ Project Preview Snapshot

![Food Delivery Project Preview](Food%20Delivery.webp)

🖥️ Dashboard View

![Food Delivery Project Preview](Final%20Dashboard.png)

---
