<div align="center">
  <h1>Orly Kagan | Data Analyst Portfolio</h1>
  <p><strong>MSc in Information Science & Data Analytics Professional</strong></p>
  
  <a href="https://www.linkedin.com/in/orlikagan/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:orlyka2020@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</div>

---
###  Technical Toolkit
<p align="center">
  <img src="https://img.shields.io/badge/SQL-CC292B?style=flat-square&logo=postgresql&logoColor=white" alt="SQL">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/BigQuery-669DF2?style=flat-square&logo=googlecloud&logoColor=white" alt="BigQuery">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black" alt="Power BI">
</p>
## Featured Data Analytics Projects

<table width="100%">
  <tr>
    <td width="100%" valign="top">
      <h3> E-Commerce Customer Behavior & Multi-Category Funnel Analysis</h3>
      <p><strong>Executive Summary:</strong> Analysed a massive dataset of 2,097,150 user session events (views, cart additions, cart removals, and purchases) spanning 332,902 distinct users over October and November 2019. Built an end-to-end relational data pipeline in SQL Server (SSMS) to join fragmented operational logs, isolate data anomalies, map out drop-off metrics, and evaluate how pricing dynamics and brand equity impact user conversion lifecycles.</p>
      <p> <em>Tools used: T-SQL, Microsoft SQL Server Management Studio (SSMS), Relational Schema Design</em></p>
      
      <!-- Action Buttons for Download and View -->
      <p>
        <a href="https://github.com/Orlikagan/Portfolio/blob/Projects/SQL/SQL%20Project.docx?raw=true"><b>📥 Download Full Project Report (.docx)</b></a> &nbsp;|&nbsp; 
        <a href="https://github.com/Orlikagan/Portfolio/tree/Projects/SQL"><b>📁 Browse Raw SQL Scripts</b></a>
      </p>
    </td>
  </tr>
</table>

<details>
<summary><b> Step-by-Step SQL Architecture & Query Mapping</b></summary>
<br>

The analysis was executed across 5 sequential script files available in the repository folder:

1. **Data Consolidation (`2_Oct_Nov_new table sql.sql`):** Combined isolated daily multi-million row CSV files into a unified operational table using optimal data type casting (e.g., transforming continuous streams to `BIGINT` and raw strings to structured `DATETIME` formats).
2. **Data Cleansing & Integrity Defences (`3_cleaning_brand &update.sql`):** Leveraged staging structures to isolate items linked to multi-brand data corruption anomalies while safely ignoring them to safeguard overall data cleanliness.
3. **Aggregations & Trend Evaluation (`4_Joining table analysis.sql`):** Engineered multi-table `JOIN` functions and Multi-Stage CTEs to calculate Month-over-Month (MoW) revenue growth, identifying an initial revenue shift of **1.56%** between October ($5,566,813) and November ($5,653,876).
4. **Analytical Table Engineering (`5_creating product table.sql`):** Modeled and populated a dedicated analytics table storing aggregated performance metrics per product (`count_views`, `count_purchased`, `% purchased`, `% abandoned`).
5. **Advanced Business Discovery (`6_investigation Product table.sql`):** Implemented Window Functions (`RANK() OVER (PARTITION BY...)`) to extract top 5 trending products per category, trace multi-session users, and capture cart abandonment thresholds.
</details>

<details>
<summary><b> Strategic Business Insights & Conclusions</b></summary>
<br>

* **The Revenue vs. Volume Paradox:** Apple generated the highest total dollar revenue due to premium pricing tiers. However, when evaluating pure volume and customer preference thresholds, Samsung dominated the "electronics.smartphone" category rankings, and budget-friendly Xiaomi registered the single highest continuous purchase count per individual product item (197 units in October vs. 169 in November).
* **Identification of Funnel & System Anomalies:** Identified clear systemic data anomalies where products (e.g., *computers.peripherals.keyboard* from Canyon) registered successful conversions with **0 preceding views**. This signals potential tracking bugs or off-platform direct link sharing behaviors where users bypass the traditional browsing funnel entirely.
* **Friction and Multi-Session Delays:** Deep funnel evaluation revealed that a high percentage of users required multiple distinct active sessions before finalizing a purchase. This highlights a cognitive barrier to conversion, proving that users actively use the shopping cart tool as a temporary consideration deck or wishlist, requiring retargeted marketing campaigns to close the deal.
* **Analytical Limitation Note:** Because the available dataset tracks behavior strictly on the first day of each consecutive month, the findings represent structural snapshots rather than fluid seasonal habits. Broader, continuous data pipelines are recommended to establish accurate long-term forecasting models.
</details>

---
## Featured Projects

<table width="100%">
  <tr>
    <td width="50%" valign="top">
      <h3> E-Commerce Performance & Customer Insights</h3>
      <p><strong>Business Problem:</strong> Conducted a deep-dive analysis on e-commerce transaction patterns to uncover core metrics, seasonal revenue drivers, and user drop-off trends.</p>
      <p>🔧 <em>Tools used: Jupyter Notebook, Python (Pandas, Seaborn), Matplotlib</em></p>
      <a href="./Python/Marketing%20Portfolio.ipynb"><b>📈 View Interactive Notebook</b></a>
    </td>
    <td width="50%" valign="top">
      <h3>🔍 Mobile Location-to-Store Distance Analysis</h3>
      <p><strong>Business Problem:</strong> Evaluated the spatial correlation between user mobile device locations and their proximity to physical retail outlets to target marketing campaigns.</p>
      <p>🔧 <em>Tools used: Google Colab, Python, PowerPoint Presentation</em></p>
      <a href="./Python/"><b>📁 View Source Files</b></a>
    </td>
  </tr>
  
  <tr>
    <td width="50%" valign="top">
      <h3> Relational Database & Advanced SQL Analysis</h3>
      <p><strong>Business Problem:</strong> Engineered data transformations, table definitions, and multi-stage joins to convert messy raw operational data into pristine, report-ready business metrics.</p>
      <p>🔧 <em>Tools used: SQL, Relational Schema Design, Business Report</em></p>
      <a href="./SQL/"><b>🛠️ View SQL Scripts</b></a>
    </td>
    <td width="50%" valign="top">
      <h3> Predictive Analytics / Academic Seminar Work</h3>
      <p><strong>Business Problem:</strong> Brief one-sentence summary of a high-impact university research or advanced analytics project.</p>
      <p>🔧 <em>Tools used: Python, Advanced Statistics</em></p>
      <a href="#"><b> Read Research Summary</b></a>
    </td>
  </tr>
</table>

### Core Analytical Capabilities & Frameworks

<details>
<summary><b>Data Cleaning & Preprocessing Framework</b></summary>
<br>
Whenever handling raw datasets (such as the E-Commerce portfolio project), I follow a strict preprocessing protocol:
1. Identifying and isolating structural anomalies or missing values.
2. Normalizing skewed continuous variables for visualization accuracy.
3. Writing highly performant SQL CTEs to streamline transformations before analytical execution.
</details>

<details>
<summary><b> Business Intelligence & Reporting</b></summary>
<br>
Data is only as valuable as the decisions it drives. I complement my programming work by creating executive presentations (as seen in the Retail Store project) that translate complex data models into clear, actionable business strategies for cross-functional stakeholders.
</details>
