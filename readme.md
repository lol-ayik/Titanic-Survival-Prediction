# Titanic Survival Prediction

![Titanic](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fd/RMS_Titanic_3.jpg/1200px-RMS_Titanic_3.jpg)

## Project Overview
This machine learning project predicts passenger survival from the 1912 Titanic disaster using passenger data. The project demonstrates a complete ML workflow including data exploration, feature engineering, model training, and evaluation.

## Dataset
The dataset contains information about 891 Titanic passengers, including:
- Passenger class
- Name
- Sex
- Age
- Number of siblings/spouses aboard
- Number of parents/children aboard
- Ticket number
- Fare
- Cabin
- Embarkation port

## Installation
1. Clone the repository:
```bash
git clone https://github.com/Harshit-Patel01/Titanic-Survival-Prediction.git
```
2. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage
1. Run the Jupyter notebook for data analysis and model training:
```bash
jupyter notebook Titanic_Survival_Prediction.ipynb
```
2. For prediction using the trained model:
```python
from prediction import predict_survival

# Example passenger data
passenger_data = {
    'Pclass': 1,
    'Sex': 'female',
    'Age': 25,
    'SibSp': 0,
    'Parch': 0,
    'Fare': 50,
    'Embarked': 'S'
}

prediction = predict_survival(passenger_data)
print(f"Survival prediction: {'Survived' if prediction else 'Did not survive'}")
```

## Results
The model achieves the following performance metrics:
- Accuracy: [Your Accuracy Score]%
- Precision: [Your Precision Score]
- Recall: [Your Recall Score]
- F1-Score: [Your F1 Score]

Key findings:
- [Add 2-3 interesting insights from your analysis]

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
Distributed under the MIT License. See `LICENSE` for more information.

## Acknowledgments
- Kaggle for the Titanic dataset
- Scikit-learn documentation
- Python community for open-source libraries