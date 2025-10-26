# IVT-Ad-Traffic-Fraud-Analysis
The analysis of six advertising apps confirms that the Invalid Traffic (IVT) system is highly effective and primarily targets extreme device spoofing. The key differentiator between Valid and Invalid traffic streams is the idfa_ua_ratio (Unique Devices per Unique User-Agent). 

# Project Overview
This analysis investigates six advertising applications (three valid, three flagged) to identify the core statistical patterns and chronological markers that lead to **Invalid Traffic (IVT)** flagging. The goal was to rigorously **reverse-engineer the detection logic** using comparative statistical benchmarking against established 'normal' traffic patterns.

# Key Findings
## 1. Primary IVT Driver: Device Spoofing
The final IVT score is primarily driven by **device spoofing**, as proven by the high sensitivity to the idfa_ua_ratio (Unique Devices per Unique User-Agent).

## 2. Quantified Anomaly: Extreme Deviation
Invalid apps exhibited an average idfa_ua_ratio that was **over 96% below** the 95th percentile of normal traffic—a statistical signature confirming mass, non-human activity.

## 3. Flagging Timeline: Chronological Detection
The order of flagging was strictly chronological and determined by the onset and severity of this idfa_ua_ratio anomaly in each app's traffic feed.

# Repository Contents
`ivt_analysis.py`: The complete Python script (Pandas, Matplotlib, Seaborn) used for data cleaning, statistical analysis, and visualization.

`App Valid/Invalid.csv`: The six raw data files used in the analysis.

`invalid_app_time_series_analysis.png`: The final visualization linking the fraud metric to the IVT spike.

`README.md`: This project overview.

`IVT-Ad-Traffic-Fraud-Analysis`: The final formal report (for reference).
