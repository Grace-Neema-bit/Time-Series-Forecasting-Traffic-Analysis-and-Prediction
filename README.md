# Time-Series-Forecasting-Traffic-Analysis-and-Prediction
## BUSINESS UNDERSTANDING
#### PROBLEM STATEMENT
Urban traffic congestion is a growing challenge that affects mobility, economic productivity, and environmental sustainability. Despite the availability of traffic data, there is often limited use of this data to proactively predict congestion patterns. This project aims to analyze time-based traffic data collected at 15-minute intervals and develop predictive models to forecast traffic volume and congestion levels. The goal is to provide data-driven insights that can support effective traffic management, planning, and decision-making.

---
#### KEY QUESTIONS
1. How can historical traffic data be used to forecast future traffic volume and congestion levels?

2. What temporal patterns influence traffic congestion?

3. Which models provide the most accurate predictions?

4. How can these predictions support decision-making?
---
## DATA UNDERSTANDING
## Dataset

* Time-based traffic data (15-minute intervals)
* Features:

  * Vehicle counts (Car, Bike, Bus, Truck)
  * Total traffic volume
  * Days of the week
  * Time
  
* Target variable = Traffic Situation
---

## Models Used

* Logistic Regression (L1 & L2)
* Random Forest
* Voting Ensemble

---

## Evaluation Metrics

* Accuracy
* F1 Score (macro)
* Confusion Matrix
* ROC-AUC
* Cross-validation

---

## Results

* Ensemble model achieved the best performance
* Cross-validation confirms model stability
* Model performs well on majority classes but struggles slightly with minority classes

---

## Limitations

* Class imbalance affects performance
* Limited temporal feature engineering

---

## Recommendations

- Implement an automated signal control system that uses the model’s real-time 15-minute forecasts to extend durations during predicted heavy or high congestion periods.

- Focus road maintenance and expansion on segments that consistently have heavy congestion during non-peak hours, as this indicates structural issues rather than just surges.

- Integrate these predictive insights into a commuter app or dashboard to inform the public about expected congestion 15–30 minutes in advance, encouraging a shift in travel start times.

- Use the prediction to deploy traffic officers during peak hours

---

## 🧠 Conclusion

Traffic patterns show strong dependence on time of day and vehicle volume, with peak congestion occurring during high vehicle density periods. Machine learning models, particularly ensemble methods, provide reliable classification of traffic conditions. However, overlapping patterns between normal and high traffic reduce classification precision. The model demonstrates good generalization through cross-validation and supports traffic monitoring systems.
The analysis successfully addressed the core problem of forecasting urban traffic congestion using a 15-minute interval dataset. Key findings include:

- Model Performance: The Ensemble Voting Classifier achieved high accuracy and F1-scores

- Temporal Drivers: Traffic intensity is highly cyclical. Peak hours are clearly identifiable through the 24-hour cycle line plots, with significant variance between weekdays and weekends.

- Feature Importance: Total vehicle count is the strongest predictor of our target variable

- Predictive Capability: The model shows high AUC scores across all classes (Low, Normal, High, Heavy), proving it is a reliable tool for real-time congestion classification.

---

## Dashboard

Interactive Tableau Dashboard:
https://public.tableau.com/views/Trafficforecastinganalysis/Dashboard1


