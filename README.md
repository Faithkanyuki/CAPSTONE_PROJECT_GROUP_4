# CAPSTONE_PROJECT_GROUP_4
# Rush Hour Roulette: Matatu Madness
## Predicting Peak-Hour Transport Delays in Nairobi Using Machine Learning
Gemini_Generated_Image_f7fp6tf7fp6tf7fp.png
## Project Overview
The objective of this project is to build a supervised machine learning classification model to predict when and where overcrowding will occur at bus and matatu stops in Nairobi. By identifying these high-risk periods—driven by factors like peak hours and rainy seasons—transport operators (SACCOs) can proactively deploy additional vehicles to reduce passenger queues before they form.

## Key Questions
1. When are bus stops most likely to experience overcrowding (e.g., peak hours, rainy days)?

2. Which routes are most vulnerable to congestion-driven delays?

3. What combination of factors (weather, time, route characteristics) best predicts overcrowding?

4. Can we flag high-risk periods before queues form?

## Business & Social Impact
1. **For Transport Operators (SACCOs)**: Revenue optimization through better deployment and improved fleet efficiency.

2. **For Commuters**: Reduced wait times, improved reliability, and a safer, less frustrating boarding experience.

3. **For Urban Planning**: Data-driven decisions for infrastructure and better traffic management.

## Data Understanding & Cleaning
The project utilizes four primary datasets to capture the multifaceted nature of urban transport:

1. **GTFS Hourly Stop-Level Data**: Represents transport supply patterns (vehicle frequency per stop per hour).

2. **Matatu Travel Time**: Acts as a proxy for traffic congestion and delay severity.

3. **Matatu Congestion Data**: Contains route-level congestion indicators.

4. **Weather Data**: Captures rainfall and temperature, which significantly influence travel delays.

## Feature Engineering Highlights
**Low Supply During Peak Hours**: A binary feature capturing operational stress when vehicle frequency is below the median during peak times.

**Distance from CBD**: Spatial risk factor calculated using Euclidean distance from Nairobi's Central Business District.

**Severe Delay Signals**: Indicators based on the 90th percentile of travel times to capture extreme congestion.

**Weather Impact Signals**: Binary flags for rain and heavy rain to detect weather-triggered congestion early.

## Tech Stack
**Language**: Python

**Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn.

**Models Explored**: Logistic Regression, Random Forest Classifier.

## Methodology
**Phase 1**: Business Understanding: Defining objectives and success metrics.

**Phase 2**: Data Understanding: Exploring dataset structures and completeness.

**Phase 3**: Data Cleaning: Standardizing types, handling missing values, and validating time ranges.

**Phase 4**: Feature Engineering: Creating domain-specific indicators like "Supply Pressure" and "Spatial Risk".

**Phase 5**: Modeling & Evaluation: Building and testing classification models to predict overcrowding events.

## Conclusion
By integrating supply-side data (GTFS) with demand-side signals (weather and congestion), this project provides a predictive tool that transforms transport management from reactive to proactive, ultimately easing the "Matatu Madness" of Nairobi's rush hour.