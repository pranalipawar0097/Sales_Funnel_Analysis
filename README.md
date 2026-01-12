Sales Funnel Analysis using Python

Project Overview
This project analyzes an e-commerce sales funnel to understand how users move
through different stages of the customer journey and where drop-offs occur.
The analysis helps identify bottlenecks that impact conversion rates and
provides actionable business insights.

---

Business Problem
In e-commerce platforms, a large number of users visit the website, but only a
small percentage complete a purchase. Understanding where users drop off in the
sales funnel allows businesses to optimize user experience, improve conversions,
and increase revenue.

---

Dataset
- Source: Kaggle – Sales Funnel User Drop-off Dataset  
- Type: Event-based user activity data  
- Files Used:
  - `home_page_table.csv` – Users visiting the home page
  - `search_page_table.csv` – Users viewing products
  - `payment_page_table.csv` – Users reaching checkout
  - `payment_confirmation_table.csv` – Users completing purchase

Each file represents a different stage of the funnel.

---

Funnel Stages
| Stage Name        | Description                  |
|-------------------|------------------------------|
| Visit             | User visits the home page    |
| Product_View      | User views/searches products |
| Checkout          | User reaches payment page   |
| Purchase          | User completes the purchase |

---

Tools & Technologies
- Python  
- Pandas  
- NumPy  
- Jupyter Notebook  
- Matplotlib (for optional visualization)

---

## 🔍 Methodology
1. Loaded multiple datasets representing funnel stages
2. Assigned a funnel stage label to each dataset
3. Selected only relevant columns (`user_id`, `stage`)
4. Combined all stages into a single dataframe
5. Counted unique users at each funnel stage
6. Calculated stage-wise conversion rates
7. Identified major drop-off points

---

Key Insights
- The **largest drop-off** occurs between **Product View and Checkout**
- Only a small fraction of users who visit the site complete a purchase
- Checkout is the most critical stage for conversion improvement

---

Business Recommendations
- Simplify the checkout process to reduce friction
- Retarget users who viewed products but did not proceed to checkout
- Improve payment UX to increase completed purchases

---

How to Run the Project
1. Clone this repository
2. Ensure all CSV files are in the same directory as the notebook
3. Open `sales_funnel_analysis.ipynb`
4. Run all cells from top to bottom

---

Conclusion
This project demonstrates how Python and Pandas can be used to perform
end-to-end funnel analysis, transform raw event data into insights, and support
data-driven business decisions.
