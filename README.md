
# Marathon Winning Times Analysis and Forecasting

## Project Overview

This project analyzes historical data from major marathons, with a particular focus on the Boston Marathon. The goal is to understand trends in marathon 
winning times and to predict future winning times using advanced time series forecasting techniques. The analysis reveals how marathon performance has evolved
over the years and provides insights into potential future trends.

## Table of Contents

1. [Dataset](#dataset)
2. [Objectives](#objectives)
3. [Analysis Steps](#analysis-steps)
   - [Data Cleaning](#data-cleaning)
   - [Trend Analysis](#trend-analysis)
   - [Country and Gender Analysis](#country-and-gender-analysis)
   - [Time Series Forecasting](#time-series-forecasting)
4. [Results](#results)
5. [How to Run the Project](#how-to-run-the-project)
6. [Conclusions](#conclusions)
7. [Future Work](#future-work)

## Dataset

The dataset used in this project includes historical winning times from major marathon events like Boston, Berlin, NYC, and others.
The data covers various years, genders, and countries, providing a comprehensive view of marathon performances over time.

- **File**: `world_marathon_majors.csv`
- **Columns**:
  - `year`: The year of the marathon.
  - `winner`: Name of the marathon winner.
  - `gender`: Gender of the winner.
  - `country`: Country of the winner.
  - `time`: Winning time of the marathon.
  - `marathon`: The marathon event name.

## Objectives

The main objectives of this project are:
1. To analyze historical trends in marathon winning times across different events.
2. To explore the dominance of different countries and genders in marathon events.
3. To forecast future marathon winning times using the ARIMA time series model.

## Analysis Steps

### Data Cleaning
- The dataset was loaded, and any rows containing null values were removed to ensure the analysis was based on complete and accurate data.
- The `time` column, which originally contained times as strings, was converted into a `timedelta` format to allow for numerical analysis.

### Trend Analysis
- Historical winning times were plotted to visualize trends over the years for various marathons.
- The analysis revealed a significant decrease in winning times over the decades, reflecting improvements in athlete performance and race conditions.

### Country and Gender Analysis
- The number of marathon wins was aggregated by country to identify which countries have dominated marathon events.
- A similar analysis was conducted based on gender, showing how the representation and performance of male and female athletes have evolved over time.
- Visualizations included bar charts showing total wins by country and cumulative win trends over time.

### Time Series Forecasting
- For the Boston Marathon, a specific time series analysis was conducted using the ARIMA model.
- The model was trained on historical data and used to predict future winning times, with confidence intervals provided to indicate the uncertainty of these predictions.
- The analysis included visualizations comparing the model's predictions against actual data, along with confidence intervals.

## Results

- **Trend Analysis**: The winning times for major marathons have become faster and more consistent over the years, particularly after the 1980s.
- This indicates improvements in training methods, sports science, and the overall competitiveness of marathon events.
- **Country and Gender Dominance**: Certain countries, notably Kenya and Ethiopia, have emerged as dominant forces in marathon running.
- The analysis also showed that the gender gap in winning times has narrowed over time, reflecting the growing competitiveness of female athletes.
- **Forecasting**: The ARIMA model successfully predicted future winning times for the Boston Marathon, with predictions closely matching actual outcomes.
- The confidence intervals provided a reliable estimate of the uncertainty in these predictions.

## Conclusions

- The analysis reveals significant improvements in marathon performances over the years, with a marked increase in the competitiveness of the events.
- The ARIMA model proved effective in forecasting future marathon times, providing both accurate predictions and a quantifiable measure of uncertainty.
- These insights are valuable for athletes, coaches, and marathon organizers looking to understand past trends and anticipate future performance levels.

## Future Work

- Expand the analysis to include other major marathon events and compare trends across different races.
- Experiment with more advanced forecasting models such as Prophet or machine learning-based approaches.
- Incorporate additional variables such as weather conditions, course difficulty, and athlete profiles to enhance the accuracy of predictions.

---

