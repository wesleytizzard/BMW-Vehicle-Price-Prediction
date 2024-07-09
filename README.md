### Project: BMW Vehicle Price Prediction

**Project Summary:**
This project aims to predict the prices of BMW vehicles using data cleaning and preprocessing techniques. The original dataset contains various information about different BMW models, including features such as mileage, power, registration date, fuel type, color, among others.

**Project Objectives:**
1. Perform thorough cleaning of the dataset, removing duplicate data and handling missing values.
2. Apply data preprocessing techniques to prepare the dataset for use in predictive models.
3. Explore and visualize the data to identify significant patterns and relationships between variables.
4. Establish a solid foundation for future predictive models of vehicle prices, although the final prediction is not performed in this stage.

**Methodology:**
1. **Importing Libraries and Loading the Dataset:**
   - Libraries such as pandas, numpy, matplotlib, seaborn, sklearn, folium, and plotly are used for data manipulation, visualization, and preprocessing.
   - The dataset `bmw_pricing_v3.csv` is loaded from Google Drive.

2. **Removing Duplicate Data:**
   - Duplicate records are removed from the dataset.

3. **Handling Missing Values:**
   - Missing values in each column are identified and handled according to their context:
     - `modelo`: Missing values are replaced with 'desc'.
     - `km` and `potencia`: Missing values are replaced with the median, as they do not have a normal distribution.
     - `fecha_registro`: Missing values are replaced with 'No info'.
     - `tipo_gasolina` and `color`: Missing values are replaced with the mode of the corresponding model.
     - `tipo_coche`, `volante_regulable`, `aire_acondicionado`, `bluetooth`, `alerta_lim_velocidad`: Missing values are replaced with the mode of the model.
     - `camara_trasera` and `elevalunas_electrico`: Records with missing values are removed due to their low quantity.
     - `precio`: Missing values are replaced with the mean according to the model.
     - `fecha_venta`: The single missing value is removed.

4. **Visualization and Exploratory Analysis:**
   - Histograms and distribution plots are created to understand the dispersion and patterns of the data.
   - Interactive maps and charts are used to explore the geographical distribution and characteristics of the vehicles.

5. **Preparation for Predictive Modeling:**
   - Although the main objective is cleaning and preprocessing, a foundation is laid for future predictive models that can use this clean dataset to train machine learning algorithms and predict BMW vehicle prices.

This project demonstrates key skills in data manipulation and cleaning, as well as using Python libraries for data analysis, which are essential for roles in data analysis and data science.
