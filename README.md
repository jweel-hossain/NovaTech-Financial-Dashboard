📊 NovaTech Solutions Ltd — 5-Year Financial Dashboard
Power BI | DAX | Financial Modeling | Data Visualization
🏢 Project Overview
A fully interactive 5-Year Financial Dashboard built in Power BI for NovaTech Solutions Ltd, a technology services company. The dashboard covers 2025–2029 and provides a comprehensive view of financial performance across three core financial statements.
📸 Dashboard Preview
Overview 
Income Statement
Balance Sheet
Cash FlowShow 
📋 Pages & Features
Page 1 — Executive Overview

KPI Cards: Revenue 4.74M | Net Profit 1.57M | Net Margin 32.29% | Net Cash Flow 1.11M
Revenue vs Net Profit Combo Chart
Margin Trend Analysis (Gross vs Net Margin)
Cashflow Breakdown Chart
5-Year Summary with Revenue CAGR 19.49%
Interactive Year Slicer (2025–2029)

Page 2 — Income Statement

KPI Cards: Gross Profit 4.01M | EBIT 2.10M | Total Expenses 1.92M | Corporate Tax 523.85K
Revenue to Net Profit Waterfall Chart
Gross vs Net Margin Trend Line Chart
EBIT vs Net Profit Clustered Column Chart
Detailed Income Statement Breakdown Table

Page 3 — Balance Sheet

KPI Cards: Total Assets 2.04M | Total Liabilities 470.10K | Total Equity 1.57M
Assets Breakdown Stacked Bar Chart
Liabilities vs Equity Chart
Assets, Liabilities & Equity Trend Line Chart
Balance Sheet Breakdown Table

Page 4 — Cash Flow Statement
KPI Cards: Operating CF 1.45M | Investing CF -167.31K | Net CF 1.11M
Cash Flow Breakdown Chart
Net Cash Flow Trend Line Chart
Cash Flow Waterfall Chart
Cash Flow Table with Conditional Formatting
🛠️ Tools & Technologies
ToolPurposePower BI DesktopDashboard DevelopmentDAX25+ Custom MeasuresPower QueryData Transformation & CleaningMicrosoft ExcelData Source
📐 Key DAX Measures
-- Revenue YoY Growth
Revenue YoY % = 
VAR SelectedYear = SELECTEDVALUE('FinancialData'[Year])
VAR ThisYr = CALCULATE(SUM('FinancialData'[Value]), 'FinancialData'[Year] = SelectedYear)
VAR LastYr = CALCULATE(SUM('FinancialData'[Value]), 'FinancialData'[Year] = SelectedYear - 1, REMOVEFILTERS('FinancialData'[Year]))
RETURN DIVIDE(ThisYr - LastYr, LastYr, 0)

-- Revenue CAGR
Revenue CAGR = 
VAR FirstYr = CALCULATE(SUM('FinancialData'[Value]), 'FinancialData'[Year] = 2025, REMOVEFILTERS('FinancialData'[Year]))
VAR LastYr = CALCULATE(SUM('FinancialData'[Value]), 'FinancialData'[Year] = 2029, REMOVEFILTERS('FinancialData'[Year]))
RETURN (POWER(DIVIDE(LastYr, FirstYr, 0), 1.0/4) - 1) * 100
Dashboard Preview section:
![Overview Dashboard](https://github.com/user-attachments/assets/022e724a-30fa-4ad0-8b6a-c2235468c759)
![Income Statement](https://github.com/user-attachments/assets/f2809733-2d86-43f1-b352-ce92767065e6)
![Balance Sheet](https://github.com/user-attachments/assets/a8c10d9c-ef95-4e78-be3f-4b88921b7d9f)
![Cash Flow](https://github.com/user-attachments/assets/25b83c8c-66b5-4edf-bb86-93949b43ab03)
 🎬 Dashboard Demo
[![Watch Demo](https://github.com/user-attachments/assets/022e72
📈 Key Financial Insights
Metric       2025      2029     Growth
Revenue      642K      1.31M    +104%
Net Profit   177K      485K     +174%
Gross Margin 82.5%     85.8%    +3.3pp
Net Margin   27.59%    37%      +9.4pp
Operating CF 163K      645K     +296%
Total Assets 203K      672K     +231%
🎨 Design Highlights
Dark Navy Theme — #0D1B2A background
Color-coded KPI Cards — unique accent per metric
Interactive Year Slicer — filters all visuals simultaneously
Conditional Formatting — negative values in red, positive in green
Consistent Layout — same structure across all 4 pages
 Project Structure
📁 NovaTech-Financial-Dashboard
├── 📊 Financial_Model.pbix       # Power BI Dashboard File
├── 📋 FinancialData.xlsx          # Raw Data Source
└── 📄 README.md                   # Project Documentation
🚀 How to Use
Download Financial_Model.pbix
Open with Power BI Desktop (free download from Microsoft)
Use Year Slicer to filter by year
👨‍💻 About Me
I specialize in building interactive financial dashboards and data visualizations using Power BI and DAX. Available for freelance projects on Fiverr.[https://www.fiverr.com/s/1qG4zq6](https://www.fiverr.com/users/jweel_dataentry/manage_gigs/create-power-bi-dashboard-for-sales-profit-ecommerce-and-finance-analysis/edit)
⭐ If you found this useful, please star the repository!
