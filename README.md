# Forecasting Crime Trends in Calgary: A Data-Driven Approach  

## Project Overview  
This initiative focuses on analyzing historical crime data from Calgary to identify patterns and develop an advanced predictive model. Leveraging the *Crime and Disorder Dataset* (2018-2024) from the City of Calgary's open data portal, we employ machine learning techniques to forecast crime trends and support data-informed decision-making for public safety.  

---

## Methodology  
Our approach consists of six systematic phases:  

1. **Data Acquisition & Preliminary Analysis**  
   - Load and inspect the dataset to understand its structure, variables, and potential gaps  

2. **Data Preparation**  
   - Clean and transform raw data (handling missing values, correcting formats, and ensuring consistency)  

3. **Exploratory Data Analysis (EDA)**  
   - Investigate crime distributions across communities, categories, and time to uncover hidden trends  

4. **Neural Network Development**  
   - Design an LSTM-based model tailored for time-series forecasting of crime occurrences  

5. **Model Optimization**  
   - Fine-tune hyperparameters and validate performance using training/validation splits  

6. **Future Crime Prediction**  
   - Deploy the trained model to generate forecasts for upcoming months  

---

## Key Findings from EDA  

### 1. High-Risk Communities  
- **Beltline** ranked highest in crime frequency (11.4%), followed by **Forest Lawn** (10.7%) and **Downtown Commercial Core** (10.2%)  
- The safest areas included **13M** (22.7% of lowest crime rates) and districts **02K/02B** (13.6% each)  

### 2. Dominant Crime Categories  
- **Theft from Vehicle** (21.7%) and **Theft of Vehicle** (16.7%) were most prevalent  
- **Break and Enter - Commercial** accounted for 13.8% of incidents  

### 3. Temporal Trends  
- **Peak Activity**: 2019 recorded the highest crime volume, with 2022 and 2018 also showing elevated numbers  
- **Seasonality**: Monthly fluctuations suggested periodic spikes, potentially linked to seasonal factors  

### 4. Community-Specific Patterns  
- **Forest Lawn** had frequent *Break & Enter - Other Premises*, while **Marlborough** reported minimal *Commercial Robbery* cases  

---

## Predictive Modeling with LSTM  

### Model Architecture  
- **Input**: Sequential crime data (time-series format)  
- **LSTM Layers**: 50-unit memory cells to capture long-term dependencies  
- **Regularization**: Dropout layer (20%) to mitigate overfitting  
- **Output**: Dense layer with linear activation for regression  

### Training & Evaluation  
- **Optimizer**: Adam (adaptive learning rate)  
- **Loss Metric**: Mean Squared Error (MSE)  
- **Performance**: Training over 100 epochs showed steady loss reduction, with validation loss confirming generalization capability  

---

## Implications & Future Applications  

1. **Proactive Policing**: Predictions enable targeted patrols in high-risk areas during forecasted crime surges  
2. **Resource Allocation**: Data-driven insights assist in optimizing emergency service deployments  
3. **Public Awareness**: Seasonal trends can inform community safety campaigns  
