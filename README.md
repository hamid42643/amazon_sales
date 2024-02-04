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
w_ax (Wrist Accelerometer X-axis): (-2 to +2 g) This measures the acceleration along the X-axis (side-to-side) of the wrist. It is used to detect motion and activity.

w_ay (Wrist Accelerometer Y-axis): (-2 to +2 g) This measures the acceleration along the Y-axis (up-and-down) of the wrist. It is used to detect vertical motion and orientation changes.

w_az (Wrist Accelerometer Z-axis): (-2 to +2 g) This measures the acceleration along the Z-axis (forward-and-backward) of the wrist. It helps in detecting movements along the depth of the wrist.

w_bvp (Wrist Blood Volume Pulse): (30-200 bpm) This is a derived signal from photoplethysmography (PPG) and represents changes in blood volume in the wrist, often used to measure heart rate and can provide insights into cardiovascular activity.

c_ecg (Chest Electrocardiogram): (0.5-4.0 mV) Although measured at the wrist with the Apple Watch's ECG feature, it is a standard electrocardiogram signal that records the electrical activity of the heart, helping to detect irregular heart rhythms.

# potential use cases:
1. Stress Prediction Model:
    • Develop a stress prediction model based on HRV and EDA features. Use machine learning techniques to predict stress levels or classify stress states.
2. Exploratory Data Analysis (EDA):
    • Explore the relationships between HRV, EDA, and stress levels through visualization and statistical analysis.
    • Identify patterns or trends that could inform your stress prediction model.
3. Model Evaluation:
    • Evaluate the performance of different machine learning models for stress prediction, such as decision trees, random forests, support vector machines, or neural networks.
