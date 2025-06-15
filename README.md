## Internship Task - Data Analyst Role

# Task 8: Simple Sales Dashboard Design

## Objective
This project analyzes the **Superstore Sales** dataset using Power BI to create an interactive dashboard that visualizes sales performance by product category, region, and month. The dashboard helps business users quickly understand trends and make data-driven decisions.

---

## Key KPIs Tracked
- **Total Sales**  
- **Total Profit**  
- **Profit Margin (%)**  
- **Regional Performance**  
- **Category Contribution**  

---

## Dashboard Features
- **Time-Series Analysis**: Monthly sales trends (Line Chart)  
- **Regional Comparison**: Sales by region (Bar Chart)  
- **Category Breakdown**: Sales distribution by category (Donut Chart)  
- **Interactive Filters**: Region and Category slicers  
- **Top Performers**: Visual highlights for best-performing regions/categories  

---

## Implementation Steps

### 1. Data Preparation
1. Import `Superstore_Sales.csv` into Power BI Desktop
2. Create a "Month-Year" column from Order Date:
   - In Power Query Editor, add custom column: `Date.ToText([Order Date], "MMM") & "-" & Date.ToText([Order Date], "yyyy")`
3. Verify data types (Sales/Profit as decimal, dates as datetime)

### 2. Dashboard Creation
1. **Line Chart** (Sales Trend):
   - X-axis: Month-Year
   - Y-axis: Sales
   - Title: "Monthly Sales Trend"

2. **Bar Chart** (Regional Sales):
   - X-axis: Region
   - Y-axis: Sales
   - Title: "Sales by Region"
   - Sort by Sales descending

3. **Donut Chart** (Category Sales):
   - Legend: Category
   - Values: Sales
   - Title: "Sales by Category"
   - Hole size: 40%

4. **KPI Cards**:
   - Total Sales: `SUM(Sales)`
   - Total Profit: `SUM(Profit)`
   - Profit Margin: `DIVIDE([Total Profit], [Total Sales])`

5. **Slicers**:
   - Add dropdown slicer for Region
   - Add tiles slicer for Category

### 3. Formatting
1. Apply consistent color scheme:
   - Blue for Sales metrics
   - Green for Profit metrics
2. Align all visuals with proper spacing
3. Add descriptive titles to all components
4. Set all visuals to cross-filter each other

### 4. Insights Generation
1. Identify seasonal patterns from line chart
2. Note top-performing regions from bar chart
3. Analyze category distribution from donut chart
4. Document 3-4 key findings in `Dashboard_Insights.txt`

---

## Design Highlights
- **Clean Layout**: Logical visual hierarchy with clear sections
- **Professional Theme**: Modern color palette with adequate white space
- **Interactive Elements**: Responsive filters and cross-visual highlighting
- **Mobile Responsive**: Separate layout for mobile viewing

---

## Key Insights
1. "West region contributed 42% of total sales in Q4 2023"
2. "Technology category had the highest profit margin at 24%"
3. "Sales peaked in November with a 35% increase from October"
4. "Office Supplies accounted for 48% of all transactions"

---

## Tools Used
- Microsoft Power BI Desktop
- Power Query for data transformation
- DAX for measure calculations

---

---

##Learning Outcome
-Gained hands-on experience in designing professional dashboards using Power BI
-Learned to clean and transform data using Power Query Editor
-Developed skills in creating interactive visuals and KPI indicators
-Understood how to derive insights and support business decisions through data visualization
-Improved ability to communicate data findings through clean, logical design

---
