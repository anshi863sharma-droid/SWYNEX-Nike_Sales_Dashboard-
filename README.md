# 👟 Nike | Sales Performance Dashboard

An interactive Power BI dashboard that analyses Nike's sales across Indian cities, product lines and sales channels. It helps answer questions like: *Which region earns the most? Which product line drives revenue? How do sales change month to month?*

## 🛠️ Tools Used

- **Power BI Desktop**: data modelling, DAX measures, visuals
- **Excel / CSV**: source data
- **DAX**: KPI calculations

## 🎛️ Interactive Filters (Slicers)

| Slicer | Purpose |
|---|---|
| **Gender** | Filter by Kids / Men / Women |
| **Product Name** | Filter by shoe model (Air Force 1, Air Jordan, Air Zoom, etc.) |
| **Region** | Filter by city: Bengaluru, Delhi, Hyderabad, Kolkata, Mumbai, Pune |

All visuals update together when a slicer is selected.

## 📊 KPI Cards Using Measures

| KPI | Description |
|---|---|
| **Total Orders** | Number of orders placed |
| **Total Profit Margin** | Profit as a percentage of revenue |
| **Total Revenue** | Total sales value |
| **Total Units Sold** | Total quantity of products sold |
| **Total Profits** | Total profit earned |

## 📈 Visuals Explained

### 1. Monthly Sales Trend (Line Chart)
Shows how revenue changes from January to December. It helps spot peak and low-demand months. For the Kids segment, sales peak around **November**, which suggests a festive-season demand, and dip sharply in **February–March and August**.

### 2. Revenue by Region (Clustered Bar Chart)
Compares revenue across the six cities, sorted in descending order. **Pune (~60K)** and **Delhi (~58K)** lead, followed by Bengaluru. **Mumbai and Hyderabad** contribute the least.

### 3. Product Line Analysis (Clustered Column Chart)
Breaks revenue down by product category. **Lifestyle (~72K)** and **Running (~70K)** are the top performers, while **Soccer and Basketball** contribute the least.

### 4. Total Revenue by Sales Channel (Donut Chart)
Shows the revenue split between the two sales channels. The split is almost even (**51.33% vs 48.67%**), so neither channel dominates, and both are important for the business.

## 💡 Key Insights (Kids Segment)

- Total revenue: **216.46K** from **632 units sold**.
- **Pune and Delhi** together contribute more than 50% of regional revenue.
- **Lifestyle and Running** make up the majority of product-line revenue, so inventory and marketing should focus here.
- Sales channels are almost equally balanced, which suggests there is no need to over-invest in just one channel.
- Strong **November** sales point to a seasonal opportunity for campaigns.

## ⚠️ Data Notes

- Total Profit Margin and Total Profits are currently being reviewed, as the profit values are higher than revenue. The measure logic is being fixed.
- A `(Blank)` value appears in the Monthly Trend because of null dates in the source data.

## 🚀 How to Use

1. Clone or download this repository.
2. Open the `.pbix` file in **Power BI Desktop**.
3. Use the slicers (Gender, Product Name, Region) to explore the data.
4. Click any bar, column or donut slice to cross-filter the other visuals.

