# Smart Hospital ER Analytics: Predictive Modeling & Visual Insights

## Project Overview
This project focuses on optimizing Emergency Room (ER) operations by analyzing and predicting patient wait times. Using simulated operational parameters from 20,000 healthcare interactions, a machine learning regression framework was built to forecast wait-time escalations based on resource load and patient triage urgency. The analytics pipeline transitions seamlessly from backend data engineering and predictive modeling in Python to an interactive executive analytics interface in Power BI.

## Core Architecture
1. **Data Engineering & Simulation (Python):** Generated 20,000 granular patient records modeling feature variables such as Triage Levels (1-5), Staff Shift Densities, Emergency Entry Modes (Ambulance, Helicopter, Walk-in), and continuous Severity Scores.
2. **Predictive Analytics Engine (Scikit-Learn):** Trained a regression model evaluating how organizational bottlenecks and patient metrics impact patient wait times, exporting predicted outputs alongside error tracking arrays (Residual Analysis).
3. **Business Intelligence Analytics (Power BI):** Developed an advanced visual dashboard mapping clinical workloads, staffing correlations, and process flows.

---

## Interactive Dashboard Sneak Peek
*Replace these placeholders with the actual image files uploaded to your repo!*
![Dashboard Overview](images/dashboard_main_screenshot.png)
![Triage & Operational Bottlenecks](images/dashboard_triage_screenshot.png)

---

## Dataset & Feature Variables
The model features 20,000 operational observations with data elements including:
- `Triage_Level`: Priority rank assigned based on clinical urgency (1 to 5).
- `Current_Occupancy`: Total patient counts inside the ER assessing department crowding.
- `Doctors_on_Shift`: Active medical staffing during the observation block.
- `Severity_Score`: Granular evaluation (0-10) quantifying condition acuity.
- `Arrival_Mode`: Transportation categories impacting priority response parameters (Helicopter, Ambulance, Walk-in, Private Vehicle).
- `Wait_Time_Minutes` (Target Variable): Derived via complex clinical workflows capturing occupancy bottlenecks mitigated by staffing levels.

## Key Technical Achievements
- **Machine Learning Rigor:** Built standard preprocessing pipelines for categorical features and executed an operational train/test split.
- **Model Quality:** Captured core resource variations, producing an operational $R^2$ Score matching the underlying baseline clinical logic precisely.
- **Advanced Visual Infrastructure:** Augmented default Power BI visuals with customized Sankey Diagrams and Performance Bubble Charts to clearly isolate operational throughput limitations.

## How to Run the Repository

### 1. Python Analysis & Modeling Pipeline
To recreate the data generation engine and predictive model, run the Jupyter Notebook:
```bash
pip install -r requirements.txt
jupyter notebook Smart_Hospital_ER_Analytics.ipynb
