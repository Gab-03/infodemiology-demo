# Infodemiology- Software Engineering Documentation

## Website 
https://gab-03.github.io/infodemiology-demo/

# Infodemiological Disease Surveillance  

## How to Run the Model  
1. **Clone the repository** – Follow the cloning instructions below.  
2. **Install dependencies** – Run:  
   ```bash
   pip install -r requirements.txt
   ```  
3. **Run the ARIMAX model** – Execute:  
   ```bash
   python arimax.py
   ```  
   This will process and update the data used in the website.  
4. **Run the server** – Start the server and make changes locally as needed.  

## Data Sources  
1. **FASSSTER & Ateneo Social Computing Laboratory Collaboration** – The primary COVID-19 case datasets used in this project were obtained through a collaboration between **[FASSSTER]** and the **Ateneo Social Computing Laboratory**. A GitHub repository can be requested from the Ateneo Social Computing Lab for data access.  

2. **Google Trends Data** – This project leverages **Google Trends** data to collect **Relative Search Volume (RSV)** for COVID-19 symptom-related keywords (e.g., **cough, fever, flu**). Google Trends allows tracking of public interest in symptoms, which can serve as an early indicator of potential outbreaks. You can explore Google Trends data at **[Google Trends](https://trends.google.com/trends/)**.  

3. **Regional Google Trends Data Extraction** – Google Trends provides an option to obtain data at the **regional level**. This project extracts and downloads **per-region** Google Trends data to correlate search interest in symptoms with actual COVID-19 cases. The extracted data is stored in the **GT Folder**, where you can find the specific keywords used for data collection per region.  

## BibTeX Citation  
If you use this project in your research, please cite it as follows:  

```bibtex
@software{Lagustan_2024,
  author = {Mon Gabriel Lagustan & Dr. Maria Regina Justina E. Estuar},
  title = {Infodemiological Disease Surveillance},
  year = {2024},
  version = {1.0},
  url = {https://github.com/Gab-03/mlagustan},
  institution = {Ateneo Social Computing Lab}
}
```  

## Files  
1. **`*.csv` files** – Contain **regional COVID-19 data**, including daily confirmed cases per region in the Philippines. These files serve as input for forecasting models.  

2. **`arimax.py`** – A Python script that processes and analyzes COVID-19 case data for various regions in the Philippines using **ARIMAX models**. It integrates Google Trends data on key symptoms (**cough, fever, flu**) to enhance forecasting accuracy. The script performs the following tasks:  
   - Reads and preprocesses regional COVID-19 case data.  
   - Extracts relevant features and computes correlations between **symptom search trends** and **reported COVID-19 cases**.  
   - Trains and updates ARIMAX models to generate short-term forecasts for case trends.  

3. **`GT Folder`** – Stores **Google Trends data files**, which contain **time-series data on symptom-related search queries** (e.g., **cough, fever, flu**). These files are used as external predictors in the ARIMAX model.  

4. **`regional Folder`** – Contains **all regional COVID-19 data files**. Each file represents a specific region and includes **time-series data on daily confirmed cases**. These files are essential for model training and forecasting.  

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

