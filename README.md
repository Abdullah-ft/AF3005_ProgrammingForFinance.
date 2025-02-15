# 📘 AF3005 – Programming for Finance  
## Smart Financial Management System 

 ### 📂 Repository Overview
This repository contains the implementation of a **Smart Financial Management System** developed as part of the **AF3005 – Programming for Finance** course. The system is designed to automate various financial operations, including loan eligibility checks, investment risk assessment, loan repayment tracking, stock price monitoring, and currency exchange rate tracking. The implementation uses **Python** and **ipywidgets** to create an interactive and user-friendly interface.

---
## 🎯 Features  
The system provides the following features:  

1. **Loan Eligibility & Interest Rate Calculation**  
   - Checks if a customer is eligible for a loan based on employment status, income, and credit score.  
   - Calculates the interest rate or rejects the loan based on predefined criteria.
  
2. **Investment Risk Assessment**  
   - Evaluates a portfolio of stocks and classifies the risk level as **High**, **Medium**, or **Low** based on stock returns.  

3. **Loan Repayment Tracker**  
   - Simulates loan repayment by deducting monthly payments and tracking the remaining balance until the loan is fully paid.  

4. **Stock Price Monitoring**  
   - Tracks daily stock prices and triggers an alert when the price reaches a target value (e.g., PKR 200).  

5. **Currency Exchange Rate Tracker**  
   - Simulates daily increases in the exchange rate (PKR/USD) and stops when the target rate is reached.  

---
## 🛠️ Implementation Details  

### **1. Loan Eligibility & Interest Rate Calculation**  
- **Inputs:**  
  - Employment status (Employed/Unemployed).  
  - Monthly income (PKR).  
  - Credit score.  

- **Logic:**  
  - If the applicant is unemployed, the loan is rejected immediately.  
  - If the income is below PKR 50,000, the loan is rejected.  
  - If the credit score is:  
    - **750+ → 5% Interest Rate**  
    - **650-749 → 8% Interest Rate**  
    - **Below 650 → Loan Rejected**  

- **ipywidgets Used:**  
  - Dropdown for employment status.  
  - Sliders for income and credit score.  
  - Button to check eligibility.  

---

### **2. Investment Risk Assessment**  
- **Inputs:**  
  - A list of stock returns (e.g., `10, -2, 7, 4`).  

- **Logic:**  
  - If any stock has a negative return → **High Risk**.  
  - If all stocks have positive returns but at least one is below 5% → **Medium Risk**.  
  - If all stocks have returns of 5% or above → **Low Risk**.  

- **ipywidgets Used:**  
  - Textbox for entering stock returns.  
  - Button to analyze risk.  

---

### **3. Loan Repayment Tracker**  
- **Inputs:**  
  - Initial loan amount (PKR).  
  - Monthly payment (PKR).  

- **Logic:**  
  - Deducts the monthly payment from the loan balance until the balance reaches zero.  
  - Displays the remaining balance after each payment.  

- **ipywidgets Used:**  
  - Sliders for initial loan amount and monthly payment.  
  - Button to start tracking repayment.  

---

### **4. Stock Price Monitoring**  
- **Inputs:**  
  - A list of daily stock prices (e.g., `150, None, 200`).  

- **Logic:**  
  - Skips missing data (`None` values).  
  - Stops tracking when the stock price reaches or exceeds PKR 200.  

- **ipywidgets Used:**  
  - Textbox for entering stock prices.  
  - Button to start tracking.  

---

### **5. Currency Exchange Rate Tracker**  
- **Inputs:**  
  - Starting exchange rate (PKR/USD).  
  - Target exchange rate (PKR/USD).  

- **Logic:**  
  - Simulates daily increases in the exchange rate by 1 PKR until the target rate is reached.  
  - Displays the exchange rate for each day.  

- **ipywidgets Used:**  
  - Sliders for starting and target exchange rates.  
  - Button to start tracking.  

---

## **🚀 How to Use the System**  
1. **Clone the Repository:**  
   ```bash
   git clone https://github.com/[YourUsername]/AF3005_ProgrammingForFinance.git
   ```

2. **Open the Jupyter Notebook:**  
   - Navigate to the repository and open the file `i222264_AF3005_Assignment1.ipynb` in Jupyter Notebook.

3. **Run the Cells:**  
   - Execute each cell to load the interactive widgets.  
   - Use the sliders, dropdowns, and textboxes to input data.  
   - Click the buttons to see the results.  

---

## **🌟 Why ipywidgets?**  
- **Interactive Inputs:**  
  - ipywidgets provide sliders, dropdowns, and textboxes, making it easy for users to input data interactively.  

- **User-Friendly Interface:**  
  - The widgets create a clean and intuitive interface, allowing users to interact with the system without writing code.  

- **Real-Time Feedback:**  
  - Results are displayed immediately after clicking the buttons, providing real-time feedback.  

---

## **📜 Code Structure**  
The code is structured into **5 parts**, each corresponding to a feature of the system. Each part:  
1. Defines input widgets using `ipywidgets`.  
2. Implements the logic using loops and conditional statements.  
3. Links the widgets to the logic using button clicks.  

---

## **📂 Repository Structure**  
```
AF3005_ProgrammingForFinance/
├── i222264_AF3005_Assignment1.ipynb  # Main Jupyter Notebook
├── README.md                         # This file
```

## **🙏 Acknowledgments**  
- Special thanks to **Dr. Usama Arshad** for guiding this project.  
- Inspired by real-world financial systems and automation tools.  

---

**Happy Coding! 🚀**  

---
