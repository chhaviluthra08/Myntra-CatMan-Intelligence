## Myntra Category Intelligence & Seller Health Pipeline

### Overview
This project is a data intelligence pipeline designed to analyze large-scale e-commerce datasets to drive strategic business decisions. Utilizing a dataset of 1.06 million Myntra SKUs, the system identifies "Anchor Products," evaluates seller performance, and pinpoints selection gaps within the catalog. The project demonstrates an AI-First approach to category management by bridging technical data engineering with commercial growth strategies.

---

### Core Objectives
* **Scale Management:** Efficiently process and analyze a high-volume dataset (1M+ rows) to extract actionable commercial insights.
* **Brand Health Audit:** Evaluate seller performance based on customer satisfaction metrics and pricing strategies.
* **Inventory Optimization:** Identify high-potential categories where customer demand (ratings) outweighs current inventory variety (SKU count).
* **Margin Protection:** Analyze discount depth to identify potential margin erosion and optimize pricing structures.

---

### Technical Architecture
The pipeline is modularized into four primary analytical units:
1.  **Data Acquisition:** Automated retrieval and initialization of relational data using KaggleHub and Pandas.
2.  **Demand Identification:** Calculation of a weighted Popularity Score (Rating $\times$ RatingTotal) to define market-leading products.
3.  **Seller Performance Matrix:** Aggregation of multi-dimensional KPIs including average rating, product volume, and mean discount percentage.
4.  **Selection Gap Analysis:** Algorithmic identification of under-served categories with high consumer satisfaction but low SKU density.

---

### Key Business Insights Derived
* **Anchor Identification:** Successfully isolated the top 0.01% of products driving social proof and organic traffic.
* **Seller Segmentation:** Classified partners into High-Volume, Premium-Quality, and Margin-At-Risk segments.
* **Growth Opportunity:** Identified specific category proxies that exhibit high ratings but fall below median price points, suggesting a viable entry point for new D2C brand onboarding.

---

### Technology Stack
* **Language:** Python
* **Data Libraries:** Pandas, NumPy
* **AI Integration:** Gemini API (Strategic Forecasting & Executive Summarization)
* **Environment:** Google Colab / Jupyter Notebook
* **Data Source:** Myntra Products Dataset (1.06M SKUs)

---

### Implementation Instructions
1. Clone the repository or open the notebook in Google Colab.
2. Ensure necessary libraries are installed via pip: `pandas`, `kagglehub`, `google-generativeai`.
3. Configure your Google AI Studio API key for the Strategic Summary module.
4. Execute the cells sequentially to generate the Seller Health and Selection Gap reports.
