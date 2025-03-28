# Nobel Prize Data Analysis and Exploration (1901-2024)

Inspired by Nobel winner Han Kang, this project explores over a century of Nobel Prize data (1901-2024) to uncover trends among laureates. Data from multiple sources was acquired, cleaned, and merged using Python (`pandas`), then loaded into a MySQL database. This project aims to provide a comprehensive analysis of Nobel Prize laureates and awards. The analysis focuses on identifying trends, distributions, and interesting patterns, **with a specific lens on the achievements of women Nobel Prize winners**, within the data.

## Data Sources

* **Historical (1901-2023):** Harvard Dataverse - [Link to Harvard Dataset, e.g., https://doi.org/10.7910/DVN/28207] (CSV)
* **Recent (2023-2024):** Nobel Prize Official Website ([https://www.nobelprize.org/](https://www.nobelprize.org/)) - Manually compiled using Excel.
## Tech stack & Workflow

* **Tools:** Python (`pandas`), Microsoft Excel, MySQL, MySQL Workbench, VS Code.
* **Workflow Summary:** Data acquired -> Cleaned & Merged (Python) -> Loaded into MySQL DB (Workbench) -> Validated & Analyzed (mySQLn in VS code).

## Validation, Analysis & Code
Extensive data validation was performed using SQL to ensure integrity and consistency, including checks for duplicates, value ranges, unique constraints, and standardization of fields like `birth_country`.

Subsequent SQL analysis explored various aspects:
* Laureate demographics (gender, birth country distribution).
* Trends in female representation over decades.
* Prize distribution across categories.
* Identification of multiple prize winners (individuals and organizations).
* Patterns in prize sharing over time.

## Data processing:
*[`Data processing`](./link1.sql)*

## Database schema:
| Field                | Type          | Null | Key | Default | Extra |
| :------------------- | :------------ | :--- | :-- | :------ | :---- |
| `year`               | `int`         | YES  |     | NULL    |       |
| `category`           | `varchar(500)`| YES  |     | NULL    |       |
| `prize`              | `varchar(500)`| YES  |     | NULL    |       |
| `motivation`         | `varchar(500)`| YES  |     | NULL    |       |
| `prize_share`        | `varchar(500)`| YES  |     | NULL    |       |
| `laureate_type`      | `varchar(500)`| YES  |     | NULL    |       |
| `full_name`          | `varchar(500)`| YES  |     | NULL    |       |
| `birth_date`         | `varchar(500)`| YES  |     | NULL    |       |
| `birth_city`         | `varchar(500)`| YES  |     | NULL    |       |
| `birth_country`      | `varchar(500)`| YES  |     | NULL    |       |
| `sex`                | `varchar(500)`| YES  |     | NULL    |       |
| `organization_name`  | `varchar(500)`| YES  |     | NULL    |       |
| `organization_city`  | `varchar(500)`| YES  |     | NULL    |       |
| `organization_country`| `varchar(500)`| YES  |     | NULL    |       |
| `death_date`         | `varchar(500)`| YES  |     | NULL    |       |
| `death_city`         | `varchar(500)`| YES  |     | NULL    |       |
| `death_country`      | `varchar(500)`| YES  |     | NULL    |       |


## SQL scripts for data validation and exploratory analysis:
- *[`Data validation`](./link2.sql)*
- *[`EDA`](./link3.sql)*


