# How to run the code
#### download Biometrics for stress monitoring dataset here:
https://www.kaggle.com/datasets/qiriro/stress

#### create a new usd_team5 python environment
conda create --name usd_team5 python=3.8

#### activate new environment
conda activate usd_team5

#### install packages
pip install -r requirements.txt

#### change data_set variable in stress_detection.ipynb file to the path where WESAD is downloaded:
data_set = r"/Users/hamidhooshmandi/Downloads/WESAD/S2"


#### sample data
![alt text](image.png)

# data description 
1. w_ax:
    1. Mean: Calculate the average wrist movement on the X-axis.
    2. Real-World Range: Typically between -2.0 and 2.0 (representing acceleration in meters per second squared).
    3. Example: Detecting wrist movements while typing on a keyboard; a value of 1.5 might indicate rapid typing, and -1.0 could represent a sudden stop.
2. w_ay:
    1. Standard Deviation: Measure the variation in arm movement on the Y-axis.
    2. Real-World Range: Typically between -2.0 and 2.0.
    3. Example: Arm being at rest or slightly lifted; a value of -0.5 could indicate a stable arm position, while -1.8 might suggest rapid, erratic movements.
3. c_az:
    1. Minimum and Maximum: Identify the range of chest movement on the Z-axis.
    2. Real-World Range: Typically between -5.0 and 5.0.
    3. Example: Monitoring breathing patterns; a value of -4.5 might represent a deep inhalation, and 4.0 could indicate a forceful exhalation.
4. c_ecg:
    1. Median: Find the middle value of heart electrical activity.
    2. Real-World Range: Typically between -2.0 and 2.0 (in millivolts).
    3. Example: Observing heart rhythm during a resting state; a value of -0.5 might correspond to a calm heartbeat, while -1.8 could indicate a rapid, irregular heartbeat.
5. c_emg:
    1. Standard Deviation: Assess the variability in chest muscle activity.
    2. Real-World Range: Typically between -5.0 and 5.0 (in millivolts).
    3. Example: Detecting muscle tension; a value near -4.5 could indicate significant muscle contraction, while 0.2 might represent relaxed muscles.
6. w_az:
    1. Mean: Calculate the average wrist rotation on the Z-axis.
    2. Real-World Range: Typically between -2.0 and 2.0.
    3. Example: Tracking wrist rotation; a value of 1.0 might show a moderate twist of the wrist, and -2.0 could represent an extreme, full rotation.
7. w_bvp:
    1. Percentiles: Determine the 25th and 75th percentiles of wrist blood volume pulse for distribution insights.
    2. Real-World Range: Typically between 30 and 150 (in beats per minute).
    3. Example: Measuring heart rate variability; a value of 140 might reflect a high-stress situation, while 60 could indicate a very relaxed state.
8. w_label:
    1. Count: Count the occurrences of each label (0 and 1) for stress detection analysis.
    2. Real-World Range: Binary (0, 1), representing different states or categories.
    3. Example: Labeling data for stress detection; a 0 could indicate data collected during a period of no stress, and 1 might represent high-stress situations.


# simple statistical operations:
    1. w_ax:
        a. Mean: Calculate the average wrist movement on the X-axis.
    2. w_ay:
        a. Standard Deviation: Measure the variation in arm movement on the Y-axis.
    3. c_az:
        a. Minimum and Maximum: Identify the range of chest movement on the Z-axis.
    4. c_ecg:
        a. Median: Find the middle value of heart electrical activity.
    5. c_emg:
        a. Standard Deviation: Assess the variability in chest muscle activity.
    6. w_az:
        a. Mean: Calculate the average wrist rotation on the Z-axis.
    7. w_bvp:
        a. Percentiles: Determine the 25th and 75th percentiles of wrist blood volume pulse for distribution insights.
    8. w_label:
        a. Count: Count the occurrences of each label (0 and 1) for stress detection analysis.


# potential use cases:
1. Stress Prediction Model:
    • Develop a stress prediction model based on HRV and EDA features. Use machine learning techniques to predict stress levels or classify stress states.
2. Exploratory Data Analysis (EDA):
    • Explore the relationships between HRV, EDA, and stress levels through visualization and statistical analysis.
    • Identify patterns or trends that could inform your stress prediction model.
3. Model Evaluation:
    • Evaluate the performance of different machine learning models for stress prediction, such as decision trees, random forests, support vector machines, or neural networks.
