# Waze User Churn Analysis

## Overview

This project was completed as part of the Google Advanced Data Analytics course in the "Get Started with Python" chapter. This project analyzes user churn patterns from a synthetic dataset provided by Waze. The goal is to identify characteristics of churned vs. retained users based on their app usage, driving behavior, and device type. The insights gained from this analysis are intended to guide future efforts to improve user retention and provide a better user experience for Waze's diverse audience.

## Dataset

The dataset used in this project contains 14,999 unique users and includes the following columns:

- `ID`: A sequentially numbered index
- `label`: Binary target variable (“retained” vs “churned”) indicating whether a user has churned
- `sessions`: The number of occurrences of a user opening the app during the month
- `drives`: The number of occurrences of driving at least 1 km during the month
- `device`: The type of device used by the user (iPhone or Android)
- `total_sessions`: Estimated total number of sessions since onboarding
- `n_days_after_onboarding`: Number of days since the user signed up
- `total_navigations_fav1`: Total navigations to the user’s favorite place 1
- `total_navigations_fav2`: Total navigations to the user’s favorite place 2
- `driven_km_drives`: Total kilometers driven during the month
- `duration_minutes_drives`: Total driving time in minutes during the month
- `activity_days`: Number of days the user opened the app during the month
- `driving_days`: Number of days the user drove at least 1 km

## Objective

The purpose of this analysis is to:

- Inspect the dataset for missing data and identify patterns.
- Analyze the behavior of churned vs. retained users, focusing on driving activity and app usage.
- Investigate potential device-specific differences in churn rates.
- Provide actionable insights for improving user retention.

## Key Findings

1. **Missing Data:** The `device` column had missing values with no clear pattern of missingness between iPhone and Android users.
2. **Churn Analysis:** Churned users drove more and had higher driving durations but used the app on fewer days compared to retained users.
3. **Device Distribution:** No significant difference in churn rates between Android and iPhone users.
4. **User Engagement:** Retained users were more consistent in app usage, while churned users exhibited more intense but less frequent driving.

## Next Steps

1. **Investigate Long-Haul Drivers:** Explore if long-haul drivers contribute disproportionately to churn.
2. **Segment Users:** Segment users based on driving behavior to create targeted retention strategies.
3. **Feature Engineering:** Explore new features to better understand user behavior and driving patterns.
4. **A/B Testing:** Test changes to app features to improve retention, especially for high-mileage users.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn

## How to Run

1. Clone the repository:
git clone https://github.com/yourusername/waze-user-churn-analysis.git

2. Install the required dependencies:
pip install -r requirements.txt

3. Run the analysis notebook:
jupyter notebook waze_analysis.ipynb

## License
This project is licensed under the MIT License - see the LICENSE file for details.

### Notes:
- Replace `yourusername` with your GitHub username in the clone URL.
- Ensure you add a `requirements.txt` file with the necessary dependencies (e.g., pandas, numpy, etc.).
- If you have a license file (MIT or others), make sure to include it in your repo.
