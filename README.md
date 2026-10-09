# 🍱 Food Waste Redistribution System – MYSQL Database Project

**SQL | MySQL |  Relational  Database Design | ER Modeling |Data management | Social Impact | stored Procedures**


\


## 🌟 1. Project Overview

Welcome to my **Food Waste Redistribution System – Data Analytics Project**.

This project focuses on analyzing food donations, managing surplus food inventory, tracking collection centers, and understanding food distribution to recipients using MySQL and SQL queries.

The project demonstrates how database management and data analytics can help identify food distribution gaps, monitor inventory, compare donor contributions, and support better decisions for reducing food waste.

### 🎯 Project Objectives

- Maintain organized records of donors, donations, food items, and collection centers.
- Track food distribution to recipients.
- Analyze donated and distributed food quantities.
- Identify food items at risk of expiry.
- Compare collection-center capacity and stock levels.
- Generate meaningful insights using SQL queries, charts, and an ER diagram.

## 📊 2. Project Highlights

| Area              | Details                                                      |
| ----------------- | ------------------------------------------------------------ |
| Project           | Food Waste Redistribution System                             |
| Domain            | Data Analytics and Database Management                       |
| Database          | MySQL                                                        |
| Relational Tables | 8                                                            |
| Total Donated     | 1,250 units                                                  |
| Total Distributed | 360 units                                                    |
| Distribution Rate | 28.8%                                                        |
| SQL Analysis      | 30 queries, including one view, plus 2 stored procedures     |
| Documentation     | PowerPoint presentation, ER diagram, SQL queries, and charts |

*Note: Figures represent the sample project data, not real-world operational statistics.*

## 🚀 3. Problem Statement

Food businesses such as restaurants, hotels, catering services, and supermarkets may have surplus food while charities and communities need food assistance.

Without an organized system, surplus food can remain unused, expire, or be wasted. At the same time, recipients may not receive sufficient supplies.

This project uses a relational database and SQL analytics to organize food donation records, monitor available stock, track distributions, and identify opportunities to improve redistribution.

### 💡 Proposed Solution

The system connects donors, food donations, collection centers, volunteers, food inventory, and recipients through a structured MySQL database.

SQL queries generate reports that help users understand:

- Which donors contribute the most food.
- Which food categories have the highest stock.
- Which collection centers have limited capacity remaining.
- How much food each recipient receives.
- Which food items require priority distribution because of approaching expiry dates.

## 🛠️ 4. Technology Stack

| Technology                     | Purpose                                            |
| ------------------------------ | -------------------------------------------------- |
| MySQL                          | Relational database management                     |
| SQL                            | Data insertion, retrieval, filtering, and analysis |
| ER Modeling                    | Database entities and relationships                |
| MySQL Workbench / MySQL Client | Database development and query execution           |
| Charts                         | Visual comparison of project data                  |
| PowerPoint                     | Project explanation and presentation               |
| GitHub                         | Project documentation and version control          |

## 📁 5. Repository Structure

```text
Food-Waste-Redistribution-System/
│
├── README.md
├── Food_Waste_Redistribution_Analytics.pptx
├── SQL_Queries.txt
├── ER_Diagram.png
│
└── charts/
    ├── donor_contributions.png
    ├── food_item_donations.png
    ├── category_stock.png
    ├── center_capacity.png
    └── recipient_distribution.png
```

### 📂 File Description

- **README.md:** Project introduction, database explanation, analytical insights, and documentation.
- **Food_Waste_Redistribution_Analytics.pptx:** Complete 19-slide project presentation.
- **SQL_Queries.txt:** SQL table definitions, sample data, analytical queries, view, and stored procedures.
- **ER_Diagram.png:** Visual representation of database entities and their relationships.
- **charts/:** Individual charts used to present the analytical findings.

*Upload these files and folders to your GitHub repository using the same filenames and folder structure. The images below will display after the corresponding files are uploaded.*

## 🗂️ 6. Entity–Relationship (ER) Diagram

The ER diagram represents the relational database structure and explains how food donation and distribution records are connected.



### Main Database Entities

| Entity               | Description                                                            |
| -------------------- | ---------------------------------------------------------------------- |
| DONORS               | Stores donor information                                               |
| DONATIONS            | Records food donations, quantities, and dates                          |
| FOOD_ITEMS           | Stores food stock, category, expiry date, and status                   |
| COLLECTION_CENTERS   | Maintains collection-center details and capacity                       |
| VOLUNTEERS           | Stores volunteer details and center assignments                        |
| RECIPIENTS           | Maintains recipient organization information                           |
| DISTRIBUTIONS        | Records food distribution events                                       |
| DISTRIBUTION_DETAILS | Records individual food items and quantities included in distributions |

### 🔗 Relationships

- One donor can make multiple donations.
- Donation records connect donors with donated food.
- Collection centers are associated with stored food items and volunteers.
- A recipient can receive multiple distributions.
- A distribution can include multiple food items through `DISTRIBUTION_DETAILS`.

Primary keys and foreign keys help maintain relationships between the database tables.

## 📈 7. Data Visualization and Analysis

The charts make it easier to understand donation patterns, food inventory, center capacity, and recipient distribution.

### 7.1 Donor Contributions



This chart compares the total quantity contributed by each donor.

**Key insight:** Fresh Bites Restaurant and Annapurna Catering each contributed 300 units in the sample dataset.

### 7.2 Food Item Donations



This chart compares the quantities associated with different food items and helps identify major contributors to the inventory.

### 7.3 Food Category Analysis



This chart compares stock quantities across food categories.

**Key insight:** Grains account for 800 units, representing approximately 44.4% of the 1,800 units of food stock recorded in the sample data.

### 7.4 Collection Center Capacity



This chart compares stock levels with the capacity of collection centers.

**Key insight:** Central Food Center is operating at 80% of its recorded capacity, while Community Food Hub is at 36.7%.

### 7.5 Recipient Distribution



This chart compares the quantities distributed to recipient organizations.

**Key insight:** Care Children Center received 90 units, the largest individual quantity among the recipients in the sample data.

## 🧮 8. SQL Analysis and Methodology

The project uses SQL concepts at basic, intermediate, and advanced levels.

### Basic SQL

- `CREATE DATABASE` and `CREATE TABLE`
- `INSERT INTO`
- `SELECT`
- `WHERE`
- `COUNT()`, `SUM()`, `AVG()`, `MIN()`, and `MAX()`

### Intermediate SQL

- `INNER JOIN`
- `LEFT JOIN`
- `GROUP BY`
- `HAVING`
- `ORDER BY`
- `LIMIT`

### Advanced SQL

- Subqueries
- `NOT IN`
- Views for reusable reports
- Stored procedures with parameters
- Primary-key and foreign-key constraints

These techniques support reporting, donor comparisons, stock analysis, center-capacity analysis, and recipient distribution reports.

## 📌 9. Key Analytical Findings

### Donation and Distribution

- Total donated quantity: **1,250 units**
- Total distributed quantity: **360 units**
- Distribution rate: **28.8%**
- Difference between donated and distributed quantities: **890 units**

The 890-unit difference is a gap between the recorded donation and distribution totals. It should not automatically be interpreted as verified current stock because the database needs stock reconciliation.

### Inventory and Expiry

Milk, Vegetable Curry, Bread, and Fruits are identified as priority items in the sample expiry analysis.

An expiry-first distribution strategy and automatic expiry alerts could help reduce avoidable food waste.

### Collection Center Management

Central Food Center has the highest recorded capacity utilization at 80%.

Community Food Hub has the lowest utilization at 36.7% and only one assigned volunteer in the sample data.

### Recipient Analysis

Care Children Center received the largest recorded quantity among the five recipients. Recipient-level reports help identify distribution patterns and potential opportunities to improve coverage.

## ⚠️ 10. Current Limitations

The current version is primarily a database and analytics project rather than a complete live redistribution application.

- Food inventory is not automatically reduced when a distribution is recorded.
- Automated expiry notifications are not implemented.
- Recipient requests and automated donor-recipient matching are not implemented.
- Pickup tracking and food-quality verification need additional tables and workflows.
- Further validation rules, role-based permissions, and audit logs are needed.

## 🔮 11. Future Enhancements

### Phase 1: Database Improvements

- Add inventory-update triggers or transactions.
- Introduce automated expiry alerts.
- Add request, pickup, and verification tables.
- Improve data validation and indexing.

### Phase 2: Application Development

- Build a web or mobile application.
- Develop a REST API.
- Introduce role-based login for donors, NGOs, and volunteers.
- Add SMS or WhatsApp notifications.
- Develop dashboards using Power BI or Tableau.

### Phase 3: Intelligent Redistribution

- Add location-based pickup routing.
- Explore machine learning for food-demand forecasting.
- Introduce QR-code-based distribution verification.
- Consider cold-chain temperature monitoring.
- Support expansion across multiple cities.

## 🖥️ 12. PowerPoint Presentation – Slide-by-Slide Explanation

The accompanying presentation contains 19 slides. Each slide covers a specific part of the project.

| Slide | Topic                              | Explanation                                                                                       |
| ----- | ---------------------------------- | ------------------------------------------------------------------------------------------------- |
| 1     | Project Title                      | Introduces the Food Waste Redistribution Analytics project.                                       |
| 2     | Why This Project Matters           | Explains the food waste problem and its social and environmental impact.                          |
| 3     | Project Overview                   | Describes how food moves from donors to recipients.                                               |
| 4     | Database Architecture              | Introduces the relational schema and ER model.                                                    |
| 5     | Technology Stack                   | Explains MySQL, SQL, ER modeling, constraints, and stored procedures.                             |
| 6     | Database Implementation            | Introduces the implementation details of the database.                                            |
| 7     | Donor Analysis                     | Compares the contributions of different donors.                                                   |
| 8     | Donation and Distribution Analysis | Examines donation records and distribution quantities.                                            |
| 9     | Inventory Analysis                 | Explores food stock and distribution-related data.                                                |
| 10    | Category Analysis                  | Compares stock across food categories.                                                            |
| 11    | Collection Center Analysis         | Examines capacity utilization and volunteer assignments.                                          |
| 12    | Recipient Analysis                 | Compares the quantities received by recipient organizations.                                      |
| 13    | Distribution Performance           | Highlights the distribution rate and the gap between donated and distributed quantities.          |
| 14    | Expiry Risk                        | Identifies food items requiring priority distribution.                                            |
| 15    | SQL Analytical Methodology         | Explains basic, intermediate, and advanced SQL techniques.                                        |
| 16    | Current Limitations                | Describes missing automation, validation, security, and tracking features.                        |
| 17    | Future Improvements                | Presents the three-phase improvement roadmap.                                                     |
| 18    | Strategic Outlook                  | Summarizes recommendations for expiry management, center balancing, and distribution improvement. |
| 19    | Conclusion                         | Summarizes the database, analytical insights, and future development opportunities.               |

*For the exact implementation and findings, refer to the presentation and `SQL_Queries.txt` file.*

## ▶️ 13. How to Run the Project

1. Install MySQL Server or use an existing MySQL environment.
2. Open MySQL Workbench or a MySQL command-line client.
3. Open `SQL_Queries.txt`.
4. Execute the database creation and table creation statements.
5. Insert the sample records.
6. Run the analytical SQL queries.
7. Review the results and compare them with the charts.
8. Open the PowerPoint presentation to understand the complete project.

## 🎓 14. Learning Outcomes

Through this project, I practiced:

- Relational database design.
- ER diagram creation and relationship mapping.
- SQL queries and data aggregation.
- Multi-table joins and subqueries.
- Views and stored procedures.
- Data interpretation and chart-based reporting.
- Identifying operational gaps and proposing improvements.
- Documenting a technical project for GitHub.

## 🌍 15. Conclusion

The Food Waste Redistribution System demonstrates how MySQL and SQL analytics can organize food donation and distribution records and uncover actionable insights.

The project establishes a database foundation for donor tracking, food inventory management, collection-center monitoring, and recipient analysis. Future improvements can introduce inventory automation, expiry alerts, recipient requests, and intelligent redistribution.

The ultimate goal is to support a more organized, transparent, and efficient approach to surplus food redistribution.

## 👩‍💻 Author

**Project:** Food Waste Redistribution System – Data Analytics

**Focus Areas:** SQL | MySQL | Data Analytics | Database Design | Data Visualization

**Repository:** [Food Waste Redistribution System](.)

---

⭐ If you find this project useful, feel free to explore the SQL queries, ER diagram, charts, and PowerPoint presentation.

