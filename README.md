# Customer Service Requests Analysis
**Project**: Customer Service Requests Analysis  
**Tools**: Python, NumPy, Pandas, Matplotlib, Seaborn, SciPy  

---

## Project Overview

The goal of this project is to analyze and uncover patterns from the NYC 311 service requests dataset. NYC 311 is a centralized platform that allows New York City residents to file non-emergency service requests, including complaints such as noise disturbances, plumbing issues, and illegal parking. Each day, thousands of requests are recorded and forwarded to the appropriate agencies, which handle and resolve the issues.

This analysis focuses on data wrangling techniques and visualization to extract meaningful insights from the dataset. Through the exploratory analysis, we aim to understand complaint trends, response times, and performance across different boroughs.

---

## Objectives

- **Data Wrangling**: Clean and preprocess the dataset for analysis.
- **Exploratory Data Analysis (EDA)**: Identify trends and insights from 311 service requests.
- **Statistical Testing**: Perform statistical tests to evaluate hypotheses about response times.
- **Data Visualization**: Present major findings through informative graphs and charts.

---

## Key Features

1. **Request Processing Time**:
   - Calculate the time taken to resolve complaints by creating a new `Request_Closing_Time` column (difference between request creation and closure).
2. **Complaint Trends**:
   - Visualize complaint types based on frequency, severity, and location.
3. **Response Time Analysis**:
   - Group complaints by borough and analyze the average response time.
4. **Hypothesis Testing**:
   - Perform statistical tests (e.g., chi-square) to examine whether complaint types influence response times across different boroughs.

---

## Steps to Run the Project

### Prerequisites

Before running the project, ensure you have the following installed:

- Python 3.9+
- NumPy, Pandas, Matplotlib, Seaborn, SciPy

You can install the required libraries by running:

```bash
pip install -r requirements.txt
```

### Running the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/MOHAMED-EL-HADDIOUI/service-requests-analysis.git
   cd service-requests-analysis
   ```

2. Ensure the dataset is available in the `./Dataset/` directory as `Service_Requests_from_2010_to_Present.csv`.

3. Launch the Jupyter Notebook and run all cells to perform the analysis.

   ```bash
   jupyter notebook Customer_Service_Requests_Analysis.ipynb
   ```

---

## Data Summary

The dataset contains millions of records with the following key attributes:

- **Unique Key**: Unique ID for the complaint.
- **Created Date**: Date when the service request was made.
- **Closed Date**: Date when the service request was closed.
- **Complaint Type**: Type of complaint (e.g., Noise, Illegal Parking, Blocked Driveway).
- **Agency**: NYC agency responsible for addressing the complaint.
- **Location**: Latitude, longitude, and borough of the complaint.

---

## Results

### Major Findings

1. **Top Complaint Types**: Noise complaints are the most frequent, especially in Manhattan and Brooklyn.
2. **Average Resolution Time**: The average time to resolve a complaint is significantly longer in the Bronx compared to other boroughs.
3. **Complaint Location Impact**: Complaint types such as 'Illegal Parking' and 'Blocked Driveway' show location-specific patterns, particularly in residential areas.

### Visualizations

- Bar charts representing the top 5 complaint types across different boroughs.
- Heatmaps illustrating response times by complaint type.
- Statistical test results on whether response times vary significantly by borough.

---

## Conclusion

This analysis provides insights into the most common service requests made by NYC residents and highlights areas for improvement in response times. Future work could focus on predictive modeling to anticipate complaint trends and optimize resource allocation.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
