# Diabetes Detection using Machine Learning

This repository contains the code and resources for a machine learning project aimed at diabetes detection. We have implemented multiple machine learning models and data visualization techniques to build an accurate diabetes detection system.

## Models Used

We employed the following machine learning models for our project:

1. Decision Tree
2. Logistic Regression
3. Support Vector Machine
4. Random Forest
5. XGBoost

## Visualization Techniques

In addition to the models, we used various visualization techniques to gain insights from the data and evaluate model performance. These visualizations include:

1. Histograms: Used to visualize the distribution of key features in the dataset.
2. Correlation Matrix Graph: Helps in understanding the relationships between different features and their impact on the target variable.
3. ROC Curve: A graphical representation of the Receiver Operating Characteristic to evaluate the model's performance.

## Results

After thorough experimentation and evaluation, we found that the Decision Tree model performed exceptionally well for diabetes detection, achieving an accuracy of 78%. This result demonstrates the potential of machine learning in accurately identifying diabetes cases.

## Project Structure

- `diabetes.csv/`: Contains the dataset used for training and testing.
- `Diabetes.ipynb/`: Jupyter notebooks with the code for the project, including data preprocessing, model training, and visualization.
- `README.md`: This document, providing an overview of the project.

## Getting Started

To get started with this project, follow these steps:

1. Clone this repository to your local machine.
2. Navigate to the `notebooks/` directory and open the Jupyter notebooks to explore the code.
3. Ensure you have the required libraries and dependencies installed. You can do this using `pip install -r requirements.txt`.
4. Run the notebooks to train and evaluate the machine learning models and visualize the results.

## Dependencies

To run the code in this repository, you will need to have the following Python libraries and packages installed:

- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn
- xgboost

You can install these dependencies using `pip` with the provided `requirements.txt` file.

```bash
pip install -r requirements.txt
```

## Acknowledgments

This project was developed with the support of various open-source libraries and resources. We would like to thank the community for their contributions and the dataset providers for making their data available for research and analysis.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Feel free to explore, contribute, or use the code in your own projects. If you have any questions or suggestions, please open an issue or reach out to the project maintainers. We welcome your feedback and collaboration!
