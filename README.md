# NCAA Dataform Star Schema Project

This repository contains a complete star schema data modeling project using NCAA College Basketball data. The entire project was built on **Google Cloud Platform** using **BigQuery** and **Dataform**.

## 🔍 Project Overview

- Data Source: NCAA College Basketball Statistics
- Tools Used: Dataform (Cloud), BigQuery
- Schema: Star schema with dimension and fact tables
- Modeling Layers: Staging → Dimension/Fact → Views
- Views: Analytical queries answering business-like questions

## 🧱 Star Schema Structure

### Fact Tables
- `fact_players_performance`
- `fact_teams_games_stats`
- `fact_teams_performance`
- `fact_games`

### Dimension Tables
- `dim_players`
- `dim_teams`
- `dim_games`

## 📊 Analytical Views

This project answers the following questions:

1. Which teams had the highest average points per season?
2. Who are the top 10 players by average points?
3. What are the win-loss stats of each team per season?
4. Which teams performed best in tournaments?
5. Who are the most consistent players?
6. How do teams perform in home vs away games?

Each question is answered via a dedicated `.sqlx` view inside the `definitions/views` folder.

## 📁 Project Structure
ncaa-dataform-star-schema/

├── README.md

├── dataform.json

├── package.json

├── creds/

│ └── service_account_key.json

├── definitions/

│ ├── models/

│ │ ├── staging/

│ │ ├── dim/

│ │ └── fact/

│ └── views/


## ⚙️ How to Use

1. Upload `service_account_key.json` in `creds/` to authenticate with GCP.
2. Open the project in Google Dataform (Cloud Workbench).
3. Run all models and views in the `definitions/` directory.

---

**Author:** Ahmet Bartu Tanacan  
**Contact:** [LinkedIn](https://linkedin.com/in/ahmetbartutanacan)



