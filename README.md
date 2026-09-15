# 📺 YouTube Recommendation Performance Dashboard

An end-to-end analytics project examining the performance of a simulated YouTube recommendation system. The analysis explores how content category, device, time of day, video length, and quarterly trends relate to recommendation click-through rate, subscription conversion, and watch completion.

The project combines **Python, Power BI, DAX, and automated rule-based insights** for data preparation, performance analysis, interactive visualization, and business interpretation.

---

## 🎯 Project Objective

The primary business question for this project was:

> How does recommendation performance vary across content categories, devices, viewing times, and video lengths, and which segments should be prioritized for improvement?

The analysis was designed to identify meaningful performance patterns and translate the findings into actionable insights for product, content, and recommendation strategy teams.

---

## 🔍 Analysis Approach

The project followed an end-to-end analytical workflow:

### 1. Data Preparation and Cleaning

* Reviewed and cleaned the synthetic YouTube interaction dataset
* Handled missing, inconsistent, and invalid values
* Standardized content categories, devices, and time-of-day values
* Converted timestamps into appropriate date formats
* Created analysis-ready variables

### 2. Feature Engineering

* Created quarterly time periods for trend analysis
* Grouped video durations into video-length categories
* Calculated watch-completion percentages
* Created recommendation click and subscription indicators
* Prepared dimensions required for Power BI slicers and visualizations

### 3. Performance Analysis

* Calculated overall recommendation click-through rate
* Calculated post-recommendation subscription rate
* Compared category CTR against the overall CTR
* Evaluated device and time-of-day combinations
* Analyzed quarterly recommendation performance
* Examined watch completion across video-length groups

### 4. Automated Insight Generation

* Created rule-based Python logic to interpret calculated metrics
* Identified the strongest and weakest device–time segments
* Summarized the latest quarterly trend
* Evaluated category performance ranges
* Identified video-length engagement patterns
* Generated recommended areas for further testing

### 5. Power BI Dashboard Development

* Created DAX measures for the primary performance indicators
* Designed KPI cards and interactive slicers
* Built trend, variance, heatmap, and engagement visuals
* Added an automated performance summary
* Added hover tooltips containing detailed business interpretations
* Published the final dashboard through Power BI Service

---

## 📊 Interactive Dashboard

### [View the Live Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYTcyYjQ5ZjgtNDNlMS00NjRlLTk4NDQtMDlmNWE0NjgxZjc5IiwidCI6ImJjMTBlMDUyLWIwMWMtNDg0OS05OTY3LWVlN2VjNzRmYzlkOCIsImMiOjZ9)

The dashboard includes interactive filters for:

* Category
* Device
* Time of day
* Year

---

## 📈 Key Performance Indicators

The dashboard tracks six primary KPIs:

| KPI                                   | Result |
| ------------------------------------- | -----: |
| Total Interactions                    |     1M |
| Unique Users                          |   100K |
| Unique Videos                         |    50K |
| Average Watch Completion              |  75.0% |
| Recommendation CTR                    |  30.0% |
| Post-Recommendation Subscription Rate |   5.0% |

These values describe the synthetic portfolio dataset and do not represent actual YouTube performance.

---

## 💡 Key Insights

### Recommendation Performance

The overall recommendation click-through rate remained close to **30%**, with moderate variation across quarters.

### Category Performance

News and Education performed above the overall CTR, while Music and Lifestyle showed the largest negative differences from the overall benchmark.

### Device and Time-of-Day Performance

Recommendation performance varied across device and time-of-day combinations. 

### Video-Length Engagement

Average watch completion declined as video duration increased. Videos under 10 minutes showed the highest completion, while videos between 50 and 60 minutes showed the lowest completion.

### Business Interpretation

The results suggest that recommendation strategy should consider the interaction between content category, device, viewing time, and video length rather than applying the same approach to every user segment.

---

## ⚙️ Automated Performance Summary

The dashboard includes an automated summary generated using transparent Python rules.

The summary identifies:

* Overall recommendation status
* Strongest device–time segment
* Lowest-performing segment
* Latest quarterly movement
* Category performance range
* Video-length engagement pattern
* Recommended area for testing

---

## 🛠️ Tools and Technologies

| Tool     | Application                                                                             |
| -------- | --------------------------------------------------------------------------------------- |
| Python   | Data cleaning, transformation, feature engineering, aggregation, and automated insights |
| pandas   | Data manipulation and performance calculations                                          |
| NumPy    | Conditional logic and video-length classification                                       |
| Power BI | Data modeling, dashboard development, and interactive reporting                         |
| DAX      | KPI measures and analytical calculations                                                |
| GitHub   | Project documentation and version control                                               |

---

## 📁 Repository Structure

```text
youtube-recommendation-performance-dashboard/
├── README.md
├── Automation/
│   └── Analysis_Insights.csv
├── data/
│   └── sample_raw_youtube_data.csv
└── Script/
    └── youtube_recommendation_data_pipeline.ipynb
```

---

## 📂 Data Availability

The complete raw and transformed datasets are excluded from this repository because of their size.

A reproducible **1,000-row sample of the raw dataset** is provided to demonstrate the original data structure. The complete transformed dataset can be reproduced by running the Python notebook with the original Kaggle dataset.

The Power BI `.pbix` file is also excluded because of its size. The completed interactive dashboard is available through the public Power BI link above.

---

## 📚 Data Source

The project uses the following Kaggle dataset:

[YouTube Trending Analytics Dataset – Multi-Region](https://www.kaggle.com/datasets/edudev-commons-org/youtube-trending-analytics-dataset-multi-region)

---



