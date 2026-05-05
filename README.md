# IT3040 – Assignment 1 (Option 1)

## Transliteration Accuracy Testing

### Student Details

* **IT Number:** IT23817708

---

## 📌 Project Overview

This project focuses on testing the accuracy of a Sinhala transliteration system available at:
https://www.pixelssuite.com/chat-translator

The objective is to evaluate how accurately the system converts **Singlish (Sinhala typed using English letters)** into **Sinhala Unicode text**.

A set of **50 negative test cases** were designed where the system fails to produce the correct output. These test cases were automated using **Playwright** and results were recorded in an Excel file.

---

## 🛠 Technologies Used

* Python 3.11
* Playwright
* OpenPyXL
* Google Chrome

---

## 📂 Project Structure

test_automation/
├── test_automation.py
├── Assignment 1 - Test cases.xlsx

---

## ⚙️ Setup Instructions

### 1. Install Python

Download and install Python (version 3.11 or higher).

### 2. Install Dependencies

Open Command Prompt and navigate to the project folder:

cd /d D:\test_automation

Run the following commands:

pip install -U pip
pip install playwright openpyxl
playwright install

---

## ▶️ How to Run the Automation Script

Run the following command:

python test_automation.py --excel "Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open

---

## 📊 Test Case Details

* Total Test Cases: 50
* Type: Negative Test Cases
* Input: Singlish text
* Expected Output: Correct Sinhala translation
* Actual Output: System-generated output
* Status: Automatically marked as Pass/Fail

Each test case covers different Singlish input patterns such as:

* Questions
* Commands
* Slang
* Emojis
* English word insertions
* Numbers, dates, and symbols

---

## 📝 Notes

* Only failure scenarios were considered as per assignment requirements.
* Expected outputs were manually defined based on correct Sinhala translations.
* Actual outputs and status were generated automatically using the script.

---

## 🔗 GitHub Repository

(Add your GitHub repository link here)

---

## ✅ Conclusion

This project demonstrates the limitations of the transliteration system when handling informal Singlish inputs. The automation approach helps efficiently validate multiple scenarios and identify inaccuracies in the system.

---
