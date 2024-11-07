# **Formula 1 Race Position Prediction**

### **Overview**
This project leverages historical Formula 1 race data to predict driver finishing positions using machine learning models. By integrating data on races, drivers, constructors, circuits, and results, this project explores various predictive algorithms to uncover patterns and factors influencing race outcomes.

### **Objective**
To build an effective predictive model that can forecast the finishing position of a Formula 1 driver based on pre-race and race-specific data. The project examines neural network architectures and compares their performance with tree-based ensemble methods.

### **Datasets Used**
- **drivers.csv**: Driver information, including unique identifiers and nationalities.
- **constructors.csv**: Details of constructor (team) information.
- **races.csv**: Contains race event details, including year, round, and circuit.
- **results.csv**: Contains race results for each driver, our primary target variable.
- **qualifying.csv**: Qualifying session results, providing performance data before the race.
- **circuits.csv**: Information on race circuits, including location and country.

### **Project Structure**
- **Data Loading and Cleaning**: Load and merge datasets, perform initial cleaning, and handle missing values to prepare data for analysis.
- **Feature Selection and Preprocessing**: Select relevant features, encode categorical variables, and scale numerical features to ensure uniformity.
- **Model Development**: Build and experiment with various neural network architectures, applying techniques like dropout, batch normalization, and alternative activation functions.
- **Comparative Analysis**: Compare neural network models with tree-based models (e.g., XGBoost) to identify the best-performing algorithm.
- **Evaluation**: Use regression metrics (MSE and R² Score) to assess model performance and visualize training progress.

### **Getting Started**

#### **Requirements**
- Python 3.7+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `tensorflow`, `xgboost`, `scikit-learn`

### **Results and Findings**
After testing multiple model architectures, XGBoost was identified as the most effective model for predicting race positions, outperforming neural network configurations in terms of accuracy and robustness. Key features identified include driver nationality, team, grid position, and previous race results.

### **Future Enhancements**
- **Feature Engineering**: Incorporate additional race conditions (e.g., weather, tire choices) to improve model accuracy.
- **Hyperparameter Tuning**: Further optimize models to enhance performance.
- **Explainability**: Use SHAP values or feature importance for insights into which features most influence predictions.

### **License**
This project is licensed under the MIT License.

### **Contact**
For questions or contributions, please contact [Hamza Atout](mailto:hsa60@mail.aub.edu). 

_This project showcases the intersection of data science and motorsports, offering insights into the dynamics of Formula 1 racing through data-driven analysis._