# User-Data-Validation-Text-Analysis-System-Python

# User Data Validation & Text Analysis System

This project presents a **Python-based** text processing and validation module designed to clean, verify, and analyze raw user input before it is stored in a system. The application simulates a real-world data intake scenario commonly found in online platforms, focusing on reliable data handling using core Python concepts. The solution emphasizes structured validation, clarity of logic, and robustness while strictly relying on built-in string methods without the use of regular expressions or external libraries.

---

## 📌 Problem Overview

Online applications often receive **unclean and inconsistent user data**. This system processes raw string inputs, validates them, and generates a summary report identifying valid and invalid records.

### Given Input

```python
user_data = [
 " Anu, anu@gmail.com , 21 ",
 "Ravi ,ravi123gmail.com, 17",
 " Suresh,suresh@gmail.com,25 ",
 "Meena,meena@gmail,22",
 ",invalid@gmail.com,30"
]
```

---

## 🎯 Objectives

The system performs the following tasks:

### 1️⃣ Data Cleaning

* Remove extra spaces
* Split name, email, and age
* Convert name to **Title Case**
* Convert email to **lowercase**

### 2️⃣ Email Validation

An email is valid if:

* Contains exactly **one '@'**
* Contains at least **one '.' after '@'**
* Does **not start or end with '@'**

### 3️⃣ Age Validation

* Convert age to integer
* Check eligibility (**age ≥ 18**)

### 4️⃣ Invalid Record Identification

A record is invalid if it has:

* Missing name
* Invalid email format
* Invalid or non-numeric age

### 5️⃣ Summary Report

The system generates:

* Total records processed
* Number of valid users
* Number of invalid users
* Eligible users (18+)
* Underage users (<18)

### 6️⃣ Output Formatting

Each valid record is displayed as:

```
Name: Anu | Email: anu@gmail.com | Age: 21
```

---

## ⭐ Bonus Features

* Extract email domains (e.g., `gmail.com`)
* Count number of users per domain

---

## ⚙️ Constraints

* Uses **only Python string methods**
* ❌ No regular expressions
* ❌ No external libraries

---

## 🧠 Concepts Covered

* String manipulation (`strip()`, `split()`, `lower()`, `title()`)
* Conditional logic (`if-else`)
* Data validation
* List processing
* Basic reporting and analysis

---

## 📄 Sample Output

```
Name: Anu | Email: anu@gmail.com | Age: 21
Name: Suresh | Email: suresh@gmail.com | Age: 25

Total Records: 5
Valid Users: 2
Invalid Users: 3
Eligible Users: 4
Underage Users: 1
```

---

## 👤 Author

**Aparna Murali**
Beginner Python Developer | Data Analytics Enthusiast
