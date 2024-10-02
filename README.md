# Megafon Statistical Analysis

## Project Objective
The objective of this project is to analyze customer satisfaction with Megafon’s cellular and internet services. Using survey responses and technical performance data, the goal is to predict which technical features have the greatest impact on customer satisfaction. By understanding these drivers, Megafon can improve service quality and enhance customer experiences.

### Partner
* Megafon (Cellular & Internet Service Provider)

### Methods Used
* Data Preprocessing
* Logistic Regression
* Data Visualization
* Bootstrap Sampling
* Confidence Interval Estimation

### Technologies
* Python
* Jupyter
* R
* Pandas
* NumPy
* Matplotlib
* Logistic Regression (R)
* Bootstrap Sampling (R)

## Project Description
This project focuses on analyzing the relationship between customer satisfaction and various technical performance metrics provided by Megafon. The dataset includes responses to two survey questions as well as several key performance indicators (KPIs) related to data usage, download speeds, retransmission rates, and latency metrics.

Key areas of focus include:
1. Preprocessing the dataset by handling invalid entries and reformatting data.
2. Using Logistic Regression to predict customer satisfaction based on technical features.
3. Estimating confidence intervals and using bootstrap sampling to validate findings.
4. Visualizing relationships between survey responses and technical performance metrics.

The project is divided into two parts:
1. Preprocessing (Python): Cleaning and preparing the data for analysis.
2. Statistical Analysis (R): Performing statistical modeling and confidence interval estimation.

## Project Needs
- Data exploration and preprocessing
- Statistical modeling using logistic regression
- Bootstrap sampling for validation
- Data visualization and reporting

## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Download the `megafon.csv` dataset, which contains survey responses and technical performance metrics.
3. The primary Jupyter notebook for data preprocessing is located in `preprocess.ipynb`.
4. The R notebook for statistical analysis is in `Megafon_Stat_Analysis.Rmd`.
5. Install the dependencies listed in `requirements.txt` (for Python) and use an appropriate R environment to run the R notebook.

## Featured Notebooks
* [preprocess.ipynb](https://github.com/vladvintenbakh/MegafonStatisticalAnalysis/blob/main/preprocess.ipynb)
* [Megafon_Stat_Analysis.Rmd](https://github.com/vladvintenbakh/MegafonStatisticalAnalysis/blob/main/Megafon_Stat_Analysis.Rmd)

## Codebook
The dataset `megafon.csv` contains the following columns:
- **user_id** — Customer’s unique ID.
- **Q1** — Response to the first satisfaction survey question.
- **Q2** — Response to the second satisfaction survey question.
- **Total Traffic(MB)** — The volume of data transfer traffic.
- **Downlink Throughput(Kbps)** — Average downlink throughput.
- **Uplink Throughput(Kbps)** — Average uplink throughput.
- **Downlink TCP Retransmission Rate(%)** — Frequency of retransmissions.
- **Video Streaming Download Throughput(Kbps)** — Speed of video streaming downloads.
- **Video Streaming xKB Start Delay(ms)** — Delay before video playback starts.
- **Web Page Download Throughput(Kbps)** — Speed of web page downloads.
- **Web Average TCP RTT(ms)** — Average round-trip time for web requests.

The first technical feature represents a sum over a one-week period before the survey, while the rest are averages over the same time frame.
