# download Biometrics for stress monitoring dataset here:
https://www.kaggle.com/datasets/qiriro/stress

# create a new usd_team5 python environment
conda create --name usd_team5 python=3.8

# activate new environment
conda activate usd_team5

# install packages
pip install -r requirements.txt

# change data_set variable in stress_detection.ipynb file to the path where WESAD is downloaded:
data_set = r"/Users/hamidhooshmandi/Downloads/WESAD/S2"


# sample data
![alt text](image.png)

# data description 
w_ax:
    - Full name: Wrist Accelerometer X-axis
    - Measures: Movement on the X-axis of a wrist-worn device
    - Range: Approximately 0.80 to 0.95 in the dataset
    - Example: Detecting wrist movements while typing on a keyboard; a value of 0.90 might indicate a light movement.

w_ay:
    - Full name: Wrist Accelerometer Y-axis
    - Measures: Movement on the Y-axis of a wrist-worn device
    - Range: About -0.22 to -0.16
    - Example: Arm being at rest or slightly lifted; a value of -0.20 could indicate a stable arm position with minimal movement.

c_az:
    - Full name: Chest Accelerometer Z-axis
    - Measures: Movement on the Z-axis of a chest-worn device
    - Range: Approximately -0.34 to -0.55
    - Example: Monitoring breathing patterns; a value of -0.50 might represent a normal inhalation or exhalation.

c_ecg:
    - Full name: Chest Electrocardiogram
    - Measures: Electrical activity of the heart
    - Range: About -1.16 to -1.15
    - Example: Observing heart rhythm during a resting state; a value of -1.15 might correspond to a normal resting heartbeat.

c_emg:
    - Full name: Chest Electromyography
    - Measures: Electrical activity of chest muscles
    - Range: Around -0.02 to 0.01
    - Example: Detecting muscle tension; a value near 0.00 could indicate relaxed muscles.

w_az:
    - Full name: Wrist Accelerometer Z-axis
    - Measures: Movement on the Z-axis of a wrist-worn device
    - Range: Around 5.24 to 5.26
    - Example: Tracking wrist rotation; a value of 5.25 might show a slight twist of the wrist.

w_bvp:
    - Full name: Wrist Blood Volume Pulse
    - Measures: Blood flow, indicative of heart rate
    - Range: About 30.07 to 30.12
    - Example: Measuring heart rate variability; a value of 30.10 could reflect a stable heart rate during a calm state.

w_label:
    - Full name: Label
    - Measures: Classification label (e.g., stress vs. no stress)
    - Range: Binary (0, 1), only 0 in the dataset
    - Example: Labeling data for stress detection; a 0 could label data collected during a period of no stress.


# potential use cases:
1. Stress Prediction Model:
    • Develop a stress prediction model based on HRV and EDA features. Use machine learning techniques to predict stress levels or classify stress states.
2. Exploratory Data Analysis (EDA):
    • Explore the relationships between HRV, EDA, and stress levels through visualization and statistical analysis.
    • Identify patterns or trends that could inform your stress prediction model.
3. Model Evaluation:
    • Evaluate the performance of different machine learning models for stress prediction, such as decision trees, random forests, support vector machines, or neural networks.
