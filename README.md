## Project Description  
I analyzed customer response to three sales strategies—Email, Call, and Email+Call—over a six‑week pilot for a new stationery product line. It validates and explores data, defines an efficiency metric, and delivers recommendations to maximize revenue and optimize team effort.


## Business Context  
Pens & Printers, founded in 1984, supplies high‑quality office products to enterprises. In response to evolving buying habits, the team tested three outreach methods over a six‑week pilot:
- **Email**: Two rounds of product launch emails.  
- **Call**: 30‑minute sales calls.  
- **Email + Call**: One email followed by a 10‑minute call.

The goal: identify which method drives the most revenue per customer while balancing team effort.

## Data Description  
The dataset (`data/product_sales.csv`) includes one record per customer, with columns:
- `week` – weeks since launch (0–6)  
- `sales_method` – “Email”, “Call”, or “Email+Call”  
- `customer_id` – unique customer code  
- `nb_sold` – number of new items sold  
- `revenue` – total revenue (USD)  
- `years_as_customer` – tenure since 1984  
- `nb_site_visits` – web visits in last 6 months  
- `state` – shipping location  

## Analysis Steps

1. **Data Validation & Cleaning**  
   - Checked for missing or invalid entries in each column.  
   - Standardized labels and dropped duplicates.  
   - Verified numeric ranges (e.g. non‑negative revenue, weeks 0–6).

2. **Exploratory Data Analysis**  
   - **Single‑variable visuals**: Customer counts by method (bar chart), revenue distribution (boxplot).  
   - **Multi‑variable visuals**: Revenue over time by method (line plot), site visits vs. revenue (scatter).  
   - Documented key insights alongside each plot.

3. **Metric Definition**  
   - **Revenue per Team‑Hour**:  
     \[
       	ext{Revenue per Hour} = rac{	ext{Total Revenue}}{	ext{Avg. Time per Customer}}
     \]  
   - Estimated initial values using known call durations and email effort.

4. **Recommendations**  
   - **Email+Call** yields the highest revenue per customer and solid efficiency.  
   - **Call‑only** delivers strong revenue but is time‑intensive.  
   - **Email‑only** requires minimal effort but drives lower revenue.  
   - Scale Email+Call, monitor Revenue per Hour weekly, segment by tenure.

## Detailed Walkthrough 🚀

### 🔍 1. Project Kickoff
- ✉️ Received the request from Sales Rep & Head of Analytics  
- 📅 Set milestone: deliver written report and slides within 4 weeks  

### 🧹 2. Data Validation & Cleaning
- ✅ Checked every column for missing values  
- 🏷️ Standardized `sales_method` labels (Email, Call, Email+Call)  
- 🔢 Ensured numeric fields were within valid ranges  
- 🗑️ Dropped duplicates and invalid entries

### 🔎 3. Exploratory Data Analysis
- 📊 **Bar chart**: number of customers per method  
- 📦 **Boxplot**: revenue spread across methods  
- 📈 **Line chart**: revenue trend over weeks by method  
- 🔄 **Scatterplot**: site visits vs. revenue  
- 📝 Annotated each chart with key observations (“Email+Call drives early spikes in sales”, etc.)

### 📏 4. Metric Definition
- 🕒 Defined **Revenue per Team‑Hour**  
- 🧮 Calculated initial estimates: 30 min/customer for Call, 10 min+email for Email+Call, minimal for Email

### 💡 5. Key Findings & Recommendations
- ⭐ **Top Method**: Email+Call for best balance of revenue and time  
- 📞 **Call‑only**: high revenue but 30 min/customer  
- ✉️ **Email‑only**: lowest resource but lower returns  
- ▶️ **Next Steps**: scale pilot, monitor weekly, segment by customer tenure

