# Exploratory Data Analysis Telco Customer Churn


This repository contains an exploratory data analysis (EDA) of the Telco Customer Churn dataset. The dataset includes information about Telco customers, their service subscriptions, account information, demographic details, and whether they have churned.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Analysis Steps](#analysis-steps)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction
Customer churn is a critical issue for businesses, particularly in the telecommunications sector. This project aims to analyze customer churn patterns and identify key factors that contribute to churn using exploratory data analysis techniques.

## Dataset
The dataset used in this analysis is publicly available on Kaggle: [Dataset Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) by BLASTCHAR.

### Features
The dataset consists of several features, including:
1. `customerID`: Customer ID
2. `gender`: Customer Gender ("Male", "Female")
3. `SeniorCitizen`: Whether the customer is a senior citizen (1: "Yes", 0: "No")
4. `Partner`: Whether the customer has a partner ("Yes", "No")
5. `Dependents`: Whether the customer has dependents ("Yes", "No")
6. `tenure`: Length of customer tenure
7. `PhoneService`: Whether the customer has phone service
8. `MultipleLines`: Whether the customer has multiple lines
9. `InternetService`: Whether the customer has internet service
10. `OnlineSecurity`: Whether the customer has online security service
11. `OnlineBackup`: Whether the customer has online backup service
12. `DeviceProtection`: Whether the customer has device protection service
13. `TechSupport`: Whether the customer has tech support service
14. `StreamingTV`: Whether the customer has streaming TV service
15. `StreamingMovies`: Whether the customer has streaming movies service
16. `Contract`: Type of payment contract ("Month-to-Month", "One Year", "Two Year")
17. `PaperlessBilling`: Whether the customer uses paperless billing
18. `PaymentMethod`: Type of payment method used by the customer
19. `MonthlyCharges`: Customer's monthly bill
20. `TotalCharges`: Customer's total bill
21. `Churn`: Whether the customer churned ("Yes", "No")

## Installation
To run the notebook, you need to have Python installed along with the necessary libraries. You can install the required libraries using the following command:

```bash
pip install -r requirements.txt
```

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/harshithas003/telcom-customer-churn.git
   ```
2. Navigate to the project directory:
   ```bash
   cd telcom-customer-churn
   ```
3. Open the Jupyter notebook:
   ```bash
   jupyter notebook telcom-customer-churn.ipynb
   ```

## Analysis Steps
The following steps were performed in the notebook:
1. **Data Preparation**
2. **Data Cleaning** (Handling missing values, removing duplicates)
3. **Data Understanding**
4. **Exploratory Data Analysis**
   - Univariate Analysis
   - Bivariate Analysis
   - Multivariate Analysis
   - Deep Dive Exploration
5. **EDA Conclusion**

## Results
1. The `TotalCharges` column was converted to float after removing whitespace strings, resulting in 7032 valid records.
2. There is no duplicate data.
3. The `SeniorCitizen` column is discrete with two unique values.
4. The `tenure` column shows a bimodal distribution, mostly around 1-5 months.
5. The `MonthlyCharges` column shows a distribution mostly around 20.
6. The `TotalCharges` column shows a right-skewed distribution mostly between 0-200.
7. There is a strong relationship between `tenure` and `TotalCharges`, and between `MonthlyCharges` and `TotalCharges`.
8. Gender and partner status do not significantly affect churn rates.
9. The majority of customers are young and do not have dependents.
10. Churn is most prevalent among young customers but is highest in percentage among senior customers.
11. Churn is high among customers with 0-20 months of tenure, likely due to high monthly and total charges.
12. Churn is higher among customers with minimal services and those using Fiber Optic internet.

## Contributing
Contributions are welcome! If you have any suggestions or improvements, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements
Special thanks to BLASTCHAR for providing the dataset and to the open-source community for their invaluable resources and tools.

---

Feel free to customize this README file further based on your specific requirements and preferences. Let me know if you need any additional modifications!
