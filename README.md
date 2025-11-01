# Predicting-Startup-Acquisition-and-Machine-Learning-Pipeline

This project aims to predict the outcome of startups (Operating, IPO, Acquired, or Closed) using supervised machine learning. The project includes an end-to-end pipeline for data preprocessing, model training, evaluation, and deployment.

## Data:

## Link to raw data(Huge JSON and Excel fiel):
           https://drive.google.com/file/d/1tWYkHYHm2HoiCajZ49Cs1K7sklWTdAbV/view?usp=sharing

---

### 📘 **Startup Acquisition Dataset – Variable Dictionary**

| **Variable Name**           | **Definition** |
|----------------------------|----------------|
| `id`                       | Unique identifier for each startup record. |
| `Unnamed: 0.1`             | Likely an unnecessary index column generated during CSV export. Can be dropped. |
| `entity_type`              | Type of entity (e.g., company, investor, school, etc.). |
| `entity_id`                | Unique internal ID associated with the entity. |
| `parent_id`                | ID of the parent company if the startup is a subsidiary. |
| `name`                     | Official name of the startup. |
| `normalized_name`         | Lowercase or standardized version of the startup name (used for matching/search). |
| `permalink`                | URL-friendly version of the startup name for web referencing. |
| `category_code`           | Industry or sector the startup belongs to (e.g., fintech, edtech, healthcare). |
| `status`                   | Current status of the startup – Operating, Acquired, IPO, or Closed. |
| `founded_at`               | Date the startup was founded. |
| `closed_at`                | Date the startup shut down (if applicable). |
| `domain`                   | Domain name of the startup's website (e.g., example.com). |
| `homepage_url`            | URL of the startup’s homepage. |
| `twitter_username`        | Twitter handle of the startup. |
| `logo_url`                 | URL linking to the startup’s logo. |
| `logo_width`               | Width of the startup's logo image. |
| `logo_height`              | Height of the startup's logo image. |
| `short_description`       | Brief description or tagline for the startup. |
| `description`              | Longer form of the startup’s mission or business details. |
| `overview`                 | Comprehensive overview of the startup’s operations, mission, and market. |
| `tag_list`                 | Comma-separated tags or keywords associated with the startup. |
| `country_code`             | 2-letter ISO country code where the startup is based (e.g., US, IN, UK). |
| `state_code`               | State or province code within the country. |
| `city`                     | City where the startup is headquartered. |
| `region`                   | Geographic region or area of operation. |
| `first_investment_at`     | Date of the first investment received. |
| `last_investment_at`      | Date of the most recent investment. |
| `investment_rounds`       | Number of investment rounds the startup has gone through. |
| `invested_companies`      | Count of companies this startup has invested in (if it acts as an investor). |
| `first_funding_at`        | Date the startup received its first funding round. |
| `last_funding_at`         | Date the startup received its most recent funding round. |
| `funding_rounds`          | Total number of funding rounds. |
| `funding_total_usd`       | Total funding amount received in USD. |
| `first_milestone_at`      | Date of the first milestone achieved (e.g., launch, exit). |
| `last_milestone_at`       | Date of the most recent milestone achieved. |
| `milestones`              | Number of key milestones achieved. |
| `relationships`           | Number of known professional relationships or founders, board members, etc. |
| `created_by`              | ID or name of the user/system that created the record. |
| `created_at`              | Date the record was created in the database. |
| `updated_at`              | Date the record was last updated. |
| `lat`                     | Latitude coordinate of the startup’s location. |
| `lng`                     | Longitude coordinate of the startup’s location. |
| `ROI`                     | Return on Investment – profit ratio indicator (if provided or calculated). |

---

## Project Details:

- **Problem Statement**: Predict whether a startup will operate, go for an IPO, be acquired, or close down.
- **Tech Stack**: Python, Scikit-learn, Pandas, Flask/FastAPI (for deployment), Docker (optional), Jupyter Notebook.
- **Data Source**: Startup data from Crunchbase/Kaggle or other startup datasets.

## Project Structure:

- **`data/`**: Contains raw and processed data.
- **`notebooks/`**: Jupyter Notebooks for EDA, data preprocessing, and model training.
- **`src/`**: Python scripts for data preprocessing, feature engineering, model training, and prediction.
- **`deployment/`**: Flask or FastAPI app for serving model predictions via an API.

## Setup:

1. Clone the repository:
```bash
git clone https://github.com/Technocolabs100/Predicting-Startup-Acquisition-and-Machine-Learning-Pipeline.git
