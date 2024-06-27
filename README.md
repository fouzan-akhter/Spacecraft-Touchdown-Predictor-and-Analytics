<h1>Spacecraft-Touchdown-Predictor-and-Analytics</h1>

 ### [IBM Data Science Professional Certificate](https://github.com/fouzan-akhter/Spacecraft-Touchdown-Predictor-and-Analytics)

## <div style="display: flex; align-items: center; justify-content: center;"><img align="left" alt="Python Logo" width="25px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /><span style="margin-left: 5px;">Overview</span></div>

This project aims to predict the success of the Falcon 9's first-stage landing using various data analysis and machine learning techniques. Accurate predictions are crucial as SpaceX's ability to reuse the first stage of their rockets significantly reduces launch costs, offering competitive pricing compared to other providers.

## <div style="display: flex; align-items: center; justify-content: center;"><img align="left" alt="Python Logo" width="25px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /><span style="margin-left: 5px;">Project Objectives</span></div>

1. **Data Sourcing:** Collect and parse data from SpaceX's API and web scraping techniques.
2. **Data Wrangling:** Clean and preprocess raw data for analysis.
3. **Exploratory Data Analysis (EDA):** Use SQL and visualization to extract meaningful insights.
4. **Predictive Modeling:** Develop and enhance models to predict landing success.
5. **Presentation:** Communicate findings through a comprehensive, engaging narrative.

## <div style="display: flex; align-items: center; justify-content: center;"><img align="left" alt="Python Logo" width="25px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /><span style="margin-left: 5px;">Workflow</span></div>

### 1. Data Collection & Preparation

- **API Data:** Request and parse data from the SpaceX API.
  - Extract information such as booster names, payload details, launch site coordinates, and core details.
- **Web Scraping:** Use BeautifulSoup to scrape historical Falcon 9 launch records from Wikipedia.
  - Extract HTML tables and convert them into a Pandas DataFrame.

### 2. Data Wrangling

- **Handling Missing Values:** Replace missing payload mass values with the mean. Retain `None` values for missing landing pad data.
- **Data Filtering:** Focus on Falcon 9 launches by filtering the `BoosterVersion` column. Exclude Falcon 1 data.
- **Data Enrichment:** Use API-derived lists to enrich the dataset with booster and payload information.

### 3. Exploratory Data Analysis (EDA)

- **SQL Queries:** Analyze launch frequencies and success rates per launch site.
- **Data Visualization:** Examine relationships between payload mass, orbit type, and success rates.
  - **Success Rates:** CCAFS LC-40 (60%), KSC LC-39A (77%), VAFB SLC 4E (77%).
  - **Payload Mass:** High success for payloads >7000 kg and under 5500 kg at specific sites.

### 4. Predictive Modeling

- **Model Development:** Create regression and machine learning models to forecast landing outcomes.
  - **Models:** Logistic Regression, SVM, Decision Trees, KNN.
- **Model Evaluation:**
  - **Jaccard Score:** 0.833 (LogReg), 0.845 (SVM), 0.811 (Tree), 0.819 (KNN)
  - **F1 Score:** 0.909 (LogReg), 0.916 (SVM), 0.896 (Tree), 0.901 (KNN)
  - **Accuracy Score:** 0.867 (LogReg), 0.878 (SVM), 0.844 (Tree), 0.856 (KNN)

### 5. Presentation

- **Final Output:** Create a narrative that effectively communicates the analysis and findings.
- **Interactive Dashboard:** Utilize visual analytics to provide insights into optimal launch site locations and other influential factors.

## <div style="display: flex; align-items: center; justify-content: center;"><img align="left" alt="Python Logo" width="25px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /><span style="margin-left: 5px;">Key Features</span></div>

- **Data Analysis & Engineering:** 
  - Data cleaning, feature engineering, and model evaluation to improve performance.
- **Predictive Insights:** 
  - Develop models to estimate launch costs by predicting Falcon 9 landing success.
- **Exploratory Analysis:** 
  - Use SQL and visualization to uncover variable relationships and success determinants.

## <div style="display: flex; align-items: center; justify-content: center;"><img align="left" alt="Python Logo" width="25px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /><span style="margin-left: 5px;">Technologies & Tools</span></div>

- **Languages:** Python
- **Libraries:** Pandas, BeautifulSoup, SQLAlchemy, Matplotlib, Scikit-learn
- **Data Sources:** SpaceX API, Wikipedia

## <div style="display: flex; align-items: center; justify-content: center;"><img align="left" alt="Python Logo" width="25px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /><span style="margin-left: 5px;">Results & Findings</span></div>

- **Launch Site Analysis:** Success rates vary significantly by launch site.
- **Payload Mass:** Higher success rates with specific payload mass ranges.
- **Orbit Analysis:** Some orbits show higher success rates; others have mixed outcomes.

## <div style="display: flex; align-items: center; justify-content: center;"><img align="left" alt="Python Logo" width="25px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /><span style="margin-left: 5px;">Disclaimer</span></div>

The code presented here is not owned by me, and there are likely numerous other attempts at the same exercise. This project represents my interpretation and implementation of the IBM Data Science Professional Certificate Capstone Project. All rights are reserved by IBM, and they reserve the right to take down the code or content associated with their materials at their discretion.

## <div style="display: flex; align-items: center; justify-content: center;"><img align="left" alt="Python Logo" width="25px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /><span style="margin-left: 5px;">Contributing</span></div>

Contributions are welcome! Please fork the repository and submit a pull request for feature additions or bug fixes.

## <div style="display: flex; align-items: center; justify-content: center;"><img align="left" alt="Python Logo" width="25px" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" /><span style="margin-left: 5px;">License</span></div>

This project is licensed under the MIT License - see the [LICENSE](https://github.com/fouzan-akhter/Spacecraft-Touchdown-Predictor-and-Analytics/blob/main/LICENSE) file for details.
