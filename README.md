
# Predictive Maintenance of Motors using KMeans Clustering

## Project Overview
This project focuses on identifying defective motors using KMeans clustering. The dataset contains key operational parameters such as **current**, **voltage**, **temperature**, **humidity**, and **vibration**. The goal is to apply machine learning techniques for predictive maintenance, enabling early detection of motor defects and reducing operational downtime.

## Dataset
The dataset consists of the following features:

- **Current**: Electric current measured in amperes (A).
- **Voltage**: Voltage supplied to the motor measured in volts (V).
- **Temperature**: Motor's operating temperature measured in degrees Celsius (°C).
- **Humidity**: Humidity level in the operating environment measured in percentage (%).
- **Vibration**: Vibration levels of the motor measured in arbitrary units.

These parameters are critical for monitoring motor health and detecting potential faults.

## Objective
- Use KMeans clustering to classify motors into different clusters based on their operating conditions.
- Identify defective motors by analyzing clusters that indicate abnormal or risky behavior.
- Implement predictive maintenance by leveraging the insights from clustering to take corrective actions before motor failure occurs.
- 
## Methodology

1. **Data Preprocessing**:
   - Cleaned the dataset by handling missing or erroneous values.
   - Scaled the data using standardization techniques to normalize feature values.
   
2. **KMeans Clustering**:
   - Implemented KMeans clustering to classify motors into two clusters:
     - **Cluster 1**: Normal operating motors.
     - **Cluster 2**: Potentially defective motors based on abnormal readings in one or more parameters.
   - Determined the optimal number of clusters using the **Elbow Method**.

3. **Model Evaluation**:
   - Visualized the clustering results using scatter plots to analyze the separation of clusters.
   - Used Seaborn for detailed analysis of feature distributions within each cluster.

## Results
The KMeans model successfully classified motors into two distinct clusters based on their operating conditions. Cluster 2, which showed abnormal behavior, represents motors with potential defects that require maintenance.

Key findings:
- Motors in **Cluster 2** had higher values of vibration and temperature, which are common indicators of wear or damage.
- **Predictive maintenance** actions were suggested based on the clustering results to prevent motor failures.

## Tools and Technologies
- **Python**: Used for data analysis and model development.
- **Pandas**: For data manipulation and preprocessing.
- **Scikit-learn**: For implementing KMeans clustering.
- **Seaborn & Matplotlib**: For data visualization and cluster analysis.


## Future Improvements
- Incorporate additional features such as load and power factor for a more comprehensive analysis.
- Explore other clustering techniques like DBSCAN or hierarchical clustering to improve model accuracy.
- Implement real-time data streaming and anomaly detection for live monitoring of motors.

## Conclusion
This project demonstrates how KMeans clustering can be applied to predict motor defects and enhance maintenance strategies. By leveraging this approach, businesses can optimize motor performance, reduce maintenance costs, and prevent unexpected failures.
