# Machine Learning Project
This is the final project for my Machine Learning class at Rangsit University. It was completed as a team project, with each member responsible for specific parts of the data collection, preprocessing, modeling, and evaluation.

## Objective
Predict hotel price categories (Low / Medium / High) based on attributes such as star rating, location, room type, and amenities.

## My Role and Contributions
I was responsible for:
- **Data Collection**: Sourcing hotel data (~40 entries) from booking.com, including star ratings, locations, room types, amenities, and customer reviews.
- **Excel Modeling**: Structuring the full dataset in Excel for preprocessing and analysis, including:
  - Calculating the "Amenity Score" by combining individual facility indicators.
  - Binning the price into three categories using equal-frequency binning.
- **k-Nearest Neighbors Execution in Excel**:
  - Implementing the distance formula (Euclidean) for classification manually in Excel.
  - Setting k = 5 for neighbor selection.
  - Performing 5-fold cross-validation by splitting data (~160 training, ~40 testing each fold).
  - Personally responsible for structuring and calculating results for the final 20 test samples in one fold.
    
## Data Overview
- ~200 hotel records from 5 cities in Thailand via booking.com
- Attributes collected:
  - Star Rating (1–5)
  - Location Type (Major City / Beach / Countryside)
  - Room Type (Budget, Standard, Superior, Deluxe+)
  - Amenities (pool, gym, spa, etc.)
  - Customer Reviews (0–10)
  - Price (numeric)

## Preprocessing
- Combined binary amenity features into a single "Amenity Score" (0–5 scale).
- Applied equal-frequency binning to divide price into three classes:
  - Low (≤1170)
  - Medium (1171–3200)
  - High (>3200)
    
## Method
- Algorithm: k-Nearest Neighbors (k=5)
- Distance Metric: Euclidean
- Validation: 5-fold cross-validation (~160 training, ~40 testing per fold)
- Manual implementation of KNN classification in Excel, with detailed tracking of neighbor distances and class assignment.

## Results
- Approx. 70% accuracy overall
- Observed good classification performance for Low and Medium categories
- Struggled to distinguish High price category
- Confusion matrix created for fold analysis

## Tools Used
- **Excel**: Data cleaning, feature engineering, manual KNN calculations, cross-validation folds


