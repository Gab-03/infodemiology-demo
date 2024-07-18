# Infodemiology- Software Engineering Documentation

## Introduction
This repository contains the software engineering documentation for Infodemiology-, a web-based platform for timely COVID-19 surveillance and health risk mapping in the Philippines. The website integrates Google Trends data and ARIMAX model to predict COVID-19 spread across regions and provides insights into health capacity for optimal resource allocation.

## Architecture
### Overview
Infodemiology follows a client-server architecture using Django framework for the backend and HTML/CSS/JavaScript for the frontend. It leverages Google Trends API for real-time disease activity indicators and integrates health capacity data for informed decision-making.

### Components
- **Backend:** Django framework with Python for backend logic.
- **Frontend:** HTML, CSS, JavaScript for user interface.
- **Data Sources:** Google Trends API, real-time health capacity data.

#### Diagram
![Architecture Diagram](link_to_your_architecture_diagram)

## Technologies Used
### Backend
- **Python:** Backend development language.
- **Django:** Web framework for rapid development.
- **ARIMA Model:** Time series forecasting for COVID-19 predictions.
- **Google Trends API:** Real-time search data on COVID-19 symptoms.

### Frontend
- **HTML, CSS, JavaScript:** Frontend development technologies.

## Data Integration
### Google Trends and ARIMA Model
- Automated retrieval of Google Trends data for COVID-19 symptom-related queries.
- Implementation of ARIMA model for predictive analytics of COVID-19 spread.

### Health Capacity Data
- Real-time integration of health capacity data for hospital resource insights.

## Deployment
### Environment Setup
- Local development setup instructions.
- Deployment using CI/CD pipelines integrated with GitHub.

## Predictive Models Evaluation
### Comparison
- Evaluation of ARIMAX model against traditional models (AR, standard ARIMA, LSTM).
- Performance metrics demonstrating ARIMAX's predictive accuracy.

## User Interface and Features
- Real-time display of COVID-19 activity and health capacity information.
- Health risk mapping across regions.
- Automated resource allocation recommendations based on transmission risk.

## Future Enhancements
- Continued refinement of predictive models.
- Integration of user feedback mechanisms.
- Expansion to cover additional diseases and health-related metrics.

---

## Cloning Instructions
To clone this repository and set up [Your Website Name] locally, follow these steps:

1. **Clone the repository:**
git clone <repo_name>


2. **Navigate into the project directory:**

6. **Access the application:**
Open your web browser and navigate to `http://localhost:8000` to view [Your Website Name] locally.

---

## Updating Data

To update the data files for all regions in the Philippines, use the Python script `arimax.py`. Follow these steps:

1. **Run the script:**
python3 arimax.py

