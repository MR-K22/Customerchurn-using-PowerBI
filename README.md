# Customer Churn Analysis Power BI Dashboard

## Overview

This project analyzes customer churn for a banking dataset using an interactive Power BI dashboard. Using .csv and .xlsx files (customer info, churn details, demographic/category attributes), the dashboard delivers deep insights into churn rates, customer segmentation, and retention strategies with clear, actionable visualizations.[2][3][4][5][6][7][8][1]

***

## Datasets

- **Bank_Churn.csv:** Main transaction/customer profile dataset (CreditScore, Geography, Gender, Age, Tenure, Balance, Products, Card Usage, Active Status, Salary, Exited, DOJ).[3]
- **CustomerInfo.csv:** CustomerId and Surname mapping for profile enrichment.[4]
- **ActiveCustomer.xlsx:** Active vs. Inactive member mapping.[5]
- **CreditCard.xlsx:** Credit card holder/non-holder category.[6]
- **ExitCustomer.xlsx:** Exit (churned)/Retain categories.[7]
- **Gender.xlsx:** Gender mapping (Male/Female).[8]
- **Geography.xlsx:** Location mapping for segmentation.[4]

***

## Dashboard Features

- **Churn% by Year/Month:** Year-wise, month-wise churn trends visualized with KPIs and conditional formats.[1]
- **Customer Demographics:** Pie charts for Geography, Gender, CreditCard status showing distribution of active, retained, and churned customers.[2]
- **Retention Metrics:** Total, active, retain, inactive, and exit customer counts (Top KPIs).
- **Segmented Analysis:** Ability to filter by Year, Month, Location, Active Status, Cardholding, Exit Status, Gender.[2]
- **Exit Analysis:** Breakdown of exits by month, category, and gender to uncover key churn drivers.
- **Time Series:** Trends of exits vs. previous month exits to spot patterns and alert on anomalies.

***

## Full Process

### 1. Data Preparation

- Clean and preprocess CSV/XLSX data in Power Query.
- Map categorical columns using lookup sheets (ActiveCustomer, CreditCard, ExitCustomer, Gender, Geography).
- Merge datasets and resolve customer IDs across all attribute files for unified analysis.[3][5][6][7][8][4]

### 2. Model Building

- Create relationships in Power BI Model view for easy cross-filtering.
- Establish hierarchies for Date, Geography, and Categories.
- Design calculated columns/measures for churn rates, retention, and segmentation.

### 3. Visualization

- Design dashboard pages using KPI cards, bar charts, pie charts, combo/time series charts, and conditional icons.
- Implement slicers for multi-level drilldown (Year, Month, Geography, Gender, Exit/Active/CC Category).[1][2]
- Apply DAX calculations for advanced metrics and dynamic filtering.

### 4. Interactivity & Insights

- Enable slicers and interactive filtering so users can investigate churn by any dimension.
- Use bookmarks and tooltips for added context and easy navigation.
- Highlight correlation and anomaly points (churn spikes, retention dips, demographic impacts).

### 5. Export & Share

- Export dashboard as Power BI report (.pbix) or publish to Power BI Service/Workspace.
- Include screenshots in the repository for visual reference.[1][2]
- Add README/documentation for user guidance and reproducibility.

***

## Repository Structure

```
├── data/
│   ├── Bank_Churn.csv
│   ├── CustomerInfo.csv
│   ├── ActiveCustomer.xlsx
│   ├── CreditCard.xlsx
│   ├── Geography.xlsx
│   ├── Gender.xlsx
│   ├── ExitCustomer.xlsx
├── dashboard/
│   ├── customerchurn-ss.jpg
│   ├── customerchurn-ss-1.jpg
│   └── (additional visual assets)
├── README.md
└── (PowerBI .pbix file, if sharing source)
```

***

## How to Use

1. Download and open the PowerBI .pbix dashboard.
2. Place all dataset files into the relevant `data/` directory.
3. Update data sources in Power BI to point to local copies (if necessary).
4. Use in-dashboard slicers and visualizations to explore churn patterns by any attribute.

***

## Screenshots

Visual samples are included as evidence of dashboard features and design aesthetics.[2][1]

***

## Credits

- Data and analysis: [Contributor Name]
- Tool: Microsoft Power BI
- Sample Banking Churn Data (CSV/XLSX) and custom mapping sheets.[5][6][7][8][3][4]

***

This README covers the datasets, dashboard features, and full Power BI build process for a professional exploratory churn analytics project with interactive visuals and actionable insights.[6][7][8][3][4][5][1][2]

[1](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/images/68022021/697be799-8184-4813-999d-f6327049633d/customerchurn-ss-1.jpg?AWSAccessKeyId=ASIA2F3EMEYE4ZJUT4YT&Signature=r8bOBJQZaUNYBeGA4u41hOTBe1A%3D&x-amz-security-token=IQoJb3JpZ2luX2VjEKD%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJIMEYCIQDKJvtzh7ZF40GRzbR%2BUKOw%2Fx1ntcpuZj%2BbobInVM0LnAIhAMCvCbT6%2FS%2BGcLr%2B%2FQ9ruYeF0rVy0Vw7gCp7gqpUev%2FHKvEECCgQARoMNjk5NzUzMzA5NzA1Igyk40iuCXX0xgo0fgMqzgSaRL5qi9EIAtCwwRboOF%2BrGSd8aTfaJMQ0NrJ9vid8zc9bwcJSDUpxw107sQvC2reviVzOXSfWfEWSbIjkKZk9ficc3UTs5M0n9z%2Bou0y0fm31uV393FktqY3M%2BQCFAGiJifE%2BFLwIS49AKdRQOJ3MHsAfn0UsBygvIZeqhIv8VzPzsNl2ozmSWR7qfrh0KiTHE12GQZ42dg3O2zKEo4Mtp3EoWDC%2BoktOjy652rVtRrbqRkgS%2BdgusO62lBmnVm8GttJ5dzK9c2UAfh7EFCvVjJpF%2FW3IjUEWof4YLaFjRpLnYdN%2Bpq3g7mck6O26Qlxs9Uj%2F0ZihP%2BwhOSIXygEKsrzYuN%2BLd5Lkae8sOd%2Fyx%2BZTiJiQ6FFxTaOByLV%2FL91NQGiclO7dRjIBgrK%2BQVSzpGxRW8MQZPOhH6XbtzdX6wPIyJO3NlUisF8Pr90U2i7texQwClkGV2hapvnZMZ7adqWDz8d5Iel1xSPTAkODdkokX7mCYvk8MQbhuQGPoAI5AMAuGq8m1519jFduh%2Bwu0tu1879xaewQvgPOGfN6lB9zPwkSwphnsVwAotjRUO6jG6HUOgHuwrigLIEhVPgbPwVBxoDu1XIcxNFrS1PvQbs71zc8AM9lRA5DCkgrsYdJlSMqFoTU48Y%2BaDvac5W69EMwV%2FokkJGrXSqXhkIwTjIqnBZUP8%2Fr%2B%2FSxYB%2BoZrvwnRvCzprKOX%2FUMCyZaZUO4%2Buw8NIn3m%2FXI2NaeoehT071jDNHZC2cShBICG8vmnrqhuQc8aGheyXPqVnpWzDS8cPGBjqZAYLGLaJkgmWsToASidU%2B7kCtumpugwBEnVdvGMLoIF7jUrmEDHkZMdZZucyJqMDfPE9GUnsPkPsEnwGusRsmYKW4RX6cQn0y4J0akI5NLEzyERTsCg9cygoZBVn0G908XedHUZo4Je3dnoW4vuznOF0%2BvHdGia50jXrSj6nCkm77sOOteH%2Bsfu40mdEb0coIpqwNs1vhN8jl6g%3D%3D&Expires=1758527713)
[2](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/images/68022021/e77b349c-ac82-47e3-a951-81efe678c429/customerchurn-ss.jpg?AWSAccessKeyId=ASIA2F3EMEYE4ZJUT4YT&Signature=OPX06uQuUpSrNxaXUupTTQhEa2U%3D&x-amz-security-token=IQoJb3JpZ2luX2VjEKD%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJIMEYCIQDKJvtzh7ZF40GRzbR%2BUKOw%2Fx1ntcpuZj%2BbobInVM0LnAIhAMCvCbT6%2FS%2BGcLr%2B%2FQ9ruYeF0rVy0Vw7gCp7gqpUev%2FHKvEECCgQARoMNjk5NzUzMzA5NzA1Igyk40iuCXX0xgo0fgMqzgSaRL5qi9EIAtCwwRboOF%2BrGSd8aTfaJMQ0NrJ9vid8zc9bwcJSDUpxw107sQvC2reviVzOXSfWfEWSbIjkKZk9ficc3UTs5M0n9z%2Bou0y0fm31uV393FktqY3M%2BQCFAGiJifE%2BFLwIS49AKdRQOJ3MHsAfn0UsBygvIZeqhIv8VzPzsNl2ozmSWR7qfrh0KiTHE12GQZ42dg3O2zKEo4Mtp3EoWDC%2BoktOjy652rVtRrbqRkgS%2BdgusO62lBmnVm8GttJ5dzK9c2UAfh7EFCvVjJpF%2FW3IjUEWof4YLaFjRpLnYdN%2Bpq3g7mck6O26Qlxs9Uj%2F0ZihP%2BwhOSIXygEKsrzYuN%2BLd5Lkae8sOd%2Fyx%2BZTiJiQ6FFxTaOByLV%2FL91NQGiclO7dRjIBgrK%2BQVSzpGxRW8MQZPOhH6XbtzdX6wPIyJO3NlUisF8Pr90U2i7texQwClkGV2hapvnZMZ7adqWDz8d5Iel1xSPTAkODdkokX7mCYvk8MQbhuQGPoAI5AMAuGq8m1519jFduh%2Bwu0tu1879xaewQvgPOGfN6lB9zPwkSwphnsVwAotjRUO6jG6HUOgHuwrigLIEhVPgbPwVBxoDu1XIcxNFrS1PvQbs71zc8AM9lRA5DCkgrsYdJlSMqFoTU48Y%2BaDvac5W69EMwV%2FokkJGrXSqXhkIwTjIqnBZUP8%2Fr%2B%2FSxYB%2BoZrvwnRvCzprKOX%2FUMCyZaZUO4%2Buw8NIn3m%2FXI2NaeoehT071jDNHZC2cShBICG8vmnrqhuQc8aGheyXPqVnpWzDS8cPGBjqZAYLGLaJkgmWsToASidU%2B7kCtumpugwBEnVdvGMLoIF7jUrmEDHkZMdZZucyJqMDfPE9GUnsPkPsEnwGusRsmYKW4RX6cQn0y4J0akI5NLEzyERTsCg9cygoZBVn0G908XedHUZo4Je3dnoW4vuznOF0%2BvHdGia50jXrSj6nCkm77sOOteH%2Bsfu40mdEb0coIpqwNs1vhN8jl6g%3D%3D&Expires=1758527713)
[3](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/68022021/53b545fc-7334-43ea-ae85-975dde17446c/Bank_Churn.csv)
[4](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/68022021/a56408cd-ef30-45b0-bf45-a09c312083d2/CustomerInfo.csv)
[5](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/68022021/29675459-4134-45a1-ab60-19ff5d86625a/ActiveCustomer.xlsx)
[6](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/68022021/39a0d268-42af-4c59-b42b-a77903dd802d/CreditCard.xlsx)
[7](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/68022021/32e907a1-1b36-4011-be62-f25c7bd8903c/ExitCustomer.xlsx)
[8](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/68022021/a140129d-24ad-446f-b3a1-c13cf9e0bdcb/Gender.xlsx)
