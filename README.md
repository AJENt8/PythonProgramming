# 🐍 Python Basics (TryHackMe)

> **Summary:** Learned Python fundamentals including variables, loops, functions, data structures, Boolean logic, file operations, and conditionals. Applied these concepts in small projects: a shipping cost calculator and a Bitcoin investment tracker.

---

## 🎯 Objective
Build a foundation in Python programming for automation and security scripting by practicing core syntax, operators, functions, and control flow.

---

## 🛠️ Environment
- Platform: TryHackMe — *Python Basics* room  
- Language: Python 3  
- Focus: Writing small, functional scripts to solve real-world problems  

---

## 🚀 Workflow

### 1) Python Fundamentals Learned
- **Variables** → storing values for reuse  
- **Loops** → iterating through lists and ranges  
- **Functions** → reusable blocks of logic  
- **Data Structures** → lists, dictionaries, sets  
- **Logical/Boolean Operators** → comparisons, `and`/`or`  
- **If statements** → decision making  
- **File Operations** → reading, appending, writing text files  

---

### 2) Project 1 — Shipping Cost Calculator
Calculated the customer’s basket cost including shipping fees, unless they qualified for free shipping.
- ```python
    shipping_cost_per_kg = 1.20
    customer_basket_cost = 34
    customer_basket_weight = 44

    if (customer_basket_cost >= 100):
        print('Free shipping!')
    else:
        shipping_cost = customer_basket_weight * shipping_cost_per_kg
        customer_basket_cost = 34 + shipping_cost

    print("Total basket cost including shipping is " + str(customer_basket_cost))
  

Output:
- ```python
  Total basket cost including shipping is 86.8

### 3) Project 2 — Bitcoin Investment Tracker
Created a function to convert Bitcoin to USD and trigger an alert if value dropped below $30,000.

Ex. 1
 - ```python
    investment_in_bitcoin = 1.2
    bitcoin_to_usd = 40000

    # Function to convert Bitcoin to USD
    def bitcoinToUSD(bitcoin_amount, bitcoin_value_usd):
        usd_value = bitcoin_value_usd * bitcoin_amount
        return usd_value

    investment_in_usd = bitcoinToUSD(investment_in_bitcoin, bitcoin_to_usd)

    if investment_in_usd <= 30000:
        print("Investment below $30,000! SELL!")
    else:
        print("Investment above $30,000")
Output:
- ```python
    Investment above $30,000

Ex. 2
- ```python
    investment_in_bitcoin = 1.2
    bitcoin_to_usd = 24000

    # Function to convert Bitcoin to USD
    def bitcoinToUSD(bitcoin_amount, bitcoin_value_usd):
        usd_value = bitcoin_value_usd * bitcoin_amount
        return usd_value

    investment_in_usd = bitcoinToUSD(investment_in_bitcoin, bitcoin_to_usd)

    if investment_in_usd <= 30000:
        print("Investment below $30,000! SELL!")
    else:
        print("Investment above $30,000")
Output:
- ```python
    Investment below $30,000! SELL!

### ✅ Outcome
- Gained hands-on practice with Python basics
- Built and tested two functional programs with real-world applications
- Understood how conditionals and functions make programs flexible and maintainable

### 🧩 Skills Demonstrated
- Python syntax and program flow
- Writing functions for reusability
- Working with variables, operators, and data structures
- File handling concepts (read, append, write)
- Applying logic to solve real-world scenarios
